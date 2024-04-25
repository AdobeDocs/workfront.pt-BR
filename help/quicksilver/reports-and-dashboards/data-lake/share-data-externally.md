---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Estabelecer uma conexão com o data lake da Workfront
description: O data lake da Workfront permite usar os dados Workfront de sua organização com ferramentas populares de business intelligence ou armazená-los em um data warehouse externo.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# Estabelecer uma conexão com o data lake da Workfront

O data lake da Workfront permite usar os dados Workfront de sua organização com ferramentas de business intelligence ou armazená-los em um data warehouse externo.

Para conectar seus dados do data lake da Workfront incluir na lista de permissões a um produto externo, primeiro adicione os IPs necessários ao arquivo, conforme descrito em [Adicionar IPs ao incluo na lista de permissões](#add-ips-to-the-allowlist) abaixo. Além disso, a maioria dos produtos exigirá informações adicionais sobre seu data lake para estabelecer uma conexão:

| Nome do campo | Valor |
|---------------|-------------|
| Servidor | O URL da conexão, sem o parâmetro `https://` porção (encontrada no **Acesso aos dados** página no Workfront*) |
| Porta | `443` |
| Banco de dados | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Esquema | `WF` |
| Função | `READER_ROLE` |
| Nome de usuário | O nome de usuário escolhido ao criar a conexão (encontrado no **Acesso aos dados** página no Workfront*) |
| Senha | A senha escolhida no primeiro logon de Snowflake* |

*Para obter informações sobre onde encontrar o **Acesso aos dados** contendo suas conexões de data lake, consulte [Criar uma conta de leitor (serviço) para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Depois que uma entrada é adicionada ao arquivo de inclui na lista de permissões IP, todos os outros endereços IP não são mais permitidos. Verifique se você inseriu todos os endereços IP necessários, para as experiências de criação e leitura da ferramenta de visualização, antes de tentar usar a ferramenta. Caso contrário, você poderá encontrar um erro relacionado às credenciais inválidas.

## Adicionar IPs ao incluo na lista de permissões

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Configuração**.

1. No painel esquerdo, clique em **Sistema** > **Acesso aos dados**.

1. Clique no link **IPs permitidos** e, em seguida, clique na guia **Adicionar um endereço IP ao seu Incluo na lista de permissões** botão.

1. Insira um nome para o endereço IP em **Descrição do endereço IP** e insira o endereço IP da ferramenta que deseja usar no **Endereço IP** e, em seguida, clique em **Adicionar IP ao Incluo na lista de permissões**.

   ![Adicionar endereço IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Remover um endereço IP da inclui na lista de permissões

1. Clique em **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível), clique no link **[!UICONTROL Menu principal]** ícone ![Menu principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Configuração**.

1. No painel esquerdo, clique em **Sistema** > **Acesso aos dados**.

1. Clique no link **IPs permitidos** e, em seguida, clique no ícone da lixeira ![Ícone Excluir](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à direita do endereço IP que deseja remover.

1. Na janela exibida, marque a caixa para confirmar e clique em **Excluir**.

## Compartilhar dados com ferramentas de Business Intelligence

Várias ferramentas comuns de business intelligence estão listadas abaixo; os links levarão você ao site de documentação do serviço para saber mais sobre como se conectar ao seu data lake.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Armazenar dados em um data warehouse externo

Vários data warehouses comuns estão listados abaixo; os links o levarão para o site de documentação de cada serviço, onde você poderá saber mais sobre como se conectar ao seu data lake.

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
