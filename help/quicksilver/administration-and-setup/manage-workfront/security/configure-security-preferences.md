---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar preferências do sistema
description: Como administrador do Adobe Workfront, você pode configurar preferências para seu sistema Workfront, incluindo preferências de segurança.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: cb9a6536c4995080887032aa84539eff040338f8
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 4%

---

# Configurar preferências do sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode configurar preferências para seu sistema Workfront, incluindo:

* Acesso ao Workfront por meio de aplicativos móveis e outros aplicativos integrados
* Regras para incorporar o Workfront em um iframe

As alterações feitas nas preferências do sistema afetam todos os usuários no sistema e a experiência deles no Workfront.

Recomendamos que você configure as preferências do sistema durante a implementação do Workfront e somente ocasionalmente as revise depois disso.

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar as preferências do sistema

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema** > **Preferências**.

1. Selecione qualquer um dos campos a seguir para estabelecer as configurações de sua organização:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Habilitar o processo de lançamento rápido</p> </td> 
      <td>Permite ativar versões mensais do Workfront para sua organização em vez de versões trimestrais.</p><p>Para obter mais informações sobre o processo de lançamento rápido, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">Habilitar ou desabilitar lançamentos rápidos para sua organização</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Permitir a incorporação do Workfront em um iframe</p> </td> 
      <td>Permite incorporar o Workfront em um iframe.<p>Essa opção está desabilitada por padrão.</p><p><b>IMPORTANTE</b>: exibir um aplicativo baseado na Web em um iframe torna o aplicativo susceptível a uma vulnerabilidade de segurança de clickjacking.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir autenticação SAML 2.0 nos suplementos do Office 365</td> 
      <td> <p>Permite incorporar o Workfront em um iframe somente para suplementos do Office 365 quando o Workfront é integrado a uma solução de logon único SAML 2.0. </p> <p>Essa opção está ativada por padrão.</p> <p><b>OBSERVAÇÃO</b>: se você habilitar a opção acima <strong>Permitir incorporação do Workfront em um iframe</strong>, a opção <strong>Permitir autenticação SAML 2.0 nos suplementos do Office 365</strong> será habilitada e esmaecida.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ativar o uso de informações da sessão ao criar URLs de páginas externas</td> 
      <td> <p>Permite que os usuários usem as informações de ID da sessão de um site ao adicionar uma Página externa a um Painel.</p> <p>Essa opção não é segura e está desativada por padrão. Em vez disso, é recomendável usar o OAuth para integrações.</p> <p>Para obter mais informações sobre como adicionar Páginas Externas a um Painel, consulte <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporar uma página da Web externa a um painel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que as pessoas usem os aplicativos móveis da Workfront e o suplemento para o Workfront Outlook</td> 
      <td> <p>Permite que os usuários acessem os aplicativos móveis (Workfront View para iPad e aplicativos de celular) e o aplicativo Workfront Outlook.</p> <p>Essa opção está ativada por padrão. </p> <p>Para obter informações sobre o Modo de Exibição Workfront, consulte <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Usar o Modo de Exibição Adobe Workfront</a>. Para obter mais informações sobre os aplicativos móveis, consulte <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Usar o aplicativo móvel do Adobe Workfront: índice do artigo</a>.</p> <p>Para obter mais informações sobre o plug-in do Outlook, consulte <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configurar Adobe Workfront para Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Colaborar com pessoas sem contas do Workfront usando endereços de email</p> </td> 
      <td>Permite que os usuários do Workfront compartilhem determinados itens com pessoas sem uma conta do Workfront incluindo seu endereço de email em vez do nome. Os usuários podem compartilhar os seguintes itens com usuários externos usando seus endereços de email:
       <ul>
        <li>Documento<br></li>
        <li>Solicitação de documento<br></li>
        <li>Aprovação de documento</li>
        <li>Calendário</li>
       </ul><p>Essa opção está ativada por padrão.</p> <p><b>Importante</b>: o nível de acesso Usuário Externo não estará disponível na sua instância do Workfront se esta opção estiver desabilitada. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Níveis de acesso predefinidos</a>.</p> </td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> -->
     <tr> 
      <td role="rowheader">URL de Ajuda</td> 
      <td>Permite definir um site de ajuda personalizado interno para o ícone de ajuda do Menu principal ir para. Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurar uma URL de ajuda personalizada</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Habilitar a lista de trabalho Prioridades </td> 
      <td>Permite optar por habilitar ou desabilitar a experiência da lista de trabalho de prioridades para seus usuários. Os usuários ainda verão os ícones de Prioridades no Workfront, mas não terão acesso à funcionalidade. Para obter mais informações sobre prioridades, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Introdução às prioridades</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Ativar IA </td> 
      <td>Permite optar por ativar a IA, incluindo o Assistente de IA. <p><b>Observação</b>: sua organização deve atender aos requisitos específicos para habilitar a IA. Para obter mais informações sobre IA, incluindo os requisitos, consulte <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">Visão geral do Assistente de IA</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Preenchimento automático de formulário </td> 
      <td>Permite que você opte por ativar a capacidade de preencher formulários de solicitação automaticamente com base em dados de solicitação anteriores. Para obter mais informações sobre o Preenchimento Automático de Formulário, consulte <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Preencher automaticamente uma solicitação a partir de dados anteriores</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Aceitar o AI Betas </td> 
      <td>Permite optar por ativar os recursos de IA que estão atualmente no Beta. Se você habilitar essa opção, poderá selecionar quais recursos do AI Beta devem ser habilitados. Para obter mais informações sobre cada recurso do AI Beta, clique no ícone de informações ao lado desse recurso.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Ambientes de Teste</td> 
      <td>Permite acessar os ambientes de teste do Workfront. Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">O Ambiente de Sandbox de Visualização do Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

   As alterações salvas aqui afetam a experiência de todos os usuários no Workfront e de qualquer pessoa que interaja com o sistema como um usuário externo.
