---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

Orientação do agente para o repositório **workfront.en** (Adobe Workfront em inglês
documentação). Esse arquivo aponta para as instruções canônicas para que qualquer agente —
independentemente do arquivo de convenção lido — o segue as mesmas regras.

## Arquivos de instrução canônicos

- **Regras de todo o repositório**: [.github/copilot-instructions.md](.github/copilot-instructions.md)
— pesquisa de artigos candidatos, propor antes da edição, confirmar mensagens e formatos de RP,
e &quot;preencha as lacunas de forma inteligente&quot;.
- **Padrões de escrita** (aplica-se automaticamente a `help/**/*.md`):
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md),
com detalhes completos em
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md).
- **Notas de versão** (aplica-se automaticamente a `product-announcements/product-releases/**`):
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md).
- **Limpeza de realce de visualização** (fluxo de trabalho sob demanda):
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md).

## Comportamentos não negociáveis

1. **Localizar artigos candidatos antes de criar novos.** Quando o novo conteúdo chegar
no, pesquise `help/` e exiba uma lista classificada de artigos existentes que ele pode conter,
em seguida, pergunte a onde ele pertence antes de redigir.
2. **Proponha alterações antes de editar qualquer artigo de ajuda `.md`.** Mostrar o
comparar e aguardar aprovação explícita. A única exceção é quando eu digo &quot;apenas corrigir
it&quot; ou &quot;don&#39;t ask, just edit&quot; na mesma jogada. Pesquisa somente leitura e bate-papo
a redação está sempre boa.
3. **Preencha as lacunas de forma inteligente.** Quando a intenção estiver clara, confirme com a
resposta de práticas recomendadas e correspondência dos cabeçalhos do artigo ao redor,
terminologia e estrutura em vez de apresentar menus de opções.
4. **Aplicar os padrões de gravação de forma proativa** em cada edição de `help/` — não aguarde
para ser lembrado.

## Convenções de confirmação e PR

Consulte [.github/copilot-instructions.md](.github/copilot-instructions.md) para obter informações completas
formato de mensagem de confirmação (assunto imperativo ≤ ~50 caracteres; 📖 para adições, ✏️ para
modificações) e estrutura de PR (ID Jira do nome da ramificação; `# Summary`,
`# Changes` por arquivo, `# Context` → `## Jira`).
