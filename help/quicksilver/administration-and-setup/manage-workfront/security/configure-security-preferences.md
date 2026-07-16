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
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/46D3BBajFk39FP-dMDk0SuSSGM5nYPKas11Bs159R9Y
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: b5ce8718-c3af-4fdb-a1a9-fca32f83a87cid: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: b0dd2c2c448c829b2ce1559ddc87880c9a47a68f
workflow-type: tm+mt
source-wordcount: 1218
ht-degree: 10%

---

# Configurar preferências do sistema

{{preview-fast-release-general}}

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

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
      <td role="rowheader">Permitir que as pessoas usem os aplicativos móveis da Workfront</td> 
      <td> <p>Permite que os usuários acessem os aplicativos móveis (Workfront View para iPad e aplicativos de telefone celular)</p> <p>Essa opção está ativada por padrão. </p> <p>Para obter informações sobre o Modo de Exibição Workfront, consulte <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Usar o Modo de Exibição Adobe Workfront</a>. Para obter mais informações sobre os aplicativos móveis, consulte <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Usar o aplicativo móvel do Adobe Workfront: índice do artigo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Colaborar com pessoas sem contas do Workfront usando endereços de email</p> </td> 
      <td>Permite que os usuários do Workfront compartilhem determinados itens com pessoas sem uma conta do Workfront incluindo seu endereço de email em vez do nome. Os usuários podem compartilhar os seguintes itens com usuários externos usando seus endereços de email:
       <ul>
        <li>Documento<br></li>
        <li>Solicitação de documento<br></li>
        <li>Aprovação de documento</li>
        <li>Calendário</li>
       </ul><p>Essa opção está ativada por padrão.</p> <p><b>IMPORTANTE</b>: o nível de acesso Usuário Externo não estará disponível na sua instância do Workfront se esta opção estiver desabilitada. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Níveis de acesso predefinidos</a>.</p> </td> 
     </tr> 
     <!--
     <tr> 
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
     </tr>
     -->
     <tr> 
      <td role="rowheader">URL de Ajuda</td> 
      <td>Permite definir um site de ajuda personalizado interno para o ícone de ajuda do Menu principal ir para. Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md">Configurar uma URL de ajuda personalizada</a>.</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">Desativar a atualização automática nos níveis de acesso</td> 
      <td>Você pode desativar o processo de atualização automática para os níveis de acesso do Colaborador. Quando esta configuração é marcada, os usuários com licença de colaborador que excederam seu limite de decisão de aprovação devem ser atualizados manualmente para uma nova licença pelo administrador.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Habilitar a lista de trabalho Prioridades </td> 
      <td>Permite optar por habilitar ou desabilitar a experiência da lista de trabalho de prioridades para seus usuários. Os usuários ainda verão os ícones de Prioridades no Workfront, mas não terão acesso à funcionalidade. Para obter mais informações sobre prioridades, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md">Introdução às prioridades</a>.</td> 
     </tr>
     <tr>
      <td>Sempre exigir campos obrigatórios na edição em massa</td>
      <td><p>Permite escolher se força os usuários a inserir informações em campos obrigatórios ao editar objetos em massa.</p> <p>Quando essa opção é selecionada, os campos obrigatórios devem ter valores antes de salvar no modo de edição em massa. Se o campo obrigatório não tiver um valor para pelo menos um objeto selecionado em massa, não será permitido salvar.</p> <p>Quando essa opção não está selecionada, os campos obrigatórios só são aplicados quando um usuário modifica o campo. Se um campo não for modificado, será tratado como opcional e não validado.</p></td>
     </tr>
     <tr> 
      <td role="rowheader">Preferências de armazenamento </td> 
      <td>Nesta seção, você pode ativar as preferências de nuvem do Adobe. Permite optar por habilitar ou desabilitar o armazenamento em nuvem do Adobe para toda a organização ou para grupos específicos. 
      <p>Atualize as seguintes informações:</p>
      <ul><li><b>Padrão</b>: escolher o armazenamento herdado do Workfront ou o armazenamento na nuvem do Adobe</li>
      <li><b>Permitir que os usuários selecionem o provedor de armazenamento</b>: permite que os usuários escolham entre os dois tipos de armazenamento ao criar objetos Workfront.</li>
      <li><b>Aplica-se a</b>: escolha se as configurações padrão se aplicam a toda a organização ou a grupos específicos</li>
      <li><b>Selecionar portfólios para converter em armazenamento na nuvem do Adobe</b>: selecione portfólios que você deseja converter automaticamente do armazenamento herdado do Workfront para o armazenamento na nuvem do Adobe. Os portfólios são convertidos quando você salva as Preferências do sistema.</li></ul>     
    Para obter mais informações sobre o Adobe Cloud Storage, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md">Habilitar o Adobe Cloud Storage para sua organização</a>.</td></tr>
    <tr> 
      <td role="rowheader">Selecionar portfólios para converter no armazenamento em nuvem da Adobe </td> 
      <td>Permite converter portfólios de armazenamento herdados do Workfront existentes em armazenamento na nuvem da Adobe. Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/convert-portfolios-to-acs.md">Converter portfólios herdados para o armazenamento na nuvem da Adobe</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Habilitar IA </td> 
      <td>Ao ativar as configurações na área Preferências de IA, você pode ativar a IA, incluindo o Assistente de IA. <p><b>OBSERVAÇÃO</b>: sua organização deve atender aos requisitos específicos para habilitar a IA. Para obter mais informações sobre IA, incluindo os requisitos, consulte <a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">Visão geral do Assistente de IA</a>.</p></td> 
     </tr>
    <tr> 
      <td role="rowheader">Preenchimento de formulário com IA </td> 
      <td>Permitir que as pessoas usem Preenchimento de formulário com IA para preencher automaticamente um formulário de solicitação. Para obter mais informações, consulte <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-from-prompt-document.md">Usar preenchimento de formulário fornecido pela IA para preencher uma solicitação usando prompts ou documentos</a>.</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">Preenchimento automático inteligente em formulários de solicitação </td> 
      <td>Permite que você opte por ativar a capacidade de preencher formulários de solicitação automaticamente com base em dados de solicitação anteriores. Para obter mais informações sobre o Preenchimento Automático de Formulário, consulte <a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md">Preencher automaticamente uma solicitação a partir de dados anteriores</a>.</td> 
     </tr>
    <tr> 
      <td role="rowheader">Designer do Planning</td> 
      <td>Isso está disponível somente para clientes que compraram um pacote do Workfront Planning. Ativar esta configuração permite que seus usuários criem e editem espaços de trabalho usando o Planning Designer. Para obter informações, consulte <a href="/help/quicksilver/planning/general/planning-ai-designer.md">Introdução ao Adobe Workfront Planning Designer</a>.</td> 
     </tr>
     <tr> 
      <td role="rowheader">Aceitar versões beta da IA </td> 
      <td>Permite optar por ativar os recursos de IA que estão atualmente no Beta. Se você habilitar essa opção, poderá selecionar quais recursos do AI Beta devem ser habilitados. Para obter mais informações sobre cada recurso do AI Beta, clique no ícone de informações ao lado desse recurso.</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Ferramentas MCP somente leitura</span></td> 
      <td><span class="preview">Permite que o servidor MCP do Workfront execute ações de leitura em dados do Workfront — por exemplo, localizar ou listar projetos, tarefas ou outros itens. Essa opção está ativada por padrão.<p>Para obter mais informações sobre o servidor Workfront MCP, consulte <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configurar o servidor Adobe Workfront MCP</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">Gravar ferramentas MCP</span></td> 
      <td><span class="preview">Permite que o servidor MCP do Workfront execute ações de criação, atualização e exclusão em dados do Workfront. Essa opção está desabilitada por padrão.<p>Para obter mais informações sobre o servidor Workfront MCP, consulte <a href="/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md">Configurar o servidor Adobe Workfront MCP</a>.</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader">Ambientes de Teste</td> 
      <td>Permite acessar os ambientes de teste do Workfront. Para mais informações, consulte <a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">O ambiente de sandbox de pré-visualização do Adobe Workfront</a>.</p></td> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

   As alterações salvas aqui afetam a experiência de todos os usuários no Workfront e de qualquer pessoa que interaja com o sistema como um usuário externo.
