---
title: Excluir uma condição personalizada
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Você pode excluir uma condição personalizada.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# Excluir uma condição personalizada

## Requisitos de acesso

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Excluir uma condição personalizada

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Preferências do projeto** > **Condições**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. Selecione a guia do tipo de objeto (**Projeto**, **Tarefa** ou **Problema**) onde está localizada a condição que você deseja excluir.

1. Passe o mouse sobre a condição que deseja excluir e clique no ícone ![](assets/delete.png) de **Excluir**, que aparece na extremidade direita.
1. Na mensagem de confirmação exibida, clique em **Excluir Condição**.

1. Na caixa **Excluir Condição** exibida, selecione uma nova condição na lista suspensa para todos os projetos que estavam usando a condição que você está excluindo.

   As condições personalizadas só estarão disponíveis na lista suspensa se forem equivalentes à mesma condição interna que aquela que você está excluindo. Por exemplo, se você estiver excluindo uma condição que equivale a Em risco, apenas condições personalizadas que também equivalem a Em risco estarão disponíveis para seleção.

1. Clique em **Excluir Condição**.

>[!NOTE]
>
>Não é possível excluir as condições incorporadas, que são No destino, Em risco e Com problema. Entretanto, é possível alterar os nomes e as cores.

Para obter informações sobre condições personalizadas, consulte [Condições personalizadas](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
