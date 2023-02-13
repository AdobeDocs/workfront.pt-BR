---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Criar tipos de despesas personalizadas
description: Como um [!DNL Adobe Workfront] administrador, você pode criar tipos de despesas personalizados para definir e acompanhar as despesas associadas às suas tarefas e projetos. As despesas são custos não relacionados à mão de obra que podem ser associados a tarefas ou projetos.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '438'
ht-degree: 3%

---

# Criar tipos de despesas personalizadas

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como um [!DNL Adobe Workfront] administrador, você pode criar tipos de despesas personalizados para definir e acompanhar as despesas associadas às suas tarefas e projetos. As despesas são custos não relacionados à mão de obra que podem ser associados a tarefas ou projetos.

Você pode editar ou excluir quaisquer tipos de despesas que criar. Não é possível excluir ou editar o [!DNL Workfront] tipos de despesas.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de Despesa Padrão

Os Tipos de Despesa que estão [!DNL Workfront] por padrão, não pode ser excluído ou editado, inclua o seguinte:

* [!UICONTROL Propaganda]
* [!UICONTROL Consultoria]
* [!UICONTROL Entretenimento]
* [!UICONTROL Geral]
* [!UICONTROL Materiais]
* [!UICONTROL Viagens]

## Criar tipos de despesas personalizadas

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].
1. Clique em **[!UICONTROL Tipos de Despesa]**.
1. Clique em **[!UICONTROL Novo Tipo de Despesa]**.
1. No **[!UICONTROL Novo Tipo de Despesa]** , especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Especifique um nome para a despesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Especifique uma descrição para a despesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unidade calculada]</td> 
      <td> <p>Selecione a unidade de medida para o seu tipo de despesa na lista suspensa.</p> <p>Estão disponíveis as seguintes unidades de medida:</p> 
       <ul> 
        <li>Milha</li> 
        <li>Quilômetro</li> 
        <li>Quilograma</li> 
        <li>Dólar</li> 
        <li>Dólar</li> 
        <li>Dia</li> 
        <li>Outro - a seleção dessa opção solicita que você nomeie a unidade de medida e defina a unidade de medida como algo familiar à sua organização.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxa</td> 
      <td> <p>Especifique o preço por unidade. Este é um campo formatado por moeda e representa o custo de cada unidade estabelecida no <strong>[!UICONTROL Unidade calculada]</strong> campo. </p> <p>A taxa pode conter um valor numérico com até 4 números após a casa decimal. Por exemplo, 1.0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar Tipo de Despesa]**.\
   O tipo de despesa agora está disponível para os usuários associá-lo às suas despesas em projetos e tarefas.

## Modificar Tipos de Despesa Personalizados

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront].
1. Clique em **[!UICONTROL Tipos de Despesa]**.
1. Selecione o tipo de despesa que deseja modificar e clique em **[!UICONTROL Editar]**.

   O **[!UICONTROL Editar Tipo de Despesa]** será exibida.

1. Faça as alterações desejadas e clique em **[!UICONTROL Salvar alterações]**.\
   O tipo de despesa agora está disponível para os usuários associá-lo às suas despesas em projetos e tarefas.

Para obter mais informações sobre como usar as despesas e como elas podem afetar o custo de um projeto, consulte o artigo [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
