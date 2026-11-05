---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '769'
ht-degree: 1%
---
# Copilot instructions for workfront.pt-BR

Este repositório contém a documentação em inglês do Adobe Workfront. As regras
abaixo se aplicam a todas as solicitações neste espaço de trabalho. Padrões específicos de tópicos estão em uso
`.github/instructions/*.instructions.md` e carregar automaticamente ao editar
arquivos correspondentes.

## Localizar artigos candidatos antes de criar novos

Quando o novo conteúdo entra em cena, um documento de entrada, feedback de clientes ou de especialistas, um
Colar transcrição/Slack, capturas de tela com anotações ou perguntas de suporte — **não
proponha criar um novo artigo primeiro.** Pesquisar o repositório e o candidato da superfície
artigos existentes onde o conteúdo pode caber.

Fluxo de trabalho necessário:

1. **Leia o novo conteúdo primeiro** para identificar o tópico, o público-alvo (administrador vs. final)
e os fatos ou etapas específicos que adiciona.
2. **Pesquise `help/` por candidatos** usando grep e pesquisa de arquivos. Procure
artigos que já abrangem o mesmo recurso, área ou fluxo de trabalho.
3. **Retorne uma lista classificada** de artigos candidatos (normalmente de 3 a 7), cada um com:
   - O caminho do arquivo (como um link clicável).
   - Um motivo de uma linha para ser um candidato (em qual seção ele se encaixaria ou por quê)
     é a correspondência tópica mais próxima).
   - Quaisquer limitações (por exemplo, &quot;incompatibilidade de público-alvo — trata-se de um usuário final, a entrada é
     administração&quot;).
4. **Pergunte onde colocá-lo** antes de fazer um rascunho ou uma edição. Expressão da pergunta
explicitamente, por exemplo, &quot;Para quais desses eu devo elaborar?&quot; ou &quot;Quer que eu faça
encaixe-o em #2, ou você acha que ele precisa de seu próprio artigo?&quot;
5. **Sugira um novo artigo** somente se nenhum artigo existente for adequado e
explique por que nenhum dos candidatos trabalha.

Mesmo que o conteúdo &quot;obviamente&quot; pertença a um artigo conhecido, ainda apareça 2-3
alternativas para que a colocação possa ser confirmada. Isso captura dados quase duplicados
locais onde o conteúdo já estava parcialmente coberto.

## Propor alterações antes de editar artigos de ajuda

Quando você estiver prestes a editar qualquer artigo de ajuda do `.md` em `help/`, **não edite o arquivo
ainda.** Primeiro, mostre o que você planeja alterar e aguarde a aprovação explícita.

Para cada arquivo que você pretende tocar:

1. Nomeie o arquivo (caminho).
2. Mostrar a alteração proposta como um fragmento de diff/snippet — texto antigo e novo texto —
com contexto circundante suficiente para serem inequívocos.
3. Indicar sucintamente o motivo (uma frase).
4. Termina com uma pergunta explícita, por exemplo &quot;Aplicar as alterações?&quot; ou &quot;Quer que eu faça
continuar?&quot;

Somente após a aprovação explícita (&quot;sim&quot;, &quot;ir&quot;, &quot;aplicar&quot;, &quot;fazer&quot; etc.) você deve
chame as ferramentas de edição.

Isso se aplica à edição de **a cada** em um artigo de ajuda `.md` — erros de digitação, correções de links,
trocas de palavra única, limpeza de terminologia, novas seções e regravações. Não
exceções, a menos que o usuário diga explicitamente &quot;apenas corrija&quot; ou &quot;não pergunte, apenas
editar&quot; no mesmo turno.

Para alterações que abrangem vários artigos, agrupe as diferenças propostas por arquivo em
uma resposta. Se o conjunto for grande, liste os arquivos afetados primeiro com um resumo de uma linha
cada, em seguida, mostrar diferenças em lotes e confirmar antes de cada lote.

Isso faz **não** bloquear pesquisa somente leitura (grep, leitura) ou rascunho/exploração
no chat (nenhum arquivo é gravado).

## Preencher lacunas de forma inteligente

Quando a intenção for clara do contexto, confirme-se com a resposta das práticas recomendadas em vez de
apresentação de menus de opções. Aplicar os padrões de escrita (consulte
`.github/instructions/writing-quality.instructions.md`) proativamente — não aguardar
para ser lembrado de segui-los. Fazer a correspondência do novo texto com o do artigo ao redor
cabeçalhos, terminologia e estrutura. Perguntar somente quando uma ambiguidade genuína
alterar o resultado.

## Mensagens de Git commit

### Linha de assunto

- Cerca de **50 caracteres ou menos**.
- Resuma a alteração no **humor imperativo** (&quot;Adicionar...&quot;, &quot;Corrigir...&quot;, &quot;Refatorar...&quot;).

### Corpo

- Deixe uma linha em branco após o assunto antes do corpo da mensagem.
- Quebrar linhas com aproximadamente **72 caracteres**.
- Use **linhas de marcador** para a explicação. Cada marcador deve começar exatamente com
um de:
  - **📖** — quando a alteração **adiciona** algo novo: novos arquivos, novas seções, novo
    recursos, novos cabeçalhos, linhas novas líquidas ou outro conteúdo greenfield.
  - **✏️** — quando a alteração **modifica** trabalho existente: edita para linhas existentes,
    atualizações em seções existentes, refatores ou alterações no conteúdo atual.

Exemplo:

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```

## Solicitações de pull

### Derivação do problema da Jira

- Derivar a ID de problema do Jira do **nome da ramificação Git atual** (por exemplo, um
segmento correspondente `FFENT-8796`).
- **Se o nome da ramificação incluir uma ID Jira:**, use essa ID no título da PR e no link
em `# Context` → `## Jira`.
- **Se o nome da ramificação não incluir uma Jira ID:** omita a chave Jira da PR
título. Ainda inclui `## Jira` com exatamente `No ticket`.

### Título da PR

- **Com Jira ID:** `{type}/{JIRA-ID}- {short task description}`
  - Exemplo: `feat/FFENT-8001- Add validation for numVariations in OCAPI request`
- **Sem Jira ID:** `{type}- {short task description}`
  - Exemplo: `docs- Refresh Object Composite API changelog`

Tipos de confirmação: **recurso** (novo recurso), **correção** (correção de erro), **refatoração** (reestruturar
sem alteração de comportamento), **perf** (desempenho), **style** (somente formatação),
**teste** (testes), **documentos** (somente documentação, novo conteúdo), **compilação** (build/CI/
dependências), **ops** (infraestrutura/implantação), **chore** (diversos).

### Corpo da PR — seções obrigatórias

- `# Summary` — breve visão geral do que mudou e o porquê.
- `# Changes` — organizado por arquivo. Para cada arquivo tocado, use um cabeçalho de nível 2
com o caminho em acentos graves e, em seguida, marcadores.
- `# Context` — sempre inclua uma subseção `## Jira` com o problema vinculado, ou
  `No ticket`.

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```
