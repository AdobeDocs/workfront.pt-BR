---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurar o backlog em uma placa de workflow
description: Você pode optar por exibir uma coluna de backlog em um quadro em um workflow e definir uma consulta para os cartões que são extraídos para o backlog do quadro a partir da lista de cartões de workflow.
author: Courtney
feature: Agile
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/ECCX25ZQGtYXBdo8Xkds3OjtFUjoWGXIr9lOOiwwCe8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 10%
---
# Configurar a lista de pendências em um quadro de fluxo de trabalho

>[!IMPORTANT]
>
>Os fluxos de trabalho só estão disponíveis para um grupo específico de clientes.

Você pode optar por exibir uma coluna de backlog em um quadro em um workflow e definir uma consulta para os cartões que são extraídos para o backlog do quadro a partir da lista de cartões de workflow.

>[!NOTE]
>
>Se você adicionar um novo cartão na coluna de backlog que não corresponda aos critérios de consulta, o cartão desaparecerá do backlog quando o quadro for atualizado e só estará disponível na lista de cartões. Você pode alterar a consulta a qualquer momento para ajustar quais cartões aparecem na coluna de backlog.

A coluna de backlog e o query não estão disponíveis em quadros independentes. Para obter informações sobre como adicionar uma coluna de entrada a um quadro independente, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar a lista de pendências em um quadro de fluxo de trabalho

{{step1-to-boards}}

1. Abra o fluxo de trabalho no qual deseja trabalhar. Para abrir um fluxo de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Clique em qualquer quadro no fluxo de trabalho para abri-lo.
1. Clique em [!UICONTROL **Configurar**] à direita do quadro para abrir o painel Configurar.
1. Ativar [!UICONTROL **Incluir uma coluna de lista de pendências neste quadro**].

   A coluna de backlog é adicionada à esquerda do quadro. Permanece em branco até que você aplique uma consulta a ele.

1. Expandir [!UICONTROL **Consulta de lista de pendências**].

   >[!NOTE]
   >
   >Uma consulta padrão pode já ter sido aplicada ao backlog, mostrando todos os itens de trabalho da lista de cartões que têm um status e o status não é Concluído.

1. Clique em [!UICONTROL **Adicionar condição**] e clique no campo &quot;vazio&quot;.
1. Selecione o campo para consultar.

   Os campos que você pode escolher são os campos padrão em um cartão.

1. Selecione o modificador de consulta.

   As opções do modificador dependem dos campos aos quais podem ser aplicadas. Por exemplo, o campo &quot;nome&quot; não tem &quot;maior que&quot; ou &quot;menor que&quot; como opções do modificador, pois esses modificadores se aplicam apenas a números.

1. Selecione o valor.

   O valor não está disponível quando você usa &quot;existe&quot; ou &quot;não existe&quot; como modificador.

   Por exemplo, se você escolher &quot;Data de vencimento&quot; e &quot;existe&quot;, o backlog exibirá cartões com datas de vencimento atribuídas. Qualquer cartão sem data de vencimento não será extraído para o backlog.

1. (Opcional) Clique em [!UICONTROL **Adicionar condição**] para adicionar outra condição à consulta.

   ![Consulta de lista de pendências](assets/backlog-query-wrkstrm-board.png)

1. (Opcional) Clique em [!UICONTROL **Criar grupo**] para adicionar um grupo de condições conectadas à primeira condição com um operador OR.
1. Clique em [!UICONTROL **Salvar consulta**].

   A consulta é aplicada e os cartões que atendem aos critérios aparecem na coluna de backlog.
