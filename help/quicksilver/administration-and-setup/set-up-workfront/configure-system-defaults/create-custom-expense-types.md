---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Criar Tipos de Despesas Personalizadas
description: Como administrador do  [!DNL Adobe Workfront] , você pode criar tipos de despesas personalizados para definir e acompanhar as despesas associadas às suas tarefas e projetos. Despesas são custos não mão de obra que podem ser associados a tarefas ou projetos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b76b9e8-fbb8-45a7-9e26-1ddc6d5176d8
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 4%

---

# Criar tipos de despesas personalizados

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador do [!DNL Adobe Workfront], você pode criar tipos de despesas personalizados para definir e acompanhar as despesas associadas às suas tarefas e projetos. Despesas são custos não mão de obra que podem ser associados a tarefas ou projetos.

É possível editar ou excluir qualquer tipo de despesa criada. Não é possível excluir ou editar os tipos de despesas [!DNL Workfront] predefinidos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de Despesas Padrão

Os Tipos de Despesas que estão em [!DNL Workfront] por padrão não podem ser excluídos ou editados incluem o seguinte:

* [!UICONTROL Advertising]
* [!UICONTROL Consultoria]
* [!UICONTROL Entretenimento]
* [!UICONTROL Geral]
* [!UICONTROL Materiais]
* [!UICONTROL Viagem]

## Criar tipos de despesas personalizados

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Tipos de Despesas]**.
1. Clique em **[!UICONTROL Novo Tipo de Despesa]**.
1. Na caixa **[!UICONTROL Novo Tipo de Despesa]** que é exibida, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Especifique um nome para a despesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Especifique uma descrição para a despesa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unidade Calculada]</td> 
      <td> <p>Selecione a unidade de medida para seu tipo de despesa na lista suspensa.</p> <p>As seguintes unidades de medida estão disponíveis:</p> 
       <ul> 
        <li>Milha</li> 
        <li>Quilômetro</li> 
        <li>Quilograma</li> 
        <li>Dólar</li> 
        <li>Dólar</li> 
        <li>Dia</li> 
        <li>Outro - A seleção dessa opção solicita que você nomeie sua unidade de medida e defina a unidade de medida como algo familiar à sua organização.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxa</td> 
      <td> <p>Especifique o preço por unidade. Este é um campo com formato de moeda e representa o custo de cada unidade estabelecida no campo <strong>[!UICONTROL Unidade Calculada]</strong>. </p> <p>A taxa pode conter um valor numérico com até 4 números após a casa decimal. Por exemplo, 1,0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar Tipo de Despesa]**.\
   O tipo de despesa agora está disponível para que os usuários o associem às suas despesas em projetos e tarefas.

## Modificar Tipos de Despesas personalizados

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Tipos de Despesas]**.
1. Selecione o tipo de despesa que você deseja modificar e clique em **[!UICONTROL Editar]**.

   A caixa de diálogo **[!UICONTROL Editar Tipo de Despesa]** é exibida.

1. Faça as alterações desejadas e clique em **[!UICONTROL Salvar alterações]**.\
   O tipo de despesa agora está disponível para que os usuários o associem às suas despesas em projetos e tarefas.

Para obter mais informações sobre como usar as despesas e como elas podem afetar o custo de um projeto, consulte o artigo [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
