---
user-type: administrator
product-area: system-administration
navigation-topic: single-sign-on-in-workfront
title: Atualize os metadados SAML 2.0 no seu provedor de identidade
description: Você pode atualizar metadados SAML 2.0 em seu provedor de identidade.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 75cd0ab5-8d76-40a4-96a8-00e9f0f4fec6
source-git-commit: 96f1d50024605328713ca2019f3b726e27dc569c
workflow-type: tm+mt
source-wordcount: '961'
ht-degree: 0%

---

# Atualize os metadados SAML 2.0 no seu provedor de identidade

{{important-admin-console-onboard}}

As seções a seguir descrevem como atualizar os metadados SAML (Security Assertion Markup Language) 2.0 ao usar os Serviços de Federação do Ative Diretory (ADFS) como seu provedor de identidade.

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

## Usar o ADFS como seu provedor de identidade

Você pode atualizar seus metadados ADFS antes que o Adobe Workfront atualize o certificado SAML 2.0 ou posterior. Se optar por atualizar os metadados ADFS antes de o Workfront atualizar o certificado SAML 2.0, são necessárias etapas adicionais.

* [Atualizar os metadados do ADFS](#update-your-adfs-metadata)
* [Forçar a atualização dos metadados do ADFS](#force-your-adfs-metadata-to-update)

### Atualizar os metadados do ADFS {#update-your-adfs-metadata}

Para definir seus metadados ADFS para atualizar automaticamente, complete as etapas desta seção.

Por padrão, o ADFS é configurado para verificar automaticamente se há atualizações em todos os metadados de confiança da parte confiadora; no entanto, o padrão é definir para pesquisar somente a cada 24 horas. Você pode alterar esse valor com comandos powershell.

1. Faça logon no servidor ADFS e abra o Console de Gerenciamento ADFS.
1. No painel à esquerda, expanda **ADFS 2.0,** em seguida, expanda **Relacionamentos de Confiança.**

1. Clique no botão **Confianças de terceiros confiáveis** pasta.
1. Selecione a confiança da terceira parte confiável que você configurou anteriormente para ser usada com o Workfront e, no painel direito, clique em **Atualização dos metadados de federação**.
1. (Condicional) Se essa opção estiver esmaecida (o que significa que a confiança da parte confiadora foi configurada anteriormente usando um arquivo de metadados), preencha o seguinte.

   1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

   1. Clique em **Sistema** > **Logon único (SSO)**.

   1. Clique em **Editar configurações.**
   1. Clique em **Editar configuração**, em seguida selecione **SAML 2.0** no **Tipo** lista suspensa.

   1. Copie o **URL de metadados**, que devem ser semelhantes ao seguinte:

      `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`

   1. No servidor ADFS, clique com o botão direito do mouse na confiança da entidade confiadora que você configurou anteriormente e clique em **Propriedades.**
   1. Clique no botão **Monitoramento** em seguida, cole o URL que você copiou do Workfront na **URL de metadados de federação da terceira parte confiável** campo.

   1. Marque as opções para **Monitorar parte confiadora** e **Atualizar entidade confiadora automaticamente**.

   1. Clique em **Ok.**
   1. Selecione a confiança da terceira parte confiável que você configurou anteriormente para ser usada com o Workfront; em seguida, no painel direito, clique em **Atualização de metadados de federação.**

1. Clique em **OK** para ignorar a mensagem sobre algum conteúdo nos metadados da federação que não é suportado pelo ADFS 2.0.
1. Abrir **Módulos do Windows Powershell.**
1. Depois que todos os módulos forem carregados, execute o seguinte comando no powershell:

   `Get-ADFSProperties`

1. Procure o valor ao lado de **Intervalo de monitoramento.**

   Será um número que representa o número de minutos entre as pesquisas. O padrão deve ser 1440 (1440 minutos = 24 horas).

1. Defina um novo valor executando o seguinte comando no powershell:

   `Set-ADFSProperties -MonitoringInterval 1`

   Isso altera o intervalo de monitoramento de 24 horas para cada minuto. Você pode alterar o valor 1 para outro valor maior se quiser que ele pesquise com menos frequência.

1. Para verificar se isso está funcionando corretamente, use o **Visualizador de eventos** para procurar as seguintes informações nos logs ADFS2.0:

   **ID de evento 156 e 157**

### Forçar a atualização dos metadados do ADFS {#force-your-adfs-metadata-to-update}

Para atualizar os metadados ADFS, conclua as etapas da seção a seguir.

Para forçar a troca de metadados entre o Workfront e seu provedor SAML 2.0 ao usar os Serviços de Federação do Ative Diretory (ADFS):

>[!NOTE]
>
>Algumas dessas alterações podem precisar ser feitas pelo departamento de TI.

1. Faça logon no servidor ADFS e abra o **Console de Gerenciamento ADFS**.
1. No painel à esquerda, expanda **ADFS 2.0**, em seguida expanda **Relacionamentos de Confiança**.

1. Clique no botão **Confianças de terceiros confiáveis** pasta.
1. Selecione a confiança da terceira parte confiável que você configurou anteriormente para ser usada com o Workfront e, no painel direito, clique em **Atualização dos metadados de federação**.

   Se essa opção estiver esmaecida e não puder ser selecionada, preencha o seguinte:

   (A opção fica esmaecida somente quando a confiança da parte confiadora foi configurada anteriormente usando um arquivo de metadados.)

   1. No Workfront, na área Configuração, copie o **URL de metadados** na tela de configuração do Logon único da Workfront.

      Para acessar as informações do **URL de metadados**:

      1. Clique em **Configuração** próximo ao canto superior direito do Adobe Workfront na Barra de navegação global.
      1. Clique em > **Sistema** > **Logon único (SSO)**.
      1. Clique em **Editar configurações.**
      1. Clique em **Editar configuração**, em seguida selecione **SAML 2.0** no **Tipo** lista suspensa.
      1. Copie o **URL de metadados**, que devem ser semelhantes ao seguinte:

         `https://<yourdomain>.my.workfront.com/sso/downloadSAML2MetaData`
   1. No servidor ADFS, clique com o botão direito do mouse na confiança da entidade confiadora que você configurou anteriormente e clique em **Propriedades.**
   1. Clique no botão **Monitoramento** em seguida, cole o URL que você copiou do Workfront na **URL de metadados de federação da terceira parte confiável** campo.
   1. Marque as opções para **Monitorar parte confiadora** e **Atualizar entidade confiadora automaticamente**.
   1. Clique em **OK**.
   1. Selecione a confiança da terceira parte confiável que você configurou anteriormente para ser usada com o Workfront e, no painel direito, clique em **Atualização de metadados de federação.**


1. Clique em **OK** para ignorar a mensagem sobre algum conteúdo nos metadados da federação que não é suportado pelo ADFS 2.0.
1. Clique em **Atualizar** para concluir a atualização dos metadados da federação.

Usuários que têm permissão para acessar o Workfront por meio da tela de logon nativa usando credenciais de logon do Workfront (isso pode ser configurado na página de perfil de cada usuário na variável **Acesso** ) pode fazer logon usando seu nome de usuário e senha do Workfront navegando até o seguinte URL: `https://<yourdomain>.my.workfront.com/Workfront/login.cmd`.

## Uso de outros provedores de identidade

Ao usar provedores de identidade diferentes de ADFS (como Ping, Okta ou Centrrify), você deve fazer upload novamente dos metadados do Workfront para seu provedor de identidade.

Para obter mais informações sobre como obter um novo URL de metadados do Workfront, consulte [Atualizar os metadados do ADFS](#update-your-adfs-metadata).

Para obter informações adicionais sobre o uso do Ative Diretory Federation Services (ADFS) com SAML 2.0 no Workfront, consulte [Configurar o Adobe Workfront com o SAML 2.0 usando ADFS](../../../administration-and-setup/add-users/single-sign-on/configure-workfront-saml-2-adfs.md).
