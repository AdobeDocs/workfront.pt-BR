---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Gerenciar chaves de API
description: Para minimizar as vulnerabilidades de segurança da API, os administradores do Adobe Workfront podem gerenciar as Chaves de API usadas para permitir que os aplicativos acessem o Workfront em nome de um usuário.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 1176d899-0585-430d-87f2-0823bda2f1be
source-git-commit: 8934c3f5681c09c00769442900013844ee7a80ef
workflow-type: tm+mt
source-wordcount: '1336'
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
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

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
>Você também pode gerar uma Chave de API por meio da API. Para obter mais informações, consulte a seção [API de Assinatura de Evento](../../../wf-api/general/event-subs-api.md) em [API de Assinatura de Evento](../../../wf-api/general/event-subs-api.md).

{{step-1-to-setup}}

1. Clique em **Sistema >** **Informações do Cliente.**
1. (Condicional) Execute uma das seguintes ações:

   Para gerar uma Chave de API: Na seção **Configurações da Chave de API**, clique em **Gerar Chave de API**.

   Ou\
   Para redefinir uma Chave de API: Na seção **Configurações da Chave de API**, clique em **Redefinir** e depois em **Redefinir.**

   Ou

   Para remover a Chave de API: Na seção **Configurações da Chave de API**, clique em **Remover** e depois em **Remover**.

## Gerar uma chave de API para usuários não administradores

Você pode gerar e gerenciar chaves de API para usuários em funções diferentes da de administrador do Workfront.

>[!NOTE]
>
>Isso não estará disponível se a instância Workfront da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

1. (Condicional) Se sua organização usar o gerenciamento de acesso de Logon único (SSO), desative temporariamente a opção que exige autenticação SSO.

   {{step-1-to-setup}}

   1. Expanda **Sistema** e clique em **Logon Único (SSO)**.
   1. No campo **Tipo**, selecione o tipo de SSO que sua organização usa.
   1. Com o tipo selecionado, role para baixo e desmarque a caixa de seleção **Habilitar**.
      ![Habilitar SSO](assets/sysadmin-security-sso-disable-31620-350x320.png)
   1. Clique em **Salvar**.


1. Na barra de endereços de um navegador, insira a seguinte chamada de API:

   `<domain>`.my.workfront.com/attask/api/v7.0/user?action=generateApiKey&amp;username=**username**&amp;password=**password**&amp;method=PUT

   Substitua `<domain>` pelo nome de domínio, nome de usuário e senha do Workfront pelas credenciais Workfront do usuário.

1. (Condicional) Ative a opção que exige autenticação SSO se ela tiver sido desativada na Etapa 1.

   {{step-1-to-setup}}

   1. Expanda **Sistema** e clique em **Logon Único (SSO)**.

   1. Selecione seu método SSO no menu suspenso **Type**.
   1. Marque a caixa de seleção que requer autenticação SSO.

## Configurar quando as chaves de API expiram

Você pode configurar as Chaves de API para expirarem para todos os usuários em seu sistema. Quando a chave de API de um usuário expira, o usuário deve se autenticar novamente em qualquer aplicativo que use a API do Workfront para acessar o Workfront. Você pode alterar a frequência com que as Chaves de API expiram. Você também pode configurar se as Chaves de API expiram quando a senha de um usuário expira.

{{step-1-to-setup}}

1. Clique em **Sistema** > **Informações do cliente**.
1. Na área **Configurações da Chave de API**, na lista suspensa **Após a criação**, as **chaves de API expiram em**, selecione o período em que deseja que as chaves de API expirem.

   Ao alterar essa opção, o novo período começa a partir do momento em que você fez a alteração. Por exemplo, se você alterar esta opção de *1 mês* para *6 meses*, as Chaves de API expirarão em 6 meses a partir do momento em que você fizer a alteração.

   Por padrão, as Chaves de API expiram a cada mês.

1. Para configurar as Chaves de API para expirarem no momento em que as senhas dos usuários expirarem, habilite **Remover chave de API quando a senha de um usuário expirar**.

   Por padrão, essa opção não está ativada.

   Para obter informações sobre como configurar senhas de usuário para expirar, consulte [Configurar preferências de segurança do sistema](../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

1. Clique em **Salvar**.

## Remover as chaves de API de todos os usuários

Se você estiver preocupado com uma violação de segurança específica em relação ao seu sistema Workfront, poderá remover as Chaves de API simultaneamente para todos os usuários.

>[!IMPORTANT]
>
>Remover as chaves de API de todos os usuários invalida TODAS as chaves de API de todos os usuários do sistema. Essa ação causará falha em todas as suas integrações no Workfront até que você gere uma nova Chave de API no Workfront e atualize todas as suas integrações.

{{step-1-to-setup}}

1. Expanda **Sistema** e clique em **Informações do cliente**.

1. Na área **Configurações da Chave de API**, clique em **Remover todas as chaves de API** e em **Remover** **Tudo**.

## Restrição de logons da API com um certificado X.509

>[!IMPORTANT]
>
>O procedimento descrito nesta seção se aplica apenas a organizações que ainda não foram integradas à Adobe Business Platform. Fazer logon no Workfront por meio da API do Workfront não estará disponível se sua organização tiver sido integrada à Adobe Business Platform.
>
>Para obter uma lista de procedimentos que diferem dependendo de sua organização ter sido integrada à Adobe Business Platform, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>Isso não estará disponível se a instância Workfront da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

Aplicativos de terceiros podem se comunicar com o Workfront por meio da API. Para aumentar a segurança do site do Workfront, você pode configurar o Workfront para restringir solicitações de logon da API fazendo upload de um certificado X.509 no Workfront. Depois de habilitada, todas as solicitações de logon por meio da API devem incluir um certificado de cliente, além do nome de usuário e da senha.

* [Obter o certificado X.509](#obtain-the-x-509-certificate)
* [Carregar o certificado para o Workfront](#upload-the-certificate-to-workfront)
* [Verifique se as chamadas de logon da API são restritas](#verify-api-login-calls-are-restricted)

### Obter o certificado X.509 {#obtain-the-x-509-certificate}

Obtenha um certificado X.509 válido de uma Autoridade de certificação confiável (como a Verisign) e salve-o em um local temporário na sua estação de trabalho.

### Fazer upload do certificado para o Workfront {#upload-the-certificate-to-workfront}

Depois de obter o certificado X.509 da sua autoridade de certificação, é necessário carregá-lo no Workfront.

1. Clique no ícone **Menu principal** ![Ícone do menu principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique no ícone **Configurar** ![Configurações de engrenagem](assets/gear-icon-settings.png).

1. Expanda **Sistema** e clique em **Informações do cliente**.

1. Na área **Configurações da Chave de API**, selecione **Exigir Certificado X.509 para logons de API**.
1. Clique em **Alterar Certificado**.
1. Na estação de trabalho, navegue até o certificado X.509 que você baixou anteriormente e selecione-o.
1. (Opcional) Clique em **Exibir Detalhes** ao lado do nome do certificado para exibir os seguintes detalhes sobre o certificado:

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

Antes de configurar sua instância do Workfront para exigir um certificado X.509, execute uma solicitação de API para o ponto de extremidade `/login` usando parâmetros válidos de nome de usuário e senha. Você receberá uma resposta 200 que contém uma sessionID.

Depois de fazer do certificado X.509 um requisito por meio da página de informações do cliente em sua instância do Workfront, faça outra tentativa de logon. Desta vez você receberá uma resposta de erro 500 com a seguinte mensagem: &quot;Solicitação não confiável. Entre em contato com o administrador do sistema e anexe um certificado.&quot;

Depois de confirmar que o certificado X.509 é necessário, execute a mesma solicitação de logon com um parâmetro adicional para apiCertificate definido como o valor do seu certificado. Se essa operação tiver sido executada corretamente, você receberá uma resposta 200 que contém uma sessionID válida.
