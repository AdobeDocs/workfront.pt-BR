---
content-type: reference
product-area: reports and dashboards
navigation-topic: data lake
title: Criar uma conta de leitor (serviço) para o Snowflake
description: Para acessar os dados no Workfront Data Lake, primeiro você deve criar uma conta de leitor para o Snowflake.
author: Nolan
feature: Reports and Dashboards
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7d24659833f0ac0ceeecb245358f2ade8bd08a17
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

# Criar uma conta de leitor (serviço) para o Snowflake

Para acessar os dados do data lake da Workfront, primeiro você deve criar uma conta de leitor para o Snowflake. Incluir na lista de permissões Além disso, você deve adicionar IPs ao para procurar quaisquer ferramentas externas que planeje conectar aos dados.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Ultimate</td> 
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

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Configuração**.

1. No painel esquerdo, clique em **Sistema** > **Acesso aos dados**.

1. Clique em **Criar nova conexão**

1. Na janela exibida, digite um nome para a conexão no campo **Descrição da referência de conexão** e um nome de usuário no **Usuário de conexão** e, em seguida, clique em **Gerar conexão**.

   ![Criar conta do leitor](/help/quicksilver/reports-and-dashboards/data-lake/assets/new-reader-connection.png) {width="500"}

1. A **Senha padrão** serão gerados, bem como um URL no qual seus dados podem ser visualizados por meio do Snowflake. Você precisará usar a senha em conjunto com o nome de usuário que você escolheu para entrar no Snowflake pela primeira vez, para garantir que você mantenha um registro dela, bem como o URL. Marque a caixa solicitando que você o fez e clique em **Fechar**.

   ![Senha da conta padrão](/help/quicksilver/reports-and-dashboards/data-lake/assets/default-password-reader-account.png) {width="500"}

1. Abra o Snowflake usando um navegador para navegar até o URL da etapa anterior, digite o nome de usuário selecionado e a senha padrão da etapa anterior e clique em **Fazer logon**.

1. Depois de entrar pela primeira vez com êxito, você será solicitado a escolher uma nova senha. Insira uma senha de sua escolha nas **Nova senha** e **Confirmar senha** e clique em **Enviar**.

   ![Redefinir senha Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/assets/reset-snowflake-password.png) {width="300"}

1. Agora é possível usar seu nome de usuário e nova senha para acessar o data lake da Workfront no Snowflake.

## Adicionar IPs ao incluo na lista de permissões

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Configuração**.

1. No painel esquerdo, clique em **Sistema** > **Acesso aos dados**.

1. Clique no link **IPs permitidos** e, em seguida, clique na guia **Adicionar um endereço IP ao seu Incluo na lista de permissões** botão.

   ![Adicionar endereço IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

1. Insira um nome para o endereço IP em **Descrição do endereço IP** e insira o endereço IP da ferramenta que deseja usar no **Endereço IP** e, em seguida, clique em **Adicionar IP ao Incluo na lista de permissões**.

## Revogue uma conta de leitor ou remova um endereço IP da inclui na lista de permissões

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Configuração**.

1. No painel esquerdo, clique em **Sistema** > **Acesso aos dados**.

1. Clique no ícone de lixeira ![Ícone Excluir](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à direita da conta que deseja revogar.

   OU

   Clique no link **IPs permitidos** e, em seguida, clique no ícone da lixeira ![Ícone Excluir](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à direita do endereço IP que deseja remover.

1. Na janela exibida, marque a caixa para confirmar e clique em **Excluir**.
