---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# Solicitações de pull (PRs)

Quando você rascunhar ou revisar um título ou descrição de solicitação de pull (por exemplo, no GitHub/GitLab ou quando solicitado no bate-papo com o agente), siga estas convenções.

## Derivação do problema da Jira

- **Source da verdade:** Derive a ID de problema Jira do **nome da ramificação Git atual** (por exemplo, um segmento que corresponde ao padrão de chave do seu projeto, como `FFENT-8796`).
- **Se o nome da ramificação incluir uma Jira ID:** Use essa ID no título da PR (veja abaixo) e vincule-a em `# Context` → `## Jira`.
- **Se o nome da ramificação não incluir uma ID Jira:** Trate a PR como não associada a um tíquete. **Omitir** a chave Jira do título da PR (não invente um tíquete). Ainda inclui `# Context` → `## Jira`, com o conteúdo exato: `No ticket` (sem link).

## Título da PR

**Quando o nome da filial incluir uma ID de problema Jira**, inclua **ambos**:

1. A **ID de problema da Jira** (por exemplo, `FFENT-8001`).
2. O **tipo de confirmação** (veja a lista abaixo), usando este padrão:

`{type}/{JIRA-ID}- {short task description}`

Exemplo:

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

Use uma descrição concisa com estilo imperativo após a ID. Corresponder ao padrão de espaçamento mostrado: tipo, barra, tecla Jira com hífen à direita, espaço e a descrição.

**Quando o nome da filial não incluir uma ID de problema Jira**, omita o tíquete do título e use:

`{type}- {short task description}`

Exemplo:

`docs- Refresh Object Composite API changelog`

### Tipos de confirmação aceitáveis (use exatamente esses rótulos antes de `/`)

- **feat** — adiciona um novo recurso. Quando um novo item do sumário é adicionado ou o JIRA é conectado a outro `feat`- rotulado Jira.
- **corrigir** — corrige um erro
- **refator** — reescreve/reestrutura o código sem alterar o comportamento
- **perf** — melhora o desempenho (refatoração especial)
- **style** — formatação/espaço em branco somente; sem alteração de significado. Somente edições
- **test** — adiciona ou corrige testes
- **docs** — Novo conteúdo adicionado. somente documentação
- **compilação** — ferramentas de compilação, IC, dependências, versão do projeto, etc.
- **ops** — infraestrutura, implantação, backup, recuperação etc.
- **tarefa** — diversas (ex.: `.gitignore`)

## Corpo da PR — seções obrigatórias

Usar **exatamente estas seções de nível superior** (cabeçalhos do Markdown):

### 1. `# Summary`

Breve visão geral do **o que** mudou e **por que** (intenção comercial ou técnica).

### 2. `# Changes`

Organizar por **arquivo**. Para cada arquivo tocado, use um cabeçalho de nível 2 com o caminho em acentos graves e, em seguida, marcadores descrevendo edições.

Formato:

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

Sempre inclua uma subseção **Jira** em `# Context`.

**Quando o nome da ramificação incluir uma Jira ID:** Use um link clicável para solucionar o problema (derivar a chave do nome da ramificação).

Formato:

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Substitua a chave e o URL pelo tíquete real. Se vários tíquetes se aplicarem, liste cada um em sua própria linha na mesma subseção.

**Quando o nome da ramificação não incluir uma ID Jira:**, mantenha `## Jira` e use exatamente:

```markdown
# Context

## Jira
No ticket
```

## Exemplo (descrição completa da PR)

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## Exemplo (descrição completa da PR, ramificação sem uma ID Jira)

**Título:** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
