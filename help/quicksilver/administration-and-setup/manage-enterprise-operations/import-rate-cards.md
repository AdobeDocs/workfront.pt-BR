---
user-type: administrator
product-area: system-administration;setup
title: Importar cartões de taxa de um modelo
description: Você pode usar um arquivo de modelo para criar seus cartões de taxa no Excel e importá-los para o Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: debe90e7-08c2-4385-96fb-8d349dec6741
source-git-commit: aa774419e65e9e4a5785382d3cb2b22bdb0389c9
workflow-type: tm+mt
source-wordcount: '1812'
ht-degree: 2%

---

# Importar cartões de taxa de um modelo

Você pode usar um arquivo de modelo para criar seus cartões de taxa no Excel e importá-los para o Adobe Workfront, em vez de adicionar todas as funções de trabalho e taxas manualmente.

Para ver os cartões de taxa de exemplo descritos neste artigo, baixe o [arquivo de amostra](assets/rate-cards-sample.zip).

Para obter mais informações sobre cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Regras importantes para trabalhar com o arquivo de modelo

* Informe a Função da Ordem de Produção OU a Categoria de Recurso Não Mão-de-Obra, mas não ambas.
* A sequência de cartões de taxa na guia RATE_RTCRD deve corresponder à ordem dos cartões na guia RTCRD (1 para o primeiro, 2 para o segundo etc.).
* A Data inicial e a Data final devem seguir os formatos permitidos.
* Os cartões de taxa podem ser importados sem taxas e atualizados posteriormente.
* Atributos personalizados (agência, centro de custos etc.) pode variar. Consulte o administrador do sistema para obter os requisitos exatos.
* As linhas excluídas no modelo não excluirão registros existentes no sistema.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Padrão]</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a [!UICONTROL Rate Cards]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Preencha o arquivo de modelo

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Clique em **Novo cartão de taxa** e em **Baixar modelo do Excel**.
1. Siga os prompts do navegador para salvar o arquivo de modelo no seu computador.
1. Abra o arquivo de modelo no Excel.

   >[!TIP]
   >
   > Salve o arquivo com um novo nome se desejar manter o arquivo de modelo vazio e usá-lo novamente mais tarde.

   O modelo tem duas guias. Ambas as guias devem ter as informações corretas para importar os cartões de taxa com êxito.

   * RTCRD: Definir os cartões de taxa (informações básicas)
   * RATE_RTCRD: Defina as taxas detalhadas associadas a cada cartão de taxa

### Preencha a guia RTCRD (Configuração de cartão de taxa)

Crie e liste todos os cartões de taxa nesta guia. Cada linha representa um cartão de taxa.

![Guia RTCRD no arquivo de modelo de importação de cartão de taxa](assets/rate-card-import-template-tab1.png)

1. Especifique as informações para um cartão de taxa em cada linha:

   * **Nome** (obrigatório): o nome do cartão de taxa, como &quot;Cobrança Global 2025&quot;.

     Esse nome é o identificador principal do cartão de taxa. Cada cartão de tarifa deve ter um nome exclusivo.

   * **Descrição** (opcional): uma descrição de texto de forma livre do cartão de taxa. Use-a para descrever a finalidade, o escopo ou a validade, por exemplo, &quot;Aplica-se a projetos da América do Norte&quot;.
   * **Empresa** (opcional): pode ser o nome ou a ID da empresa. A importação reconhecerá ambos.

     Exemplo: Coffesta ou _68c0234e00000541dd8c0757723daa68_

   * **Grupo** (opcional): pode ser o nome do grupo ou a ID do grupo. A importação reconhecerá ambos.

     Exemplo: Marketing ou _68c0234e00000541dd8c0757723daa68_

   * **Campos personalizados** (opcional): você pode adicionar mais colunas com nomes de campos personalizados se seu ambiente tiver requisitos específicos.

   >[!NOTE]
   >
   >* No mínimo, você deve digitar o Nome de cada cartão de tarifa.
   >* Cada cartão de taxa recebe automaticamente um número de sequência com base em sua posição de linha. Por exemplo, o primeiro cartão de taxa definido (na linha 2) é a sequência 1, o próximo é 2 e assim por diante. Esses números de sequência são usados na guia RATE_RTCRD para anexar taxas.

### Preencha a guia RATE_RTCRD (Configuração de Taxas)

Defina todas as taxas que pertencem aos cartões de taxa nesta guia.

Cada linha na guia define uma taxa específica. Você pode criar várias taxas no mesmo cartão de taxa repetindo a sequência do cartão de taxa.

Certifique-se de que as datas não se sobreponham, a menos que seja o esperado.

![Guia RATE_RTCRD no arquivo de modelo de importação de cartão de taxa](assets/rate-card-import-template-tab2.png)

1. Especifique as informações para uma taxa em cada linha:

   * **Nome** (obrigatório): um rótulo para a linha de taxa.

     A prática recomendada é reutilizar o nome do cartão de taxa para maior clareza, como &quot;Faturamento global 2025 - Taxa do desenvolvedor&quot;.

   * **Referência do Cartão de Taxa** (obrigatório): o número de sequência do cartão de taxa ao qual essa taxa pertence.

     Se o cartão de taxa foi o primeiro que você listou na guia RTCRD (linha 2), digite 1. Se for o segundo, digite 2 e assim por diante.

   * **Função de Trabalho** (necessária se a Categoria de Recursos Não Mão-de-Obra não for usada): a função de trabalho à qual a taxa se aplica. Pode ser o nome ou a ID da função de trabalho. A importação reconhecerá ambos.

     Exemplo: Designer ou _68c0234e00000541dd8c0757723daa68_

   * **Categoria de Recursos Não Mão-de-Obra** (necessária se a Função de Trabalho não for usada): a categoria de recursos não mão de obra à qual a taxa se aplica. Pode ser o nome da categoria ou a ID da categoria. A importação reconhecerá ambos.

     Exemplo: Câmera ou _68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >Você não pode inserir dados nas colunas **Função** e **Categoria de Recursos Não Mão-de-Obra**. Um é obrigatório.

   * **Data de Início** (opcional): a data em que a taxa se torna efetiva.

     A data deve seguir um dos formatos compatíveis (dependendo da sua localização): MM/dd/aaaa, dd/MM/aaaa, MM/DD/AAAA, DD/MM/AAAA, M/d/aa, d/M/aa, aaaa/MM/dd, aaaa/dd/MM, aaaa-MM-dd, aaaa-dd-dd-dd

     Exemplo: 01/01/2025

     Para obter mais informações, consulte [Requisitos de formatação de data](#date-formatting-requirements), abaixo.

   * **End Date** (optional): The date when the rate stops being effective.

     This date must follow the same supported formats as the start date.

     Para obter mais informações, consulte [Requisitos de formatação de data](#date-formatting-requirements), abaixo.

   * **Value** (optional): The numeric rate value, for example 150. O valor padrão é 0.
   * **Currency** (optional): The currency for the rate, for example USD, EUR, GBP. The default is the system currency.
   * **Locked** (optional): Indicates if the rate is locked. Valid values are True or False.
   * **Attributes** (optional / custom): The last columns (Agency, Location, Cost Center, etc.) are Rate Attributes that differ by customer configuration. These are customizable fields and may vary per customer environment.

     Example: Agency = &quot;1: Agency,&quot; Location = &quot;Chicago,&quot; Cost Center = &quot;22: Cost Center&quot;

### Fill out the RSALS (Rate Card Alias) tab

Create and list all of the aliases on this tab. Each row represents one alias.

When the rate card is attached to a project, the alias appears on information such as placeholder assignments, expenses, and reports, instead of the internal job role name. Only one alias can exist for each job role and attribute combination within a single rate card.

An alias is added to the system, but it is not connected to a job role based on the information on this tab.

![RSALS tab on rate card import template file](assets/rsals-tab-rate-card-import.png)

1. Enter the name of an alias on each row.

   Only enter one alias name per row: a job role alias, a non-labor resource category alias, or an expense type alias.

### Fill out the RCRMET_RTCRD_RSALS (Rate Card Metadata) tab

On this tab you can define the connections between resources and aliases for a specific rate card.

![RCRMET_RTCRD_RSALS tab on rate card import template file](assets/rcrmet-tab-rate-card-import.png)

1. Enter the information on each row:

   * **Rate Card** (required): The name or the sequence number of the rate card that the resource and alias belong to. The rate card must be listed on the RTCRD tab.

     For a sequence number: If the rate card was the first one you listed on the RTCRD tab (row 2), enter 1. Se for o segundo, digite 2 e assim por diante.

   * **Job Role** (required if Expense Type and Non-Labor Resource Category are not used): The job role that the alias is connected to. Pode ser o nome ou a ID da função de trabalho. A importação reconhecerá ambos.

     Exemplo: Designer ou _68c0234e00000541dd8c0757723daa68_

   * **Expense Type** (required if Job Role and Non-Labor Resource Category are not used): The expense type that the alias is connected to. This can be either the expense type name or the expense type ID. A importação reconhecerá ambos.

     Example: Travel or _68c0234e00000541dd8c0757723daa68_

   * **Non-Labor Resource Category** (required if Job Role and Expense Type are not used): The non-labor resource category that the alias is connected to. Pode ser o nome da categoria ou a ID da categoria. A importação reconhecerá ambos.

     Exemplo: Câmera ou _68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >You cannot enter all three of the **Job Role**, **Expense Type**, and **Non-Labor Resource Category** columns. Um é obrigatório.

   * **Resource Alias**: The alias entered on the RSALS tab.

### Date formatting requirements

When preparing rate card data for importing, you must ensure that the date columns are formatted as **General**, not as **Date**.

If the columns are set to Date format, the system may misinterpret values during the import process, leading to errors or failed uploads. Using the General format preserves the raw numeric or text representation of the date, allowing the system to correctly validate and apply the values.

Following these steps will prevent unnecessary issues and ensure a smooth and accurate import of rate data.

1. Before saving or uploading the file, select the date columns in the spreadsheet.
1. Alterar o formato da coluna para **Geral**.
1. Verifique se os valores ainda são exibidos corretamente (por exemplo, 01/01/2025 ou 2025-01-01).

## Importar o arquivo de modelo

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Clique em **Novo cartão de taxa** e em **Importar novos cartões de taxa**.
1. Arraste e solte o arquivo na caixa de diálogo ou clique em **Selecionar um arquivo do Excel** para procurar o arquivo no computador.
1. Clique em **Iniciar importação**.

   Se não houver problemas com o arquivo, uma mensagem de confirmação será exibida e os novos cartões de taxa serão exibidos na lista.

1. Se o arquivo contiver problemas, uma mensagem de erro será exibida. Clique em **Ver problemas** para exibir os problemas em uma tela separada.

   Você deve corrigir os problemas no arquivo do Excel e importá-lo novamente antes que os cartões de taxa existam no Workfront.

## Atualizar cartões de taxa existentes

Você pode atualizar as taxas em seus cartões de taxa existentes usando o mesmo modelo do Excel e fazer upload dessas alterações para o Workfront.

Somente a guia RATE_RTCRD (Configuração de Taxas) é necessária para atualizar taxas existentes.

>[!NOTE]
>
>As taxas de upload de um cartão de taxa existente substituem todas as funções e taxas de trabalho atuais no cartão de taxa.
>
>Por exemplo, se você tiver cinco funções de trabalho com taxas no cartão de taxa existente e o arquivo do Excel tiver uma função de trabalho, o cartão de taxa terá uma função de trabalho após o upload. Para manter as outras 5 funções de trabalho e suas taxas no cartão de taxa, você deve incluí-las no arquivo do Excel.

Para atualizar cartões de taxa existentes:

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Clique em **Novo cartão de taxa** e em **Importar atualizações do cartão de taxa**.
1. Arraste e solte o arquivo na caixa de diálogo ou clique em **Selecionar um arquivo do Excel** para procurar o arquivo no computador.
1. Clique em **Iniciar importação**.

   Se não houver problemas com o arquivo, uma mensagem de confirmação será exibida e os novos cartões de taxa serão exibidos na lista.

1. Se o arquivo contiver problemas, uma mensagem de erro será exibida. Clique em **Ver problemas** para exibir os problemas em uma tela separada.

   Você deve corrigir os problemas no arquivo do Excel e importá-lo novamente antes que as atualizações do cartão de taxa existam no Workfront.


