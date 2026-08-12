---
name: clean-el-traffic-csv
description: Limpa uma exportação bruta de CSV de tráfego do Experience League/Adobe Analytics para páginas somente do Workfront, classificada por Exibições de página. Use quando o usuário fornecer um CSV de tráfego de página do Experience League (colunas como "URL da página genérico", "Visitantes únicos", "Visitas", "Exibições de página") e solicitar que ele limpe, filtre ou processe ou mencionar planilhas de "rastreamento de documentação" / "artigos mais visualizados".
source-git-commit: e22d43e9962b2b00793577fd14ac00587e8a2a6d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# Limpar CSV de tráfego do Experience League

Transforma uma exportação bruta de tabela de forma livre do Adobe Analytics do tráfego de página do Experience League em um CSV limpo, somente Workfront, desduplicado classificado por Exibições de página, substituindo o arquivo original e também salvando uma cópia datada na Área de trabalho.

## Formas de entrada

A entrada pode ser uma de duas formas:

1. **Exportação bruta** — começa com linhas de comentário de metadados (`#===`, `# Freeform`, `# Report suite: ...`, `"# Date: <range>"`, etc.), seguidas por uma tabela de detalhamento hierárquico (por exemplo, `Solution (v2)` → `workfront` → `Page URL Generic (v33)` → linhas de URL individuais). A célula literal `Page URL Generic (v33)` (ou rótulo `Page URL Generic ...` semelhante) aparece parcialmente para baixo, na segunda coluna.
2. **CSV já limpo** — a primeira linha já é um cabeçalho simples como `Page URL Generic (v33),Unique Visitors,Visits,Page Views`, sem linhas de metadados ou colunas à esquerda extras.

Detectar qual forma você tem antes de começar: se a linha 1 for uma linha de cabeçalho simples que corresponda à forma 2, pule diretamente para a Etapa 2 (nenhum intervalo de datas estará disponível, então pule também a Etapa 7, a menos que o usuário forneça um intervalo de datas separadamente).

## Fluxo de trabalho (WRK)

### Etapa 0: Capture o intervalo de datas (somente exportação bruta, antes de excluir qualquer item)

Localize a linha de metadados próxima ao(s) `# Date: <range>` correspondente(s) superior(es) (por exemplo: `"# Date: Jul 1, 2026 - Jul 31, 2026"`). Registro `<range>` (por exemplo, `Jul 1, 2026 - Jul 31, 2026`) — é necessário posteriormente na Etapa 7. Faça isso antes da exclusão de qualquer linha.

### Etapa 1: retirar a exportação bruta para uma tabela simples (apenas exportação bruta)

1. Localize a linha que contém a célula `Page URL Generic (...)` (está na segunda coluna na exportação padrão).
2. Exclua todas as linhas acima dessa linha, incluindo as linhas de comentário de metadados e as linhas de subtotal `Solution (v2)` / `workfront`.
3. Exclua todas as colunas à esquerda da célula `Page URL Generic` (na exportação padrão, essa é apenas a coluna A).
4. Nessa mesma linha (agora a linha de cabeçalho), substitua os valores de subtotal numérico à direita de `Page URL Generic (...)` pelos cabeçalhos literais, na ordem: `Unique Visitors`, `Visits`, `Page Views`. Deixe a célula `Page URL Generic (...)` inalterada.

Resultado: um CSV simples com cabeçalho `Page URL Generic (v33),Unique Visitors,Visits,Page Views` seguido de uma linha por URL.

### Etapa 2: manter somente linhas do Workfront

Para cada linha de dados, verifique se a URL contém a subsequência literal `/workfront/` (barra em ambos os lados). O prefixo da localidade não importa (`/en/`, `/zh-hans/`, etc. — todos permanecem enquanto o segmento de produto corresponder).

- Exclua a linha se a URL **não** contiver `/workfront/` como um segmento de caminho — isso remove outros produtos, como `workfront-fusion`, `workfront-learn`, `proofhqpapi`, etc. (uma subcadeia de caracteres como `tutorials-workfront` contiver **não** — a correspondência deve ser o segmento exato `/workfront/`).
- Caso contrário, mantenha a linha.

### Etapa 3: Cortar o URL

Para cada linha sobrevivente, localize `/using` na URL e mantenha somente a parte de (e incluindo) a `/` que a segue, descartando tudo antes e incluindo `/using`.

Exemplo: `https://experienceleague.adobe.com/pt-br/docs/workfront/using/home` → `/home`

Se `/using` não for encontrado na URL de uma linha do Workfront, deixe essa URL inalterada e marque-a para o usuário, em vez de adivinhar.

### Etapa 4: retirar sufixos de fragmento/consulta

Se a URL aparada contiver um `#` ou `?`, exclua esse caractere e tudo o que vem depois dele.

Exemplo: `/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### Etapa 5: Mesclar duplicatas

Depois de aparar, várias linhas agora podem compartilhar o mesmo URL (por exemplo, duas linhas de localidade diferentes que são recolhidas para o mesmo caminho). Combine todas as linhas com uma URL idêntica em uma linha, somando `Unique Visitors`, `Visits` e `Page Views` independentemente.

Exemplo: `/home,2,2,3` e `/home,5,6,7` → `/home,7,8,10`

### Etapa 6: Classificar por exibições de página

Classificar todas as linhas de dados por `Page Views` em ordem decrescente (maior primeiro). A linha de cabeçalho permanece fixa na parte superior, acima dos dados classificados.

### Etapa 7: adicionar a linha de intervalo de datas (somente exportação bruta, se capturada na Etapa 0)

Antes de inseri-lo, remova qualquer vírgula fora do intervalo de datas capturado (por exemplo, `Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`) — o intervalo bruto tem vírgulas que de outra forma seriam lidas incorretamente como separadores de coluna CSV nessa linha.

Insira uma nova linha na parte superior, acima da linha de cabeçalho, contendo apenas o intervalo de datas removido por vírgulas.

Ordem final da linha: intervalo de datas linha → linha do cabeçalho → linhas de dados classificadas.

### Etapa 8: salvar

Substitua o arquivo de entrada original no local com o resultado limpo.

### Etapa 9: salvar uma cópia datada na Área de Trabalho (somente exportação bruta, se um intervalo de datas tiver sido capturado na Etapa 0)

Crie uma versão segura para nome de arquivo do intervalo de datas: remova vírgulas e substitua qualquer um dos `\ / : * ? " < > |` por `-` (esses caracteres são inválidos nos nomes de arquivos do Windows e poderiam aparecer em um intervalo de datas dependendo da localidade/formato de exportação).

Salve uma cópia adicional do CSV limpo (mesmo conteúdo da Etapa 8) na área de trabalho do usuário atual, chamada:

`Documentation tracking report <filename-safe date range>.csv`

Exemplo: um intervalo capturado de `Apr 1, 2026 - Apr 30, 2026` torna-se `Documentation tracking report Apr 1 2026 - Apr 30 2026.csv`.

Ignore esta etapa para um CSV já limpo (forma 2), a menos que o usuário forneça um intervalo de datas separadamente.

## Fora do escopo

Publicar ou compartilhar o CSV limpo (por exemplo, no Slack) é uma etapa separada, ainda não definida. Não tente anexar ou carregar o arquivo em nenhum lugar como parte dessa habilidade.

## Implementação (exportação bruta)

Para uma exportação bruta, execute as Etapas 0 a 8 com este script do PowerShell testado em vez de editar linhas manualmente — é mais rápido e menos propenso a erros para arquivos com centenas de linhas. Substituir o caminho real do arquivo por `$path`.

Antes de executar, verifique se o arquivo está bloqueado (por exemplo, aberto no Excel) — se `Set-Content` falhar ao &quot;ser usado por outro processo&quot;, peça ao usuário para fechá-lo e execute novamente.

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8

# Step 9: also save a dated copy to the Desktop
$safeDateRange = ($dateRange -replace ',', '') -replace '[\\/:*?"<>|]', '-'
$desktopPath = Join-Path ([Environment]::GetFolderPath('Desktop')) "Documentation tracking report $safeDateRange.csv"
Set-Content -Path $desktopPath -Value $outLines -Encoding UTF8
```

Para um CSV já limpo (forma de entrada 2), ignore a realocação de cabeçalho, a lógica de intervalo de datas e a Etapa 9 — basta executar as Etapas 2 a 6 e 8 no cabeçalho/linhas existentes como estão.
