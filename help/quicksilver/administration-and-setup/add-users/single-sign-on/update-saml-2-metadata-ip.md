---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Atualizar metadados do SAML 2.0 no provedor de identidade
description: Você pode atualizar os metadados do SAML 2.0 no provedor de identidade.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '994'
ht-degree: 0%

---

# Atualizar metadados do SAML 2.0 no provedor de identidade

{{important-admin-console-onboard}}

As seções a seguir descrevem como atualizar os metadados da SAML (Security Assertion Markup Language) 2.0 ao usar os ADFS (Serviços de Federação do Ative Diretory) como provedor de identidade.

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
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Usar o ADFS como seu provedor de identidade

Você pode atualizar os metadados do ADFS antes ou depois da atualização do certificado SAML 2.0 pela Adobe Workfront. Se você optar por atualizar os metadados do ADFS antes da atualização do certificado SAML 2.0 pela Workfront, serão necessárias etapas adicionais.

* [Atualizar os metadados de ADFS](#update-your-adfs-metadata)
* [Forçar a atualização dos metadados do ADFS](#force-your-adfs-metadata-to-update)

### Atualizar os metadados de ADFS {#update-your-adfs-metadata}

Para definir que os metadados do ADFS sejam atualizados automaticamente, conclua as etapas desta seção.

Por padrão, o ADFS é configurado para verificar automaticamente se há atualizações para todos os metadados de confiança da terceira parte confiável; no entanto, o padrão é definido para sondar somente a cada 24 horas. Você pode alterar esse valor com comandos do powershell.

1. Faça logon no servidor ADFS e abra o Console de Gerenciamento do ADFS.
1. No painel esquerdo, expanda **ADFS 2.0,** em seguida expandir **Relações de confiança.**

1. Clique em **Terceiras Partes Confiáveis** pasta.
1. Selecione o objeto de confiança de terceira parte confiável configurado anteriormente para ser usado com o Workfront e, no painel direito, clique em **Atualização de Metadados de Federação**.
1. (Condicional) Se essa opção estiver esmaecida (o que significa que o objeto de confiança da terceira parte confiável foi configurado anteriormente usando um arquivo de metadados), conclua o seguinte.

   1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

   1. Clique em **Sistema** > **Logon único (SSO)**.

   1. Clique em **Editar configurações.**
   1. Clique em **Editar configuração** e selecione **SAML 2.0** no **Tipo** lista suspensa.

   1. Copie o **URL de metadados**, que deve ser semelhante ao seguinte:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. No servidor ADFS, clique com o botão direito do mouse no objeto de confiança da terceira parte confiável configurado anteriormente e clique em **Propriedades.**
   1. Clique em **Monitoramento** e cole o URL que você copiou do Workfront na **URL de metadados de federação da terceira parte confiável** campo.

   1. Marque as opções para **Monitorar terceira parte confiável** e **Atualizar a terceira parte confiável automaticamente**.

   1. Clique em **OK.**
   1. Selecione o objeto de confiança de terceira parte confiável configurado anteriormente para ser usado com o Workfront e, no painel direito, clique em **Atualização de Metadados de Federação.**

1. Clique em **OK** para ignorar a mensagem sobre alguns conteúdos nos metadados de federação não suportados pelo ADFS 2.0.
1. Abertura **Módulos Do Windows Powershell.**
1. Depois que todos os módulos forem carregados, execute o seguinte comando no powershell:

   `Get-ADFSProperties`

1. Procure o valor ao lado de **Intervalo de monitoramento.**

   Será um número que representa o número de minutos entre as enquetes. O padrão deve ser 1440 (1440 minutos = 24 horas).

1. Defina um novo valor executando o seguinte comando no powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   Isso altera o intervalo de monitoramento de cada 24 horas para cada minuto. Você pode alterar 1 para outro valor maior se quiser que ele seja sondado com menos frequência.

1. Para verificar se isso está funcionando corretamente, use o **Visualizador de eventos** para procurar as seguintes informações nos registros do ADFS2.0:

   **ID de evento 156 e 157**

### Forçar a atualização dos metadados do ADFS {#force-your-adfs-metadata-to-update}

Para atualizar os metadados do ADFS, conclua as etapas da seção a seguir.

Para forçar a troca de metadados entre o Workfront e seu provedor SAML 2.0 ao usar os Serviços de Federação do Ative Diretory (ADFS):

>[!NOTE]
>
>Algumas dessas alterações podem precisar ser feitas pelo departamento de TI.

1. Efetue logon no servidor ADFS e abra o **Console de Gerenciamento do ADFS**.
1. No painel esquerdo, expanda **ADFS 2.0**, em seguida, expandir **Relações de confiança**.

1. Clique em **Terceiras Partes Confiáveis** pasta.
1. Selecione o objeto de confiança de terceira parte confiável configurado anteriormente para ser usado com o Workfront e, no painel direito, clique em **Atualização de Metadados de Federação**.

   Se essa opção estiver esmaecida e não puder ser selecionada, conclua o seguinte:

   (A opção fica esmaecida somente quando o objeto de confiança da terceira parte confiável foi configurado anteriormente usando um arquivo de metadados.)

   1. No Workfront, na área Configuração, copie o **URL de metadados** na tela de configuração do Workfront Single Sign-On.

      Para acessar as informações do **URL de metadados**:

      1. Clique em **Configuração** próximo ao canto superior direito do Adobe Workfront na Barra de navegação global.
      1. Clique em > **Sistema** > **Logon único (SSO)**.
      1. Clique em **Editar configurações.**
      1. Clique em **Editar configuração** e selecione **SAML 2.0** no **Tipo** lista suspensa.
      1. Copie o **URL de metadados**, que deve ser semelhante ao seguinte:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. No servidor ADFS, clique com o botão direito do mouse no objeto de confiança da terceira parte confiável configurado anteriormente e clique em **Propriedades.**
   1. Clique em **Monitoramento** e cole o URL que você copiou do Workfront na **URL de metadados de federação da terceira parte confiável** campo.
   1. Marque as opções para **Monitorar terceira parte confiável** e **Atualizar a terceira parte confiável automaticamente**.
   1. Clique em **OK**.
   1. Selecione o objeto de confiança de terceira parte confiável configurado anteriormente para ser usado com o Workfront e, no painel direito, clique em **Atualização de Metadados de Federação.**

1. Clique em **OK** para ignorar a mensagem sobre alguns conteúdos nos metadados de federação não suportados pelo ADFS 2.0.
1. Clique em **Atualizar** para concluir a atualização dos metadados de federação.

Usuários que têm permissão para acessar o Workfront por meio da tela de logon nativa usando credenciais de logon do Workfront (isso pode ser configurado na página de perfil de cada usuário na **Access** ) podem fazer logon usando o nome de usuário e a senha do Workfront navegando até o seguinte URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Uso de outros provedores de identidade

Ao usar provedores de identidade diferentes do ADFS (como Ping, Okta ou Centrify), você deve fazer upload novamente dos metadados do Workfront para seu provedor de identidade.

Para obter mais informações sobre como obter um novo URL de metadados do Workfront, consulte [Atualizar os metadados de ADFS](#update-your-adfs-metadata).

Para obter informações adicionais sobre o uso dos Serviços de Federação do Ative Diretory (ADFS) com SAML 2.0 no Workfront, consulte [Configurar o Adobe Workfront com SAML 2.0 usando ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
