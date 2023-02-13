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
source-wordcount: '857'
ht-degree: 5%

---

# Gerenciar finanças da tarefa na seção Detalhes da tarefa

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

Você pode exibir ou editar as informações financeiras de uma tarefa acessando a área Visão geral da seção Detalhes da tarefa . Há um número limitado de campos que você pode visualizar ou editar nessa área. Para obter informações sobre como editar todas as informações financeiras de uma tarefa, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

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
   <td> <p>Trabalho ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Tarefas</p> <p>Exibir o acesso aos dados financeiros ou superior</p> <p>Você deve ter o acesso Editar aos Dados Financeiros para editar informações financeiras sobre tarefas</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para a tarefa que incluem Exibir Finanças ou superior</p> <p>Você deve ter permissões de Gerenciamento na tarefa que inclui Editar Finanças para editar informações financeiras em tarefas</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Editar finanças da tarefa na seção Detalhes da tarefa

1. Vá para um projeto onde deseja exibir uma tarefa.

   >[!NOTE]
   >
   >Para localizar uma tarefa, você também pode pesquisá-la e clicar no nome para acessar a tarefa. Para obter mais informações sobre a pesquisa de objetos no Workfront, consulte [Pesquisar Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. Clique em **Tarefas** no painel esquerdo.
1. Clique no nome de uma tarefa que deseja visualizar.
1. Clique em **Detalhes da tarefa**.
1. (Opcional) Clique no botão **Recolher tudo** no canto superior direito da página Detalhes da tarefa.

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront ou o administrador do Grupo configura nosso Modelo de layout, os campos na seção Detalhes da tarefa podem ser reorganizados ou não serem exibidos. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Clique em **Finanças** para expandir e exibir as informações financeiras da tarefa.

   Clique no botão **Editar** ícone ![](assets/edit-icon.png) no canto superior direito da seção Detalhes e clique em **Finanças**.

1. Edite qualquer campo disponível para edição, clicando uma vez no campo ou clicando em **+Adicionar** para adicionar informações a um campo vazio.
1. Revise ou edite as seguintes informações na **Finanças** área :

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Tipo de Custo</td> 
      <td> <p>Especifique o Tipo de Custo da tarefa. Isso determinará como o custo da tarefa é calculado, com base no número de horas nas tarefas. </p> <p>Selecione dentre as seguintes opções: </p> 
       <ul> 
        <li> <p>Sem Custo</p> </li> 
        <li> <p>Horas por Valor de Hora Fixo </p> </li> 
        <li> <p> Horas por Valor da Hora do Recurso </p> </li> 
        <li> <p> Horas por Valor da Hora do Perfil</p> </li> 
       </ul> <p>Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a> . O administrador do Workfront ou um administrador de grupo seleciona a configuração padrão de Tipo de Custo para as tarefas em seu sistema ou grupo. Para obter informações sobre a definição de padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Receita</td> 
      <td> <p>Especifique o Tipo de receita para a tarefa. Isso determinará como a Receita na tarefa será calculada, com base no número de horas nas tarefas. </p> <p>Selecione dentre as seguintes opções: </p> 
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
       </ul> <p>Para obter mais informações sobre o rastreamento de receita, consulte<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Visão Geral da Faturamento e Receita</a> . </p> <p>O administrador ou administrador de grupo da Workfront seleciona a configuração padrão Tipo de receita para as tarefas em seu sistema ou grupo. Para obter informações sobre a definição de padrões do projeto, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo Planejado</td> 
      <td> <p>Este é um cálculo que mostra o custo da tarefa com base nas horas planejadas, no tipo de custo e na taxa horária para usuários ou funções de job. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo real</td> 
      <td> <p> Este é um cálculo que mostra o custo da tarefa com base nas horas reais, no tipo de custo e na taxa horária de usuários ou funções de job. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita Planejada</td> 
      <td> <p>Este é um cálculo que mostra a receita associada à tarefa com base nas horas planejadas, no tipo de receita e na taxa horária para usuários ou funções de job. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita real</td> 
      <td> <p>Este é um cálculo que mostra a receita associada à tarefa com base nas horas reais, no tipo de receita e na taxa horária para usuários ou funções de trabalho. Para obter mais informações sobre o rastreamento de custos, consulte <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Rastrear custos</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI / SPI / CSI</strong> </td> 
      <td> <p>Essas são métricas de desempenho de tarefas que mostram o desempenho de sua tarefa em um determinado momento. Seus valores são calculados com base no Método de Índice de Desempenho do projeto.<br>Para obter mais informações, consulte os seguintes artigos:</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcular Índice de Desempenho de Custo (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcular o Índice de Desempenho da Programação (SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcular CSI (Cost Schedule Performance Index, Índice de Desempenho da Programação de Custo)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Estimativa na Conclusão (EAC)</td> 
      <td> <p>Este é um cálculo que mostra o custo total da sua tarefa, na conclusão. Para obter mais informações sobre a estimativa na conclusão, consulte <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular Estimativa na Conclusão (EAC)</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se você estiver editando os campos na seção Finanças , clique em **Salvar***Alterações**.
