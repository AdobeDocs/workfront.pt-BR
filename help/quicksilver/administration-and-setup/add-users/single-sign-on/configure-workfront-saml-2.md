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
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 8%

---

# Configurar o Adobe Workfront com SAML 2.0

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->



>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas à Adobe Admin Console.
>
>Para mapear atributos de usuário em organizações que foram integradas à Adobe Admin Console, consulte [Mapear atributos de usuário na experiência unificada da Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) no artigo Mapear atributos de usuário.

Como administrador do Adobe Workfront, você pode configurar os aplicativos móveis e da Web do Workfront para se integrarem a uma solução SAML (Security Assertion Markup Language) 2.0 para logon único (SSO).

Depois de configurar o SAML 2.0 no Workfront, conforme descrito nas seções a seguir, você pode manter a configuração, conforme descrito em [Atualizar metadados do SAML 2.0 no seu provedor de identidade](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td><p>Standard</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilitar autenticação para o Workfront com SAML 2.0

{{step-1-to-setup}}

1. Clique em **Sistema** > **Logon Único (SSO).**

1. Na lista suspensa **Tipo**, selecione **SAML 2.0.**

1. Próximo à parte superior das opções exibidas, clique em **Baixar SAML 2.0 Metadata** para baixar o arquivo em seu computador.

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
      <td role="rowheader">Tipo de Associação</span> </td>
      <td> <p>Selecione o método compatível com o servidor IDP para enviar informações de autenticação:</p>
       <ul>
       <li>POST</li>
       <li>REDIRECIONAR</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">Preencher campos a partir dos metadados do provedor de identidade </td> 
      <td>Na solução Provedor de identidade SAML 2.0, exporte um arquivo XML de metadados do provedor de serviços e salve-o em um local temporário no computador. Selecione <strong>Escolher Arquivo</strong>, localize e selecione o arquivo salvo para adicioná-lo à sua configuração do Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">URL do Portal de Logon</span> </td> 
      <td>Insira o portal de logon comum da sua organização. Este é o URL no qual os usuários fazem logon para acessar o Workfront e todos os outros aplicativos integrados ao SAML 2.0.</td> 
     </tr>
     <tr>
      <td role="rowheader">URL de Saída</span> </td> 
      <td> <p>Insira o URL de saída do servidor IDP. O Workfront envia uma solicitação HTTP para esse URL antes de sair do Workfront. Isso fecha a sessão do usuário no servidor remoto quando a sessão do Workfront é encerrada.</p> <p><b>OBSERVAÇÃO</b>: você será redirecionado para a URL de saída somente se tiver a opção <strong>Permitir apenas a Autenticação SAML 2.0</strong> habilitada em seu perfil de usuário.</p> </td>
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
      <td role="rowheader">Usuários Provisionados Automaticamente</span> </td> 
      <td> <p>Esta opção cria automaticamente um usuário no sistema quando um novo usuário com um nome de usuário e senha de diretório tenta fazer logon no Workfront pela primeira vez.</p> <p>Para criar usuários no Workfront, você deve mapear atributos de dados do Workfront com os seguintes atributos de dados do usuário no provedor de diretório:</p> 
       <ul> 
       <li>Nome</li> 
       <li>Sobrenome</li> 
       <li>Endereço de email</li> 
       </ul> 
       <p>Ao marcar a caixa de seleção, as seguintes opções são exibidas:</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>Selecione o Atributo de Usuário do Workfront que deseja mapear na lista drop-down e, em seguida, especifique o Atributo de Diretório correspondente no diretório de usuário.</p> 
       <p>O campo <strong>Atributo de Diretório</strong> deve conter o Nome de Atributo de Diretório da tabela de Atributo de Usuário que você salvou ao testar com êxito a configuração do SAML 2.0.</p> 
       <p>Você pode definir um Valor padrão do Workfront no campo <strong>Valor padrão</strong>. Você também pode definir regras com base nos valores do seu Provedor de Identidade SAML 2.0.</p> 
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
      <li> <p>Grupo principal</p> </li> 
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
      <td> <p>Ativa o SSO no sistema Workfront. Certifique-se de ter comunicado as instruções de logon aos usuários.</p> <p>Depois de habilitar a configuração de SSO no Workfront, você deve habilitar a configuração <strong>Permitir apenas a autenticação SAML 2.0</strong> para todos os usuários para que eles possam usar o SSO.</p> <p>Para obter mais informações sobre como atualizar usuários para SSO, consulte <a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">Atualizar usuários para logon único</a>.</p> <p>Para obter mais informações sobre configurações de usuário, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Editar perfil de usuário</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Confirma a Configuração </td> 
      <td> 
      <p>Clique em <strong>Testar Conexão</strong> para verificar se o Workfront e o Provedor de Identidade SAML 2.0 podem se comunicar. Essa conexão só terá êxito se você tiver trocado os arquivos XML.
      </p> 
      <p>Depois de testar com êxito o link entre o Provedor de identidade SAML 2.0 e o Workfront, você verá uma tela semelhante à imagem abaixo.</p>
      <p><b>OBSERVAÇÃO</b>: esta tela é exibida em um pop-up do navegador, portanto, desative os bloqueadores de pop-up no navegador.</p>
      <p>Salve as informações exibidas na tabela para uso posterior.</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar** para salvar a configuração do SAML 2.0.
