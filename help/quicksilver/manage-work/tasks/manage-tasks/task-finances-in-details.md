---
product-area: projects
navigation-topic: manage-tasks
title: Gerenciar finanças da tarefa na seção Detalhes da tarefa
description: Gerenciar finanças da tarefa na seção Detalhes da tarefa
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 4%

---

# Gerenciar finanças da tarefa na seção Detalhes da tarefa

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

É possível exibir ou editar as informações financeiras de uma tarefa acessando a área Visão Geral da seção Detalhes da Tarefa. Há um número limitado de campos que você pode exibir ou editar nessa área. Para obter informações sobre como editar todas as informações financeiras de uma tarefa, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Trabalhar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a projetos e tarefas</p> <p>Exibir acesso a Dados Financeiros ou superior</p> <p>Você deve ter acesso de Edição a Dados Financeiros para editar informações financeiras sobre tarefas</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para a tarefa que incluem Exibir Finanças ou superior</p> <p>Você deve ter permissões de Gerenciamento na tarefa que inclui Editar finanças para editar informações financeiras sobre tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Editar finanças da tarefa na seção Detalhes da tarefa

1. Vá para um projeto em que deseja exibir uma tarefa.

   >[!NOTE]
   >
   >Para localizar uma tarefa, você também pode pesquisá-la e clicar no nome para acessá-la. Para obter mais informações sobre a pesquisa de objetos no Workfront, consulte [Pesquisar Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Clique em **Tarefas** no painel esquerdo.
1. Clique no nome de uma tarefa que deseja exibir.
1. Clique em **Detalhes da tarefa**.
1. (Opcional) Clique no ícone **Recolher tudo** na parte superior direita da página Detalhes da tarefa.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou do Administrador de grupo configura nosso Modelo de layout, os campos na seção Detalhes da tarefa podem ser reorganizados ou não ser exibidos. Para obter informações, consulte [Personalizar o modo de exibição de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Clique em **Finanças** para expandir e exibir as informações financeiras da tarefa.

   Clique no ícone **Editar** ![](assets/edit-icon.png) no canto superior direito da seção Detalhes e em **Finanças**.

1. Edite qualquer campo disponível para edição clicando uma vez no campo ou clicando em **+Adicionar** para adicionar informações a um campo vazio.
1. Revise ou edite as seguintes informações na área **Finanças**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de Custo</td> 
      <td> <p>Especifique o Tipo de Custo para a tarefa. Isso vai determinar como o custo da tarefa é calculado, com base no número de horas nas tarefas. </p> <p>Selecione entre as seguintes opções: </p> 
       <ul> 
        <li> <p>Sem Custo</p> </li> 
        <li> <p>Horas por Valor de Hora Fixo </p> </li> 
        <li> <p> Horas por Valor da Hora do Recurso </p> </li> 
        <li> <p> Horas por Valor da Hora do Perfil</p> </li> 
       </ul> <p>Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>. O administrador do Workfront ou um administrador de grupo seleciona a configuração Tipo de custo padrão para as tarefas no seu sistema ou grupo. Para obter informações sobre como definir padrões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Receita</td> 
      <td> <p>Especifique o Tipo de Receita para a tarefa. Isso vai determinar como a Receita na tarefa é calculada, com base no número de horas nas tarefas. </p> <p>Selecione entre as seguintes opções: </p> 
       <ul> 
        <li> <p> Não Faturável </p> </li> 
        <li> <p>Horas por Valor da Hora do Recurso </p> </li> 
        <li> <p>Horas por Valor da Hora do Perfil </p> </li> 
        <li> <p>Horas por Valor de Hora Fixo </p> </li> 
        <li> <p>Horas por Valor da Hora dos Recursos, com Teto </p> </li> 
        <li> <p>Horas por Valor da Hora do Perfil, com Teto </p> </li> 
        <li> <p>Horas por Valor da Hora do Recurso mais Taxa Fixa </p> </li> 
        <li> <p>Horas por Valor da Hora do Perfil mais Taxa Fixa </p> </li> 
        <li> <p>Receita com Valor Fixo </p> </li> 
       </ul> <p>Para obter mais informações sobre o rastreamento da receita, consulte<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral de Faturamento e Receita</a>. </p> <p>O administrador do Workfront ou do grupo seleciona a configuração Tipo de receita padrão para as tarefas no seu sistema ou grupo. Para obter informações sobre como definir padrões de projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto do sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo Planejado</td> 
      <td> <p>Este é um cálculo que mostra o custo da tarefa com base nas horas planejadas, o tipo de custo e a taxa horária para usuários ou funções de trabalho. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo Efetivo</td> 
      <td> <p> Este é um cálculo que mostra o custo da tarefa com base nas horas reais, o tipo de custo e a taxa horária para usuários ou funções de trabalho. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita Planejada</td> 
      <td> <p>Este é um cálculo que mostra a receita associada à tarefa com base nas horas planejadas, o tipo de receita e a taxa horária para usuários ou funções de trabalho. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita Efetiva</td> 
      <td> <p>Este é um cálculo que mostra a receita associada à tarefa com base nas horas reais, no tipo de receita e na taxa horária para usuários ou funções de trabalho. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI/SPI/CSI</strong> </td> 
      <td> <p>Estas são métricas de desempenho de tarefa que mostram como sua tarefa está se saindo em um determinado momento. Seus valores são calculados com base no Método de indexação de desempenho do projeto.<br>Para obter mais informações, consulte os seguintes artigos:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcular Índice de Desempenho de Custo (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcular SPI (Índice de Desempenho de Agendamento) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcular CSI (Índice de Desempenho de Agendamento de Custos)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimativa no término (EAC)</td> 
      <td> <p>Este é um cálculo que mostra o custo total da sua tarefa, na conclusão. Para obter mais informações sobre a estimativa na conclusão, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular Estimativa na Conclusão (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você estiver editando os campos na seção Finanças, clique em **Salvar***Alterações**.
