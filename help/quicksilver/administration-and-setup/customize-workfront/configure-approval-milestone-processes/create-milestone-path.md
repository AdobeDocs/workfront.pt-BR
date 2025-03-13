---
title: Criar um Caminho de Etapas
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-approval-and-milestone-processes
description: Como administrador do Adobe Workfront, você pode criar caminhos de etapas que podem ser aplicados a qualquer projeto no sistema. As alterações feitas nos caminhos de marcos nessa área afetam todo o sistema do Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: c1e2f374-576c-4f1c-b502-281e8ee9e7df
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 3%

---

# Criar um caminho de marcos

<!--Audited: 07/2024-->

<!--
NOTE: DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como administrador do Adobe Workfront, você pode criar caminhos de etapas que podem ser aplicados a qualquer projeto no sistema. As alterações feitas nos caminhos de marcos nessa área afetam todo o sistema do Workfront.

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
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Etapas e caminhos de etapas

Você pode associar as principais tarefas de um projeto a marcos predefinidos. Essa função pode fornecer aos gerentes e outras partes interessadas uma visão geral de alto nível sobre o progresso de um projeto.

A soma de todos os marcos predefinidos é chamada de caminho de marcos.

A primeira etapa na criação de um caminho de marcos é identificar quais são as etapas de marcos e estabelecer os marcos. Como é possível associar um caminho de etapas a vários projetos, as etapas de etapas devem ser fases ou estágios gerais de qualquer projeto.

Para obter mais informações sobre como associar um caminho de etapas a um projeto e uma etapa a uma tarefa, consulte [Associar etapas a tarefas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).

## Criar um caminho de marcos

{{step-1-to-setup}}

1. Clique em **Processos** > **Caminhos de Etapas**.
1. Clique em **Novo Caminho de Etapas.**
1. Especifique as seguintes informações na área **Informações Básicas**:

   <table style="table-layout:auto">
    <tr>
      <td>Nome do Caminho de Etapas</td>
       <td>Insira um nome para o caminho de etapas.</td>
    </tr>
    <tr>
      <td>Descrição</td>
      <td>Insira uma descrição para definir o caminho de etapas.</td>
    </tr>
    <tr>
       <td>Está ativo</td>
      <td>Marque essa caixa de seleção se desejar que o caminho de etapas esteja ativo. Outros usuários podem encontrar esse caminho e anexá-lo a projetos ao criar ou editar projetos. Caminhos de etapas inativos não podem ser anexados a projetos. Isso é ativado por padrão.</td>
    </tr>
    <tr>
      <td>Grupos</td>
      <td>Selecione os grupos listados para permitir que os usuários desses grupos vejam e apliquem esse caminho de etapas aos seus projetos. O grupo inicial do usuário que entra no caminho de etapas é selecionado por padrão.</td>
    </tr>
   </table>

1. Especifique as seguintes informações na área **Etapas**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td>Digite nomes descritivos para cada marco.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>Digite uma descrição para a etapa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Escolha uma cor para associar ao marco. </p> <p>Se você não escolher uma cor, o sistema escolherá a última cor usada em um caminho de etapas. Recomendamos que você escolha uma cor exclusiva para cada marco. A cor é usada para fins visuais e de relatório.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Adicionar Etapa** e continue adicionando etapas conforme necessário até que o caminho seja concluído.

1. Clique em **Criar Caminho de Etapas** para salvar suas alterações.

   Seu caminho de etapas está pronto para ser associado a um projeto.

   Para obter mais informações sobre como associar caminhos de etapas a projetos e etapas a tarefas, consulte [Associar etapas a tarefas](../../../manage-work/tasks/manage-tasks/associate-milestones-with-tasks.md).


1. <span class="preview">(Opcional) Clique no ícone **Exportar** ![Ícone Exportar](assets/export-icon.png) e selecione um dos seguintes formatos para exportar a lista de caminhos de etapas para um arquivo: </span>

   * PDF
   * Excel
   * Excel (xlsx)
   * Delimitado por tabulação

1. <span class="preview">(Opcional) Selecione uma etapa na lista de etapas e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) para editar as informações da etapa. </span>
1. <span class="preview">(Opcional) Selecione uma etapa na lista de etapas e clique no ícone **Excluir** ![Excluir ícone](assets/delete-icon.png) para excluí-la. </span>
1. <span class="preview">Clique em **Sim, exclua-o**. </span>
   <span class="preview">A etapa foi excluída e não pode ser recuperada. Todas as informações do projeto associadas à etapa e todas as informações de tarefas associadas aos caminhos de etapas também são excluídas. </span>


<div class="preview">

## Exibir detalhes do caminho de etapas em um relatório

Você pode visualizar os detalhes de um caminho de etapas em um relatório de projeto.

Você deve associar um caminho de etapas a um projeto antes de ver seus detalhes em um relatório de projeto.

Para obter informações sobre como associar caminhos de etapas a projetos, consulte [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

{{step1-to-reports}}

1. Clique em **Novo Relatório** e em **Projeto**.
1. Clique em **Adicionar coluna**.
1. Na área **Mostrar nesta coluna**, comece digitando **Caminho de Etapas** e clique em **Nome do Caminho de Etapas** quando for exibido.
1. (Opcional) Clique em **Filtros** e adicione o seguinte filtro ao relatório: **A ID do Caminho de Etapas do Projeto não está em branco**.

   O filtro garante a exibição apenas de projetos associados a um caminho de etapas no relatório.

1. Clique em **Salvar + Fechar**.
1. Adicione um nome para o relatório e clique em **Aplicar**.

   O relatório do projeto é exibido. Os caminhos de etapas associados a cada projeto são exibidos na última coluna do relatório.
1. Clique no nome de um caminho de etapas na última coluna do relatório.

   Os detalhes do caminho de etapas são exibidos.

   <div class="preview">

   ![Detalhes do caminho de etapas do relatório de projeto](assets/milestone-details-from-project-report.png)

   A página de detalhes do caminho de etapas exibe as seguintes informações:

   * Nome, ID e Descrição do caminho de etapas
   * Grupos de caminhos de etapas
   * Nomes de etapas, descrições, cores e ícones de cores

1. (Opcional) Clique em **Voltar** para voltar ao relatório do projeto.

</div>


