---
title: Aprovar uma solicitação
description: Quando um usuário envia uma solicitação a um formulário de solicitação associado a uma aprovação no Adobe Workfront Planning, os aprovadores recebem uma notificação e um email sobre a aprovação pendente. Eles devem aprovar a solicitação antes que o Workfront Planning crie um objeto.
hide: true
hidefromTOC: true
source-git-commit: 8d5006532e93dc687beb79e817b725f18b0c65d3
workflow-type: tm+mt
source-wordcount: '783'
ht-degree: 1%

---


<!--

---
title: Approve a Request
description: When a user submits a request to a request form associated with an approval in Adobe Workfront Planning, approvers receive a notification and an email about the pending approval. They must approve the request before Workfront Planning creates an object. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---

-->


# Aprovar uma solicitação

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!-- do you need to add that only workspace owners can view the Submitted/ Planning tab?? - asking team in slack-->

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Quando um usuário envia uma solicitação a um formulário de solicitação associado a uma aprovação no Adobe Workfront Planning, os aprovadores recebem uma notificação e um email sobre a aprovação pendente. Eles devem aprovar a solicitação antes que o Workfront Planning crie um objeto.

Este artigo descreve como um gerenciador de espaço de trabalho pode aprovar uma solicitação enviada para o Workfront Planning para criar um registro.

Recomendamos que você também veja os seguintes artigos:

* [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)
* [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)
* [Adicionar uma aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md)

## Considerações sobre a aprovação de solicitações e status de solicitação

As solicitações enviadas são exibidas na guia Planejamento da seção Enviado na área Solicitações do Workfront com um dos seguintes status de solicitação:

* **Revisão pendente**: este status é mostrado quando nenhum dos aprovadores abriu o objeto de solicitação.
* **Em revisão**: o status muda para **Em revisão** quando pelo menos um aprovador abre o objeto de solicitação. O status da solicitação permanece **Em revisão** até que todos os aprovadores aprovem a solicitação.
* **Aprovado**: quando um aprovador aprova o objeto de solicitação, seu status individual torna-se
* **Aprovado**, mas o status geral do objeto de solicitação permanece **Em revisão** até que todos os aprovadores tenham tomado suas decisões.
* **Concluído**: se todos os aprovadores aprovarem o objeto de solicitação, seu status será alterado para **Concluído** ou se a solicitação não precisar de aprovação.
* **Rejeitada**: se qualquer aprovador rejeitar o objeto de solicitação, o status será **Rejeitada**.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Produtos</p> </td>
   <td>
   <ul><li><p> Adobe Workfront</p></li>
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td>
  </tr>  
 <tr>
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td>
   <td>
<p>Qualquer um dos seguintes planos da Workfront:</p>
<ul><li>Selecionar</li>
<li>Prime</li>
<li>Ultimate</li></ul>
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p>
   </td>

<tr>
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td>
   <td>
<p>Qualquer </p>  
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </td>

<tr>
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td>
   <td>
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p>
   </td>
  </tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões de objeto</p></td>
   <td>
   <ul>
   <li><p>Gerenciar permissões em um espaço de trabalho</p></li>
    <li><p>Os administradores do sistema podem gerenciar espaços de trabalho que não criaram. </p></li>
    </ul>
   <p>Para obter informações sobre o compartilhamento de permissões para objetos do Workfront Planning, consulte  
   <a href="/help/quicksilver/planning/access/sharing-permissions-overview.md">Visão geral das permissões de compartilhamento no Adobe Workfront Planning</a> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aprovar uma solicitação para criar um registro

Depois que os usuários adicionam solicitações a um formulário de solicitação de tipo de registro associado a uma aprovação, a solicitação é enviada aos aprovadores.

Os aprovadores recebem as seguintes notificações sobre uma solicitação pendente de aprovação:

* Uma notificação no aplicativo
* Uma notificação por email

Para aprovar uma solicitação:

1. Siga um destes procedimentos:

   * Se você tiver acesso ao Workfront Planning, clique em **Menu Principal** ![](assets/dots-menu.png) no canto superior direito da tela ou no **Menu Principal** ![](assets/lines-menu.png) no canto superior esquerdo, se disponível, em seguida, clique em **Solicitações** > **Enviadas** > **Planejamento** e clique na solicitação com o status de **Em revisão**. <!--did they change this to Pending approval; logged  a bug-->

     >[!TIP]
     >
     >    Se você não tiver acesso ao Workfront Planning, poderá acessar apenas uma solicitação para aprová-la usando suas notificações.


   * Vá para a área **Notificações** no canto superior direito da tela e clique na notificação sobre uma solicitação pendente de aprovação para abrir a solicitação.
   * Vá para a notificação por email no seu email que notifica sobre uma solicitação pendente de aprovação e clique em para abrir a solicitação. <!--add the name of the button here, from the email-->

   A página de solicitação é aberta no modo somente leitura.

   ![](assets/read-only-reqeust-page-in-review-status.png)
1. (Opcional) Clique no ícone ![](assets/approvals-icon.png) de **Aprovações** no canto superior direito da solicitação para ver os aprovadores.
1. Clique em **Revisar e aprovar** e escolha uma das seguintes opções: <!--did they fix the button and removed the &??-->

   * **Aprovar**: aprova a solicitação. Um registro é criado imediatamente para o tipo de registro associado ao formulário de solicitação.
   * **Rejeitar**: essa ação rejeita a solicitação. Nenhum registro é criado para o tipo de registro associado ao formulário de solicitação. <!--check to see if there is a notification sent to the requestor about it being rejected OR approved??--> <!--checking with PM what happens with the other approvers when one of them is rejecting it: does it ask them to approve it? Deleted the request? -->