---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: calcular diferenças de data e hora"
description: Você pode calcular a diferença entre o seguinte - EDIT ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '650'
ht-degree: 0%

---

# Exibir: calcular diferenças de data e hora

>[!IMPORTANT]
>
>Você não pode calcular a diferença de data e hora no Adobe Workfront entre dois objetos diferentes do mesmo tipo. Por exemplo, você não pode calcular a diferença de data e hora entre duas datas em dois projetos, tarefas ou problemas diferentes.

Você pode calcular a diferença entre o seguinte:

* A diferença de data e hora entre dois campos de data no mesmo objeto
* A diferença de data e hora entre o campo em um objeto e outro campo no objeto pai

>[!TIP]
>
>Esses cálculos exibem o número de dias entre as duas datas. O resultado é exibido em dias. O carimbo de data e hora no campo de data também é levado em conta, e o número de dias pode ser seguido por decimais se os carimbos de data e hora não corresponderem. Se a tarefa foi concluída com atraso, o número de dias é exibido como um valor negativo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Calcular a diferença de data e hora entre dois campos de data no mesmo objeto

Por exemplo, você pode calcular a diferença entre a Data de conclusão planejada e a Data de conclusão real de uma tarefa.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. Ir para uma lista de tarefas.
1. No **Exibir** clique em **Nova visualização**.

1. Clique em **Adicionar coluna** e comece digitando &quot;Data de conclusão planejada&quot; na caixa **Mostrar nesta coluna** e selecione-o quando ele for exibido na lista.

1. Clique em **Adicionar coluna** e comece digitando &quot;Data de conclusão efetiva&quot; na caixa **Mostrar nesta coluna** e selecione-o quando ele for exibido na lista.

1. Clique em **Adicionar coluna** e, em seguida, clique em **Alternar para modo de texto**.

1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-o pelo seguinte código:

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. Clique em **Salvar**, depois **Salvar visualização**.

## Calcular a diferença de data e hora entre o campo em um objeto e outro campo em um objeto pai

Para obter uma lista de objetos e seus pais, consulte a seção &quot;Entendendo a Interdependência e a Hierarquia de Objetos&quot; em [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Por exemplo, você pode calcular a diferença entre a Data de conclusão planejada de uma tarefa e a Data de conclusão planejada de sua tarefa pai ou do projeto em que a tarefa está.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. Ir para uma lista de tarefas.
1. No **Exibir** clique em **Nova visualização**.

1. Clique em **Adicionar coluna** e comece digitando &quot;Data de conclusão planejada do projeto&quot; ou &quot;Data de conclusão pai&quot; na **Mostrar nesta coluna** e selecione-o quando ele for exibido na lista.

1. Clique em **Adicionar coluna** e comece digitando &quot;Data de conclusão planejada&quot; na caixa **Mostrar nesta coluna** e selecione-o quando ele for exibido na lista.

1. Clique em **Adicionar coluna** e, em seguida, clique em **Alternar para modo de texto**.

1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar o texto**.
1. Remova o texto localizado na **Modo de texto** e substitua-a por um dos seguintes códigos:

   * Para exibir a diferença entre a Data de conclusão planejada do projeto e a da tarefa:

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * Para exibir a diferença entre a Data de Conclusão Planejada da tarefa-pai e a da tarefa:

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. Clique em **Salvar**, depois **Salvar visualização**.
