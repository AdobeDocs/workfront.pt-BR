---
title: Aprovar uma solicitação no Adobe Workfront Planning
description: Quando um usuário envia uma solicitação a um formulário de solicitação associado a uma aprovação no Adobe Workfront Planning, os aprovadores recebem uma notificação e um email sobre a aprovação pendente. Eles devem aprovar a solicitação antes que o Workfront Planning crie um objeto.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: aca9b313-3420-43f6-8f6c-dd74888bd120
source-git-commit: 5b1993d49ff675b3bab1d470bc756b987fe19d1c
workflow-type: tm+mt
source-wordcount: '885'
ht-degree: 1%

---

# Aprovar uma solicitação no Adobe Workfront Planning

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Quando um usuário envia uma solicitação a um formulário de solicitação associado a uma aprovação no Adobe Workfront Planning, os aprovadores recebem uma notificação e um email sobre a aprovação pendente. Eles devem aprovar a solicitação antes que o Workfront Planning crie um objeto.

Este artigo descreve como um gerenciador de espaço de trabalho pode aprovar uma solicitação enviada para o Workfront Planning para criar um registro.

Recomendamos que você também veja os seguintes artigos:

* [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)
* [Adicionar uma aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Considerações sobre a aprovação de solicitações

* As solicitações enviadas são exibidas na guia Planejamento da seção Enviado na área Solicitações do Workfront com um dos seguintes status de solicitação:

   * **Revisão pendente**: este status é mostrado quando nenhum dos aprovadores abriu o objeto de solicitação.
   * **Em revisão**: o status de **Revisão pendente** muda para **Em revisão** quando pelo menos um aprovador abre o objeto de solicitação. O status da solicitação permanece **Em revisão** até que todos os aprovadores aprovem a solicitação.
   * **Aprovado**: quando um aprovador aprova o objeto de solicitação, seu status individual torna-se **Aprovado**, mas o status geral do objeto de solicitação permanece **Em revisão** até que todos os aprovadores tenham tomado suas decisões. Quando todos os aprovadores aprovam uma solicitação, o status da solicitação se torna **Aprovado**.
   * **Concluído**: se todos os aprovadores aprovarem o objeto de solicitação, seu status será alterado para **Concluído** ou se a solicitação não precisar de aprovação.
   * **Rejeitada**: se qualquer aprovador rejeitar o objeto de solicitação, o status será **Rejeitada**. Nenhum registro é criado e uma nova solicitação deve ser enviada para criar o registro.

* Você pode exibir informações de aprovação em um registro criado submetendo um formulário de solicitação nos campos Aprovado por e Data de aprovação. Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e qualquer pacote do Planning</p>
Ou
<p>Qualquer pacote de fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Qualquer</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e tipo de registro</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aprovar uma solicitação para criar um registro

Depois que os usuários adicionam solicitações a um formulário de solicitação de tipo de registro associado a uma aprovação, a solicitação é enviada aos aprovadores.

Os aprovadores recebem as seguintes notificações sobre uma solicitação pendente de aprovação:

* Uma notificação no aplicativo
* Uma notificação por email

>[!NOTE]
>
>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para que os usuários possam receber notificações por email e no aplicativo.

Para aprovar uma solicitação:

1. (Condicional) Se você estiver usando a experiência de solicitação herdada no Workfront, abra a solicitação seguindo um destes procedimentos:

   * Se você tiver acesso ao Workfront Planning e puder exibir pelo menos um espaço de trabalho, clique em **Menu Principal** ![Menu principal Pontos](assets/dots-menu.png) no canto superior direito da tela ou no **Menu Principal** ![Menu principal Linhas](assets/lines-menu.png) no canto superior esquerdo, se disponível, clique em **Solicitações** > **Enviadas** > **Planejamento** e clique na solicitação com o status **Revisão pendente** ou **Em revisão**.

     >[!TIP]
     >
     >Se você não tiver acesso ao Workfront Planning ou se não tiver acesso para exibir espaços de trabalho, poderá acessar apenas uma solicitação para aprová-la usando suas notificações por email ou no aplicativo.

   * Clique no ícone da área **Notificações** ![Ícone da área Notificações no Unified Shell](assets/notifications-area-icon-unified-shell.png), no canto superior direito da tela, e clique na notificação sobre uma solicitação pendente de aprovação para abrir a solicitação.
   * Vá para a notificação por email no seu email que notifica você sobre uma solicitação pendente de aprovação e clique em **Abrir solicitação** para abrir a solicitação. <!--add the name of the button here, from the email-->

   A página de solicitação é aberta no modo somente leitura.

   ![Página de solicitação somente leitura no status de revisão](assets/read-only-reqeust-page-in-review-status.png)
1. Se você estiver usando a nova experiência de solicitação no Workfront, clique em **Menu Principal** ![Menu principal Pontos](assets/dots-menu.png) no canto superior direito da tela ou no **Menu Principal** ![Menu principal Linhas](assets/lines-menu.png) no canto superior esquerdo, se disponível, clique em **Solicitações** e clique na solicitação que deseja aprovar com o status de **Revisão pendente** ou **Na revisão**.
1. (Opcional) Clique no ícone **Aprovações** ![Ícone Aprovações](assets/approvals-icon.png) no canto superior direito da solicitação para exibir os aprovadores.
1. Clique em **Revisar e aprovar** e escolha uma das seguintes opções:

   * **Aprovar**: aprova a solicitação. Um registro é criado imediatamente para o tipo de registro associado ao formulário de solicitação depois que todos os aprovadores aprovam a solicitação.
   * **Rejeitar**: rejeita a solicitação, mesmo quando você é o único aprovador que a rejeita. Nenhum registro é criado para o tipo de registro associado ao formulário de solicitação.

   O usuário que enviou a solicitação recebe notificações por email e por aplicativo quando a solicitação é aprovada ou rejeitada.

   O status da solicitação muda para o seguinte, dependendo da decisão de aprovação:

   * **Concluída**: a solicitação foi aprovada.
   * **Rejeitada**: a solicitação foi rejeitada.

   A solicitação permanece na guia Planejamento da seção Enviado na área Solicitações do Workfront.
