---
title: Criar ou personalizar severidades de problemas
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Seus usuários podem usar severidades para definir a gravidade de um problema. Você pode personalizar qualquer uma das cinco severidades padrão existentes no Adobe Workfront ou criar uma nova severidade para seus usuários.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 5c80dca8a9f7dd5a693db9bf22738602da8b521b
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 4%

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

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador de Sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Severidades de problema embutidas

O Workfront tem cinco severidades de problema integradas:

* Cosmética
* Causa Confusão
* Problema com Solução
* Problema Sem Solução
* Erro Fatal

É possível editar o seguinte para essas severidades:

* Nome
* Cor

  A cor de uma severidade é preservada em um relatório de gráfico, se você agrupar os resultados por Severidade do Problema. Para obter informações sobre relatórios de gráficos, consulte [Adicionar um gráfico a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Qual severidade é o padrão

  Para obter mais informações sobre severidades padrão, consulte [Criar ou editar a severidade de um problema](#create-or-edit-an-issue-severity) neste artigo.

* Descrição
* Se uma severidade está oculta no Workfront

  Para obter mais informações sobre como ocultar uma severidade, consulte [Criar ou editar a severidade de um problema](#create-or-edit-an-issue-severity) neste artigo.

* Excluir uma severidade

  Ao fazer isso, você deve selecionar uma severidade de substituição.

## Criar ou editar a severidade de um problema {#create-or-edit-an-issue-severity}

Como administrador do Workfront, você pode criar e editar severidades de problemas para atender às necessidades dos usuários.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Preferências do projeto** > **Severidades**.

1. Se você estiver criando uma nova severidade, clique em **Nova linha** na parte inferior da tabela.
1. Configure as seguintes opções para a nova severidade ou edite-as para uma existente:

   * **Nome da Severidade**: Digite um nome para a severidade.
   * **Importância**: aumente ou diminua o nível de seriedade, originalmente atribuído pela Workfront, para a severidade.

     O número de importância para cada severidade deve ser exclusivo. O número mais alto corresponde ao nível mais alto de severidade.

     Não é possível editar esse número depois de salvar a severidade.

   * **Cor**: escolha uma cor para a severidade.

     A cor da severidade é usada em relatórios de gráfico quando você agrupa seus resultados por Severidade do Problema. Para obter informações sobre relatórios de gráficos, consulte [Adicionar um gráfico a um relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

   * **Severidade Padrão**: Selecione a severidade que deseja que o Workfront aplique automaticamente a todas as questões recém-criadas.

     **Cosmética** é a severidade padrão para problemas no Workfront.

     Não é possível definir uma severidade oculta como padrão.

     A severidade padrão é indicada com um ícone ![Ícone de severidade padrão](assets/default-icon.png). Para escolher um novo padrão, siga um destes procedimentos:

      * Marque a caixa de seleção ao lado do nome da severidade e selecione **Tornar padrão** na barra de ações, na parte inferior da tela.
      * Passe o mouse sobre o nome da severidade e clique no menu **Mais** que aparece. Em seguida, selecione **Tornar Padrão**.

        A nova severidade padrão é rotulada com o ícone.

   * **Descrição**: digite uma descrição para a severidade para explicar sua função.
   * **Ocultar Opção**: selecione **Sim** para ocultar uma severidade que não é mais necessária.

     Uma severidade oculta não é exibida em nenhum lugar do Workfront, portanto, os usuários não podem escolhê-la para seus problemas.

     >[!IMPORTANT]
     >
     >Em vez de excluir severidades que você não deseja mais usar, sugerimos que você as oculte. Dessa forma, você mantém todos os seus dados históricos em objetos já concluídos com a severidade, enquanto impede que as pessoas usem a severidade no futuro.

1. (Opcional) Altere a ordem de listagem das severidades arrastando e soltando na ordem desejada.

   Isso altera a ordem em que são exibidos para ocorrências. Isso não altera o número de **Importância**.

1. Clique em **Salvar**.

Para obter mais informações sobre como usar severidades ao trabalhar com problemas, consulte [Atualizar severidade do problema](../../../manage-work/issues/issue-information/update-issue-severity.md).
