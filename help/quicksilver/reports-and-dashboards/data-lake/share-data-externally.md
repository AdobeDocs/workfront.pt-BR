---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Estabelecer uma conexão com a conexão de dados do Workfront
description: O Workfront Data Connect permite usar os dados do Workfront de sua organização com ferramentas de business intelligence ou armazená-los em um data warehouse externo.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: d7577da92b7efda5cba26104efac124f75a271c5
workflow-type: tm+mt
source-wordcount: '1489'
ht-degree: 4%

---

# Estabelecer uma conexão com a conexão de dados do Workfront

O Workfront Data Connect permite usar os dados do Workfront de sua organização com ferramentas de business intelligence ou armazená-los em um data warehouse externo.

Para conectar seu data lake do Data Connect a um produto externo, primeiro você deve criar uma conexão conforme descrito em [Criar uma conta ou conexão de leitor para o Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). Em seguida, adicione os IPs necessários ao incluo na lista de permissões conforme descrito em [Adicionar IPs ao incluo na lista de permissões](#add-ips-to-the-allowlist) abaixo.

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
>Depois que uma entrada é adicionada ao incluo na lista de permissões IP, todos os outros endereços IP não são mais permitidos. Verifique se você inseriu todos os endereços IP necessários, para as experiências de criação e leitura da ferramenta de visualização, antes de tentar usar a ferramenta. Caso contrário, você poderá encontrar um erro relacionado às credenciais inválidas.
>
>Se você não tiver endereços IP incluídos em seu incluo na lista de permissões, mas ainda tiver problemas para se conectar a uma ferramenta de BI, verifique a configuração do servidor proxy para a ferramenta de BI.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar IPs ao incluo na lista de permissões

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **Instalação**.

1. No painel esquerdo, clique em **Sistema** > **Conexão de Dados**.

1. Clique na guia **IPs permitidos** e clique no botão **Adicionar um endereço IP ao seu Incluo na lista de permissões**.

1. Insira um nome para o endereço IP na **descrição do Endereço IP** e insira o endereço IP (ou bloco CIDR) da ferramenta que deseja usar no **Endereço IP** e clique em **Adicionar IP ao Incluo na lista de permissões**.

   ![Adicionar endereço IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Encontrar intervalos de IP do Azure para o Microsoft Power BI

O tráfego do Microsoft Power BI para o Data Connect não vem de um único endereço fixo. O Microsoft publica os intervalos IP como blocos CIDR em um arquivo JSON grande. Esta seção explica como localizar os blocos para as regiões que você realmente usa.

### Fonte oficial do Microsoft para intervalos IP e etiquetas de serviço da Azure

A Microsoft publica a lista na [página de download da Azure IP Ranges and Service Tags - Nuvem pública](https://www.microsoft.com/en-us/download/details.aspx?id=56519). Baixe o arquivo JSON atual (o nome do arquivo geralmente é semelhante a `ServiceTags_Public_YYYYMMDD.json`). Atualize o incluo na lista de permissões quando o Microsoft atualizar o arquivo ou quando problemas de conectividade forem exibidos após uma alteração no Microsoft.

>[!NOTE]
>
>O arquivo JSON é muito grande, geralmente bem acima de 100.000 linhas. Isso é esperado. As seções necessárias são pequenas; você não precisa ler todo o arquivo manualmente.

### Power BI versus Power Query online

Os clientes às vezes relatam &quot;Power BI&quot; quando o tráfego realmente vem de componentes do Power Query que a Microsoft trata como um serviço Azure separado na lista de etiquetas de serviço.

| Se os usuários... | Procure essa etiqueta de serviço no JSON |
|----------------|---------------------------------------|
| Use o serviço Power BI, os conjuntos de dados hospedados no Azure ou os gateways no contexto da nuvem | `PowerBI` (entradas globais ou regionais como `PowerBI.EastUS`) |
| Use o Power Query Online, fluxos de dados de nuvem e experiências semelhantes | `PowerQueryOnline` (entradas globais ou regionais como `PowerQueryOnline.EastUS`) |

Se sua organização usar ambas as experiências, adicione blocos CIDR de `PowerBI` e `PowerQueryOnline` para as mesmas regiões. Se você adicionar apenas um, alguns usuários ainda poderão ser bloqueados, enquanto outros terão êxito.

### Escolha tags regionais, não o agregado global

O arquivo JSON contém uma única entrada de todas as regiões para `PowerBI` (e de forma semelhante para `PowerQueryOnline`) que agrega muitas regiões e pode conter centenas de blocos CIDR, além de muitas entradas regionais menores, como `PowerBI.WestUS`, `PowerBI.WestUS2` e `PowerBI.WestUS3`. Cada objeto regional lista apenas os prefixos dessa região, normalmente no máximo dezenas de linhas. Não recomendamos adicionar a entrada global, a menos que você tenha um requisito documentado para permitir cada região do Azure. Para a maioria dos clientes do Data Connect, as entradas regionais são o padrão correto. Adicione as regiões onde seus locatários e usuários do Power BI realmente operam, além de um pequeno buffer para redundância (por exemplo, uma região secundária de recuperação de desastres usada por sua empresa).

### Escolha suas regiões

Os nomes de região da Microsoft no arquivo são parecidos com `EastUS`, `WestEurope`, `GermanyWestCentral` e assim por diante. Use as regiões onde a capacidade do Power BI e os usuários estão hospedados, não onde o escritório está, embora eles geralmente se alinhem.

| Cenário | O que adicionar primeiro |
|----------|-------------------|
| Uso nos Estados Unidos | Comece com as regiões dos EUA que você sabe que seu locatário usa (exemplos: `EastUS`, `EastUS2`, `WestUS`, `WestUS2`, `WestUS3`, `CentralUS`, `SouthCentralUS`). Você não precisa de cada região dos EUA, a menos que o administrador do Microsoft confirme a hospedagem de várias regiões. |
| Uso na União Europeia ou no Reino Unido | Comece com as regiões que seu locatário usa (exemplos: `WestEurope`, `NorthEurope`, `FranceCentral`, `GermanyWestCentral`, `SwedenCentral`, `UKSouth`). Adicione mais somente se os usuários abrangerem regiões adicionais da Microsoft. |
| Uso no Pacífico Asiático | Adicione as regiões confirmadas pelo administrador do Power BI ou do Azure (exemplos: `SoutheastAsia`, `EastAsia`, `AustraliaEast`). |
| Várias regiões geográficas | Adicione ambos os conjuntos de marcas regionais (por exemplo, UE e EUA) para cada serviço (`PowerBI` e `PowerQueryOnline` se ambos estiverem em uso). |
| Região desconhecida | Pergunte ao administrador do Microsoft 365 ou Power BI quais regiões do Azure hospedam seus recursos do Power BI ou revise as configurações de locatário do administrador do Power BI. Se você precisar desbloquear rapidamente para testes, adicione um par de regiões conhecidas (por exemplo, `EastUS` e `WestUS`) e monitore, então restrinja a lista depois de confirmar. |

### Localizar intervalos IP e adicioná-los ao incluo na lista de permissões

Para coletar intervalos IP do Microsoft e adicioná-los ao seu incluo na lista de permissões Workfront:

1. Abra a [página de download de Intervalos IP e Marcas de Serviço da Azure - Nuvem Pública](https://www.microsoft.com/en-us/download/details.aspx?id=56519), baixe o arquivo JSON de Marcas de Serviço e salve-o localmente (por exemplo, `Downloads\ServiceTags_Public_YYYYMMDD.json`).

1. Abra o arquivo em qualquer editor que manipule bem grandes JSON, como o Visual Studio Code.

1. Use o recurso Localizar do editor (`Ctrl+F` no Windows ou `Cmd+F` no macOS) para localizar objetos JSON cujo campo `"name"` seja igual a uma marca de serviço como `PowerBI.EastUS` ou `PowerQueryOnline.WestEurope`. Pesquisas úteis:

   * `"name": "PowerBI.WestUS"` — vá para o Power BI do Oeste dos EUA.
   * `"name": "PowerQueryOnline.WestUS"` — vá para o Power Query Online do Oeste dos EUA.
   * `PowerBI.` — lista todas as tags regionais da Power BI e, em seguida, refine o nome da sua região.

1. Em cada objeto correspondente, encontre a matriz chamada `addressPrefixes`. Cada cadeia de caracteres nessa matriz é um bloco CIDR (por exemplo, `20.59.79.96/27` ou um prefixo IPv6). Esses são os valores que você adicionará ao seu incluo na lista de permissões Workfront.

1. Adicione cada CIDR ao incluo na lista de permissões Workfront conforme descrito em [Adicionar IPs ao incluo na lista de permissões](#add-ips-to-the-allowlist) neste artigo. Aguarde alguns minutos para a propagação da política, se o ambiente armazenar em cache as regras.

1. No Power BI ou Power Query Online, execute uma pequena consulta de teste em Data Connect para validar a conexão. Se falhar, capture o tempo aproximado e pergunte à sua equipe de rede se a negação está alinhada com os intervalos ausentes. Verifique novamente se você perdeu `PowerQueryOnline` quando apenas `PowerBI` foi adicionado, o que é uma lacuna comum.

Por exemplo, se o administrador do Microsoft confirmar que as cargas de trabalho do Power BI usam West US, West US 2 e West US 3, e os usuários usam Power BI e Power Query Online, você abrirá seis objetos: `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3` e o `PowerQueryOnline.<Region>` correspondente para cada um, em seguida, copie `addressPrefixes` de todos os seis.

### Referência de estrutura JSON

Cada bloco de service tag tem a seguinte aparência conceitual. Os arquivos reais incluem mais metadados.

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

A matriz `addressPrefixes` contém os blocos CIDR que você adicionará ao Workfront. Outros campos são para cenários de rede do Azure e não se aplicam aqui.

### Manter o incluo na lista de permissões

* O Microsoft altera os intervalos de IP ao longo do tempo. Quando o Microsoft publicar um arquivo JSON atualizado, atualize ou compare seu incluo na lista de permissões periodicamente, especialmente depois de um incidente de conectividade.
* Se o ambiente for compatível com IPv6 para Snowflake e o Microsoft listar prefixos IPv6, inclua-os se a política de segurança permitir IPv6. Caso contrário, fale com a equipe de rede.

## Remover um endereço IP do incluo na lista de permissões

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
