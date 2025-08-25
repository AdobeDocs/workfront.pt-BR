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
source-git-commit: 99113ac4f2ceca6bd50f078916e33cec7f577362
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 3%

---

# Configurar preferências do sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

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
     <tr> 
      <td role="rowheader">Exigir que usuários externos se registrem com uma senha</td> 
      <td> <p>Exige que os usuários externos se registrem antes de poderem visualizar itens no Workfront. Por padrão, essa opção está desativada. Ao habilitar essa opção, as pessoas sem uma conta do Workfront incluídas em determinadas atualizações por seu endereço de email serão solicitadas a criar uma conta antes de poderem exibir o item em que estão incluídas. Isso cria uma conta de usuário externo para eles.</p> <p>Essa opção está desabilitada por padrão.</p> </td> 
     </tr>
<!-- DELETE THIS SECTION MARCH 2026   <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr>  -->
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>URL de Ajuda Personalizada&lt;/td>
    &lt;td>Permite definir um site de ajuda personalizado interno para o ícone de ajuda do Menu Principal ir para. Para obter mais informações, consulte &lt;a href=&quot;/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md&quot;>Configurar um URL de ajuda personalizado&lt;/a>.&lt;/p>&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Os usuários no sistema assumirão como padrão a Nova experiência na Página inicial &lt;/td>
    &lt;td>Permite especificar se os usuários verão a Nova experiência na Página inicial por padrão. Quando habilitado, os usuários verão a Nova experiência inicial por padrão, mas ainda poderão optar por habilitar ou desabilitar a Nova página inicial individualmente. Quando desativados, os usuários não verão o banner que permite alternar para Nova página inicial. No entanto, eles ainda podem navegar até a Nova página inicial digitando manualmente &lt;code>/home/workspaces&lt;/code> no final do URL da instância. Essa configuração é ativada por padrão.&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Habilitar a lista de trabalho de Prioridades &lt;/td>
    &lt;td>Permite optar por habilitar ou desabilitar a experiência da lista de trabalho de Prioridades para seus usuários. Os usuários ainda verão os ícones de Prioridades no Workfront, mas não terão acesso à funcionalidade. Para obter mais informações sobre prioridades, consulte &lt;a href=&quot;/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md&quot;>Introdução às prioridades&lt;/a>.&lt;/td>
    &lt;/tr>
    &lt;tr>
    &lt;td role=&quot;rowheader&quot;>Ambientes de Teste&lt;/td>
    &lt;td>Permite que você acesse os ambientes de teste do Workfront. Para obter mais informações, consulte &lt;a href=&quot;/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md&quot;>O Ambiente de sandbox de visualização do Adobe Workfront&lt;/a>.&lt;/p>&lt;/td>
    &lt;/tbody>
</table>

1. Clique em **Salvar**.

   As alterações salvas aqui afetam a experiência de todos os usuários no Workfront e de qualquer pessoa que interaja com o sistema como um usuário externo.
