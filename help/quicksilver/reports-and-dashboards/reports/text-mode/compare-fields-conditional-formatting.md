---
product-area: reporting
navigation-topic: text-mode-reporting
title: Comparar campos na formatação condicional
description: Você pode usar a formatação condicional para comparar dois campos diferentes em uma exibição e destacá-los quando determinados critérios forem atendidos entre os campos.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 1%

---

# Comparar campos na formatação condicional

<!-- Audited: 1/2025 -->

Você pode usar a formatação condicional para comparar dois campos diferentes em uma exibição e destacá-los quando determinados critérios forem atendidos entre os campos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para editar a visualização em um relatório</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões em um relatório para editar a visualização em um relatório</p> <p>Gerenciar permissões para uma exibição</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exemplo: Comparar a Data Inicial Real com a Data Inicial Planejada

Por exemplo, se a Data Inicial Real de uma tarefa for posterior à Data Inicial Planejada, você poderá realçar a coluna Data Inicial Planejada usando a formatação condicional.

Para comparar a Data Inicial Planejada e a Data Inicial Real da tarefa usando a formatação condicional:

1. Ir para uma exibição de tarefa ou um relatório.
1. (Condicional) Se estiver trabalhando com um relatório, na guia **Colunas (Exibição)** do editor de relatórios, clique no cabeçalho da coluna que deseja formatar condicionalmente para selecioná-la.\
   Por exemplo, selecione a coluna **Data de Início Efetivo** se desejar adicionar a formatação condicional a ela comparando os campos Data de Início Planejada e Data de Início Efetivo.

1. Clique em **Opções Avançadas** e em Adicionar uma **Regra para esta Coluna**.

1. Informe os critérios de comparação usando os valores existentes encontrados no construtor e especifique sua formatação condicional.\
   Por exemplo, queremos destacar tarefas em que a Data de Início Efetivo seja posterior (ou posterior) à Data de Início Planejada. Selecione o modificador Maior que e selecione uma data real no campo de data.

   ![Formatação condicional para a data de início real](assets/cond-format-1-350x84.png)

1. (Opcional) Selecione **Aplicar à linha inteira** se desejar aplicar a formatação à linha inteira.
1. Clique em **Salvar**.

1. Selecione a coluna **Data de Início Efetiva** e clique em **Alternar para Modo de Texto**.

1. Clique em **Editar Modo de Texto** e adicione a seguinte linha de texto:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   No nosso exemplo:

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Se você estiver comparando um campo nativo do Workfront, use a sintaxe de camel case para o nome do campo. Se você estiver comparando um campo personalizado, use **DE:Nome Real do Campo** para o campo de nome que você está comparando com o primeiro campo.\
   >Por exemplo, se você estiver comparando a **Data de início efetiva** com um campo personalizado rotulado como **Data de entrega**, adicione a seguinte instrução no código do modo de texto:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Verifique se a linha de código `righttext` corresponde à instrução na linha de código `rightmethod`.

   ![Formatação condicional](assets/cond-format-2-350x171.png)

1. Clique em **Salvar**.
1. Clique em **Salvar + Fechar**.

   A coluna destaca os campos que atendem aos seus critérios.
