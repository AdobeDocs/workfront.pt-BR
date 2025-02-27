---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Estabelecer uma conexão com o Workfront Data Connect
description: O Workfront Data Connect permite usar os dados do Workfront de sua organização com ferramentas de business intelligence ou armazená-los em um data warehouse externo.
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# Estabelecer uma conexão com o Workfront Data Connect

O Workfront Data Connect permite usar os dados do Workfront de sua organização com ferramentas de business intelligence ou armazená-los em um data warehouse externo.

Para conectar seu data lake do Data Connect a um produto externo, primeiro você deve criar uma conexão conforme descrito em [Criar uma conta ou conexão de leitor para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Em seguida, você deve adicionar os IPs necessários ao incluo na lista de permissões, conforme descrito em [Adicionar IPs ao incluo na lista de permissões](#add-ips-to-the-allowlist) abaixo.

A maioria dos produtos exigirá as seguintes informações sobre seu data lake para estabelecer uma conexão:

| Nome do campo | Valor |
|---------------|-------------|
| Servidor | A URL para a conexão, sem a parte `https://` (encontrada na página **Conexão de dados** no Workfront*) |
| Porta | `443` |
| Banco de dados | `WORKFRONT` |
| Warehouse | `READER_WH` |
| Esquema | `WF` |
| Função | `READER_ROLE` |
| Nome de usuário | O nome de usuário escolhido ao criar a conexão (encontrado na página **Conexão de dados** no Workfront*) |
| Senha | A senha escolhida no primeiro logon do Snowflake* |

*Para obter informações sobre onde encontrar a página **Conexão de Dados** contendo suas conexões, consulte [Criar uma conta de leitor ou conexão para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Depois que uma entrada é adicionada ao arquivo de inclui na lista de permissões IP, todos os outros endereços IP não são mais permitidos. Verifique se você inseriu todos os endereços IP necessários, para as experiências de criação e leitura da ferramenta de visualização, antes de tentar usar a ferramenta. Caso contrário, você poderá encontrar um erro relacionado às credenciais inválidas.
>
>Se você não tiver nenhum endereço IP incluído na sua inclui na lista de permissões do, mas ainda tiver problemas para se conectar a uma ferramenta de BI, verifique a configuração do servidor proxy para a ferramenta de BI.

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
        <li><p>Ultimate</p></li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>O Workfront Data Connect não está disponível para planos Workfront herdados.</p> 
   </td> </td> 
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

## Adicionar IPs ao incluo na lista de permissões

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Conexão de Dados**.

1. Incluir na lista de permissões Clique na guia **IPs permitidos** e, em seguida, clique no botão **Adicionar um endereço IP à pesquisa**.

1. Incluir na lista de permissões Insira um nome para o endereço IP em **descrição do Endereço IP** e insira o endereço IP (ou bloco CIDR) da ferramenta que deseja usar em **Endereço IP** e clique em **Adicionar IP à pesquisa**.

   ![Adicionar endereço IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Remover um endereço IP da inclui na lista de permissões

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Conexão de Dados**.

1. Clique na guia **IPs permitidos** e clique no ícone da lixeira ![Ícone Excluir](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) à direita do endereço IP que você deseja remover.

1. Na janela exibida, marque a caixa para confirmar e clique em **Excluir**.

## Compartilhar dados com ferramentas de Business Intelligence

Várias ferramentas comuns de business intelligence estão listadas abaixo; visite os sites de documentação para saber mais sobre como se conectar ao seu data lake.

* Tableau
* Power BI
* Domo
* SAP HANA

## Armazenar dados em um data warehouse externo

Vários data warehouses comuns estão listados abaixo; visite os sites de documentação deles para saber mais sobre como se conectar ao seu data lake.

* Databricks
* AWS Redshift
