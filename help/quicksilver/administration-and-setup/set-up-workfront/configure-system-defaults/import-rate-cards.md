---
title: Importar cartões de taxa de um modelo
description: Você pode usar um arquivo de modelo para criar seus cartões de taxa no Excel e importá-los para o Adobe Workfront.
author: Lisa
hide: true
hidefromtoc: true
exl-id: debe90e7-08c2-4385-96fb-8d349dec6741
source-git-commit: e94cbfd9c503936539dbe011e787533222896202
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 0%

---

# Importar cartões de taxa de um modelo

Você pode usar um arquivo de modelo para criar seus cartões de taxa no Excel e importá-los para o Adobe Workfront, em vez de adicionar todas as funções de trabalho e taxas manualmente.

Para ver os cartões de taxa de exemplo descritos neste artigo, baixe o [arquivo de amostra](https://experienceleague.adobe.com/en/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/import-rate-cards/assets/rate-cards-sample.zip).

## Regras importantes para trabalhar com o arquivo de modelo

* Informe a Função da Ordem de Produção OU a Categoria de Recurso Não Mão-de-Obra, mas não ambas.
* A sequência de cartões de taxa na guia RATE_RTCRD deve corresponder à ordem dos cartões na guia RTCRD (1 para o primeiro, 2 para o segundo etc.).
* A Data inicial e a Data final devem seguir os formatos permitidos.
* Os cartões de taxa podem ser importados sem taxas e atualizados posteriormente.
* Os atributos personalizados (agência, centro de custos etc.) podem variar. Consulte o administrador do sistema para obter os requisitos exatos.
* As linhas excluídas no modelo não excluirão registros existentes no sistema.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
   <p>[!UICONTROL Plano]</p>
   </td> 
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

   * **Data de Término** (opcional): a data em que a taxa deixa de ser efetiva.

     Essa data deve seguir os mesmos formatos compatíveis que a data inicial.

     Para obter mais informações, consulte [Requisitos de formatação de data](#date-formatting-requirements), abaixo.

   * **Valor** (opcional): o valor da taxa numérica, por exemplo, 150. O valor padrão é 0.
   * **Moeda** (opcional): a moeda da taxa, por exemplo, USD, EUR, GBP. O padrão é a moeda do sistema.
   * **Bloqueado** (opcional): indica se a taxa está bloqueada. Os valores válidos são Verdadeiro ou Falso.
   * **Atributos** (opcional/personalizado): as últimas colunas (Agência, Local, Centro de Custos, etc.) são Atributos de Taxa que diferem de acordo com a configuração do cliente. Esses campos são personalizáveis e podem variar de acordo com o ambiente do cliente.

     Exemplo: Agência = &quot;1: Agência,&quot; Local = &quot;Chicago,&quot; Centro de Custo = &quot;22: Centro de Custo&quot;

### Requisitos de formatação de data

Ao preparar os dados do cartão de taxa para importação, você deve garantir que as colunas de data estejam formatadas como **Geral**, não como **Data**.

Se as colunas forem definidas no formato Data, o sistema poderá interpretar incorretamente os valores durante o processo de importação, resultando em erros ou uploads com falha. O uso do formato Geral preserva a representação numérica ou de texto bruta da data, permitindo que o sistema valide e aplique os valores corretamente.

Seguir essas etapas evitará problemas desnecessários e garantirá uma importação perfeita e precisa de dados de taxa.

1. Antes de salvar ou fazer upload do arquivo, selecione as colunas de data na planilha.
1. Alterar o formato da coluna para **Geral**.
1. Verifique se os valores ainda são exibidos corretamente (por exemplo, 01/01/2025 ou 2025-01-01).

## Importar o arquivo de modelo

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Clique em **Novo cartão de taxa** e em **Importar novos cartões de taxa**.
1. Arraste e solte o arquivo na caixa de diálogo ou clique em Selecionar um arquivo do Excel para navegar até o arquivo no computador.
1. Clique em **Iniciar importação**.

   Se não houver problemas com o arquivo, uma mensagem de confirmação será exibida e os novos cartões de taxa serão exibidos na lista.

1. Se o arquivo contiver problemas, uma mensagem de erro será exibida. Clique em **Ver problemas** para exibir os problemas em uma tela separada.

   Você deve corrigir os problemas no arquivo do Excel e importá-lo novamente antes que os cartões de taxa existam no Workfront.
