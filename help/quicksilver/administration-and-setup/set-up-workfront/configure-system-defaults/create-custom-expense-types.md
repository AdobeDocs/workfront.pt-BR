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
source-git-commit: 428e6a9365c793ce5944941ec5368a674c208c78
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 4%

---

# Criar tipos de despesas personalizados

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador do [!DNL Adobe Workfront], você pode criar tipos de despesas personalizados para definir e acompanhar as despesas associadas às suas tarefas e projetos. Despesas são custos não mão de obra que podem ser associados a tarefas ou projetos.

Você pode editar ou excluir todos os tipos de despesas que você criar. Não é possível excluir ou editar os tipos incorporados de [!DNL Workfront] despesas.

## Requisitos de acesso

+++ Expanda para visualização requisitos de acesso do funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td>[!UICONTROL Administrador de sistema]</td>
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Os requisitos de acesso na documentação](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) da Workfront.

+++

## Tipos de despesas padrão

Os tipos [!DNL Workfront] de despesas padrão que não podem ser excluídas ou editadas incluem:

* [!UICONTROL Publicidade]
* [!UICONTROL Consultoria]
* [!UICONTROL Entretenimento]
* [!UICONTROL Geral]
* [!UICONTROL Materiais]
* [!UICONTROL Viagem]

## Criar tipos de despesas personalizados

{{step-1-to-setup}}

1. Clique **[!UICONTROL em Tipos]** de despesas.
1. Clique **[!UICONTROL Novo tipo]** de despesa.
1. **[!UICONTROL Na caixa de diálogo Tipo]** de despesas da Novo, especifique as seguintes informações:

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
        <li>Outro - Selecionar essa opção solicita que você nomeie sua unidade de medida e defina a unidade de medida como algo familiar para sua organização.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxa</td> 
      <td> <p>Especifique o preço por unidade. Este é um campo com formato de moeda e representa o custo de cada unidade estabelecida no campo <strong>[!UICONTROL Unidade Calculada]</strong>. </p> <p>A taxa pode conter um valor numérico com até 4 números após a casa decimal. Por exemplo, 1,0375</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Salvar]**.

   O tipo de despesa agora está disponível para que os usuários o associem às suas despesas em projetos e tarefas.

## Modificar tipos de despesas personalizadas

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Tipos de Despesas]**.
1. Selecione o tipo de despesa que você deseja modificar e clique em **[!UICONTROL Editar]**.

   A caixa de diálogo **[!UICONTROL Editar Tipo de Despesa]** é exibida.

1. Faça as alterações desejadas e clique **[!UICONTROL Salvar]**.

   O tipo de despesa agora está disponível para os usuários associá-lo às suas despesas em projetos e tarefas.

Para obter mais informações sobre como usar despesas e como elas podem afetar o custo de um projeto, consulte o artigo [Gerenciar despesas](../../../manage-work/projects/project-finances/manage-project-expenses.md) do projeto.
