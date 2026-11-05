---
description: Regras de formatação e validação para notas de versão do Adobe Workfront (visão geral, área de produto, planejamento e páginas de aparência e comportamento).
applyTo: "help/quicksilver/product-announcements/product-releases/**/*.md"
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 0%
---

# Formatador de notas de versão

Estes arquivos são **notas de versão**, não artigos de instruções. **não** aplicar o
padrões gerais de qualidade de escrita aqui. Antes de editar, leia a fonte completa de
verdade, que inclui os modelos e o calendário de lançamento:

- [.cursor/skills/release-notes-formatter/SKILL.md](../../.cursor/skills/release-notes-formatter/SKILL.md)
- [.cursor/skills/release-notes-formatter/reference.md](../../.cursor/skills/release-notes-formatter/reference.md)

## Regra crítica — determinar primeiro o trimestre do doc

> [!IMPORTANT]
> Nunca atribua um recurso a um trimestre-documento usando matemática de trimestre-calendário em seu
> Data de Pré-visualização ou Produção. O trimestre-documento é baseado em qual versão **mensal**
> o recurso é enviado, de acordo com o agrupamento interno de calendário de lançamento do Workfront, que
> é deslocado do trimestre-calendário. Por exemplo, um recurso com uma função
> a data de 13 de agosto de 2026 pertence ao doc-quarter `26-q4`, não `26-q3`. Sempre
> verifique a tabela Calendário de versão 2026 no arquivo de referência antes de
> criar ou editar qualquer arquivo. Se uma Data de produção estiver fora dessa tabela,
> solicite um calendário atualizado em vez de adivinhar.

## Principais regras estruturais

- **Frontmatter**: `feature` deve ser exatamente `Product Announcements`;
  `recommendations` deve ser exatamente `noDisplay, noCatalog`. Nunca inventar um
  `exl-id` — inclua somente se já existir um.
- **Recursos mais recentes primeiro**: a nota de versão mais recente é a primeira H2 após
a introdução (páginas de área de produto) e a linha superior de cada tabela de recursos (visão geral
páginas).
- **Link de visão geral**: as páginas de área de produtos devem ser vinculadas a **o trimestre de cada uma delas**
arquivo de visão geral — um erro comum está vinculado ao trimestre anterior.
- **Balão de data**: cada recurso H2 é seguido por um bloco `>[!NOTE]` com
Pré-visualização/Produção liberação rápida/Produção para todas as datas, correspondendo às
linha de tabela de visão geral. Formatar datas como `Month Day, Year`; usar `TBD` se desconhecido.
- **Nomes de trimestre gravados** em H1s: &quot;Primeiro trimestre&quot;, &quot;Segundo trimestre&quot;, &quot;Terceiro
Quarter&quot;, &quot;Quarto trimestre&quot;.

## Atualizações complementares necessárias ao adicionar páginas

- **Nova página (qualquer)**: adicioná-la a `help/quicksilver/TOC.md` na mesma alteração
(visão geral primeiro, páginas de área de produto em ordem alfabética, outras melhorias por último).
- **Página de visão geral do novo trimestre**: atualize também `help/quicksilver/home.md` —
atualize o link da guia &quot;Versão mais recente&quot; e o link da atividade de planejamento e adicione
o novo trimestre para a guia de lançamentos do ano atual.

Consulte os arquivos SKILL.md e reference.md acima para obter os modelos completos,
convenções de nomenclatura de arquivo, formatos de link e o calendário de lançamento completo.
