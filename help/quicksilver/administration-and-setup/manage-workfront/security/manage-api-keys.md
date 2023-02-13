---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gerenciar chaves de API
description: Para minimizar as vulnerabilidades de segurança da API, os administradores do Adobe Workfront podem gerenciar as Chaves de API usadas para permitir que os aplicativos acessem o Workfront em nome de um usuário.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 2%

---

# Gerenciar chaves de API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Para minimizar as vulnerabilidades de segurança da API, os administradores do Adobe Workfront podem gerenciar as Chaves de API usadas para permitir que os aplicativos acessem o Workfront em nome de um usuário.

Você pode redefinir ou remover sua Chave de API do administrador atual, configurar as Chaves de API para expirar e remover as Chaves de API para todos os usuários.

Exemplos de aplicativos que usam a API do Workfront são:

* Integrações de documentos como Dropbox, Google Drive e Workfront DAM
* Aplicativos móveis Workfront

>[!IMPORTANT]
>
>Ao redefinir ou remover uma Chave de API, qualquer aplicativo que aproveite a API do Workfront e se autentique no Workfront por meio dessa Chave de API deve ser reconfigurado para recuperar o acesso ao Workfront.

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

## Chaves de API do Workfront

Cada usuário no Workfront tem uma chave de API exclusiva. Essa chave é gerada por usuário no momento em que o usuário acessa uma integração que aproveita a API do Workfront (como o aplicativo móvel Workfront ou uma integração de documento).

>[!NOTE]
>
> As chaves de API geradas no ambiente de produção são copiadas para o ambiente de Visualização durante a atualização semanal. Qualquer chave de API gerada no ambiente de Visualização será substituída pelas chaves de API de produção durante a atualização semanal.

Os administradores do Workfront também têm uma Chave de API exclusiva. Quando um aplicativo usa uma Chave da API do administrador para acessar o Workfront, ele tem acesso de administrador ao Workfront.

## Gerenciar uma chave de API de administrador

Você pode gerar, redefinir ou remover a Chave da API da conta de usuário do administrador.

>[!NOTE]
>
>Você também pode gerar uma Chave de API por meio da API. Para obter mais informações, consulte o [API de assinatura de evento](../../../wf-api/general/event-subs-api.md) seção em [API de assinatura de evento](../../../wf-api/general/event-subs-api.md).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema >** **Informações do cliente.**
1. (Condicional) Execute uma das seguintes ações:

   Para gerar uma chave de API: No **Configurações da chave da API** seção , clique em **Gerar chave de API**.

   Ou\
   Para redefinir uma chave de API: No **Configurações da chave da API** seção , clique em **Redefinir**, em seguida **Redefinir.**

   Ou

   Para remover a Chave da API: No **Configurações da chave da API** seção , clique em **Remover**, em seguida **Remover**.

## Gerar uma chave de API para usuários não administradores

Você pode gerar e gerenciar chaves de API para usuários em funções diferentes do administrador do Workfront.

>[!NOTE]
>
>Isso não estará disponível se a instância do Workfront de sua organização estiver habilitada com o Adobe IMS. Consulte seu administrador de rede ou de TI se precisar de mais informações.

1. (Condicional) Se sua organização usa o gerenciamento de acesso de Logon único (SSO), desative temporariamente a opção que requer autenticação SSO.

   1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

   1. Expandir **Sistema**, depois clique em **Logon único (SSO)**.\
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)

   1. Desative a caixa de seleção que requer autenticação SSO.

      Por exemplo, se sua organização usa o SAML 2.0, desative **Permitir apenas a autenticação SAML 2.0**.

1. Na barra de endereços de um navegador, insira a seguinte chamada de API:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**username**&amp;password=**senha**&amp;method=PUT

   Substituir `<domain>` com seu nome de domínio do Workfront e nome de usuário e senha com as credenciais do Workfront do usuário.

1. (Condicional) Ative a opção que requer autenticação SSO se você a tiver desativado na Etapa 1.

   1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

   1. Expandir **Sistema**, depois clique em **Logon único (SSO)**.

   1. Selecione seu método SSO no **Tipo** menu suspenso.
   1. Marque a caixa de seleção que requer autenticação SSO.

## Configurar quando as chaves da API expirarem

Você pode configurar as Chaves de API para expirar para todos os usuários em seu sistema. Quando a Chave da API de um usuário expira, ele deve autenticar novamente para qualquer aplicativo que use a API do Workfront para acessar o Workfront. Você pode alterar a frequência de expiração das chaves de API. Você também pode configurar se as Chaves de API expiram quando a senha de um usuário expira.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Informações do cliente**.
1. No **Configurações da chave da API** na **Após a criação**, **As chaves da API expiram em** na lista suspensa, selecione o período em que deseja que as chaves da API expirem.

   Quando você altera essa opção, o novo período começa a partir do momento em que você fez a alteração. Por exemplo, se você alterar essa opção de *1 mês* para *6 meses*, as Chaves de API expiram 6 meses a partir do momento em que você faz a alteração.

   Por padrão, as Chaves de API expiram todo mês.

1. Para configurar as Chaves de API para expirarem no momento em que as senhas dos usuários expirarem, selecione **Remover chave da API quando a senha de um usuário expirar**.

   Por padrão, essa opção não está selecionada.

   Para obter informações sobre como configurar senhas de usuário para expirar, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Clique em **Salvar**.

## Remova as chaves da API para todos os usuários

Se estiver preocupado com uma violação de segurança específica em relação ao sistema Workfront, é possível remover chaves de API simultaneamente para todos os usuários.

>[!IMPORTANT]
>
>Remover Chaves de API para todos os usuários invalida TODAS as Chaves de API para todos os usuários no sistema. Essa ação causará a falha de todas as suas integrações no Workfront até que você gere uma nova Chave de API no Workfront e atualize todas as suas integrações.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema**, depois clique em **Informações do cliente.**

1. No **Configurações da chave da API** , clique em **Remover todas as chaves da API**, depois clique em **Remover** **Todos**.

## Restrição de logons da API com um certificado X.509

>[!IMPORTANT]
>
>O procedimento descrito nesta seção aplica-se apenas a organizações que ainda não foram incorporadas à Adobe Business Platform. Fazer logon no Workfront por meio da API do Workfront não estará disponível se sua organização tiver sido integrada à Adobe Business Platform.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Plataforma de negócios do Adobe, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Aplicativos de terceiros podem se comunicar com o Workfront por meio da API. Para aumentar a segurança do site do Workfront, é possível configurar o Workfront para restringir as solicitações de logon da API carregando um certificado X.509 para o Workfront. Depois de habilitado, todas as solicitações de logon por meio da API devem incluir um certificado de cliente, além do nome de usuário e da senha.

>[!NOTE]
>
>Isso não estará disponível se a instância do Workfront de sua organização estiver habilitada com o Adobe IMS. Consulte seu administrador de rede ou de TI se precisar de mais informações.

* [Obter o certificado X.509](#obtain-the-x-509-certificate)
* [Fazer upload do certificado para o Workfront](#upload-the-certificate-to-workfront)
* [Verifique se as chamadas de logon da API estão restritas](#verify-api-login-calls-are-restricted)

### Obter o certificado X.509 {#obtain-the-x-509-certificate}

Obtenha um certificado X.509 válido de uma autoridade de certificação confiável (como Verisign) e coloque-o em um local temporário na sua estação de trabalho.

### Fazer upload do certificado para o Workfront {#upload-the-certificate-to-workfront}

Após obter o certificado X.509 da autoridade de certificação, é necessário carregá-lo na Workfront.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema**, depois clique em **Informações do cliente**.

1. No **Configurações da chave da API** , selecione **Habilitar Certificado X.509**.
1. Na estação de trabalho, procure e selecione o certificado X.509 que você baixou anteriormente.
1. (Opcional) Clique em **Exibir detalhes** ao lado do nome do certificado para exibir os seguintes detalhes sobre o certificado:

   * Nome comum do assunto
   * Organização do assunto
   * Unidade da organização do assunto
   * Nome comum do emissor
   * Organização emissora
   * Unidade da organização emissora
   * Número de série
   * Data de emissão
   * Data de expiração

1. Clique em **Salvar**.

### Verifique se as chamadas de logon da API estão restritas {#verify-api-login-calls-are-restricted}

Antes de configurar sua instância do Workfront para exigir um certificado X.509, execute uma solicitação de API para o `/login` endpoint usando parâmetros válidos de nome de usuário e senha. Você receberá uma resposta 200 contendo uma sessionID.

Depois de tornar o certificado X.509 um requisito por meio da página de informações do cliente em sua instância do Workfront, faça outra tentativa de logon. Desta vez, você receberá uma resposta de erro 500 com a seguinte mensagem: &quot;Solicitação não confiável. Entre em contato com o administrador do sistema e anexe o certificado.&quot;

Depois de confirmar que o certificado X.509 é obrigatório, execute a mesma solicitação de logon com um parâmetro adicional para apiCertificate definido como o valor do seu certificado. Se essa operação foi executada corretamente, você receberá uma resposta 200 contendo uma sessionID válida.
