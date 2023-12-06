---
title: Excluir usuários
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Quando um usuário deixa a organização, o pode remover esse usuário do Workfront, embora recomendemos desativar os usuários em vez de excluí-los.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: da57dea3-082b-4a86-ae13-5bf55401122e
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '926'
ht-degree: 0%

---

# Excluir usuários

Quando um usuário deixa a organização, você pode removê-lo do Adobe Workfront.

>[!IMPORTANT]
>
>* A exclusão de um usuário do sistema também exclui as informações associadas ao usuário que você pode querer manter. Recomendamos desativar os usuários em vez de excluí-los. Para obter mais informações, consulte [Desativar ou reativar um usuário](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).
>* O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Excluir um usuário do [!DNL Adobe Admin Console] desativa o usuário no [!DNL Workfront], mas não os exclui de [!DNL Workfront].
>
>  Para obter instruções sobre como excluir um usuário na Adobe Admin Console, consulte a seção &quot;Excluir usuários permanentemente&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou entre em contato com o administrador do Adobe Admin Console.
>
>  Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
>

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. Para obter informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>. </p> </li> 
     <li> <p><b>Usuários</b> no seu nível de acesso configurado para <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador de Usuários</b> opções ativadas em <b>Ajuste as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se o usuário <b>Administrador (Usuários de grupo)</b> estiver ativado, você deve ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> <p>Para obter mais informações sobre o <b>Usuários</b> em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Excluir vs. desativar um usuário

A desativação de um usuário faz com que as seguintes coisas aconteçam:

* Remove as licenças do usuário para o Workfront e o Workfront Proof se o componente do Workfront Proof estiver associado à sua conta do Workfront. Para obter mais informações sobre o Workfront Proof, consulte [Workfront Proof: índice do artigo](../../../workfront-proof/workfront-proof.md).
* O usuário não pode mais receber trabalho.
* O usuário não pode mais ser adicionado às atualizações.
* O usuário não pode mais ser adicionado a equipes ou grupos.
* Os objetos não podem mais ser compartilhados com o usuário.
* Sua associação com os seguintes objetos permanece intacta:

   * Tarefas, problemas, projetos, portfólios
   * Painéis de Controle

     >[!NOTE]
     >
     >Se você desativar um usuário e não puder mais exibir os relatórios ou painéis associados a um usuário, talvez seja necessário atualizar o **Executar este relatório com direitos de acesso de:** campo.\
     >Para saber mais, consulte a [Por que não posso acessar um relatório de propriedade de um usuário desativado?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#why) seção do [Perguntas frequentes sobre relatórios](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artigo.

   * Documentos
   * Atualizações
   * Horas

* Se o usuário tiver feito check-out de documentos, eles permanecerão com check-out quando você os desativar. Somente um administrador do Workfront pode fazer o check-in deles novamente. Para obter mais informações sobre como fazer check-out de documentos, consulte [Fazer check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

Excluir um usuário faz com que as seguintes coisas aconteçam:

* Remove as licenças do usuário para o Workfront e o Workfront Proof, se o componente do Workfront Proof estiver associado à sua conta do Workfront. Para obter mais informações sobre o Workfront Proof, consulte [Workfront Proof: índice do artigo](../../../workfront-proof/workfront-proof.md).
* O usuário não pode mais receber trabalho.
* O usuário não pode mais ser adicionado às atualizações.
* O usuário não pode mais ser adicionado a equipes ou grupos.
* Os objetos não podem mais ser compartilhados com o usuário.
* Exclui a associação desse usuário com os seguintes objetos:

   * Tarefas, problemas, projetos, portfólio
   * Painéis de Controle

     >[!NOTE]
     >
     >Você também perde o acesso às seções personalizadas que continham painéis associados ao usuário excluído.\
     >Para saber mais, consulte a [Como faço para acessar um painel que contém um relatório de propriedade de um usuário excluído?](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md#how) seção do [Perguntas frequentes sobre relatórios](../../../reports-and-dashboards/reports/tips-tricks-and-troubleshooting/reports-faq.md) artigo.

   * Atualizações
   * Horas

     >[!NOTE]
     >
     >Esses objetos permanecem no Workfront, mas o proprietário do objeto agora está em branco.

* Se o usuário tiver carregado algum documento na área Documentos na Barra de navegação global, os documentos também serão excluídos.
* Se o usuário tiver feito check-out dos documentos que possui e os documentos forem carregados na área Documentos principal (acessada no Menu principal), os documentos serão excluídos com o usuário. Para obter mais informações sobre como fazer check-out de documentos, consulte [Fazer check-out de documentos](../../../documents/managing-documents/check-out-documents.md).

Para obter mais informações sobre como desativar usuários, consulte [Desativar ou reativar um usuário](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

É possível excluir permanentemente os usuários, um de cada vez, ou excluir permanentemente vários usuários simultaneamente. Ao excluir usuários individuais, você deve aguardar a conclusão do processo de exclusão antes de passar para outras atividades no Workfront. O processo de exclusão de vários usuários simultaneamente é executado como um processo em segundo plano, para que você possa continuar usando o Workfront enquanto os usuários são excluídos.

## Excluir um ou mais usuários

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Usuários**.
1. Selecione pelo menos um usuário que deseja excluir e clique no menu Mais ![](assets/more-icon.png)e, em seguida, clique em **Excluir**.
1. Na caixa exibida, clique em **Excluir** para confirmar a exclusão.

   O processo de exclusão de usuários é executado como um processo em segundo plano, para que você possa continuar usando o Workfront como o usuário ou usuários são excluídos.

   Dependendo do número de usuários que você está excluindo, o processo pode levar vários minutos ou até mesmo algumas horas.

   Depois de receber a confirmação no Workfront de que os usuários foram excluídos, você pode continuar vendo-os no sistema até que o processo de exclusão seja concluído em segundo plano.

   Posteriormente, se você descobrir que um ou mais usuários não foram excluídos com êxito, tente excluí-los um de cada vez.
