---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configurar o Adobe Workfront com o SAML 2.0
description: Como administrador do Adobe Workfront, você pode configurar os aplicativos móveis e da Web do Workfront para integrar com uma solução SAML (Security Assertion Markup Language) 2.0 para logon único (SSO).
author: Becky, Caroline
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1008'
ht-degree: 8%

---

# Configurar o Adobe Workfront com o SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode configurar os aplicativos móveis e da Web do Workfront para integrar com uma solução SAML (Security Assertion Markup Language) 2.0 para logon único (SSO).

Depois de configurar o SAML 2.0 no Workfront, conforme descrito nas seções a seguir, é possível manter a configuração, conforme descrito em [Atualize os metadados SAML 2.0 no seu provedor de identidade](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Habilitar autenticação para o Workfront com SAML 2.0

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Logon único (SSO).**

1. No **Tipo** lista suspensa, clique em **SAML 2.0.**

1. Próximo à parte superior das opções exibidas, clique em **Baixar metadados do SAML 2.0** para baixar o arquivo em seu computador.

   Seu provedor de identidade SAML 2.0 requer um arquivo XML com informações geradas na instância do Workfront. Após o download do arquivo, você precisa acessar o servidor do Provedor de identidade SAML 2.0 e fazer upload do arquivo XML de metadados Workfront SAML 2.0 lá.

1. Especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Provedor de Serviço </td> 
      <td> Esse URL, já preenchido para você, identifica o Workfront ao seu provedor de identidade. Por exemplo: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de ligação</span> </td> 
      <td> <p>Selecione o método suportado pelo servidor IDP para enviar informações de autenticação:</p> 
       <ul> 
        <li>POST</li> 
        <li>REDIRECIONAR</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Preencher campos a partir dos metadados do provedor de identidade </td> 
      <td>Na solução Provedor de identidade SAML 2.0, exporte um arquivo XML de metadados do provedor de serviços e salve-o em um local temporário no computador. Selecionar <strong>Escolher arquivo</strong>e, em seguida, localize e selecione o arquivo salvo para adicioná-lo à sua configuração do Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endereço do Portal de Login</span> </td> 
      <td>Especifique o portal de logon comum de sua organização. Este é o URL no qual os usuários fazem logon para acessar o Workfront e todos os outros aplicativos integrados ao SAML 2.0.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endereço de saída do simples acesso</span> </td> 
      <td> <p>Especifique o URL de logout do servidor IDP. O Workfront envia uma solicitação HTTP para esse URL antes de sair do Workfront. Isso fecha a sessão do usuário no servidor remoto quando a sessão do Workfront é fechada.</p> <p><b>OBSERVAÇÃO</b>: Você é redirecionado para o URL de logout somente se tiver a opção Permitir somente autenticação SAML 2.0 ativada em seu perfil de usuário.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Endereço para alterar senha </td> 
      <td> <p> Especifique o URL no qual os usuários serão redirecionados para alterar suas senhas. </p> <p>Como as credenciais do SAML 2.0 são usadas para acessar o Workfront, os usuários precisam ser redirecionados para uma página em que possam alterar sua senha do SAML 2.0 em vez de concluir esta atividade por meio do Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Algoritmo de hash seguro </td> 
      <td> <p>Selecione o SHA (Secure Hash Algorithm) que o IDP suporta:</p> 
       <ul> 
        <li>SHA-1</li> 
        <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Usuários auto provisionados</span> </td> 
      <td> <p>Cria automaticamente um usuário no sistema quando um novo usuário com um nome de usuário e senha de diretório tenta fazer logon no Workfront pela primeira vez.</p> <p>Para criar usuários no Workfront, é necessário mapear os atributos de dados do Workfront com os seguintes atributos de dados do usuário no provedor de diretório:</p> 
       <ul> 
        <li>Nome</li> 
        <li>Sobrenome</li> 
        <li>Endereço de email</li> 
       </ul> 
       <p>As seguintes opções são exibidas para permitir que você faça isso:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Selecione o Atributo de Usuário do Workfront que você deseja mapear na lista suspensa e especifique o Atributo de Diretório correspondente no diretório do usuário.</p> 
       <p>O <strong>Atributo do diretório</strong> O campo deve conter o Nome do atributo de diretório na tabela Atributo do usuário que você salvou ao testar com êxito a configuração do SAML 2.0.</p> 
       <p>É possível definir um Valor padrão de Workfront na variável <strong>Valor padrão</strong> campo. Também é possível definir regras com base nos valores do Provedor de identidade SAML 2.0.</p> 
       <p><b>AVISO</b>: O Workfront tenta mapear os atributos listados abaixo sempre que um usuário faz logon no sistema. Por causa disso, não recomendamos mapear os níveis de acesso. Você pode remover facilmente o acesso administrativo se um atributo estiver mapeado incorretamente. Clique em Adicionar mapeamento para adicionar mais regras.
       </p> 
       <p>Você pode mapear os seguintes atributos do Workfront:</p> 
      <ul> 
      <li> <p>Nível de acesso</p> </li> 
      <li> <p>Endereço</p> </li> 
      <li> <p>Endereço2</p> </li> 
      <li> <p>Cobrança por hora</p> </li> 
      <li> <p>Cidade</p> </li> 
      <li> <p>Empresa</p> </li> 
      <li> <p>Custo por hora</p> </li> 
      <li> <p>Endereço de email</p> </li> 
      <li> <p>Extensão</p> </li> 
      <li> <p>Nome</p> </li> 
      <li> <p>Grupo padrão</p> </li> 
      <li> <p>Equipe interna</p> </li> 
      <li> <p>Função de trabalho</p> </li> 
      <li> <p>Sobrenome</p> </li> 
      <li> <p>Modelo de Layout</p> </li> 
      <li> <p>Gerente</p> </li> 
      <li> <p>Telefone Celular</p> </li> 
      <li> <p>Número de telefone</p> </li> 
      <li> <p>Código Postal</p> </li> 
      <li> <p>Cronograma</p> </li> 
      <li> <p>Estado</p> </li> 
      <li> <p>Perfil da Planilha de Horas</p> </li> 
      <li> <p>Título</p> </li> 
      </ul> </td> 
          <td> </td> 
         </tr> 
        </tbody> 
        <p>Clique em <strong>Salvar</strong> quando você terminar de mapear atributos do usuário.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificado </td> 
      <td> <p>Faça upload de um certificado SSL válido para garantir uma conexão segura entre o serviço de autenticação e o Workfront. Para contas OnDemand, um certificado é sempre necessário. Você pode obter esse certificado do administrador do sistema SAML 2.0.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exceções do administrador </td> 
      <td> <p>Permite que os administradores do Workfront acessem o Workfront usando o logon do Workfront. Se essa opção não estiver selecionada, os administradores do Workfront deverão usar o nome de usuário e a senha SAML 2.0.</p> 
      <p>O Workfront primeiro tenta fazer logon no Workfront via SAML 2.0 para usuários com o nível de acesso do Administrador do sistema do Workfront. Se a autenticação SAML 2.0 falhar, o Workfront usará a autenticação local para administradores do Workfront.</p> 
      <p>Recomendamos que você sempre tenha essa opção selecionada para que o administrador do Workfront possa fazer logon no Workfront se o provedor SAML 2.0 nunca estiver temporariamente indisponível.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Habilitar </td> 
      <td> <p>Ativa o SSO no sistema Workfront. Certifique-se de ter comunicado instruções de logon aos usuários.</p> <p>Após habilitar a configuração do SSO no Workfront, é necessário habilitar a variável <strong>Permitir apenas a autenticação SAML 2.0</strong> configuração para todos os usuários, para que possam usar SSO.</p> <p>Para obter mais informações sobre como atualizar usuários para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Atualizar usuários para logon único</a>.</p> <p>Para obter mais informações sobre as configurações do usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirma a Configuração </td> 
      <td> 
      <p>Clique em <strong>Testar conexão</strong> para verificar se o Workfront e o provedor de identidade SAML 2.0 podem se comunicar. Essa conexão é bem-sucedida somente se você trocou os arquivos XML.
      </p> 
      <p>Depois de testar com êxito o link entre o provedor de identidade SAML 2.0 e o Workfront, você verá uma tela semelhante à abaixo.</p>
      <p><b>OBSERVAÇÃO</b>: Essa tela é exibida em um pop-up do navegador, portanto, desative os bloqueadores de pop-up no navegador.</p>
      <p>Salve as informações exibidas na tabela para uso posterior.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** para salvar a configuração do SAML 2.0.
