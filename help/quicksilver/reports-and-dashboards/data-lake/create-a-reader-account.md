---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Criar uma conta de leitor para o Snowflake
description: Para acessar os dados do Data Connect, primeiro você deve criar uma conta do Snowflake Reader.
author: Nolan
feature: Reports and Dashboards
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Criar uma conta ou conexão de leitor para o Snowflake

Para acessar os dados do Data Connect, primeiro você deve criar uma conta de leitor (ou serviço) do Snowflake para sua organização e, em seguida, criar uma nova conexão para cada usuário ou ferramenta que você deseja que tenha acesso ao Data Connect.

Depois de criar uma conexão, você pode encontrar sua URL e nome de usuário associados clicando nela na página **Conexão de Dados** (**Menu principal** > **Configuração** > **Sistema** > **Conexão de Dados**) na guia **Conexões Existentes**.

Para obter informações sobre como usar uma conexão recém-criada com um produto externo, consulte [Estabelecer uma conexão com o Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td><p>Incluído nos seguintes planos:</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>O Workfront Data Connect não está disponível para planos Workfront herdados.</p> 
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma conta de leitor

Você deve criar uma nova conta do Snowflake Reader para sua organização antes de começar a criar conexões.

>[!IMPORTANT]
>
>Esse processo deve ser concluído apenas uma vez por organização. Se o botão **Criar Conta da Reader** não estiver presente no local descrito abaixo, sua conta de leitor já foi criada.

Para criar uma conta de leitor:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Conexão de Dados**.

1. Clique no botão **Criar Conta do Reader** para começar a criar a conta de leitor de sua organização. O processo é automático, mas pode levar alguns minutos para ser concluído.

1. Uma vez concluída, uma janela de caixa de diálogo será exibida explicando que sua conta de leitor está ativa agora. Atualize a página do navegador para obter acesso ao botão **Criar nova conexão**.

![Caixa de diálogo criada para a conta do Reader](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-reader-account-created.png)

## Criar uma conexão

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Conexão de Dados**.

1. Clique em **Criar nova conexão**

1. Na janela exibida, digite um nome para sua conexão em **Descrição da referência da conexão** e um nome de usuário em **Usuário da conexão** e clique em **Gerar conexão**.

   ![Criar nova conexão](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Uma **Senha padrão** será gerada, bem como uma URL na qual seus dados possam ser visualizados por meio do Snowflake. Você precisará usar a senha em conjunto com o nome de usuário que escolheu para fazer logon no Snowflake pela primeira vez, para garantir que você mantenha um registro dela, bem como do URL. Marque a caixa alegando que você fez isso e clique em **Fechar**.

   ![Senha da conta padrão](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Abra o Snowflake usando um navegador para navegar até a URL da etapa anterior, digite o nome de usuário selecionado e a senha padrão da etapa anterior e clique em **Entrar**.

1. Depois de entrar pela primeira vez com êxito, você será solicitado a escolher uma nova senha. Digite uma senha de sua escolha nos campos **Nova senha** e **Confirmar senha** e clique em **Enviar**.

   ![Redefinir senha do Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Agora você pode usar seu nome de usuário e nova senha para acessar seu data lake Connect no Snowflake ou a ferramenta de visualização de negócios de sua escolha.

## Revogar uma conta de leitor

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Acesso a Dados**.

1. Clique no ícone da lixeira ![Ícone Excluir](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à direita da conta que você deseja revogar.

1. Na janela exibida, marque a caixa para confirmar e clique em **Excluir**.
