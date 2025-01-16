---
title: Enviar solicitações do Adobe Workfront Planning
description: Depois que alguém compartilhar um link para um formulário de solicitação com você a partir de uma página de tipo de registro no Adobe Workfront Planning, você poderá adicionar uma solicitação para criar registros para o tipo de registro associado ao formulário de solicitação.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 635045c5-17e6-483e-912b-4e9617571137
source-git-commit: 0a65a18678bfc0aa2e080a0a983746040310b079
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 0%

---

# Enviar solicitações do Adobe Workfront Planning para criar registros

<!--update title when there will be more functionality added to the Planning requests, besides creating records-->
<!--take Preview and Prod references out when releasing to Prod all-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Depois que alguém compartilhar um link para um formulário de solicitação com você a partir de uma página de tipo de registro no Adobe Workfront Planning, você poderá adicionar uma solicitação para criar registros para o tipo de registro associado ao formulário de solicitação.

Usuários do Workfront e usuários externos podem enviar solicitações para tipos de registro do Planning e criar registros. <!--double check on the external users-->

Este artigo descreve como você pode enviar uma solicitação para adicionar novos registros a um tipo de registro.

Para obter informações sobre como um gerenciador de espaço de trabalho pode criar um formulário de solicitação e associá-lo a um tipo de registro, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

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
   <p>Licença externa, do Colaborador, do Light ou do Standard</p>
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
   <p>Exibir permissões ou mais altas para um espaço de trabalho, se você for um usuário do Workfront</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Para acessar a área do Planning no Workfront, você deve receber um modelo de layout que inclua a área do Planning no Menu principal. </p>
   <p> No entanto, para enviar solicitações ao Workfront Planning, não é necessário acessar a área Planejamento. </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Para que você possa enviar uma solicitação para um formulário de solicitação do Workfront Planning, é necessário que o seguinte esteja em vigor:

* Deve existir o seguinte no Workfront Planning:

   * Um espaço de trabalho
   * Um tipo de registro associado a um formulário de solicitação. Para obter informações, consulte [Criar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

* O formulário de solicitação deve ser compartilhado com um link para que você possa acessá-lo. Existem os seguintes cenários:

   * Se você tiver uma conta do Workfront, o link foi compartilhado somente com pessoas internas e você tem acesso de contribuir ou superior ao espaço de trabalho. Pessoas fora do Workfront não podem acessar um link compartilhado internamente.
   * Se você não tiver uma conta do Workfront, o link foi compartilhado com pessoas externas. Os usuários do Workfront também podem acessar um link compartilhado com pessoas externas.

* O link para o formulário não deve estar expirado.

## Considerações sobre o envio de solicitações ao Workfront Planning

* É possível acessar um formulário de solicitação para solicitações do Workfront Planning somente a partir de um link específico para o formulário.
* Não é possível editar uma solicitação depois de enviá-la para o Workfront Planning.
* Cada solicitação submetida cria um registro para o tipo de registro associado ao form usado se o form não estiver associado a uma aprovação ou se a aprovação tiver sido concedida por todos os aprovadores.
* Os registros criados enviando formulários de solicitação não podem ser diferenciados dos registros adicionados por qualquer outro método. Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).
* As solicitações enviadas são exibidas na guia Planejamento da seção Enviado na área Solicitações do Workfront.

<!--Not sure how to change the request status, but dev also said: Changing the names of the statuses might lead to some inconsistency between unified-approvals-service and intake-approvals-flow.-->


## Enviar uma solicitação ao Workfront Planning

1. Acesse o link compartilhado com você a partir de um tipo de registro do Workfront Planning.

1. Atualize os campos disponíveis no formulário. Os campos com um asterisco são obrigatórios.

   >[!TIP]
   >
   >   Se o campo **Assunto** estiver disponível, ele não estará visível no Workfront Planning após o envio da solicitação.
   >
   >Recomendamos que você atualize o máximo possível de campos em sua solicitação para tornar o novo registro identificável quando ele for adicionado ao tipo de registro no Workfront Planning.

1. Clique em **Enviar**.

   Seu formulário é enviado e os seguintes itens ocorrem:

   * Se o formulário de solicitação não foi associado a uma aprovação, a solicitação é adicionada à guia Planejamento da seção Enviado da área Solicitações do Workfront e um novo registro é adicionado ao tipo de registro associado ao formulário.

   * Se o formulário de solicitação foi associado a uma aprovação, a solicitação é adicionada à guia Planejamento da seção Enviado da área Solicitações do Workfront. Um novo registro é adicionado à página de tipo de registro somente após ser aprovado por todos os aprovadores.

     Para obter informações, consulte [Adicionar uma aprovação a um formulário de solicitação](/help/quicksilver/planning/requests/add-approval-to-request-form.md).

     ![](assets/planning-tab-in-requests.png)

     >[!IMPORTANT]
     >
     >Todos os usuários com acesso a pelo menos um espaço de trabalho podem exibir a guia Planejamento na área Solicitações. Você pode exibir somente as solicitações submetidas por você ou por qualquer outra pessoa aos espaços de trabalho para os quais você tem pelo menos permissões. Os administradores do Workfront podem exibir todas as solicitações enviadas para qualquer espaço de trabalho no sistema. <!--ensure this is correct; asking team in slack-->

   * Você recebe uma notificação no aplicativo e uma notificação por email informando que a solicitação foi enviada com êxito ou para revisão.
   * Se o formulário de solicitação foi associado a uma aprovação, os aprovadores recebem uma notificação no aplicativo e uma notificação por email para revisar e aprovar a solicitação.

     >[!NOTE]
     >
     >As notificações por email e no aplicativo ficam visíveis somente quando a instância da Workfront de sua organização é integrada à Experiência unificada do Adobe.




