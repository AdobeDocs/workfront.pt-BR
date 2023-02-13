---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: calcular diferenças de data e hora'''
description: Você pode calcular a diferença entre o seguinte - EDITAR-ME.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 548dd91f-02bc-43ed-8322-d0facf3488f0
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '633'
ht-degree: 0%

---

# Exibir: calcular diferenças de data e hora

>[!IMPORTANT]
>
>Não é possível calcular a diferença de data e hora no Adobe Workfront entre dois objetos diferentes do mesmo tipo. Por exemplo, não é possível calcular a diferença de tempo e data entre duas datas em dois projetos, tarefas ou problemas diferentes.

Você pode calcular a diferença entre os seguintes itens:

* A diferença de hora e data entre dois campos de data no mesmo objeto
* A diferença de data e hora entre o campo em um objeto e outro campo no objeto pai

>[!TIP]
>
>Esses cálculos exibem o número de dias entre as duas datas. O resultado é exibido em dias. O carimbo de data e hora no campo de data também é considerado e o número de dias pode ser seguido por decimais se os carimbos de data e hora não corresponderem. Se a tarefa tiver sido concluída com atraso, o número de dias será exibido como um valor negativo.

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

## Calcule a diferença de data e hora entre dois campos de data no mesmo objeto

Por exemplo, você pode calcular a diferença entre a Data de Conclusão Planejada e a Data de Conclusão Real de uma tarefa.

![](assets/view-planned-actual-completion-dates-datediff-column-350x92.png)

1. Vá para uma lista de tarefas.
1. No **Exibir** , clique em **Nova exibição**.

1. Clique em **Adicionar coluna** e comece a digitar &quot;Data de conclusão planejada&quot; no **Mostrar nesta coluna** em seguida, selecione-o quando for exibido na lista.

1. Clique em **Adicionar coluna** e comece a digitar &quot;Data de conclusão real&quot; no **Mostrar nesta coluna** em seguida, selecione-o quando for exibido na lista.

1. Clique em **Adicionar coluna**, depois clique em **Alternar para o modo de texto**.

1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a pelo seguinte código:

   ```
   displayname=Planned-Actual Completion Date<br>linkedname=direct<br>querysort=plannedCompletionDate<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({plannedCompletionDate},{actualCompletionDate}),2)<br>valueformat=HTML
   ```

1. Clique em **Salvar**, em seguida **Salvar exibição**.

## Calcule a diferença de data e hora entre o campo em um objeto e outro campo em um objeto pai

Para obter uma lista de objetos e seus pais, consulte a seção &quot;Como entender a interdependência e a hierarquia de objetos&quot; em [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
Por exemplo, você pode calcular a diferença entre a Data de Conclusão Planejada de uma tarefa e a Data de Conclusão Planejada de sua tarefa pai, ou do projeto em que a tarefa está.

![](assets/view-project-planned-task-planned-completion-dates-datediff-column-350x184.png)

1. Vá para uma lista de tarefas.
1. No **Exibir** , clique em **Nova exibição**.

1. Clique em **Adicionar coluna** e comece a digitar &quot;Data de conclusão planejada do projeto&quot; ou &quot;Data de conclusão pai&quot; na **Mostrar nesta coluna** em seguida, selecione-o quando for exibido na lista.

1. Clique em **Adicionar coluna** e comece a digitar &quot;Data de conclusão planejada&quot; no **Mostrar nesta coluna** em seguida, selecione-o quando for exibido na lista.

1. Clique em **Adicionar coluna**, depois clique em **Alternar para o modo de texto**.

1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Remova o texto que você encontrar no **Modo de texto** e substitua-a por um dos seguintes códigos:

   * Para exibir a diferença entre a Data de conclusão planejada do projeto e a da tarefa:

      ```
      displayname=Project Planned Completion - Task Planned Completion (Days)<br>textmode=true<br>valueexpression=ROUND(DATEDIFF({project}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>valueformat=HTML
      ```

   * Para exibir a diferença entre a Data de Conclusão Planejada da tarefa pai e a da tarefa:

      ```
      valueexpression=ROUND(DATEDIFF({parent}.{plannedCompletionDate},{plannedCompletionDate}),2)<br>textmode=true<br>valueformat=HTML<br>displayname=Parent Planned Completion - Planned Completion (Days)
      ```

1. Clique em **Salvar**, em seguida **Salvar exibição**.
