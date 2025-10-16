---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Excluir Funções
description: É possível excluir funções de trabalho que sua organização não usa mais. Recomendamos que você não exclua funções de trabalho se elas tiverem sido associadas a itens de trabalho no passado. Para manter todas as suas informações históricas sobre atribuições de trabalho, recomendamos desativar funções, em vez de excluí-las quando elas se tornarem obsoletas. Para obter informações sobre como desativar funções, consulte Desativar funções de trabalho.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b0e81d76-5227-4fda-9a58-68fbce3f5b94
source-git-commit: 15063d937a5ba9b5285c66a0987e8deea6cc6d74
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 0%

---

# Excluir funções de trabalho

É possível excluir funções de trabalho que sua organização não usa mais. Recomendamos que você não exclua funções de trabalho se elas tiverem sido associadas a itens de trabalho no passado.

Para manter todas as suas informações históricas sobre atribuições de trabalho, recomendamos desativar funções, em vez de excluí-las quando elas se tornarem obsoletas. Para obter informações sobre como desativar funções, consulte [Desativar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

## Requisitos de acesso

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
   <td>Acesso administrativo a Funções de trabalho</td>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir uma função de trabalho

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved from create and manage job roles)</p>
-->

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Funções de trabalho].**
1. Selecione a função de trabalho que você deseja excluir e clique em **[!UICONTROL Excluir].**
1. Se houver objetos (usuários, tarefas, problemas) atribuídos à função de trabalho, execute um dos seguintes procedimentos:

   * **Substitua a função de trabalho por uma função de trabalho diferente:** Selecione a nova função de trabalho na lista suspensa.

     Quaisquer alocações de recursos atuais e anteriores associadas à função de trabalho excluída são transferidas para a função de trabalho selecionada.

     Os usuários que têm somente uma função de trabalho atribuída a eles são reatribuídos à função de trabalho selecionada; os usuários que têm uma função de trabalho secundária atribuída a eles não são reatribuídos à função de trabalho selecionada.

   * **Excluir a função de trabalho e sua alocação de recursos:** Selecione **[!UICONTROL Nenhum]** na lista suspensa.

     >[!IMPORTANT]
     >
     >A exclusão de uma função de trabalho exclui toda a alocação de recursos atual e passada relacionada a essa função de trabalho para todos os projetos.

     &#x200B;Por exemplo, se uma tarefa ou problema for atribuído somente a essa função de trabalho, a tarefa ou problema será desatribuído após a exclusão da função de trabalho.

1. Clique Em **[!UICONTROL Sim, Exclua-O]**.
