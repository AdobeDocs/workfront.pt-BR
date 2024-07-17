---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Criar uma conta de leitor (serviço) para o Snowflake
description: Para acessar os dados no Workfront Data Lake, primeiro você deve criar uma conta de leitor para o Snowflake.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 70d83a10-f926-4229-ac10-7659f2ca5e7a
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 0%

---

# Criar uma conta de leitor (serviço) para o Snowflake

Para acessar os dados do data lake da Workfront, primeiro você deve criar uma conta de leitor de Snowflake (ou serviço) para cada nova conexão. Depois de criar uma conexão, você pode encontrar sua URL e nome de usuário associados clicando nela na página **Acesso aos dados** (**Menu principal** > **Configuração** > **Sistema** > **Acesso aos dados**) na guia **Conexões Existentes**.

Para obter informações sobre como usar uma conexão recém-criada com um produto externo, consulte [Estabelecer uma conexão com o data lake da Workfront](/help/quicksilver/reports-and-dashboards/data-lake/share-data-externally.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>A ser definido</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Criar uma conta de leitor

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Acesso a Dados**.

1. Clique em **Criar nova conexão**

1. Na janela exibida, digite um nome para sua conexão em **Descrição da referência da conexão** e um nome de usuário em **Usuário da conexão** e clique em **Gerar conexão**.

   ![Criar conta de leitor](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. Uma **Senha padrão** será gerada, bem como uma URL na qual seus dados possam ser visualizados por meio do Snowflake. Você precisará usar a senha em conjunto com o nome de usuário que você escolheu para entrar no Snowflake pela primeira vez, para garantir que você mantenha um registro dela, bem como o URL. Marque a caixa alegando que você fez isso e clique em **Fechar**.

   ![Senha da conta padrão](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Abra o Snowflake usando um navegador para navegar até a URL da etapa anterior, digite o nome de usuário selecionado e a senha padrão da etapa anterior e clique em **Entrar**.

1. Depois de entrar pela primeira vez com êxito, você será solicitado a escolher uma nova senha. Digite uma senha de sua escolha nos campos **Nova senha** e **Confirmar senha** e clique em **Enviar**.

   ![Redefinir senha de Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Agora você pode usar seu nome de usuário e nova senha para acessar o data lake da Workfront no Snowflake ou a ferramenta de visualização de negócios de sua escolha.

## Revogar uma conta de leitor

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Acesso a Dados**.

1. Clique no ícone da lixeira ![Ícone Excluir](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à direita da conta que você deseja revogar.

1. Na janela exibida, marque a caixa para confirmar e clique em **Excluir**.
