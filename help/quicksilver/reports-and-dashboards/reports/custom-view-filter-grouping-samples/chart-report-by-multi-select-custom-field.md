---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: Gráfico de um relatório por um campo personalizado de várias seleções
description: Não é possível criar um gráfico de relatório por um campo personalizado de várias seleções. É necessário criar um campo calculado adicional que faça referência ao campo personalizado de várias seleções para também fazer o gráfico do relatório pelo valor do campo personalizado de várias seleções.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: cda77319-dce6-409d-8f59-53838820cafb
source-git-commit: addcff71ff067be22e9ee80f997af545293fa5db
workflow-type: tm+mt
source-wordcount: '809'
ht-degree: 0%

---

# Gráfico de um relatório por um campo personalizado de várias seleções

<span class="preview">As informações destacadas nesta página se referem à funcionalidade ainda não disponível no geral. Ele está disponível para todos os clientes no ambiente de Visualização e para um grupo selecionado de clientes no ambiente de Produção.</span>

Não é possível criar um gráfico de relatório por um campo personalizado de várias seleções. É necessário criar um campo calculado adicional que faça referência ao campo personalizado de várias seleções para também fazer o gráfico do relatório pelo valor do campo personalizado de várias seleções.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar, você deve criar um campo personalizado calculado que mostre os valores selecionados do campo personalizado de várias seleções. Para obter informações, consulte o [Criar um campo personalizado calculado que faça referência a um campo personalizado de várias seleções](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field) neste artigo.

## Gráfico um relatório por campos personalizados de seleção múltipla

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this moved to its own article, linked in the Note above!)</p>
-->

Não é possível criar um gráfico em um relatório referenciando um campo personalizado de várias seleções. Em vez disso, é possível criar um campo calculado que registre os valores do campo personalizado de várias seleções em um determinado objeto e agrupe pelo campo calculado. 

* [Criar um campo personalizado calculado que faça referência a um campo personalizado de várias seleções](#build-a-calculated-custom-field-that-references-a-multi-select-custom-field)
* [Criar um gráfico que faça referência a um campo personalizado calculado](#build-a-chart-that-references-a-calculated-custom-field)

### Criar um campo personalizado calculado que faça referência a um campo personalizado de várias seleções {#build-a-calculated-custom-field-that-references-a-multi-select-custom-field}

Para criar um campo calculado que faça referência a um campo personalizado de várias seleções, você deve ter os seguintes pré-requisitos:

* Crie o campo personalizado de várias seleções em um formulário personalizado.\
   Para obter informações sobre como criar formulários personalizados e adicionar campos personalizados a eles, consulte o artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

* Anexe o formulário personalizado aos objetos.
* Preencha o campo personalizado de várias seleções com um valor em cada objeto.

Para criar o campo personalizado calculado que faz referência ao campo personalizado de várias seleções:

1. Crie um formulário personalizado ou edite um formulário existente.\
   Para obter informações sobre como criar formulários personalizados, consulte o artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. Selecione o objeto ou objetos que você planeja usar com o formulário personalizado.
1. Clique em **Adicionar um campo**, em seguida **Calculado** para adicionar o campo personalizado de várias seleções ao formulário.

1. No **Rótulo** nomeie o novo campo calculado para indicar que ele faz referência ao campo personalizado de várias seleções.\
   Por exemplo: &quot;Campo de seleção múltipla calculado.&quot;

1. No **Cálculo** digite o seguinte código:

   ```
   {DE:Multi-select Custom Field}
   ```

1. Substitua &quot;Campo personalizado de seleção múltipla&quot; pelo nome real do seu campo personalizado de seleção múltipla, como ele aparece no Workfront.

   ![](assets/calculated-multi-select-custom-field-nwe-350x223.png)

1. (Opcional) Se o campo personalizado de seleção múltipla já estiver nesse formulário e se esse formulário já estiver anexado a objetos, ative a opção **Atualizar cálculos anteriores** opção.\
   Isso garante que o novo campo seja automaticamente preenchido com o valor do campo personalizado de várias seleções, à medida que ele é adicionado aos formulários anexados aos objetos.

1. Clique em **Concluído**.
1. Clique em **Salvar +Fechar**.

### Criar um gráfico que faça referência a um campo personalizado calculado {#build-a-chart-that-references-a-calculated-custom-field}

1. (Opcional) Para garantir que todos os campos calculados pelos quais você deseja criar um gráfico sejam preenchidos com valores, selecione todos os objetos no relatório que contêm o formulário personalizado com o campo personalizado de várias seleções e o campo personalizado calculado, em seguida, clique em **Editar**.
1. (Opcional e condicional) Ative a opção **Recalcular expressões personalizadas** e clique em **Salvar alterações**.\
   ![](assets/recalculate-custom-expressions-350x259.png)

   >[!NOTE]
   >
   ><span class="preview">Essa opção foi eliminada da edição de projetos em massa no ambiente de Visualização.  Você ainda pode recalcular expressões para projetos em massa clicando em **Mais** ![](assets/more-icon-45x33.png) na parte superior de uma lista de projetos, em seguida **Recalcular expressões**. </span>


1. Vá para o relatório onde deseja adicionar o gráfico do campo calculado que faz referência ao campo personalizado de várias seleções.
1. Clique em **Ações de Relatório**, em seguida **Editar**.

1. Selecione o <strong>Agrupamentos</strong> e, em seguida, clique em <strong>Adicionar agrupamento</strong>.
1. Adicione o<strong>Campo de seleção múltipla calculada</strong> você criou como seu agrupamento.
1. Selecione o <strong>Gráfico</strong> e adicionar um gráfico ao relatório.<br>Para obter informações sobre como adicionar um gráfico a um relatório, consulte a seção <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md#add-a-chart" class="MCXref xref">Adicionar um gráfico a um relatório</a> no artigo <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.
1. Selecione o <strong>Campo de seleção múltipla calculada</strong> como um dos campos a serem exibidos no gráfico.
1. Clique em <strong>Salvar + Fechar</strong>.<br>O relatório exibe os resultados agrupados pelo Campo de seleção múltipla calculada em um gráfico.
