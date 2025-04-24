---
title: Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning
description: Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: f171db8474df703fddbf63a673f9bfbd2ab2db27
workflow-type: tm+mt
source-wordcount: '772'
ht-degree: 1%

---

# Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.

Este artigo descreve como um gerente de espaço de trabalho pode adicionar uma aprovação a um formulário de solicitação associado a um tipo de registro.

Para obter informações sobre como criar um formulário de solicitação no Workfront Planning, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Para obter informações sobre como enviar uma solicitação a um tipo de registro para criar um registro, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

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
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p>
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
   <li><p>Gerenciar permissões para um espaço de trabalho <span class="preview">e tipo de registro</span></p></li>
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

<!--replace the layout template info in the table with this at release: 


<p>In the Production environment, all users including the System Administrators must be assigned to a layout template that includes the Planning areas.</p>
<p><span class="preview">In the Preview environment, Standard users and System Administrators have the Planning area enabled by default.</span></p>

-->

## Considerações sobre a adição de aprovações a um formulário de solicitação

* Você pode adicionar um ou vários aprovadores a um formulário de solicitação. Você pode adicionar somente usuários como aprovadores.
* Quando você adiciona vários aprovadores a um formulário de solicitação, todos os aprovadores devem aceitar a solicitação antes que um registro seja criado no Workfront Planning.
* Se todos os aprovadores aprovarem a solicitação, um registro será criado para o tipo de registro associado ao formulário de solicitação.
* Se pelo menos um aprovador rejeitar a solicitação e todos os outros aprovarem, uma solicitação será criada para a área Solicitações no Workfront, mas nenhum registro será criado para o tipo de registro associado ao formulário de solicitação.
* Adicionar aprovações a um formulário de solicitação é opcional. O Workfront Planning cria imediatamente um registro quando uma solicitação é submetida, se o form de solicitação não estiver associado a uma aprovação.

## Adicionar uma aprovação a um formulário de solicitação

1. Comece a criar um formulário de solicitação para um tipo de registro, conforme descrito em [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Clique em **Configuração**.

   A área **Configuração** é exibida.

   ![Guia Configuração](assets/configuration-tab.png)
1. No campo **Aprovadores**, clique no ícone suspenso e selecione um ou vários nomes na lista

   Ou

   Comece a digitar o nome de um aprovador e, em seguida, selecione-o quando ele for exibido na lista.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Você pode adicionar um ou vários aprovadores a um formulário de solicitação.
   >
   >* Se você adicionar mais de um aprovador, todos os aprovadores deverão aprovar a solicitação antes que o Workfront Planning crie um registro.
   >
   >* Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o registro não será criado. A solicitação permanece na guia Planejamento da seção Enviado na área Solicitações do Workfront.
   >
   >* Todos os aprovadores devem tomar uma decisão antes que uma solicitação seja aprovada ou rejeitada.


1. (Opcional) Clique em **Publicar** se você nunca compartilhou o formulário de solicitação antes

   Ou

   Clique em **Compartilhar** para compartilhar o formulário e em **Copiar link**.
1. (Opcional) Depois que um usuário usa o link compartilhado e envia uma solicitação, o Workfront Planning envia uma notificação de aprovação no aplicativo e um email aos aprovadores.

   >[!NOTE]
   >
   >   A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para que os usuários possam receber notificações por email e no aplicativo.


   Para obter informações sobre aprovação de solicitações, consulte [Aprovar uma solicitação](/help/quicksilver/planning/requests/approve-request.md).
