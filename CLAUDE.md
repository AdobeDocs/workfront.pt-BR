---
source-git-commit: 44629631cd2d99eadbed5fd81cf33458b13702af
workflow-type: tm+mt
source-wordcount: '705'
ht-degree: 0%

---
# Localizar artigos candidatos antes de criar novos

Quando Courtney traz novos conteúdos para incorporar — um documento de entrada, feedback de clientes ou de PM, uma colagem de transcrição/Slack, capturas de tela com observações, perguntas de suporte — **não proponha criar um novo artigo primeiro.** Pesquise no repositório e exiba os artigos candidatos existentes onde o conteúdo pode caber.

## Fluxo de trabalho necessário

1. **Leia o novo conteúdo primeiro** para identificar o tópico, o público-alvo (administrador vs. usuário final) e os fatos/etapas específicos adicionados.
2. **Pesquise `help/` candidatos** usando grep e localize. Procure por artigos que já abranjam o mesmo recurso, área ou fluxo de trabalho.
3. **Retorne uma lista classificada** de artigos candidatos (normalmente de 3 a 7), cada um com:
   - O caminho do arquivo (caminho de backtick clicável).
   - Uma razão de 1 linha para ser um candidato (em qual seção ele se encaixaria ou por que é a correspondência de tópico mais próxima).
   - Quaisquer limitações (por exemplo, &quot;incompatibilidade de público-alvo — isso é para o usuário final, a entrada é voltada para o administrador&quot;).
4. **Pergunte à Courtney onde colocá-lo** antes de rascunhar ou editar. Explique a pergunta explicitamente, por exemplo, &quot;Em qual dessas perguntas devo elaborar?&quot; ou &quot;Quer que eu encaixe no #2, ou acha que precisa de um artigo?&quot;
5. **Sugira um novo artigo** somente se nenhum artigo existente for adequado e explique por que nenhum dos candidatos trabalha.

Mesmo que o conteúdo &quot;obviamente&quot; pertença a um artigo conhecido, ainda surjam 2-3 alternativas para que Courtney possa confirmar a colocação. Isso captura quase duplicados e locais em que o conteúdo já estava parcialmente coberto.

&#x200B;---

&#x200B;# Propor alterações antes de editar artigos de ajuda

Quando você estiver prestes a editar qualquer artigo de ajuda do `.md` em `help/`, **não edite o arquivo ainda**. Primeiro, mostre o que você planeja alterar e aguarde a aprovação explícita.

Para cada arquivo que você pretende tocar:

1. Nomeie o arquivo (caminho).
2. Mostrar a alteração proposta como um fragmento de diff/snippet — texto antigo e texto novo — com contexto circundante suficiente para ser inequívoco.
3. Indicar sucintamente o motivo (1 frase).
4. Finalize com uma pergunta explícita, por exemplo, &quot;Aplicar essas alterações?&quot; ou &quot;Quer que eu continue?&quot;

Somente depois que Courtney disser sim (ou &quot;ir&quot;, &quot;aplicar&quot;, &quot;fazer&quot; etc.) você deve chamar as ferramentas de edição.

Isso se aplica às edições de **a cada** em um artigo de ajuda `.md` — erros de digitação, correções de links, trocas de palavra única, limpezas de terminologia, novas seções e regravações. Nenhuma exceção, a menos que Courtney diga explicitamente &quot;apenas conserte&quot; ou &quot;não pergunte, apenas edite&quot; na mesma jogada.

Para alterações que abrangem vários artigos: agrupe as diferenças propostas por arquivo em uma única resposta. Se o conjunto for grande, liste os arquivos afetados primeiro com um resumo de uma linha cada, depois mostre as diferenças nos lotes e confirme antes de cada lote.

Isso faz **não** bloquear pesquisa somente leitura (grep, leitura) ou rascunho/exploração no chat (sem gravações de arquivo).

&#x200B;---

&#x200B;# Mensagens de Git commit

Ao redigir ou gerar uma mensagem de confirmação do Git, siga este formato.

## Linha de assunto

- Cerca de **50 caracteres ou menos**.
- Resuma a alteração no **humor imperativo** (por exemplo, &quot;Adicionar...&quot;, &quot;Corrigir...&quot;, &quot;Refatorar...&quot;).

## Corpo

- Deixe uma linha em branco após o assunto antes do corpo da mensagem.
- Quebrar linhas com aproximadamente **72 caracteres**.
- Use **linhas de marcador** para a explicação. Cada marcador deve começar com exatamente um de:
   - **📖** — use quando a alteração **adicionar** algo novo: novos arquivos, novas seções, novos recursos, novos cabeçalhos, novas linhas ou outro conteúdo de greenfield.
   - **✏️** — use quando a alteração **modificar** o trabalho existente: edições em linhas existentes, atualizações em seções existentes, refatores ou alterações no conteúdo atual.

Exemplo:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

&#x200B;---

&#x200B;# Solicitações de pull (PRs)

## Derivação do problema da Jira

- Derive a ID de problema do Jira do **nome da ramificação Git atual** (por exemplo, um segmento correspondente a `FFENT-8796`).
- **Se o nome da ramificação incluir uma ID Jira:** Use essa ID no título da PR e vincule-a em `# Context` → `## Jira`.
- **Se o nome da ramificação não incluir uma ID Jira:** Omita a chave Jira do título da PR. Ainda inclui `## Jira` com exatamente: `No ticket`.

## Título da PR

**Com Jira ID:** `{type}/{JIRA-ID}- {short task description}`
Exemplo: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`

**Sem Jira ID:** `{type}- {short task description}`
Exemplo: `docs- Refresh Object Composite API changelog`

### Tipos de confirmação

- **recurso** — adiciona um novo recurso
- **corrigir** — corrige um erro
- **refator** — reescreve/reestrutura o código sem alterar o comportamento
- **perf** — melhora o desempenho
- **style** — formatação/espaço em branco somente; sem alteração de significado
- **test** — adiciona ou corrige testes
- **documentos** — somente documentação, novo conteúdo adicionado
- **compilação** — ferramentas de compilação, CI, dependências, versão do projeto
- **ops** — infraestrutura, implantação, backup, recuperação
- **tarefa** — diversas (ex.: `.gitignore`)

## Corpo da PR — seções obrigatórias

### `# Summary`
Breve visão geral do que mudou e por quê.

### `# Changes`
Organizado por arquivo. Para cada arquivo tocado, use um cabeçalho de nível 2 com o caminho em acentos graves e, em seguida, marcadores.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.
```

### `# Context`
Sempre inclua uma subseção `## Jira`.

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

Ou se não houver tíquete: `No ticket`
