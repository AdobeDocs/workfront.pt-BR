---
product-area: reporting
navigation-topic: text-mode-reporting
title: Comparar campos na formatação condicional
description: É possível usar a formatação condicional para comparar dois campos diferentes em uma exibição e destacá-los quando determinados critérios forem atendidos entre os campos.
author: Nolan
feature: Reports and Dashboards
exl-id: da4447ba-6e76-4701-88ee-87a30393bed9
source-git-commit: 89a6d856f9f87a67b6a2ccfb4282f9f6200b977c
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Comparar campos na formatação condicional

É possível usar a formatação condicional para comparar dois campos diferentes em uma exibição e destacá-los quando determinados critérios forem atendidos entre os campos.

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
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar a exibição em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para editar a exibição em um relatório</p> <p>Gerenciar permissões para uma exibição</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exemplo: Comparar Data Inicial Real e Data Inicial Planejada

Por exemplo, se a Data inicial real de uma tarefa for posterior à Data inicial planejada, você poderá realçar a coluna Data inicial planejada usando formatação condicional.

Para comparar a Data Inicial Planejada e a Data Inicial Real da tarefa usando a formatação condicional:

1. Vá para uma exibição de tarefa ou relatório.
1. (Condicional) Se estiver trabalhando com um relatório, da variável **Colunas (Exibir)** , clique no cabeçalho da coluna que deseja formatar condicionalmente para selecioná-la.\
   Por exemplo, selecione a variável **Data de início real** para adicionar a formatação condicional, compare os campos Data inicial planejada e Data inicial real .

1. Clique em **Opções avançadas** e, em seguida, clique em Adicionar um **Regra para esta Coluna**.

1. Insira os critérios de comparação usando valores existentes encontrados no construtor e especifique a formatação condicional.\
   Por exemplo, queremos destacar tarefas nas quais a Data de início real é posterior à Data de início planejada (ou maior que). Selecione o modificador Maior que e selecione uma data real no campo de data.\
     ![](assets/cond-format-1-350x84.png)

1. (Opcional) Selecione **Aplicar a linha inteira** se desejar aplicar a formatação à linha inteira.
1. Clique em **Adicionar regra**, em seguida **Concluído**.

1. Selecione o **Data de início real** e, em seguida, clique em **Alternar para o modo de texto**.

1. **Clique para editar texto** em seguida, adicione a seguinte linha de texto:

   ```
   styledef.case.0.comparison.rightmethod= <field to compare>
   ```

   Em nosso exemplo: 

   ```
   styledef.case.0.comparison.rightmethod=plannedStartDate
   ```

   >[!NOTE]
   >
   >Se estiver comparando um campo nativo do Workfront, use a sintaxe de caso de camelo para o nome do campo. Se você estiver comparando um campo personalizado, use **DE:Nome real do campo** para o campo de nome que você está comparando com o primeiro campo.\
   >Por exemplo, se você estiver comparando a variável **Data de início real** com um campo personalizado rotulado **Data de entrega**, adicione a seguinte instrução no código do modo de texto:
   >
   >`styledef.case.0.comparison.rightmethod=DE:Delivery Date`

1. Certifique-se de que `righttext` a linha de código corresponde à declaração na variável `rightmethod` linha de código.

   ![](assets/cond-format-2-350x171.png)

1. Clique em **Salvar**.
1. Clique em **Salvar + Fechar**.

   A coluna destaca os campos que atendem aos seus critérios.
