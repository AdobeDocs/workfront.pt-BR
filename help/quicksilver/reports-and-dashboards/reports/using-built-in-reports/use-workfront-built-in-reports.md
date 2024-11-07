---
product-area: reporting
navigation-topic: using-built-in-reports
title: Usar relatórios integrados do Adobe Workfront
description: O Adobe Workfront tem uma extensa lista de relatórios integrados prontos para uso. Os administradores do Workfront podem ocultar relatórios internos para que os usuários não tenham acesso a eles.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 0022892cabb9a44fb21e33d88148b098c937f388
workflow-type: tm+mt
source-wordcount: '2964'
ht-degree: 10%

---

# Usar relatórios integrados do Adobe Workfront

<!--Audited: 11/2024-->

O Adobe Workfront tem uma lista extensa de relatórios internos que você pode usar.

Os administradores do Workfront podem ocultar relatórios internos para que os usuários não tenham acesso a eles.

Para obter mais informações sobre como ocultar relatórios internos, consulte [Ocultar relatórios internos](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Colaborador ou superior</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Solicitação ou superior</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Acesso maior ou igual a relatórios, painéis, calendários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para adicionar ou editar um filtro em um relatório</p> <p>Gerenciar permissões de um filtro para editá-lo em uma lista</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visão geral dos relatórios integrados {#overview-of-built-in-reports}

Você pode personalizar um relatório incorporado e salvá-lo como um novo relatório. Para obter mais informações sobre como personalizar relatórios internos, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Os seguintes relatórios vêm com o pacote do Workfront. Os relatórios estão disponíveis para todos os usuários que tenham pelo menos direitos de Visualização para relatórios internos em seus níveis de acesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome do Relatório</strong> </th> 
   <th><strong>Descrição do relatório</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Custo Efetivo do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que mostra o Custo Planejado e o Custo Efetivo dos projetos. O relatório é agrupado por Nome do programa, solicitado por Nome do Portfolio, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custo Efetivo do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que mostra o Custo Planejado e o Custo Efetivo dos projetos. O relatório é agrupado por Nome do projeto, solicitado por Nome do Portfolio, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Efetiva do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que mostra a Receita Planejada e a Receita Efetiva dos projetos. O relatório é agrupado por Nome do programa, solicitado por Nome do Portfolio, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Efetiva do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que mostra a Receita Planejada e a Receita Efetiva dos projetos. O relatório é agrupado por Nome do projeto, solicitado por Nome do Portfolio, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita atual por empresa</td> 
   <td>Um relatório de Projeto que mostra a Receita Efetiva e a Receita Planejada dos projetos. O relatório é agrupado por Nome da empresa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita atual por grupo</td> 
   <td>Um relatório de Projeto que mostra a Receita Efetiva e o Grupo dos projetos. O relatório é agrupado por Nome do grupo e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Todas as planilhas de horas abertas</td> 
   <td>Um relatório de Planilha de Horas que mostra Planilhas de Horas Abertas. O relatório exibe os seguintes campos: Intervalo de datas, Nome do proprietário, Horas totais, Horas extras, Nome do aprovador e Status das folhas de horas.</td> 
  </tr> 
  <tr> 
   <td>Aprovação de planilhas de horas (por seleção)</td> 
   <td>Um relatório de Planilha de Horas que mostra Planilhas de Horas Enviadas ou Planilhas de Horas Rejeitadas com os aprovadores. O relatório exibe os seguintes campos: Intervalo de datas, Proprietário, Horas totais, Horas extras, Nome do aprovador e Status das folhas de horas. O relatório é solicitado por: Data Inicial da Planilha de Horas, Data Final da Planilha de Horas, Nome do Aprovador da Planilha de Horas e Nome do Usuário.</td> 
  </tr> 
  <tr> 
   <td>Projetos em Risco</td> 
   <td>Um relatório de Projeto que mostra projetos Atuais e Planejados que têm uma Condição de Em Risco ou Com Problemas. O relatório exibe os seguintes campos: Descrição, Data de Conclusão Planejada, Data de Conclusão Projetada, Percentual de Conclusão, Status e Prioridade dos projetos. O relatório é agrupado por Nome do Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Receita faturada por empresa</td> 
   <td>Um relatório de Projeto que mostra a Empresa e a Receita Faturada dos projetos. O relatório é agrupado por Nome da empresa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita faturada por grupo</td> 
   <td>Um relatório de Projeto que mostra a Receita Faturada e o Grupo dos projetos. O relatório é agrupado por Nome do grupo e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita faturada por mês</td> 
   <td>Um relatório de Registro de faturamento que mostra o Nome do Projeto, Receita Faturada do Projeto e Data de Faturamento dos registros de faturamento. O relatório é agrupado pelo mês da Data de faturamento dos registros de faturamento e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas concluídas por semana</td> 
   <td>Um relatório de Problema que mostra a Data de Término Efetivo dos problemas. O relatório é agrupado pela semana da Data de conclusão atual dos problemas e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas concluídas por semana e por usuário</td> 
   <td>Um relatório de Problema que mostra a Data de Término Efetivo e as Atribuições dos problemas. O relatório é agrupado pelo destinatário principal e pela semana da Data de conclusão real das ocorrências, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos Atuais</td> 
   <td>Um relatórios de Projeto que mostra todos os projetos Atuais. O relatório exibe os seguintes campos: Descrição, Data de Conclusão Planejada, Data de Conclusão Projetada, Percentual de Conclusão, Status e Prioridade dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Custos de hora por usuário e por mês</td> 
   <td>Um relatório de matriz de Horas que mostra o número de Horas reportadas e seu Custo Efetivo. O relatório é agrupado pelo Nome do proprietário e pelo mês da Data de entrada das horas.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuário</td> 
   <td>Um relatório de Horas que mostra o número de horas reportadas. O relatório é agrupado por Nome do proprietário e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuário e por mês</td> 
   <td>Um relatório de Horas de matriz que mostra o número de horas reportadas nas quatro últimas semanas e a Data de Entrada das horas. O relatório é solicitado pela Data de Entrada das horas e é agrupado pelo Nome do Proprietário e pelo mês da Data de Entrada das horas.</td> 
  </tr> 
  <tr> 
   <td>Problemas por status</td> 
   <td>Um relatório de Problema que mostra o Status dos problemas. O relatório é agrupado por Status dos problemas e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas por status e por projeto</td> 
   <td>Um relatório de Problemas de matriz que mostra o Status dos problemas nos projetos Atuais e o Nome do Projeto. O relatório é agrupado por Nome do projeto e Status dos problemas.</td> 
  </tr> 
  <tr> 
   <td>Mão de obra v. Custos operacionais por Portfólio</td> 
   <td>Um relatórios de Projeto que mostra o Custo de Trabalho Planejado, o Custo de Trabalho Efetivo, o Custo de Despesas Planejadas e o Custo Efetivo das Despesas dos projetos. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Mão de obra v. Custos operacionais por programa</td> 
   <td>Um relatórios de Projeto que mostra o Custo de Trabalho Planejado, o Custo de Trabalho Efetivo, o Custo de Despesas Planejadas e o Custo Efetivo das Despesas dos projetos. O relatório é agrupado por Nome do Portfolio e Nome do programa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos mensais planejados do portfolio versus custos atuais por projeto</td> 
   <td>Um relatório de Projeto de matriz (Dados Financeiros) que mostra a Data de Alocação, o Custo Total Planejado, o Custo Total Efetivo e a Variação do Custo Total dos projetos. O relatório é agrupado pelo Nome do Projeto, o trimestre e o mês da Data de Alocação.</td> 
  </tr> 
  <tr> 
   <td>Receita mensal planejada do portfolio versus receita atual por projeto</td> 
   <td>Um relatório de Projeto de matriz (Dados Financeiros) que mostra a Data de Alocação, a Receita Total Planejada, a Receita Total Efetiva e a Variação da Receita Total dos projetos. O relatório é agrupado pelo Nome do Projeto, o trimestre e o mês da Data de Alocação.</td> 
  </tr> 
  <tr> 
   <td>Custos mensais planejados do projeto versus custos atuais</td> 
   <td>Um relatório de Projeto de matriz (Dados Financeiros) que mostra a Data de Alocação, o Custo Total Planejado, o Custo Total Efetivo e a Variação do Custo Total dos projetos. O relatório é agrupado pelo Nome do Projeto, o trimestre e o mês da Data de Alocação e é solicitado pelo Nome do Projeto.</td> 
  </tr> 
  <tr> 
   <td>Receita mensal planejada de projeto versus receita atual</td> 
   <td>Um relatório de Projeto de matriz (Dados Financeiros) que mostra a Data de Alocação, a Receita Total Planejada, a Receita Total Efetiva e a Variação da Receita Total dos projetos. O relatório é agrupado pelo Nome do Projeto, o trimestre e o mês da Data de Alocação e é solicitado pelo Nome do Projeto.</td> 
  </tr> 
  <tr> 
   <td>Meus documentos</td> 
   <td>Um relatório de Documento que mostra documentos carregados pelo usuário logado. O relatório exibe os seguintes campos: Nome do Proprietário, Data de Modificação, Tamanho, Contagem de Versão, Source e Tipo dos documentos.</td> 
  </tr> 
  <tr> 
   <td>Meus favoritos</td> 
   <td>Um relatório de Favoritos que mostra uma lista de objetos marcados como favoritos pelo usuário logado. O relatório exibe os seguintes campos: o Tipo de objeto e o Nome dos favoritos.</td> 
  </tr> 
  <tr> 
   <td>Meus problemas</td> 
   <td>Um relatório de Problema que mostra Problemas incompletos atribuídos ao usuário logado. O relatório exibe os seguintes campos: Nome do Source, Tipo de Problema, Destinatário principal, Data de Entrada, Status e Prioridade das ocorrências.</td> 
  </tr> 
  <tr> 
   <td>Meus Portfólios</td> 
   <td>Um relatório de Portfolio que mostra Portfolio ativos nos quais o usuário logado é o Gerenciador de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Meus Programas</td> 
   <td>Um relatório de Programa que mostra Programas e sua Descrição, dos quais o usuário logado é o Gerente de Programa.</td> 
  </tr> 
  <tr> 
   <td>Meus Problemas de Projeto Abertos</td> 
   <td>Um relatório de Problema que mostra problemas incompletos cuja Equipe do Projeto inclui o usuário logado. O relatório exibe os seguintes campos: Nome do Source, Tipo de Problema, Destinatário principal, Data de Entrada, Status e Prioridade das ocorrências.</td> 
  </tr> 
  <tr> 
   <td>Meus projetos</td> 
   <td>Um relatório de Projeto que mostra projetos Atuais cuja Equipe do Projeto inclui o usuário logado. O relatório exibe os seguintes campos: Descrição, Data de Conclusão Planejada, Data de Conclusão Projetada, Percentual de Conclusão, Status e Prioridade dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Meus problemas enviados</td> 
   <td>Um relatório de Problema que mostra problemas enviados pelo usuário logado, que foram fechados nos últimos três meses ou que estão atualmente abertos. O relatório exibe os seguintes campos: Nome do Source, Tipo de Problema, Data de Entrada, Status e Prioridade das ocorrências.</td> 
  </tr> 
  <tr> 
   <td>Minhas tarefas</td> 
   <td>Um relatório de Tarefa que mostra tarefas incompletas nos Projetos Atuais que são atribuídas ao usuário logado. O relatório exibe os seguintes campos: Duração planejada, Nome do projeto, destinatário principal, Início planejado, Conclusão planejada, Percentual concluído e Prioridade das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Minhas planilhas de horas</td> 
   <td>Um relatório de Planilha de Horas que mostra todas as planilhas de horas do usuário logado. O relatório exibe os seguintes campos: Intervalo de datas, Nome do proprietário, Horas totais, Horas extras, Nome do aprovador e Status das folhas de horas.</td> 
  </tr> 
  <tr> 
   <td>Minhas Problemas não Atribuídos</td> 
   <td>Um relatório de Problema que mostra problemas abertos atribuídos a qualquer uma das funções de trabalho do usuário logado e que não estão atribuídos ao usuário. O relatório exibe os seguintes campos: Nome do Source, Tipo de Problema, Data de Entrada, Status e Prioridade das ocorrências.</td> 
  </tr> 
  <tr> 
   <td>Minhas Tarefas não Atribuídas</td> 
   <td>Um relatório de Tarefa que mostra tarefas incompletas atribuídas a qualquer uma das funções de trabalho do usuário logado e que não estão atribuídas ao usuário. O relatório exibe os seguintes campos: a Duração Planejada, o Nome do Projeto, o destinatário principal, a Data Inicial Planejada, a Data de Conclusão Planejada, o Percentual de Conclusão e a Prioridade das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Minhas Próximas Tarefas</td> 
   <td>Um relatório de Tarefa que mostra tarefas incompletas que devem começar nas próximas duas semanas, estão em projetos Atuais e estão atribuídas ao usuário logado. O relatório exibe os seguintes campos: Nome do Projeto, Data de Conclusão Planejada, Data de Conclusão Projetada, Percentual de Conclusão e Status das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Planilhas de horas abertas (por seleção)</td> 
   <td>Um relatório de Planilha de Horas que mostra Planilhas de Horas Abertas. O relatório exibe os seguintes campos: Intervalo de datas, Proprietário, Horas totais, Horas extras, Nome do aprovador, Status das folhas de horas. O relatório é solicitado por: Data Inicial da Planilha de Horas, Data Final da Planilha de Horas, Nome do Aprovador da Planilha de Horas e Nome do Usuário.</td> 
  </tr> 
  <tr> 
   <td>Projetos acima do Orçamento por Portfólio</td> 
   <td>Um relatório de Projeto que mostra o Custo Planejado e Custo Efetivo dos projetos. O relatório é agrupado por Nome do Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Custo Planejado do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que mostra o Custo Planejado e Custo Efetivo dos projetos. O relatório é solicitado pelo Nome do Portfolio, agrupado pelo Nome do programa, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custo Planejado do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que mostra o Custo Planejado e Custo Efetivo dos projetos. O relatório é solicitado pelo Nome do Portfolio, agrupado pelo Nome do projeto, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Planejada do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que mostra a Receita Planejada e a Receita Efetiva dos projetos. O relatório é solicitado pelo Nome do Portfolio, agrupado pelo Nome do programa, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Planejada do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que mostra a Receita Planejada e a Receita Efetiva dos projetos. O relatório é solicitado pelo Nome do Portfolio, agrupado pelo Nome do projeto, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos planejados v. reais por Portfólio</td> 
   <td>Um relatório de Projeto que mostra o Custo Planejado e Custo Efetivo dos projetos por Portfolio. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos planejados v. reais por programa</td> 
   <td>Um relatório de Projeto que mostra o Custo Planejado e Custo Efetivo dos projetos por Programa. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita planejada v. receita real por Portfólio</td> 
   <td>Um relatório de Projeto que mostra a Receita Planejada e a Receita Efetiva dos projetos. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita planejada v. receita real por programa</td> 
   <td>Um relatório de Projeto que mostra a Receita Planejada e a Receita Efetiva dos projetos. O relatório é agrupado por Nome do programa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos agrupados do Portfolio por programa e por mês</td> 
   <td>Um relatório de Projeto de matriz que mostra o Custo Planejado, o Custo Orçado e o Custo Efetivo dos projetos. O relatório é agrupado pelo Nome do Portfolio, Nome do programa e o mês da Data de início planejada dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Projetos do portfólio por status agrupados por programa</td> 
   <td>Um relatórios de Projeto que mostra o Status dos projetos. O relatório é agrupado por Nome do programa e Status do projeto e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos do portfólio agrupados por condição e portfólio</td> 
   <td>Um relatório de Projeto que mostra o Nome do Portfolio e o Status dos projetos. O relatório é agrupado pelo Nome do Portfolio e o Status dos projetos e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que mostra o Nome do Portfolio, Nome do Programa, Receita Planejada e Receita Efetiva dos projetos. O relatório é agrupado pelo Nome do Portfolio e pelo Nome do programa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita agrupada do Portfolio por programa e por mês</td> 
   <td>Um relatório de Projeto de matriz que mostra a Receita Planejada, a Receita Efetiva, o Nome do Portfolio e o Nome do Programa. O relatório é agrupado pelo Nome do Portfolio, Nome do programa e o mês da Data de início planejada dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Custos e receitas do projeto por status de tarefa</td> 
   <td>Um relatórios de Tarefa de matriz que mostra o Custo Planejado, o Custo Efetivo, a Receita Planejada, a Receita Efetiva e o Nome do Projeto das tarefas. O relatório é agrupado pelo Nome do projeto e Status das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Custos de projetos v. receitas por Portfólio</td> 
   <td>Um relatório de Projeto que mostra o Nome do Portfolio, o Custo Efetivo e a Receita Efetiva dos projetos. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Despesas de projeto por mês e quartil</td> 
   <td>Um relatório de Despesas de matriz que mostra a Data de Entrada, o Valor Planejado, o Valor Efetivo e o Projeto das despesas. O relatório é agrupado pelo Nome do Projeto, o trimestre e o mês da Data de Entrada das despesas.</td> 
  </tr> 
  <tr> 
   <td>Custos de hora de projeto por tipo de hora e por mês</td> 
   <td>Um relatório de matriz de Horas que mostra os seguintes campos: Horas, Data de Entrada, Custo Efetivo dos projetos, Tipo de Hora, Nome do Projeto. O relatório é agrupado por Nome do projeto, mês da Data de entrada das horas e Tipo de hora.</td> 
  </tr> 
  <tr> 
   <td>Custo do trabalho e despesas do projeto por mês e por quartil</td> 
   <td>Um relatório de Projeto de matriz que mostra o Custo de Trabalho Planejado, o Custo de Trabalho Efetivo, o Custo de Despesas Planejado e o Custo Efetivo das Despesas dos projetos. O relatório é agrupado pelo Nome do projeto e pelo trimestre e mês da Data de início efetiva dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Desempenho do projeto</td> 
   <td>Um relatórios de Projeto que mostra os seguintes campos dos projetos Atuais: a Data de Conclusão, CPI, SPI, CSI, Custo Planejado, Orçamento, EAC e Despesas dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Solicitações de Projeto</td> 
   <td>Um relatórios de Projeto que mostra os projetos Solicitados. O relatório exibe os seguintes campos: Descrição, Data de Conclusão Planejada, Data de Conclusão Projetada, Percentual de Conclusão, Status e Prioridade dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Projetos por condição</td> 
   <td>Um relatório de Projeto que mostra a Condição dos projetos. O relatório é agrupado por Condição e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos por condição por grupo</td> 
   <td>Um relatórios de Projeto que mostra o Status do Progresso e o Grupo dos projetos. O relatório é agrupado por Nome do grupo e Status do progresso e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos por Prioridade</td> 
   <td>Um relatórios de Projeto que mostra a Prioridade dos projetos. O relatório é agrupado por Prioridade e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos por status de progresso</td> 
   <td>Um relatórios de Projeto que mostra o Status de Progresso dos projetos. O relatório é agrupado pelo Status do progresso e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tarefas por status do progresso</td> 
   <td>Um relatório de Tarefa que mostra o Status do Progresso de todas as Tarefas nos Projetos Atuais. O relatório é agrupado por Status do progresso e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tarefas por status</td> 
   <td>Um relatório de Tarefa que mostra o Status de todas as tarefas. O relatório é agrupado por Status e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Planilha de horas para Revisão</td> 
   <td>Um relatório de Planilha de Horas que mostra planilhas de horas Enviadas e Rejeitadas cujo aprovador é o usuário logado. O relatório exibe os seguintes campos: Intervalo de datas, Proprietário, Horas totais, Horas extras, Nome do aprovador e Status das folhas de horas.</td> 
  </tr> 
  <tr> 
   <td>Tarefas com Problemas</td> 
   <td>Um relatório de Tarefa que mostra tarefas incompletas com um Status do Progresso de Atrasada ou Fora do Cronograma, uma Data de Transferência ates do dia seguinte e onde o usuário logado é parte da Equipe do Projeto do projeto do qual as tarefas fazem parte. O relatório exibe os seguintes campos: Duração planejada, Nome do projeto, destinatário principal, Início planejado, Conclusão planejada, Percentual concluído e Prioridade das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Logins de Usuário</td> 
   <td>Um relatório de Usuário que mostra os seguintes campos: ID exclusiva, Contagem de logon (o número de vezes que o usuário fez logon desde que começou a usar o Workfront), Data do último logon dos usuários. O relatório é agrupado pelo Nível de acesso dos usuários.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Acessar relatórios integrados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

{{step1-click-main-menu}}

1. Clique em **Relatórios**.
1. Clique em **Todos os relatórios**.
1. Expanda o menu suspenso **Filtro** e selecione **Novo Filtro**.

1. Clique em **Adicionar uma Regra de Filtro**.
1. No campo **Comece a digitar o nome do campo**, comece a digitar a **ID Global**.

1. No objeto **Relatório**, selecione **ID Global**.

1. No menu suspenso do modificador de filtro, selecione **Não está em branco**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Clique em **Salvar filtro**.\
   A lista de relatórios exibe apenas relatórios internos.\
   Para obter mais informações sobre quais relatórios internos estão disponíveis, consulte a seção [Visão geral dos relatórios internos](#overview-of-built-in-reports) neste artigo.
