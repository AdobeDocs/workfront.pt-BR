---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Alterar a ordem das histórias no quadro Scrum
description: A ordem em que as matérias aparecem no storyboard não indica prioridade. No entanto, isso pode afetar a prioridade percebida, tornando as histórias mais visíveis. Por padrão, as matérias são exibidas em ordem alfabética dentro de cada [!UICONTROL status] coluna no storyboard.
author: Courtney
feature: Agile
exl-id: 326d78e0-06de-4b98-8fa6-102e0fd89d76
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/Vy3r2L1yuMPvMesRxEohYAgA6geAlKYIRsstLp1kpt8'
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
source-wordcount: '402'
ht-degree: 9%
---
# Altere a ordem das histórias no quadro [!UICONTROL Scrum]

A ordem em que as matérias aparecem no storyboard não indica prioridade. No entanto, isso pode afetar a prioridade percebida, tornando as histórias mais visíveis. A prioridade é definida no backlog e, quando as matérias são trazidas para o storyboard, elas não têm uma prioridade definida porque serão trabalhadas durante o período de iteração. Se as histórias forem retornadas ao backlog, você poderá reordená-las lá para mostrar a prioridade.

Por padrão, as matérias são exibidas em ordem alfabética dentro de cada coluna de status no storyboard. Histórias com raias são exibidas no topo do storyboard, e histórias sem raias são exibidas separadamente abaixo de qualquer raia.

Quando você reordena colunas no storyboard, todas as alterações feitas são salvas na iteração ou no projeto, de modo que as alterações são mantidas na próxima vez que você ou outro usuário visualizar o storyboard. (As alterações feitas não são revertidas ao limpar o cache do navegador.)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

Você deve ter o seguinte acesso para realizar as etapas descritas neste artigo:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p> 
   ou
   <p>Atual: [!UICONTROL Trabalho] ou superior</p> </td> 
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Alterar a ordem da história em uma iteração

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. Vá para a iteração ou projeto que contém as histórias que você deseja reordenar.
1. Arraste um storyboard ou uma raia para o local vertical desejado em uma coluna de status no storyboard.

## Alterar a ordem da história em um projeto

Diferentemente das iterações Agile, não é possível alterar a ordem da história ao visualizar um projeto em uma visualização Agile. Para modificar a ordem da matéria de um projeto, é necessário exibir o projeto em uma exibição padrão.

Para obter informações sobre como alterar a exibição de projeto, consulte [[!UICONTROL Gerenciar um projeto] na [!UICONTROL Exibição Agile]](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md). Em vez de selecionar uma visualização Agile, selecione uma visualização padrão.
