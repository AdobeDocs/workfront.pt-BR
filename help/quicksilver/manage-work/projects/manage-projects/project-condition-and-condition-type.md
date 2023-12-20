---
title: Visão geral da condição do projeto e do tipo de condição
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: A Condição do projeto é uma representação visual de como o projeto está progredindo. É uma variável reportável determinada pela relação entre as datas planejadas, projetadas e estimadas do projeto.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Visão geral da condição do projeto e do tipo de condição

<!-- Audited: 12/2023 -->

A Condição do projeto é uma representação visual de como o projeto está progredindo. É uma variável reportável determinada pela relação entre as datas planejadas, projetadas e estimadas do projeto.

## Visão geral da Condição do projeto

Considere o seguinte ao entender a Condição de um projeto:

* Como proprietário do projeto, você pode decidir se a Condição de um projeto é definida manual ou automaticamente. A condição de um projeto pode ser definida das seguintes maneiras:

   * Manualmente pelos usuários que têm acesso ao Gerenciamento do projeto e quando o Tipo de condição do projeto está definido como Manual.
   * Automaticamente pela Adobe Workfront, quando o Tipo de condição do projeto está definido como Status de progresso. O status do progresso do projeto é determinado pelo progresso das tarefas no projeto. Para obter informações sobre o status do progresso do projeto, consulte [Visão geral do status de progresso do projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

  Para obter informações sobre como atualizar o Tipo de condição do projeto, consulte [Definir o tipo de condição de um projeto](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Ao permitir que o Workfront estime a Condição do projeto automaticamente, recomendamos usar predecessores em suas tarefas para que o progresso da tarefa reflita o progresso real e o Status de progresso do projeto.
* Como proprietário de um projeto, você pode alterar o projeto para usar um Tipo de Condição Manual em vez de usar o Status do Progresso alterando o Tipo de Condição de Status do Progresso para Manual.

  >[!NOTE]
  >
  >Os projetos com qualquer um dos status a seguir são sempre marcados como No destino, independentemente das datas das tarefas e do seu progresso:
  >
  >* Ideia
  >* Solicitado(a)
  >* Aprovado
  >* Rejeitado

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Como o Workfront atualiza a condição do projeto com base no status do progresso

Quando o Tipo de condição do projeto é definido como Manual, você pode determinar qual é a Condição do projeto independentemente do Status de progresso do projeto.

No entanto, recomendamos que você defina o Tipo de condição do projeto como Status de progresso para que possa ter uma indicação clara de qual é o progresso real do projeto, com base no progresso de suas tarefas. Para obter informações sobre como o Workfront calcula o status do progresso dos projetos, consulte [Visão geral do status de progresso do projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Nesse caso, os valores da Condição do projeto podem ser:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Condição do projeto</strong></td> 
   <td><strong>Status de Progresso do Projeto</strong></td> 
   <td><strong>Indicador de Condição Workfront</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>No Prazo</td> 
   <td>Quando o status do progresso do projeto é No prazo, a condição do projeto é <strong>No Destino</strong>. </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Em Risco</td> 
   <td>Quando o status do progresso do projeto é <strong>Atrás</strong> ou <strong>Em Risco</strong>, a Condição do projeto é <strong>Em Risco</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Com problemas</td> 
   <td>Quando o status do progresso do projeto é <strong>Atrasado</strong>, a Condição do projeto é <strong>Com Problemas</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>As condições podem ser personalizadas para seu ambiente, portanto, você pode encontrar mais de três opções de Condição em seu ambiente. Os nomes das Condições podem ser diferentes dos listados acima. Para obter informações sobre como personalizar as Condições no, consulte o artigo [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Relatório de Condição do Projeto, Atualização de Condição do Projeto e Última Nota de Condição

No modo de exibição de um relatório de projeto, é possível mostrar os seguintes campos relacionados à Condição do projeto:

* **Condição do projeto:** Mostra a Condição atual do projeto.
* **Atualização da Condição do Projeto**: mostra a atualização mais recente que o proprietário do projeto forneceu no fluxo de atualização do projeto, juntamente com a nova Condição.\
  Comentários feitos em Atualizações de condição não são exibidos no **Atualização da Condição** coluna; somente a atualização principal é exibida.

* **Última Nota de Condição**: exibe a última atualização inserida em um objeto pelo proprietário do objeto. Este campo é útil para exibir a atividade ou interação mais recente do proprietário em um objeto.\
  A variável **Última Nota de Condição** fica vazia se o texto da nota da última nota de um objeto tiver sido excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna.

Para obter informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
