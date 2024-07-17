---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personalizar tipos de problemas padrão
description: Você pode personalizar os rótulos para cada tipo de problema padrão para melhor corresponder à terminologia usada em sua organização. Os tipos de problemas são úteis para personalizar status de problemas e criar filas de solicitações.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Personalizar tipos de problemas padrão

Os tipos de problemas são úteis nas seguintes circunstâncias:

* Ao personalizar status de problemas, conforme descrito em [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Ao criar uma fila de solicitações, conforme descrito em [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Você pode personalizar os rótulos para cada tipo de problema padrão para melhor corresponder à terminologia usada em sua organização.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront].</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de problema padrão

Se você tiver acesso de [!DNL Adobe Workfront] [!UICONTROL administrador], há quatro tipos de problemas padrão que você pode configurar e renomear:

* **[!UICONTROL Relatório de erros]** Usado para rastrear erros relatados no sistema.
* **[!UICONTROL Pedido de alteração]** Usado para rastrear problemas que precisam ser atualizados ou revisados.
* **[!UICONTROL Problema]** Um objeto em [!DNL Workfront] que comunica trabalho não planejado, um problema que ocorre ou algo que deve ser resolvido para que uma tarefa possa continuar.
* **[!UICONTROL Solicitação]** um tipo de problema que se aplica a uma fila de solicitações em que os usuários fazem solicitações no Workfront.

![](assets/default-issue-types.png)

## Personalizar um tipo de problema

Considere o seguinte sobre a personalização de tipos de problemas:

* Você pode modificar o rótulo de um tipo de problema, mas não pode alterar sua função.
* Você não pode criar tipos de problemas adicionais.
* Não é possível alterar os valores de filtro para o nome de um tipo de problema. Portanto, se você criar um filtro em um relatório de problemas, o valor do filtro (chave) não refletirá o nome personalizado do tipo de problema.
* Três status padrão estão associados a cada tipo de problema: [!UICONTROL Novo], [!UICONTROL Em andamento] e [!UICONTROL Fechado]. Você não pode excluir esses status ou removê-los de um tipo de problema, mas pode renomeá-los.
* Você pode reordenar as opções que aparecem no menu suspenso para cada tipo de problema.

Para personalizar um tipo de ocorrência:

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Status]**.

1. Clique na guia **[!UICONTROL Problemas]**.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o tipo de problema que deseja personalizar, clique no ícone ![](assets/edit-icon.png) de [!UICONTROL Editar] que aparece à direita e digite um novo nome para o tipo de problema.

     ![](assets/customize-issue-type.png)

   * Clique em um [!UICONTROL tipo de problema] para listar seus status associados, arraste as alças que aparecem ao passar o mouse sobre elas e solte-as na ordem em que deseja que elas apareçam no menu suspenso **[!UICONTROL Status]** do problema de seus usuários.
