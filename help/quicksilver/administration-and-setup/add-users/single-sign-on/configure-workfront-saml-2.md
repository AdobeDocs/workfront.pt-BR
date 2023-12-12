---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Configurar o Adobe Workfront com SAML 2.0
description: Como administrador do Adobe Workfront, você pode configurar os aplicativos móveis e da Web do Workfront para se integrarem a uma solução SAML (Security Assertion Markup Language) 2.0 para logon único (SSO).
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 6d2494f1ccb2f9b222a953ed8bae922bd0f26389
workflow-type: tm+mt
source-wordcount: '1024'
ht-degree: 6%

---

# Configurar o Adobe Workfront com SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

{{important-admin-console-onboard}}

Como administrador do Adobe Workfront, você pode configurar os aplicativos móveis e da Web do Workfront para se integrarem a uma solução SAML (Security Assertion Markup Language) 2.0 para logon único (SSO).

Depois de configurar o SAML 2.0 no Workfront, conforme descrito nas seções a seguir, você poderá manter a configuração, conforme descrito em [Atualizar metadados do SAML 2.0 no provedor de identidade](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

## Requisitos de acesso

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
   <td><p>Novo: Padrão </p>
       <p>ou</p> 
       <p>Atual: Plano </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Habilitar autenticação para o Workfront com SAML 2.0

{{step-1-to-setup}}

1. Clique em **Sistema** > **Logon único (SSO).**

1. No **Tipo** selecione **SAML 2.0.**

1. Ao lado da parte superior das opções exibidas, clique em **Baixar os Metadados do SAML 2.0** para baixar o arquivo no seu computador.

   O Provedor de Identidade SAML 2.0 requer um arquivo XML com informações geradas na instância do Workfront. Depois de baixar o arquivo, você deve acessar o servidor do Provedor de Identidade SAML 2.0 e carregar o arquivo XML de metadados Workfront SAML 2.0 nele.

1. Especifique as seguintes informações no Workfront:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">Provedor de Serviço </td>
      <td> Este URL, já preenchido para você, identifica o Workfront para seu provedor de identidade. Por exemplo: <code>&lt;yourcompany&gt;.com/SAML2</code>.</td>
     </tr>
     <tr>
      <td role="rowheader">Tipo de vínculo</span> </td>
      <td> <p>Selecione o método compatível com o servidor IDP para enviar informações de autenticação:</p>
       <ul>
       <li>POST</li>
       <li>REDIRECIONAR</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Preencher campos a partir dos metadados do provedor de identidade </td> 
      <td>Na solução Provedor de identidade SAML 2.0, exporte um arquivo XML de metadados do provedor de serviços e salve-o em um local temporário no computador. Selecionar <strong>Escolher arquivo</strong>, localize e selecione o arquivo salvo para adicioná-lo à sua configuração do Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL do Portal de Login</span> </td> 
      <td>Insira o portal de logon comum da sua organização. Este é o URL no qual os usuários fazem logon para acessar o Workfront e todos os outros aplicativos integrados ao SAML 2.0.</td> 
     </tr>
     <tr>
      <td role="rowheader">URL de saída</span> </td> 
      <td> <p>Insira o URL de saída do servidor IDP. O Workfront envia uma solicitação HTTP para esse URL antes de sair do Workfront. Isso fecha a sessão do usuário no servidor remoto quando a sessão do Workfront é encerrada.</p> <p><b>NOTA</b>: você será redirecionado para o URL de saída somente se tiver a opção <strong>Permitir apenas Autenticação SAML 2.0</strong> ativado no seu perfil de usuário.</p> </td>
     </tr>
     <tr>
      <td role="rowheader">Endereço para alterar senha </td> 
      <td> <p> Especifique o URL para o qual os usuários serão redirecionados para alterar suas senhas. </p> <p>Como as credenciais do SAML 2.0 são usadas para acessar o Workfront, os usuários devem ser redirecionados para uma página em que possam alterar sua senha do SAML 2.0 em vez de concluir essa atividade por meio do Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Algoritmo de hash seguro </td> 
      <td> <p>Selecione o Secure Hash Algorithm (SHA) compatível com o IDP:</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Usuários auto provisionados</span> </td> 
      <td> <p>Esta opção cria automaticamente um usuário no sistema quando um novo usuário com um nome de usuário e senha de diretório tenta fazer logon no Workfront pela primeira vez.</p> <p>Para criar usuários no Workfront, você deve mapear atributos de dados do Workfront com os seguintes atributos de dados do usuário no provedor de diretório:</p> 
       <ul> 
       <li>Nome</li> 
       <li>Sobrenome</li> 
       <li>Endereço de email</li> 
       </ul> 
       <p>Ao marcar a caixa de seleção, as seguintes opções são exibidas:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Selecione o Atributo de Usuário do Workfront que deseja mapear na lista drop-down e, em seguida, especifique o Atributo de Diretório correspondente no diretório de usuário.</p> 
       <p>A variável <strong>Diretório de Atributo</strong> O campo deve conter o Nome do atributo de diretório na tabela Atributo do usuário que você salvou ao testar com êxito a configuração do SAML 2.0.</p> 
       <p>Você pode definir um Valor padrão de Workfront na variável <strong>Valor padrão</strong> campo. Você também pode definir regras com base nos valores do seu Provedor de Identidade SAML 2.0.</p> 
       <p><b>AVISO</b>: o Workfront tenta mapear os atributos listados abaixo sempre que um usuário fizer logon no sistema. Por causa disso, não recomendamos mapear os níveis de acesso. Você poderá remover facilmente o acesso administrativo se um atributo for mapeado incorretamente. Clique em <strong>Adicionar mapeamento</strong> para adicionar outras regras.
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
      <li> <p>Função no trabalho</p> </li> 
      <li> <p>Sobrenome</p> </li> 
      <li> <p>Modelo de Layout</p> </li> 
      <li> <p>Gerente</p> </li> 
      <li> <p>Telefone celular</p> </li> 
      <li> <p>Número de telefone</p> </li> 
      <li> <p>Código postal</p> </li> 
      <li> <p>Agendar</p> </li> 
      <li> <p>Estado</p> </li> 
      <li> <p>Perfil da Planilha de Horas</p> </li> 
      <li> <p>Título</p> </li> 
      </ul>
      <p>Clique em <strong>Salvar</strong> quando terminar de mapear os atributos do usuário.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Certificado </td> 
      <td> <p>Carregue um certificado SSL válido para garantir uma conexão segura entre o serviço de autenticação e o Workfront. Para contas OnDemand, um certificado é sempre necessário. Você pode obter este certificado com o administrador do sistema SAML 2.0.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exceções do administrador </td> 
      <td> <p>Permite que os administradores do Workfront acessem o Workfront usando o logon do Workfront. Se essa opção não estiver selecionada, os administradores do Workfront deverão usar o nome de usuário e a senha do SAML 2.0.</p> 
      <p>A Workfront tenta fazer logon pela primeira vez no Workfront via SAML 2.0 para usuários com o nível de acesso de Administrador do sistema do Workfront. Se a autenticação do SAML 2.0 falhar, o Workfront usará a autenticação local para administradores do Workfront.</p> 
      <p>Recomendamos que essa opção seja sempre selecionada para que o administrador do Workfront possa fazer logon no Workfront se o provedor SAML 2.0 ficar temporariamente indisponível.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Habilitar </td> 
      <td> <p>Ativa o SSO no sistema Workfront. Certifique-se de ter comunicado as instruções de logon aos usuários.</p> <p>Após ativar a configuração de SSO no Workfront, você deve ativar o <strong>Permitir apenas Autenticação SAML 2.0</strong> para que todos os usuários possam usar o SSO.</p> <p>Para obter mais informações sobre a atualização de usuários para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Atualizar usuários para logon único</a>.</p> <p>Para obter mais informações sobre as configurações do usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar o perfil de um usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirma a Configuração </td> 
      <td> 
      <p>Clique em <strong>Testar conexão</strong> para verificar se o Workfront e o Provedor de identidade SAML 2.0 podem se comunicar. Essa conexão só terá êxito se você tiver trocado os arquivos XML.
      </p> 
      <p>Depois de testar com êxito o link entre o Provedor de identidade SAML 2.0 e o Workfront, você verá uma tela semelhante à imagem abaixo.</p>
      <p><b>NOTA</b>: essa tela é exibida em um pop-up do navegador, portanto, desative os bloqueadores de pop-up no navegador.</p>
      <p>Salve as informações exibidas na tabela para uso posterior.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** para salvar a configuração do SAML 2.0.
