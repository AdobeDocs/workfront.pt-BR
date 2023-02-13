---
title: Visão geral da condição do projeto e do tipo de condição
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: A condição do projeto é uma representação visual de como o projeto está progredindo. É uma variável relatável determinada pela relação entre as datas planejada, projetada e estimada do projeto.
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# Visão geral da condição do projeto e do tipo de condição

A condição do projeto é uma representação visual de como o projeto está progredindo. É uma variável relatável determinada pela relação entre as datas planejada, projetada e estimada do projeto.

## Visão geral da condição do projeto

Considere o seguinte ao entender a Condição de um projeto:

* Como proprietário do projeto, você pode decidir se a Condição de um projeto é definida manual ou automaticamente. A Condição de um projeto pode ser definida das seguintes maneiras:

   * Manualmente, por usuários que têm acesso para Gerenciar o projeto e quando o Tipo de condição do projeto é definido como Manual.
   * Automaticamente, pela Adobe Workfront, quando o Tipo de condição do projeto estiver definido como Status de progresso. O Status de Progresso do projeto é determinado pelo progresso das tarefas no projeto. Para obter informações sobre o Status de Andamento do projeto, consulte [Visão geral do status de progresso do projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   Para obter informações sobre como atualizar o Tipo de condição do projeto, consulte [Definir o tipo de condição de um projeto](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Ao permitir que o Workfront faça uma estimativa automática da Condição do projeto, recomendamos que você use antecessores em suas tarefas para que o progresso da tarefa reflita no progresso real e no Status de Andamento do projeto.
* Como proprietário do projeto, você pode alterar o projeto para usar um Tipo de condição manual em vez de usar o Status de progresso, alterando o Tipo de condição de Status de progresso para Manual.

   >[!NOTE]
   >
   >Os projetos que estão em qualquer um dos status a seguir são sempre marcados como No Target, independentemente das datas das tarefas e de seu progresso:
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

## Como o Workfront atualiza a condição do projeto com base no status de progresso

Quando o Tipo de condição do projeto estiver definido como Manual, você poderá determinar qual condição do projeto é independente do Status de progresso do projeto.

No entanto, recomendamos que você defina o Tipo de condição do projeto como Status de progresso, para que possa ter uma indicação clara de qual é o progresso real do projeto, com base no progresso de suas tarefas. Para obter informações sobre como a Workfront calcula o Status de Andamento de projetos, consulte [Visão geral do status de progresso do projeto](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Nesse caso, os valores para a Condição do projeto podem ser:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Condição do projeto</td> 
   <td>Status de progresso do projeto</td> 
   <td>Indicador de condição do Workfront</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>No Prazo</td> 
   <td> <li>Quando o Status de Andamento do projeto de Em Tempo, a Condição do projeto é <strong>No Target</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Em Risco</td> 
   <td>Quando o Status de Andamento do projeto é <strong>Bebehind</strong> ou <strong>Em Risco</strong>, a condição do projeto é <strong>Em Risco</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Com problemas</td> 
   <td>Quando o Status de Andamento do projeto é <strong>Atraso</strong>, a condição do projeto é <strong>Em problemas</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>As condições podem ser personalizadas para o seu ambiente, portanto, você pode encontrar mais de três opções para Condição no seu ambiente. Os nomes das Condições podem ser diferentes dos acima enumerados. Para obter informações sobre como personalizar Condições no , consulte o artigo [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## Relatório sobre condição do projeto, atualização da condição do projeto e última nota de condição

Na visualização de um relatório de projeto, é possível mostrar os seguintes campos relacionados à Condição do projeto:

* **Condição do projeto:** Mostra a condição atual do projeto.
* **Atualização da condição do projeto**: Mostra a atualização mais recente que o proprietário do projeto forneceu no fluxo de atualização do projeto, juntamente com a nova Condição.\
   Os comentários feitos nas atualizações de Condição não são exibidos na variável **Atualização de condição** coluna; somente a atualização principal é exibida.

* **Última Nota de Condição**: Exibe a última atualização inserida em um objeto pelo proprietário do objeto. Este campo é útil para exibir a atividade ou interação mais recente do proprietário em um objeto.\
   O **Última Nota de Condição** estiver vazia se o texto da nota da última nota de um objeto tiver sido excluído. Quando uma nova nota é inserida no objeto, ela se torna a última nota e é exibida novamente na coluna .

Para obter informações sobre como criar um relatório, consulte o artigo [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
