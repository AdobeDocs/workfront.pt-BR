---
title: Excluir uma condição personalizada
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Você pode excluir uma condição personalizada.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Excluir uma condição personalizada

Você poderá excluir uma condição personalizada se ela não for mais necessária.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir uma condição personalizada

{{step-1-to-setup}}

1. Clique em **Preferências do projeto** > **Condições**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Selecione a guia do tipo de objeto (**Projeto**, **Tarefa** ou **Problema**) onde está localizada a condição que você deseja excluir.

1. Passe o cursor do mouse sobre a condição que deseja excluir e clique no ícone **Excluir** ![Excluir](assets/delete.png) que aparece na extremidade direita.
1. Na mensagem de confirmação exibida, clique em **Excluir Condição**.

1. Na caixa **Excluir Condição** exibida, selecione uma nova condição na lista suspensa para todos os projetos que estavam usando a condição que você está excluindo.

   As condições personalizadas só estarão disponíveis na lista suspensa se forem equivalentes à mesma condição interna que aquela que você está excluindo. Por exemplo, se você estiver excluindo uma condição que equivale a Em risco, apenas condições personalizadas que também equivalem a Em risco estarão disponíveis para seleção.

1. Clique em **Excluir Condição**.

>[!NOTE]
>
>Não é possível excluir as condições incorporadas, que são No destino, Em risco e Com problema. Entretanto, é possível alterar os nomes e as cores.

Para obter informações sobre condições personalizadas, consulte [Condições personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
