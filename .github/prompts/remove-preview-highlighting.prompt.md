---
mode: agent
description: Remova o enquadramento da documentação somente de visualização do Workfront para o GA — visualize os trechos de formatação, class="preview" HTML e as etapas ou seções paralelas na visualização em relação às etapas ou seções em produção.
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '507'
ht-degree: 1%
---

# Remover realce da visualização

Execute este workflow somente quando eu pedir para &quot;remover o realce da visualização&quot; (ou claramente o
mesma intenção). Ele converte instruções/referências criadas por Courtney com tags de visualização
tópicos em conteúdo pronto para GA.

## Escopo

Aplicar somente quando **todos** forem verdadeiros:

1. Eu chamei este workflow.
2. O caminho do arquivo **não** contém `product-announcements` (exclua todo o
tree: notas de versão, beta, anúncios).
3. O arquivo não está listado em **Caminhos excluídos** abaixo.
4. A linha `author:` do frontmatter inclui **`Courtney`** (único ou coautor).
5. O artigo deve incluir, pelo menos, um dos seguintes elementos:
   - Linguagem de ambiente de visualização em prosa de corpo ou parágrafos de trecho reais
     (&quot;informações destacadas&quot;, &quot;Ambiente de pré-visualização&quot;, &quot;ainda não em geral
     disponíveis&quot;, notas de versão rápida) — **não** uma correspondência somente do texto do link em um
     página de índice;
   - Qualquer elemento HTML com `class="preview"` (`<span>`, `<div>`, `<p>`, `<li>`...);
   - Uma variável de trecho de visualização, como `{{highlighted-preview}}` ou
     `{{highlighted-preview-article-level}}`.

Se o escopo não estiver claro, confirme antes de editar.

**TOC / páginas de índice — sempre ignorar** quando o único texto de visualização estiver dentro de um
texto de exibição do link do markdown apontando para outro artigo, e o arquivo não tiver
`class="preview"`, nenhuma variável de trecho e nenhuma tabulação de visualização em prosa
fora de links.

### Caminhos excluídos

Nunca fazer inventário ou editar, a menos que eu substitua explicitamente:

- `help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md`
- `help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-manage-reports.md`

## Fluxo de trabalho necessário (humano no loop)

Não faça edição em massa sem aprovação.

1. **Inventário** — crie uma lista classificada de caminhos dentro do escopo (pesquisa `help/`). Omitir
   `product-announcements`, caminhos excluídos e menções somente a índice/índice.
2. **Início** — pergunta se deve começar com o primeiro artigo (ou com um caminho que eu nomeie).
3. **Por artigo — mostrar primeiro, editar após OK** — ler o arquivo, propor edições como
antes/depois de trechos ou uma comparação focalizada, aguarde a aprovação explícita.
4. **Após cada arquivo** — pergunte se deseja mover para o próximo (ou parar/ignorar).

## Regras de conteúdo (pré-visualizar conteúdo no documento)

Meta: manter o comportamento documentado para Visualização, descartar arquivos obsoletos &quot;em produção&quot;
ramificações e, em seguida, remova rótulos e invólucros somente para visualização.

- **Etapas paralelas**: remova a etapa &quot;em produção&quot;; mantenha a etapa &quot;em visualização&quot;
substância de step, mas reescreva-a para que não seja específica à Pré-visualização. Corrigir numeração. Se
sem paralelo claro, pare e pergunte qual bloco manter.
- **Seções paralelas**: remover a seção de ambiente de produção; substituí-la
com o conteúdo da seção de visualização, neutralize o texto de visualização e remova
  `class="preview"` invólucros.
- **trechos e avisos sobre o início do artigo**: remover boilerplate somente de visualização e
frases cujo único objetivo é a disponibilidade de visualização.
- **`class="preview"`**: remover as marcas de abertura e fechamento, manter o conteúdo interno.
Preservar estrutura de lista/tabela; corrigir listas corrompidas ou espaços em branco perdidos.
- **Seções comentadas (`<!-- … -->`)**: não modifique, a menos que eu explicitamente
diga isso. Se o conteúdo da visualização aparecer somente dentro de comentários, chame-o e peça.
Padrão: deixar comentários inalterados.

## Não

- Executar em `product-announcements` caminhos ou caminhos excluídos.
- Editar automaticamente blocos comentados.
- Remova &quot;Visualização&quot; quando for um nome de produto em contexto não relacionado (por exemplo, Visualização)
Ambiente de sandbox) — pergunte se não tem certeza.
- Alterar `author:` ou o assunto principal não relacionado.
- Ignore a etapa mostrar → aprovar.

## Verificações de qualidade antes de apresentar edições

- Nenhum `class="preview"` restante no escopo acordado.
- Não há cabeçalhos duplicados órfãos ou números de etapa quebrados.
- A introdução lê corretamente para GA (não &quot;apenas na Pré-visualização&quot; para recursos entregues).
