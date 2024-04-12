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
source-git-commit: f504013e202c57245a2edc3dff2b71d19bcfdbee
workflow-type: tm+mt
source-wordcount: '1386'
ht-degree: 2%

---

# Gerenciar chaves de API

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

Para minimizar as vulnerabilidades de segurança da API, os administradores do Adobe Workfront podem gerenciar as Chaves de API usadas para permitir que os aplicativos acessem o Workfront em nome de um usuário.

Você pode redefinir ou remover sua Chave de API do administrador atual, configurar as Chaves de API para expirar e remover as Chaves de API para todos os usuários.

Exemplos de aplicativos que usam a API do Workfront são:

* Integrações de documentos, como Dropbox, Google Drive e Workfront DAM
* aplicativos móveis Workfront

>[!IMPORTANT]
>
>Ao redefinir ou remover uma Chave de API, qualquer aplicativo que use a API do Workfront e seja autenticado no Workfront por meio dessa Chave de API deve ser reconfigurado para recuperar o acesso ao Workfront.

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
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Chaves de API do Workfront

Cada usuário no Workfront tem uma chave de API exclusiva. Essa chave é gerada com base no usuário no momento em que o usuário acessa uma integração que aproveita a API do Workfront (como o aplicativo móvel Workfront ou uma integração de documentos).

>[!NOTE]
>
> As chaves de API geradas no ambiente de produção são copiadas para o ambiente de Pré-visualização durante a atualização semanal. Quaisquer chaves de API geradas no ambiente de Pré-visualização serão substituídas pelas chaves de API de produção durante a atualização semanal.

Os administradores do Workfront também têm uma chave de API exclusiva. Quando um aplicativo usa uma chave de API de administrador para acessar o Workfront, ele tem acesso de administrador ao Workfront.

## Gerenciar uma chave de API do administrador

Você pode gerar, redefinir ou remover a Chave de API da conta de usuário administrador.

>[!NOTE]
>
>Você também pode gerar uma Chave de API por meio da API. Para obter mais informações, consulte [API de assinatura de evento](../../../wf-api/general/event-subs-api.md) seção em [API de assinatura de evento](../../../wf-api/general/event-subs-api.md).

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema >** **Informações do cliente.**
1. (Condicional) Execute uma das seguintes ações:

   Para gerar uma chave de API: na **Configurações da chave de API** clique em **Gerar chave de API**.

   Ou\
   Para redefinir uma chave de API: no **Configurações da chave de API** clique em **Redefinir**, depois **Redefinir.**

   Ou

   Para remover a chave de API: na guia **Configurações da chave de API** clique em **Remover**, depois **Remover**.

## Gerar uma chave de API para usuários não administradores

Você pode gerar e gerenciar chaves de API para usuários em funções diferentes da de administrador do Workfront.

>[!NOTE]
>
>Isso não estará disponível se a instância Workfront da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

1. (Condicional) Se sua organização usar o gerenciamento de acesso de Logon único (SSO), desative temporariamente a opção que exige autenticação SSO.

   1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

   1. Expandir **Sistema** e, em seguida, clique em **Logon único (SSO)**.
   1. No **Tipo** selecione o tipo de SSO que sua organização usa.
   1. Com o tipo selecionado, role para baixo e limpe a **Ativar** caixa de seleção
      ![](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Clique em **Salvar**.


1. Na barra de endereços de um navegador, insira a seguinte chamada de API:

   `<domain>`**.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**nome de usuário**&amp;senha=**senha**&amp;method=PUT

   Substituir `<domain>` com o nome de domínio do Workfront e o nome de usuário e senha com as credenciais Workfront do usuário.

1. (Condicional) Ative a opção que exige autenticação SSO se ela tiver sido desativada na Etapa 1.

   1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

   1. Expandir **Sistema** e, em seguida, clique em **Logon único (SSO)**.

   1. Selecione o método SSO no campo **Tipo** menu suspenso.
   1. Marque a caixa de seleção que requer autenticação SSO.

## Configurar quando as chaves de API expiram

Você pode configurar as Chaves de API para expirarem para todos os usuários em seu sistema. Quando a chave de API de um usuário expira, o usuário deve se autenticar novamente em qualquer aplicativo que use a API do Workfront para acessar o Workfront. Você pode alterar a frequência com que as Chaves de API expiram. Você também pode configurar se as Chaves de API expiram quando a senha de um usuário expira.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Informações do cliente**.
1. No **Configurações da chave de API** área, no **Após a criação**, **As chaves de API expiram em** selecione o período quando deseja que as chaves de API expirem.

   Ao alterar essa opção, o novo período começa a partir do momento em que você fez a alteração. Por exemplo, se você alterar essa opção de *1 mês* para *6 meses*, as Chaves de API expiram em 6 meses a partir do momento em que você faz a alteração.

   Por padrão, as Chaves de API expiram a cada mês.

1. Para configurar as Chaves de API para expirarem no momento em que as senhas dos usuários expirarem, selecione **Remover a chave de API quando a senha de um usuário expirar**.

   Por padrão, essa opção não está selecionada.

   Para obter informações sobre como configurar senhas de usuários para expirar, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Clique em **Salvar**.

## Remover as chaves de API de todos os usuários

Se você estiver preocupado com uma violação de segurança específica em relação ao seu sistema Workfront, poderá remover as Chaves de API simultaneamente para todos os usuários.

>[!IMPORTANT]
>
>Remover as chaves de API de todos os usuários invalida TODAS as chaves de API de todos os usuários do sistema. Essa ação causará falha em todas as suas integrações no Workfront até que você gere uma nova Chave de API no Workfront e atualize todas as suas integrações.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema** e, em seguida, clique em **Informações do cliente.**

1. No **Configurações da chave de API** clique em **Remover todas as chaves de API** e, em seguida, clique em **Remover** **Todos**.

## Restrição de logons da API com um certificado X.509

>[!IMPORTANT]
>
>O procedimento descrito nesta seção se aplica apenas a organizações que ainda não foram integradas à Plataforma de negócios Adobe. Fazer logon no Workfront por meio da API do Workfront não estará disponível se sua organização tiver sido integrada à Plataforma comercial Adobe.
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à Plataforma de negócios Adobe, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Aplicativos de terceiros podem se comunicar com o Workfront por meio da API. Para aumentar a segurança do site do Workfront, você pode configurar o Workfront para restringir solicitações de logon da API fazendo upload de um certificado X.509 no Workfront. Depois de habilitada, todas as solicitações de logon por meio da API devem incluir um certificado de cliente, além do nome de usuário e da senha.

>[!NOTE]
>
>Isso não estará disponível se a instância Workfront da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

* [Obter o certificado X.509](#obtain-the-x-509-certificate)
* [Fazer upload do certificado para o Workfront](#upload-the-certificate-to-workfront)
* [Verifique se as chamadas de logon da API são restritas](#verify-api-login-calls-are-restricted)

### Obter o certificado X.509 {#obtain-the-x-509-certificate}

Obtenha um certificado X.509 válido de uma Autoridade de certificação confiável (como a Verisign) e coloque-o em um local temporário na sua estação de trabalho.

### Fazer upload do certificado para o Workfront {#upload-the-certificate-to-workfront}

Depois de obter o certificado X.509 da sua autoridade de certificação, é necessário carregá-lo no Workfront.

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Expandir **Sistema** e, em seguida, clique em **Informações do cliente**.

1. No **Configurações da chave de API** , selecione **Habilitar Certificado X.509**.
1. Na estação de trabalho, navegue até o certificado X.509 que você baixou anteriormente e selecione-o.
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

### Verifique se as chamadas de logon da API são restritas {#verify-api-login-calls-are-restricted}

Antes de configurar sua instância do Workfront para exigir um certificado X.509, execute uma solicitação de API para o `/login` ponto de extremidade usando parâmetros válidos de nome de usuário e senha. Você receberá uma resposta 200 que contém uma sessionID.

Depois de fazer do certificado X.509 um requisito por meio da página de informações do cliente em sua instância do Workfront, faça outra tentativa de logon. Desta vez você receberá uma resposta de erro 500 com a seguinte mensagem: &quot;Solicitação não confiável. Entre em contato com o administrador do sistema e anexe um certificado.&quot;

Depois de confirmar que o certificado X.509 é necessário, execute a mesma solicitação de logon com um parâmetro adicional para apiCertificate definido como o valor do seu certificado. Se essa operação tiver sido executada corretamente, você receberá uma resposta 200 que contém uma sessionID válida.
