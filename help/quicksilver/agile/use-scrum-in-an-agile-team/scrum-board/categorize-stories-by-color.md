---
product-area: agile-and-teams;projects
navigation-topic: scrum-board
title: Categorizar Histórias por Cor no Quadro Scrum
description: A associação de cores padrão das matérias do quadro Scrum difere dependendo se o storyboard está localizado em uma iteração ou em um projeto.
author: Courtney
feature: Agile
exl-id: 8e351505-73d1-4c8f-b369-53c965b88c95
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/V7-dFcJoGqKbPfdk1luo43ucIZSfKg4JFaziJXRrMFw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 421
ht-degree: 8%

---

# Categorizar histórias por cor no quadro [!UICONTROL Scrum]

## Alterar a associação de cores padrão das matérias

A associação de cores padrão das histórias difere dependendo se o storyboard está localizado em uma iteração ou em um projeto:

* **[!UICONTROL Iteração]**: em uma iteração, os blocos de storyboard são codificados por cores de acordo com o projeto ao qual a história está associada. (Cada projeto recebe arbitrariamente uma cor no storyboard.) É possível alterar esse comportamento padrão para cada equipe Agile. As cores das histórias Agile em uma iteração podem ser vinculadas ao projeto (padrão), prioridade da história, proprietário ou formato livre. Para obter mais informações, consulte [Configurar como os indicadores de cor são usados para histórias no storyboard Agile](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur4) no artigo [Configurar Scrum](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

* **[!UICONTROL Projeto]**: em um projeto, todas as subtarefas correspondem à cor da tarefa pai, de modo que as cores de todas as histórias em qualquer raia sejam as mesmas. As cores são atribuídas aleatoriamente às tarefas quando são criadas se a tarefa não tiver subtarefas ou não tiver uma tarefa pai. Você pode alterar esse comportamento padrão modificando a visualização Agile. As cores das matérias Agile em um projeto podem ser vinculadas à matéria principal (padrão), prioridade da matéria, proprietário ou formato livre. Para obter mais informações, consulte [Criar ou personalizar uma exibição [!UICONTROL Agile]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) na [Visão geral das exibições [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

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

## Alterar a cor das matérias ao usar a forma livre

Se as configurações da Equipe Agile tiverem sido definidas para que a opção [!UICONTROL Associar Cor do Cartão a] seja definida como [!UICONTROL Formato Livre], os usuários poderão alterar manualmente a cor de quadros de matérias individuais. Isso pode ser útil para comunicar outros tipos de informações importantes para a equipe ou a organização:

{{step1-to-team}}

1. (Opcional) Clique no ícone **[!UICONTROL Equipe do Switch]** ![Ícone da equipe do Switch](assets/switch-team-icon.png), em seguida, selecione uma nova equipe do Scrum no menu suspenso ou procure uma equipe na barra de pesquisa.

1. No painel esquerdo, selecione **[!UICONTROL Iterações]** para escolher uma iteração específica, ou selecione **[!UICONTROL Iteração atual]**.
1. Passe o mouse sobre o banner colorido na parte superior do bloco de história.

   ![cartão de história](assets/agile-story-color1-nwe-350x140.png)

1. Clique em **[!UICONTROL Alterar cor]** e selecione a cor desejada.

   ![escolher cor](assets/agile-story-color2-nwe-350x138.png)
