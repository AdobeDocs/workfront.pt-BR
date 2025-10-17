---
title: Excluir Usuários
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Quando um usuário deixa a organização, o pode remover esse usuário do Workfront, embora recomendemos desativar os usuários em vez de excluí-los.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 1%

---

# Excluir usuários

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas à Adobe Business Platform. Se você foi integrado à Adobe Business Platform, é necessário excluir usuários na Adobe Admin Console.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Business Platform, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Quando um usuário deixa a organização, você pode removê-lo do Adobe Workfront.

>[!IMPORTANT]
>
>A exclusão de um usuário do sistema também exclui as informações associadas ao usuário que você pode querer manter. Recomendamos desativar os usuários em vez de excluí-los. Para obter mais informações, consulte [Desativar ou reativar um usuário](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
<!--
>* The procedure described on this page applies only to organizations that have not yet been onboarded to the Admin Console. If your organization has been onboarded to the Adobe Admin Console, you must perform this action through the Adobe Admin Console.
>
>Deleting a user from the [!DNL Adobe Admin Console] deactivates the user in [!DNL Workfront], but does not delete them from [!DNL Workfront].
>
>  For instructions on deleting a user in the Adobe Admin Console, see the section "Permanently delete users" in the article [Manage users individually](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) or contact your Adobe Admin Console Administrator.
>
>  For a list of procedures that differ based on whether your organization has been onboarded to the Adobe Admin Console, see [Platform-based administration differences (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>
-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. </li> 
     <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir vs. desativar um usuário

A desativação de um usuário faz com que as seguintes coisas aconteçam:

* Remove as licenças do usuário para Workfront e Workfront Proof se o componente do Workfront Proof estiver associado à sua conta do Workfront. Para obter mais informações sobre o Workfront Proof, consulte [Workfront Proof: índice do artigo](../../../workfront-proof/workfront-proof.md).
* O usuário não pode mais receber trabalho.
* O usuário não pode mais ser adicionado às atualizações.
* O usuário não pode mais ser adicionado a equipes ou grupos.
* Os objetos não podem mais ser compartilhados com o usuário.
* Sua associação com os seguintes objetos permanece intacta:

   * Tarefas, problemas, projetos, portfólios
   * Painéis

     >[!NOTE]
     >
     >Se você desativar um usuário e não puder mais exibir os relatórios ou painéis associados a um usuário, talvez seja necessário atualizar o campo **Executar este relatório com os Direitos de Acesso de:**.\
     >Para saber mais, consulte o [Por que não posso acessar um relatório de propriedade de um usuário desativado?Seção &#x200B;](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) do artigo [Perguntas frequentes sobre relatórios](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

   * Documentos
   * Atualizações
   * Horas

* Se o usuário tiver feito check-out de documentos, eles permanecerão com check-out quando você os desativar. Somente um administrador do Workfront pode fazer o check-in deles novamente. Para obter mais informações sobre o check-out de documentos, consulte [Check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

Excluir um usuário faz com que as seguintes coisas aconteçam:

* Remove as licenças do usuário para Workfront e Workfront Proof, se o componente do Workfront Proof estiver associado à sua conta do Workfront. Para obter mais informações sobre o Workfront Proof, consulte [Workfront Proof: índice do artigo](../../../workfront-proof/workfront-proof.md).
* O usuário não pode mais receber trabalho.
* O usuário não pode mais ser adicionado às atualizações.
* O usuário não pode mais ser adicionado a equipes ou grupos.
* Os objetos não podem mais ser compartilhados com o usuário.
* Exclui a associação desse usuário com os seguintes objetos:

   * Tarefas, problemas, projetos, portfólio
   * Painéis

  <!--
     >[!NOTE]
     >
     >You also lose access to custom sections that contained dashboards associated to the deleted user.  
     >To learn more, see the [How do I access a dashboard that contains a report owned by a deleted user?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) section of the [Reports FAQs](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) article.
     -->

   * Atualizações
   * Horas

     >[!NOTE]
     >
     >Esses objetos permanecem no Workfront, mas o proprietário do objeto agora está em branco.

* Se o usuário tiver carregado algum documento na área Documentos na Barra de navegação global, os documentos também serão excluídos.
* Se o usuário tiver feito check-out dos documentos que possui e os documentos forem carregados na área Documentos principal (acessada no Menu principal), os documentos serão excluídos com o usuário. Para obter mais informações sobre o check-out de documentos, consulte [Check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

Para obter mais informações sobre como desativar usuários, consulte [Desativar ou reativar um usuário](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

É possível excluir permanentemente os usuários, um de cada vez, ou excluir permanentemente vários usuários simultaneamente. Ao excluir usuários individuais, você deve aguardar a conclusão do processo de exclusão antes de passar para outras atividades no Workfront. O processo de exclusão de vários usuários simultaneamente é executado como um processo em segundo plano, para que você possa continuar usando o Workfront enquanto os usuários são excluídos.

## Excluir um ou mais usuários

{{step-1-to-users}}

1. Selecione pelo menos um usuário que você deseja excluir, clique no menu Mais ![ícone Mais](assets/more-icon.png) e em **Excluir**.
1. Na caixa exibida, clique em **Excluir** para confirmar a exclusão.

   O processo de exclusão de usuários é executado como um processo em segundo plano, para que você possa continuar usando o Workfront como o usuário ou usuários são excluídos.

   Dependendo do número de usuários que você está excluindo, o processo pode levar vários minutos ou até mesmo algumas horas.

   Depois de receber a confirmação no Workfront de que os usuários foram excluídos, você pode continuar vendo-os no sistema até que o processo de exclusão seja concluído em segundo plano.

   Posteriormente, se você descobrir que um ou mais usuários não foram excluídos com êxito, tente excluí-los um de cada vez.
