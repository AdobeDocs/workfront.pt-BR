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
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 4%

---

# Criar tipos de despesas personalizados

<!--**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Como administrador do [!DNL Adobe Workfront], você pode criar tipos de despesas personalizados para definir e acompanhar as despesas associadas às suas tarefas e projetos. Despesas são custos não mão de obra que podem ser associados a tarefas ou projetos.

É possível editar ou excluir qualquer tipo de despesa criada. Não é possível excluir ou editar os tipos de despesas [!DNL Workfront] predefinidos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
       <p>[!UICONTROL Plano]</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de despesas padrão

Os tipos de despesas padrão em [!DNL Workfront] que não podem ser excluídos ou editados incluem:

* [!UICONTROL Advertising]
* [!UICONTROL Consultoria]
* [!UICONTROL Entretenimento]
* [!UICONTROL Geral]
* [!UICONTROL Materiais]
* [!UICONTROL Viagem]

## Criar tipos de despesas personalizados

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Tipos de Despesas]**.
1. Clique em **[!UICONTROL Novo tipo de despesa]**.
1. Na caixa de diálogo **[!UICONTROL Novo Tipo de Despesa]**, insira as seguintes informações:

   * **Nome** - Um nome para a despesa.
   * **Descrição** - Uma descrição da despesa.
   * **Unidade Calculada** - Selecione a unidade de medida para o seu tipo de despesa na lista suspensa. As seguintes unidades de medida estão disponíveis:

      * Milha
      * Quilômetro
      * Quilograma
      * Dólar
      * Hour
      * Day
      * Outro - A seleção dessa opção solicita que você nomeie sua unidade de medida e defina a unidade de medida como algo familiar à sua organização.

   * **Taxa** - O preço por unidade. Este é um campo formatado por moeda e representa o custo de cada unidade estabelecida no campo **Unidade Calculada**. A taxa pode conter um valor numérico com até 4 números após a casa decimal. Por exemplo, 1.0375.

1. Clique em **[!UICONTROL Salvar]**.

   O tipo de despesa agora está disponível para que os usuários o associem às suas despesas em projetos e tarefas.

## Modificar tipos de despesas personalizadas

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Tipos de Despesas]**.
1. Selecione o tipo de despesa que você deseja modificar e clique no **[!UICONTROL ícone Editar]** ![ícone Editar](assets/edit-icon.png).

   A caixa de diálogo **[!UICONTROL Editar Tipo de Despesa]** é exibida.

1. Faça as alterações desejadas e clique em **[!UICONTROL Salvar]**.

   O tipo de despesa agora está disponível para que os usuários o associem às suas despesas em projetos e tarefas.

Para obter mais informações sobre como usar as despesas e como elas podem afetar o custo de um projeto, consulte o artigo [Gerenciar despesas do projeto](../../../manage-work/projects/project-finances/manage-project-expenses.md).
