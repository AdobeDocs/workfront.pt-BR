---
name: release-notes-formatter
description: Formatar e validar as notas de versão do Workfront para fins de consistência, estrutura correta e vinculação adequada. Use somente para arquivos de notas de versão em diretórios de versões de produtos, ou quando o usuário mencionar notas de versão, versões de produtos ou versões trimestrais. Não se aplique a artigos explicativos ou documentação geral.
source-git-commit: fa39320af72acf6d2ceaf201480baf78a07ae76e
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 2%

---


# Formatador das notas de versão

Formata e valida as notas de versão do Adobe Workfront no diretório `help/quicksilver/product-announcements/product-releases/`.

## Tipos de página

Identifique o tipo de página a partir do caminho e do conteúdo do arquivo:

| Tipo de página | Padrão do arquivo | Modelo |
|-----------|-------------|----------|
| **Visão geral** | `{YY}-q{N}-release-overview.md` | Consulte .claude/commands/_release-notes-formatter-reference.md#overview-page-template |
| **Área do produto** | `{YY}-q{N}-{area}.md` | Consulte .claude/commands/_release-notes-formatter-reference.md#product-area-page-template |
| **Planejamento** | `planning-release-activity-{YY}-q{N}.md` | Semelhante à área do produto |
| **Aparência** | `look-and-feel-updates-{YY}-q{N}.md` | Consulte .claude/commands/_release-notes-formatter-reference.md#look-and-feel-page-template |

## Etapa 0: Determinar o Trimestre (faça isso antes de qualquer outra coisa)

>[!IMPORTANT]
>
>Nunca atribua um recurso a um trimestre-documento usando a matemática do trimestre-calendário em sua data de Pré-visualização ou Produção. O trimestre-documento é baseado no qual a **versão mensal** do recurso é entregue, de acordo com o agrupamento do calendário de lançamento interno da Workfront, que é deslocado do trimestre-calendário — consulte a tabela [Calendário de lançamento de 2026](#2026-release-calendar) próximo ao final deste arquivo. Por exemplo, um recurso com uma Data de produção de 13 de agosto de 2026 pertence ao doc-quarter `26-q4`, não `26-q3`, pois a versão mensal de agosto mapeia para `26-q4`.
>
>A tabela &quot;Quarter Mapping&quot; mais abaixo (Formulário Escrito/Meses) é para escrever nomes de trimestre em títulos (por exemplo, &quot;Terceiro Trimestre&quot; para Q3) — é **não** suficiente por si só para decidir a quais arquivos de trimestre um recurso pertence. Sempre compare com a tabela do Calendário de lançamento antes de criar ou editar qualquer arquivo.
>
>Se a data de Produção de um recurso não aparecer na tabela do Calendário de lançamento (por exemplo, estiver além do intervalo de datas da tabela), peça ao usuário um calendário atualizado, em vez de adivinhar.

## Fluxo de trabalho de formatação

### Etapa 1: Validar Frontmatter

Campos obrigatórios para todas as páginas de notas de versão:

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

Regras:
- `feature` deve ser exatamente `Product Announcements`
- `recommendations` deve ser exatamente `noDisplay, noCatalog`
- Nunca inventar um `exl-id` — incluir apenas se já existir um
- Não adicionar `draft: Probably` a páginas reais (somente modelos)

### Etapa 2: validar estrutura por tipo de página

#### Páginas de área de produto

1. **H1**: `{Written Quarter} {Area} enhancements`
   - Exemplo: `# Second Quarter 2026 Administrator enhancements`
   - O trimestre deve ser escrito: &quot;Primeiro trimestre&quot;, &quot;Segundo trimestre&quot;, &quot;Terceiro trimestre&quot;, &quot;Quarto trimestre&quot;

2. **Parágrafo de introdução**: descreve a área e os links para a visão geral
   - Deve vincular ao **arquivo de visão geral** do trimestre correto
   - Erro comum: vinculação ao trimestre anterior (por exemplo, `26-q1` em vez de `26-q2`)

3. **H2 por recurso**: título do recurso como cabeçalho
   - **Recursos mais recentes primeiro** — a nota de versão mais recente deve aparecer como o primeiro H2 após o parágrafo de introdução
   - Os recursos mais antigos seguem em ordem cronológica inversa

4. **Bloco de texto explicativo de data** após cada H2:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **Corpo**: descrição do recurso e, em seguida, link para a documentação de ajuda

#### Páginas de visão geral

1. **H1**: `{Written Quarter} release overview`

2. **Parágrafo de introdução** com mês de lançamento agendado

3. **`>[!IMPORTANT]`bloco** com tabela de cronograma de lançamento

4. **H2`Adobe Workfront enhancements`** com lista de marcadores de links âncora:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. **H3 por área de produto** com a tabela de recursos do HTML (consulte .claude/commands/_release-notes-formatter-reference.md#overview-feature-table)
   - Em cada tabela, **os recursos mais recentes primeiro** — a linha mais recente aparece na parte superior da tabela (após a linha de cabeçalho)

&#x200B;6. **Seções finais** (H2): Notas de versão para outras áreas, atualizações do visualizador de provas de desktop, Avisos, versão da API, Atualizações de manutenção, Atualizações de treinamento

### Etapa 3: Validar links

- **Link de visão geral nas páginas de área de produto**: deve apontar para o mesmo trimestre
  - Correto: `26-q2-release-activity/26-q2-release-overview.md`
  - Errado: `26-q1-release-activity/26-q1-release-overview.md`
- **Ancorar links na visão geral**: deve corresponder às IDs H3 (minúsculas, hifens)
- **Links de recursos em tabelas de visão geral**: deve usar `class="MCXref xref" xrefformat="{para}"`
- **Links de documentos de ajuda**: deve começar com `/help/quicksilver/`

### Etapa 4: Validar Datas

- Formato: `{Month} {Day}, {Year}` (por exemplo, &quot;12 de março de 2026&quot;)
- Usar `TBD` para datas desconhecidas
- As datas no bloco `>[!NOTE]` da página de área de produto devem corresponder à linha correspondente da tabela de visão geral
- As datas de visualização devem preceder as datas de Produção

### Etapa 5: Correções Comuns

Aplicar essas correções ao formatar:

| Problema | Corrigir |
|-------|-----|
| Trimestre do link de visão geral incorreto | Atualizar para corresponder ao trimestre do próprio arquivo |
| Bloco de data `>[!NOTE]` ausente | Adicionar bloco após o cabeçalho do recurso H2 |
| Formato de data inconsistente | Padronizar para `Month Day, Year` |
| Linha em branco ausente antes de `>[!NOTE]` | Adicionar linha em branco |
| Espaços adicionais em linhas de texto explicativo | Cortar espaço em branco à direita |
| HTML nas páginas de área de produto | Manter como marcação (o HTML é somente para tabelas de visão geral) |
| `exl-id` ausente | Deixe-o fora — não gere um |

### Etapa 6: atualizar o sumário

Sempre que você criar uma página de notas de versão **nova** (visão geral ou área de produto), adicione-a a `help/quicksilver/TOC.md` na mesma alteração. Uma página que não esteja no índice não será exibida na navegação publicada, mesmo se os links na tabela de visão geral apontarem para ela.

Onde adicioná-lo:

- O índice tem uma seção por trimestre sob um cabeçalho como `* 2026 Q3 Release {#release-26-q3}`. Se o cabeçalho do trimestre ainda não existir (primeira página de um novo trimestre), adicione-o acima do trimestre anterior para que o trimestre mais recente fique na parte superior.
- Sob esse cabeçalho de trimestre, liste as páginas nesta ordem:
  1. **Visão geral** primeiro (`Third Quarter 2026 release overview`).
  2. **Páginas de área de produto** em ordem alfabética por nome de área (Administrador, Documentos, Operações Empresariais, Projetos, Relatórios, Solicitações).
  3. **Outras melhorias** por último (sempre após as áreas de produto alfabéticas).

Cada entrada do índice é um link de marcação que usa o título da página e o caminho absoluto do repositório:

```markdown
      * [Third Quarter 2026 Documents enhancements](/help/quicksilver/product-announcements/product-releases/26-q3-release-activity/26-q3-documents.md)
```

Corresponder recuo (seis espaços) às entradas ao redor. Use o texto integral da página H1 como o texto do link — por exemplo `Documents enhancements`, `Requesting enhancements` (não `Requests`) — portanto, os rótulos de índice correspondem aos trimestres anteriores.

Erros comuns a evitar:

- Criação de uma página da área do produto sem adicioná-la ao índice.
- Vinculação a uma visão geral de trimestre diferente da nova página da área de produto (Etapa 3).
- Inserir as páginas de um novo trimestre sob o cabeçalho do trimestre anterior.

### Etapa 7: atualizar a home page

Sempre que você criar uma **nova página de visão geral do trimestre** (isto é, esta é a primeira página de um novo trimestre, não apenas uma nova página da área de produto adicionada a um trimestre existente), atualize `help/quicksilver/home.md` com a mesma alteração:

- Na seção `>[!TAB Latest release]`, substitua o link de visão geral da versão pelo link de visão geral do novo trimestre.
- Além disso, nessa seção, atualize o link da atividade de lançamento do Adobe Workfront Planning para apontar para o arquivo de planejamento do novo trimestre (`planning-release-activity-{YY}-q{N}.md`), se existir.
- Na guia `>[!TAB {YYYY} releases]` do ano atual, adicione o link de visão geral do novo trimestre na parte superior da lista, acima da entrada do trimestre anterior.

Não toque em `home.md` ao adicionar apenas uma página da área do produto a um trimestre que já tenha uma página de visão geral listada lá.

Erros comuns a evitar:

- Criar uma nova página de visão geral do trimestre sem atualizar a guia &quot;Versão mais recente&quot; de `home.md` (continuará apontando para o trimestre antigo).
- Esquecendo-se de adicionar também o novo trimestre à lista de guias do ano atual.

## Convenções de nomenclatura de arquivos

| Tipo | Padrão | Exemplo |
|------|---------|---------|
| Visão geral | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| Área do produto | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| Diretório | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

Lesões de área padrão: `admin-and-setup`, `documents`, `projects`, `reports`, `requests`, `other`

## Mapeamento do trimestre

>[!NOTE]
>
>Essa tabela serve para anotar nomes de trimestre (por exemplo, em um H1 ou título). ELE NÃO determina a quais arquivos do trimestre um recurso pertence — use a tabela [Calendário de versão de 2026](#2026-release-calendar) abaixo para isso, pois o trimestre-doc é deslocado do trimestre-calendário.

| Trimestre | Formulário Escrito | Months |
|---------|-------------|--------|
| T1 | Primeiro trimestre | Jan-Mar |
| T2 | Segundo trimestre | Abr-jun |
| T3 | Terceiro trimestre | Jul-Set |
| T4 | Quarto trimestre | Out-Dez |

**Importante — o trimestre do documento usado nos nomes de arquivo (`26-q3`, `26-q4`, etc.) é deslocado por um mês deste mapeamento de calendário.** Em vez disso, ele segue o agrupamento interno do calendário de lançamento da Workfront, em que cada trimestre do documento = as duas versões mensais anteriores + o mês de lançamento trimestral. Por exemplo, o trimestre `26-q3` abrange as versões mensais de maio/junho/julho de 2026 (versão trimestral `2026.07`), e o trimestre `26-q4` abrange as versões mensais de agosto/setembro/outubro de 2026 (versão trimestral `2026.10`). Sempre verifique o calendário de lançamento abaixo (ou solicite um atualizado) antes de presumir o trimestre de um arquivo com base na tabela de trimestre-calendário acima.

## Calendário de lançamento de 2026

Source: &quot;Calendário de lançamento mensal de 2026&quot; (wiki do Adobe corp, espaço AWF — `wiki.corp.adobe.com`, chave de espaço AWF, título &quot;Calendário de lançamento mensal de 2026&quot;). O WebFetch não pode acessar esta página (requer Adobe SSO); peça ao usuário para colar uma PDF/tabela atualizada quando as datas forem necessárias além do que é capturado aqui.

| Mês de lançamento | Visualização final | Produção | Lançamento mensal | Versão trimestral | Trimestre do documento |
|---|---|---|---|---|---|
| Nov de 2025 | 30-out-2025 | 13-nov-2025 | 2025.11 | 2026.01 | 26-t1 |
| Dez de 2025 | 27-nov-2025 | 11-dez-2025 | 2025.12 | 2026.01 | 26-t1 |
| Janeiro de 2026 | 23-dez-2025 | 15-jan-2026 | 2026.01 | 2026.01 | 26-t1 |
| Fev de 2026 | 29-jan-2026 | 12-fev-2026 | 2026.02 | 2026.04 | 26-t2 |
| Março de 2026 | 26-fev-2026 | 12-mar-2026 | 2026.03 | 2026.04 | 26-t2 |
| Abril de 2026 | 02-abr-2026 | 16-abr-2026 | 2026.04 | 2026.04 | 26-t2 |
| Maio de 2026 | 30-abr-2026 | 14-maio-2026 | 2026.05 | 2026.07 | 26-3t |
| Junho de 2026 | 28-maio-2026 | 11-jun-2026 | 2026.06 | 2026.07 | 26-3t |
| Jul de 2026 | 07-jul-2026 | 16-jul-2026 | 2026.07 | 2026.07 | 26-3t |
| Agosto de 2026 | 30-jul-2026 | 13-ago-2026 | 2026.08 | 2026.10 | 26-4º trimestre |
| Set de 2026 | 03-set-2026 | 17-set-2026 | 2026.09 | 2026.10 | 26-4º trimestre |
| Out de 2026 | 01-out-2026 | 15-out-2026 | 2026.10 | 2026.10 | 26-4º trimestre |
| Nov de 2026 | 29-out-2026 | 12-nov-2026 | 2026.11 | 2027.01 | 27-1º trimestre |
| Dez de 2026 | 26-nov-2026 | 10-dez-2026 | 2026.12 | 2027.01 | 27-1º trimestre |
| Janeiro de 2027 | 05-jan-2027 | 14-jan-2027 | 2027.01 | 2027.01 | 27-1º trimestre |

Observações sobre o uso desta tabela:

- **Visualização Final** é a última data em que os recursos podem aparecer na Visualização daquela versão mensal — use-a para o marcador &quot;última data em que os recursos podem aparecer no ambiente de Visualização&quot; da página de visão geral (somente mês de término do trimestre).
- **Produção** é a data oficial de produção para todos para essa versão mensal.
- Para o mês de término do trimestre (aquele que corresponde à coluna Lançamento trimestral), a tabela de agendamento da página de visão geral lista a versão desse mês **duas vezes**: uma vez na coluna &quot;Lançamento mensal&quot; com a data **um dia antes** da data de Produção (a data de lançamento rápido), e uma vez na coluna &quot;Lançamento trimestral&quot; com a data de Produção real. Os meses não finais em um trimestre usam a mesma data de produção tanto na lista mensal quanto em qualquer referência de &quot;lançamento rápido&quot; — não é necessário nenhum ajuste.
- Esta tabela só vai até janeiro de 2027. Quando forem necessárias datas posteriores, peça ao usuário uma atualização do calendário, em vez de adivinhar.

A liberação trimestral da produção normalmente chega à quinta-feira da segunda semana completa do último mês do trimestre.

## Lista de verificação de validação

Ao revisar um arquivo de notas de versão, verifique:

- [ ] O Frontmatter tem todos os campos obrigatórios com valores corretos
- [ ] H1 corresponde ao formato de tipo de página
- [ ] O link de visão geral aponta para o trimestre correto
- [ ] Cada recurso tem um bloco de datas `>[!NOTE]` (páginas de área do produto)
- [ ] Formato de data consistente (`Month Day, Year`)
- [ ] As linhas da tabela de recursos na visão geral correspondem ao conteúdo da página da área de produto
- [ ] Não há links internos corrompidos
- [ ] Links de âncora na visão geral correspondem às IDs de seção H3
- [ Os recursos do ] são ordenados mais recentemente (tanto páginas de área de produtos quanto tabelas de visão geral)
- [ ] As novas páginas de notas de versão estão listadas em `help/quicksilver/TOC.md` no trimestre correto, com a primeira visão geral e as áreas de produtos em ordem alfabética (Outras por último)
- [ ] Se uma nova página de visão geral de um trimestre for criada, `help/quicksilver/home.md` a guia &quot;Versão mais recente&quot; e a guia do ano atual apontam para ela

## Recursos adicionais

- Para obter modelos e exemplos completos do HTML, consulte .claude/commands/_release-notes-formatter-reference.md
