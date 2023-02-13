---
title: Criar ou personalizar severidades de problemas
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Seus usuários podem usar severidades para definir a gravidade de um problema. Você pode personalizar qualquer uma das cinco severidades padrão existentes no Adobe Workfront ou criar uma nova severidade para seus usuários.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# Criar ou personalizar severidades de problemas

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Seus usuários podem usar severidades para definir a gravidade de um problema. Você pode personalizar qualquer uma das cinco severidades padrão existentes no Adobe Workfront ou criar uma nova severidade para seus usuários.

>[!NOTE]
>
>Tarefas e projetos não têm severidade.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Severidades de problemas embutidas

A Workfront tem cinco severidades de problemas integradas:

* Cosmética
* Causa Confusão
* Problema com Solução
* Problema Sem Solução
* Erro Fatal

<p>Você pode editar o seguinte para essas severidades:</p>

* Nome
* Cor

   A cor de uma gravidade é preservada em um relatório de gráfico, se você agrupar os resultados por Gravidade da ocorrência. Para obter informações sobre relatórios de gráfico, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Qual gravidade é o padrão

   Para obter mais informações sobre severidades padrão, consulte [Criar ou editar uma gravidade de problema](#create-or-edit-an-issue-severity) neste artigo.
* Descrição
* Se uma severidade está oculta no Workfront

   Para obter mais informações sobre como ocultar uma severidade, consulte [Criar ou editar uma gravidade de problema](#create-or-edit-an-issue-severity")

* Excluir uma severidade

   Ao fazer isso, você deve selecionar uma severidade de substituição.

## Criar ou editar uma gravidade de problema {#create-or-edit-an-issue-severity}

Como administrador da Workfront, você pode criar e editar severidades de edição para atender às necessidades dos usuários.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Preferências do projeto** > **Severidades**.

1. Se estiver criando uma nova severidade, clique em **Adicionar uma nova gravidade**.
1. Configure as seguintes opções para a nova gravidade ou edite-as para uma existente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome da Severidade</td> 
      <td>Digite um nome para a gravidade</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chave</td> 
      <td>Aumente ou diminua o nível de gravidade, originalmente atribuído pela Workfront, para a gravidade.
      <p>O número de Importância para cada gravidade deve ser exclusivo. O número mais alto corresponde ao nível mais alto de gravidade.</p> <p>Não é possível editar esse número depois de salvar a gravidade.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Escolha uma cor para a gravidade.</p> 
      <p>A cor da gravidade é usada nos relatórios do gráfico quando você agrupa os resultados por Gravidade da ocorrência. Para obter informações sobre relatórios de gráfico, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Adicionar um gráfico a um relatório</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Severidade Padrão</td> 
      <td>Selecione a severidade que deseja que o Workfront selecione automaticamente todos os problemas recém-criados.</p>
      <p>Cosmética é a severidade padrão para problemas no Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição para a gravidade para explicar sua função.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> Oculte uma severidade que não é mais necessária. 
      <p>Uma severidade oculta não é exibida em nenhum lugar do Workfront, de modo que os usuários não podem escolhê-la em razão de seus problemas.</p> 
      <p><b>IMPORTANTE</b>: Em vez de excluir severidades que você não deseja mais usar, sugerimos que você as oculte. Dessa forma, você mantém todos os seus dados históricos sobre objetos já preenchidos com a severidade, impedindo que as pessoas usem a severidade no futuro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Altere a ordem de listagem de suas severidades arrastando-as e soltando-as na ordem desejada.

   Isso altera a ordem em que são exibidos para problemas. Não altera a variável **Importância** número.

1. Clique em **Salvar**.

Para obter mais informações sobre como usar severidades ao trabalhar com problemas, consulte [Atualizar gravidade do problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
