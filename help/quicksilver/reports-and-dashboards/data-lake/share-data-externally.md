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
source-git-commit: 91371c862be6f3b99f0450ff359f601dc913dc0c
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 1%

---

# Estabelecer uma conexão com o data lake da Workfront

O data lake da Workfront permite usar os dados Workfront de sua organização com ferramentas de business intelligence ou armazená-los em um data warehouse externo.

Para conectar seus dados do data lake da Workfront a um produto externo, primeiro adicione os IPs necessários ao arquivo, conforme descrito em [Adicionar IPs ao arquivo de incluir na lista de permissões inclui na lista de permissões](#add-ips-to-the-allowlist) abaixo. Além disso, a maioria dos produtos exigirá informações adicionais sobre seu data lake para estabelecer uma conexão:

| Nome do campo | Valor |
|---------------|-------------|
| Servidor | A URL da conexão, sem a parte `https://` (encontrada na página **Acesso a dados** no Workfront*) |
| Porta | `443` |
| Banco de dados | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Esquema | `WF` |
| Função | `READER_ROLE` |
| Nome de usuário | O nome de usuário escolhido ao criar a conexão (encontrado na página **Acesso aos dados** no Workfront*) |
| Senha | A senha escolhida no primeiro logon de Snowflake* |

*Para obter informações sobre onde encontrar a página **Acesso a dados** contendo suas conexões de data lake, consulte [Criar uma conta de leitor (serviço) para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Depois que uma entrada é adicionada ao arquivo de inclui na lista de permissões IP, todos os outros endereços IP não são mais permitidos. Verifique se você inseriu todos os endereços IP necessários, para as experiências de criação e leitura da ferramenta de visualização, antes de tentar usar a ferramenta. Caso contrário, você poderá encontrar um erro relacionado às credenciais inválidas.
>
>Se você não tiver nenhum endereço IP incluído na sua inclui na lista de permissões do, mas ainda tiver problemas para se conectar a uma ferramenta de BI, verifique a configuração do servidor proxy para a ferramenta de BI.


## Adicionar IPs ao incluo na lista de permissões

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Acesso a Dados**.

1. Incluir na lista de permissões Clique na guia **IPs permitidos** e, em seguida, clique no botão **Adicionar um endereço IP à pesquisa**.

1. Incluir na lista de permissões Insira um nome para o endereço IP em **descrição do Endereço IP** e insira o endereço IP (ou bloco CIDR) da ferramenta que deseja usar em **Endereço IP** e clique em **Adicionar IP à pesquisa**.

   ![Adicionar endereço IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Remover um endereço IP da inclui na lista de permissões

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Acesso a Dados**.

1. Clique na guia **IPs permitidos** e clique no ícone da lixeira ![Ícone Excluir](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à direita do endereço IP que você deseja remover.

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
