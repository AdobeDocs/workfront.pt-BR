---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: Configurar preferências de segurança do sistema
description: Como administrador do Adobe Workfront, você pode configurar as preferências de segurança do seu sistema Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 9ebcbf43d4cf84d1f68aeff7e443f41193a9fe76
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 5%

---

# Configurar preferências do sistema

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode configurar preferências para seu sistema Workfront:

* Acesso ao Workfront por meio de aplicativos móveis e outros aplicativos integrados
* Regras para incorporar o Workfront em um iframe

As alterações feitas nas preferências do sistema afetam todos os usuários no sistema e a experiência deles no Workfront.

Recomendamos que você configure as preferências do sistema durante a implementação do Workfront e somente ocasionalmente as revise depois disso.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar as preferências do sistema

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Sistema** > **Preferências**.

1. Selecione qualquer um dos campos a seguir para estabelecer as configurações de sua organização:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Habilitar processo de revisão rápido</p> </td> 
      <td>Permite ativar versões mensais do Workfront para sua organização em vez de versões trimestrais.</p><p>Para obter mais informações sobre o processo de lançamento rápido, consulte <a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-custom-quarters-projects.md" class="MCXref xref">Habilitar ou desabilitar versões rápidas para sua organização</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Permitir incorporação de <strong>Workfront</strong> em um iframe</p> </td> 
      <td>Permite incorporar o Workfront em um iframe.<p>Essa opção está desativada por padrão.</p><p><b>IMPORTANTE</b>: a exibição de um aplicativo baseado na Web em um iframe torna o aplicativo susceptível a uma vulnerabilidade de segurança de clickjacking.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir autenticação SAML 2.0 nos suplementos do Office 365</td> 
      <td> <p>Permite incorporar o Workfront em um iframe somente para suplementos do Office 365 quando o Workfront é integrado a uma solução de logon único SAML 2.0. </p> <p>Essa opção está ativada por padrão.</p> <p><b>NOTA</b>: Se você ativar a opção acima, <strong>Permitir a incorporação do Workfront em um iframe</strong>, a opção <strong>Permitir autenticação SAML 2.0 em suplementos do Office 365</strong> está ativado e esmaecido.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Habilitar o uso de informações da sessão ao criar URLs de páginas externas</td> 
      <td> <p>Permite que os usuários usem as informações de ID da sessão de um site ao adicionar uma Página externa a um Painel.</p> <p>Para obter mais informações sobre como adicionar Páginas Externas a um Painel, consulte <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">Incorporar uma página externa da Web em um painel</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que as pessoas usem os aplicativos móveis da Workfront e a <strong>Workfront</strong> Suplemento do Outlook</td> 
      <td> <p>Permite que os usuários acessem os aplicativos móveis (Workfront View para iPad e aplicativos de celular) e o aplicativo Workfront Outlook.</p> <p>Essa opção está ativada por padrão. </p> <p>Para obter informações sobre o Workfront View, consulte <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Usar visualização do Adobe Workfront</a>. Para obter mais informações sobre os aplicativos móveis, consulte <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Usar o aplicativo móvel do Adobe Workfront</a>.</p> <p>Para obter mais informações sobre o plug-in do Outlook, consulte <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Configurar o Adobe Workfront para Outlook</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Colaborar com pessoas sem contas do Workfront usando endereços de email</p> </td> 
      <td>Permite que os usuários do Workfront compartilhem determinados itens com pessoas sem uma conta do Workfront incluindo seu endereço de email em vez do nome. Os usuários podem compartilhar os seguintes itens com usuários externos usando seus endereços de email:
       <ul>
        <li>Documento<br></li>
        <li>Solicitação de documento<br></li>
        <li>Aprovação de documento</li>
        <li>Calendário</li>
       </ul><p>Essa opção está ativada por padrão.</p> <p><b>Importante</b>: o nível de acesso Usuário externo não estará disponível na instância do Workfront se essa opção estiver desativada. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Níveis de acesso incorporados no Workfront</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exigir que os usuários externos se registrem com uma senha</td> 
      <td> <p>Exige que os usuários externos se registrem antes de poderem visualizar itens no Workfront. Por padrão, essa opção está desativada. Ao habilitar essa opção, as pessoas sem uma conta do Workfront incluídas em determinadas atualizações por seu endereço de email serão solicitadas a criar uma conta antes de poderem exibir o item em que estão incluídas. Isso cria uma conta de usuário externo para eles.</p> <p>Essa opção está desativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desconectar usuários automaticamente após</td> 
      <td> Permite especificar quando um usuário está desconectado do Workfront, após um período de inatividade. Por padrão, os usuários são desconectados após 8 horas de inatividade. <p>Essa opção também afeta clientes do Workfront que estão usando uma solução de logon único.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Desconectar usuários móveis automaticamente após </td> 
      <td>Permite especificar quando um usuário está desconectado do aplicativo Workfront, após um período de inatividade. Por padrão, os usuários são desconectados após 7 dias de inatividade. <p>Essa opção também afeta clientes do Workfront que estão usando uma solução de logon único.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Os usuários no sistema assumirão como padrão a Nova experiência na Página inicial </td> 
      <td>Permite especificar se os usuários verão a Nova experiência inicial por padrão. Em ambos os casos, os usuários podem optar por ativar ou desativar a Nova página inicial individualmente. Essa opção está ativada por padrão.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

   As alterações salvas aqui afetam a experiência de todos os usuários no Workfront e de qualquer pessoa que interaja com eles como um usuário externo.
