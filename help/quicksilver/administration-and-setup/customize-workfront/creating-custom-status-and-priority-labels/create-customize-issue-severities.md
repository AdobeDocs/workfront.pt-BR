---
title: Criar ou personalizar severidades de problemas
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Seus usuários podem usar severidades para definir a gravidade de um problema. Você pode personalizar qualquer uma das cinco severidades padrão existentes no Adobe Workfront ou criar uma nova severidade para seus usuários.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '565'
ht-degree: 5%

---

# Criar ou personalizar a gravidade de problemas

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Seus usuários podem usar severidades para definir a gravidade de um problema. Você pode personalizar qualquer uma das cinco severidades padrão existentes no Adobe Workfront ou criar uma nova severidade para seus usuários.

>[!NOTE]
>
>Tarefas e projetos não têm severidade.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
     <p>Novo: Padrão</p>
     <p>ou</p>
     <p>Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Severidades de problema embutidas

O Workfront tem cinco severidades de problema integradas:

* Cosmética
* Causa Confusão
* Problema com Solução
* Problema Sem Solução
* Erro Fatal

<p>É possível editar o seguinte para essas severidades:</p>

* Nome
* Cor

  A cor de uma severidade é preservada em um relatório de gráfico, se você agrupar os resultados por Severidade do Problema. Para obter informações sobre relatórios de gráficos, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Qual severidade é o padrão

  Para obter mais informações sobre severidades padrão, consulte [Criar ou editar a severidade de um problema](#create-or-edit-an-issue-severity) neste artigo.
* Descrição
* Se uma severidade está oculta no Workfront

  Para obter mais informações sobre como ocultar uma severidade, consulte [Criar ou editar uma severidade de problema](#create-or-edit-an-issue-severity")

* Excluir uma severidade

  Ao fazer isso, você deve selecionar uma severidade de substituição.

## Criar ou editar a severidade de um problema {#create-or-edit-an-issue-severity}

Como administrador do Workfront, você pode criar e editar severidades de problemas para atender às necessidades dos usuários.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Preferências do projeto** > **Severidades**.

1. Se você estiver criando uma nova severidade, clique em **Adicionar uma Nova Severidade**.
1. Configure as seguintes opções para a nova severidade ou edite-as para uma existente:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome da Severidade</td> 
      <td>Digite um nome para a severidade</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chave</td> 
      <td>Aumentar ou diminuir o nível de seriedade, originalmente atribuído pela Workfront, para a gravidade.
      <p>O número de importância para cada severidade deve ser exclusivo. O número mais alto corresponde ao nível mais alto de severidade.</p> <p>Não é possível editar esse número depois de salvar a severidade.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Escolha uma cor para a severidade.</p> 
      <p>A cor da severidade é usada em relatórios de gráfico quando você agrupa seus resultados por Severidade do Problema. Para obter informações sobre relatórios de gráficos, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Adicionar um gráfico a um relatório</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Severidade Padrão</td> 
      <td>Selecione a severidade que deseja que o Workfront selecione automaticamente todas as questões recém-criadas.</p>
      <p>A aparência é a gravidade padrão para problemas no Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição para a severidade para explicar sua função.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar</td> 
      <td> Ocultar uma severidade que não é mais necessária. 
      <p>Uma severidade oculta não é exibida em nenhum lugar do Workfront, portanto, os usuários não podem escolhê-la para seus problemas.</p> 
      <p><b>IMPORTANTE</b>: em vez de excluir severidades que você não deseja mais usar, sugerimos que você as oculte. Dessa forma, você mantém todos os seus dados históricos em objetos já concluídos com a severidade, enquanto impede que as pessoas usem a severidade no futuro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Altere a ordem de listagem das severidades arrastando e soltando na ordem desejada.

   Isso altera a ordem em que são exibidos para ocorrências. Isso não altera o número de **Importância**.

1. Clique em **Salvar**.

Para obter mais informações sobre como usar severidades ao trabalhar com problemas, consulte [Atualizar severidade do problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
