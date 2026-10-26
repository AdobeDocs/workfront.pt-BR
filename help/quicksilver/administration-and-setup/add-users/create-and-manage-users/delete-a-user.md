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
TQID: 'https://experienceleague.adobe.com/T5iSq2SOJEQrlvLNiQ5l69OncRMYvEs4uf6QosY9vq8'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
    internal-label: Troubleshooting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 6275fff5d615a8db678f16d99c38c96319a57155
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 9%
---
# Excluir usuários

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplicava apenas a organizações que não tinham sido integradas no Admin Console. Como sua organização foi integrada à Adobe Admin Console, você deve executar essa ação por meio da Adobe Admin Console.
>
>  Para obter instruções sobre como excluir um usuário na Adobe Admin Console, consulte a seção &quot;Excluir usuários permanentemente&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/br/enterprise/using/manage-users-individually.html) ou entre em contato com o administrador do Adobe Admin Console.

Quando um usuário deixa a organização, você pode removê-lo do Adobe Workfront.

A exclusão de um usuário deve ser realizada por meio da Adobe Admin Console. Para obter instruções, consulte a seção &quot;Excluir usuários permanentemente&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/br/enterprise/using/manage-users-individually.html) ou entre em contato com o administrador do Adobe Admin Console.

>[!IMPORTANT]
>
>A exclusão de um usuário do sistema também exclui as informações associadas ao usuário que você pode querer manter. Recomendamos desativar os usuários em vez de excluí-los. Para obter mais informações, consulte [Desativar ou reativar um usuário](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <td><p>Padrão</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador na Adobe Admin Console.</p> 
    </td> 
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
    >Para saber mais, consulte [Por que não posso acessar um relatório de propriedade de um usuário desativado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) do artigo [Perguntas frequentes sobre relatórios](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md).

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
     >
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


<!--

## Delete one or more users

{{step-1-to-users}}

1. Select at least one user that you want to delete, click the More menu ![More icon](assets/more-icon.png), then click **Delete**.
1. In the box that appears, click **Delete** to confirm the deletion.

   The process of deleting users runs as a background process, so you can continue using Workfront as the user or users are deleted.

   Depending on the number of users you are deleting, the process can take several minutes or even a few hours.

   After receiving the confirmation in Workfront that the users were deleted, you might continue to see them in the system until the deletion process is complete in the background.

   At a later time, if you discover that one or more users were not successfully deleted, try to delete them one at a time.

   -->
