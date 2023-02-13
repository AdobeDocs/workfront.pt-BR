---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: Adicionar histórias a uma iteração existente
description: Você pode adicionar histórias a uma iteração de muitas maneiras.
author: Lisa
feature: Agile
exl-id: b016fda1-789a-42b3-9f97-2c61c4ec0917
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Adicionar histórias a uma iteração existente

Você pode adicionar histórias a uma iteração de qualquer uma das seguintes maneiras:

* No backlog após a criação da iteração, conforme descrito no [Mover histórias do backlog para uma iteração ou [!UICONTROL Kanban] quadro](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#moving-stories-from-the-backlog) seção em [Gerenciar o backlog ágil](../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)

* No [!UICONTROL Detalhes] página da tarefa ou problema individual
* A partir de uma lista de tarefas ou problemas
* A partir de um relatório
* Em um painel

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL Worker] ou superior</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Acesso do [!UICONTROL Gerenciar] ao projeto no qual a história está</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Entender como a adição de histórias afeta as datas da tarefa

Por padrão, quando você adiciona uma tarefa existente a uma iteração, o [!UICONTROL Data de início planejada] e [!UICONTROL Data de Conclusão Planejada] são definidos do seguinte modo:

### Tarefa [!UICONTROL Data de início planejada]

* A tarefa usa a Data inicial da iteração quando:

   * O projeto não tem um [!UICONTROL Data de início planejada] definido.
   * O [!UICONTROL Data de início planejada] é *before* ou *on* a data de início da iteração.

* A tarefa usa o [!UICONTROL Data de início planejada] quando:

   * O [!UICONTROL Data de início planejada] é *after* a data de início da iteração.

### Tarefa [!UICONTROL Data de Conclusão Planejada]

* A tarefa usa a Data final da iteração quando:

   * O projeto não tem um [!UICONTROL Data de Conclusão Planejada] definido.
   * O [!UICONTROL Data de início planejada] é *antes ou em* a Data Inicial da iteração ou a [!UICONTROL Data de Conclusão Planejada] é *antes ou em* a Data final da iteração.

* A tarefa usa o [!UICONTROL Data de Conclusão Planejada] quando:

   * O [!UICONTROL Data de início planejada] é *after* a Data de Início da iteração e a [!UICONTROL Data de Conclusão Planejada] é *after* a Data final da iteração.

Você pode configurar equipes individuais do Scrum para usar as datas do projeto por padrão, em vez das datas de iteração. Para obter mais informações, consulte a seção [Configurar como as datas são aplicadas ao adicionar itens de trabalho a uma iteração](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5) no artigo [Configurar Sombra](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md).

## Adicionar uma história a uma iteração existente

Para adicionar histórias a uma iteração diretamente da tarefa ou edição:

>[!IMPORTANT]
>
>Depois que a tarefa for movida para a iteração, você não poderá atualizar a variável [!UICONTROL Tipo de duração] ou [!UICONTROL Restrição de tarefa]. [!UICONTROL Tipo de duração] está definida como [!UICONTROL Simples] e [!UICONTROL Restrição de tarefa] está definida como [!UICONTROL Datas fixas] para manter a linha do tempo da tarefa consistente com a linha do tempo da iteração.

### Na guia Tarefas ou problemas

É possível adicionar qualquer tarefa ou problema a qualquer iteração se você tiver acesso de Gerenciar ao projeto. Lembre-se do seguinte ao mover uma tarefa ou problema para uma iteração:

* Se você adicionar várias equipes, a tarefa ou problema poderá ser exibido somente na iteração de uma equipe. Esta é a iteração escolhida na etapa 3 abaixo.
* Se a tarefa ou o problema for atribuído a uma equipe ágil e movido para a iteração de outra equipe, a atribuição da equipe não será alterada.
* Se a tarefa ou problema não for atribuído a uma equipe, a tarefa ou problema será atribuído à equipe proprietária da iteração.
* Não é possível adicionar tarefas pai à iteração. Se você adicionar qualquer tarefa filho, a tarefa pai aparecerá no Quadro de controle como uma faixa de rodagem.

1. Vá para o projeto, relatório ou painel que contém a tarefa ou problema que deseja adicionar a uma iteração.
1. Selecione uma ou mais tarefas ou problemas.
1. Clique em **[!UICONTROL Mais]** ![](assets/more-icon.png) > **[!UICONTROL Adicionar à iteração]**.\
   Não é possível atribuir tarefas ou problemas atribuídos a equipes não ágil.

1. No **[!UICONTROL Adicionar histórias]** digite o nome da iteração.

   >[!NOTE]
   >
   >Você pode mover uma história de uma iteração existente para uma nova iteração.

1. Se você estiver adicionando tarefas, clique em **[!UICONTROL Adicionar histórias]**.\
   Ou\
   Se você estiver adicionando problemas, clique em **[!UICONTROL Adicionar problemas]**.
