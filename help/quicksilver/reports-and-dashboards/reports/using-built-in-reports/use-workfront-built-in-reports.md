---
product-area: reporting
navigation-topic: using-built-in-reports
title: Usar relatórios internos do Adobe Workfront
description: A Adobe Workfront tem uma lista abrangente de relatórios internos que você pode usar.
author: Nolan
feature: Reports and Dashboards
exl-id: 32a47c25-192a-4e97-9016-42e6b6e201b9
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2997'
ht-degree: 11%

---

# Usar relatórios internos do Adobe Workfront

A Adobe Workfront tem uma lista abrangente de relatórios internos que você pode usar.

Os administradores do Workfront podem ocultar relatórios internos para que os usuários não tenham acesso a eles.\
Para obter mais informações sobre como ocultar relatórios internos, consulte [Ocultar relatórios internos](../../../administration-and-setup/manage-workfront/configure-reports/hide-built-in-reports.md).

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
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Visualizar ou obter acesso superior a Relatórios, Painéis, Calendários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório para adicionar ou editar um filtro a um relatório</p> <p>Gerenciar permissões em um filtro para editá-lo em uma lista</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão geral dos relatórios internos {#overview-of-built-in-reports}

Você pode personalizar um relatório integrado e salvá-lo como um novo relatório. Para obter mais informações sobre como personalizar relatórios internos, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Os relatórios a seguir são fornecidos com o pacote do Workfront. Os relatórios estão disponíveis para todos os usuários que têm pelo menos direitos de Exibição para relatórios internos em seu nível de acesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Nome do relatório</strong> </th> 
   <th><strong>Descrição do relatório</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Custo Efetivo do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado e o Custo Real dos projetos. O relatório é agrupado por Nome do programa, solicitado pelo Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custo Efetivo do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado e o Custo Real dos projetos. O relatório é agrupado por Nome do projeto, solicitado pelo Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Efetiva do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que exibe a Receita Planejada e a Receita Real dos projetos. O relatório é agrupado por Nome do programa, solicitado pelo Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Efetiva do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que exibe a Receita Planejada e a Receita Real dos projetos. O relatório é agrupado por Nome do projeto, solicitado pelo Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita atual por empresa</td> 
   <td>Um relatório de Projeto que exibe a Receita Real e a Empresa dos projetos. O relatório é agrupado por Nome da empresa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita atual por grupo</td> 
   <td>Um relatório de Projeto que exibe a Receita real e o Grupo dos projetos. O relatório é agrupado por Nome do grupo e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Todas as planilhas de horas abertas</td> 
   <td>Um relatório de Folha de Horas que exibe Folhas de Horas Abertas. O relatório exibe os seguintes campos: o Intervalo de datas, Nome do proprietário, Total de horas, Hora extra, Nome do aprovador e Status das folhas de ponto.</td> 
  </tr> 
  <tr> 
   <td>Aprovação de planilhas de horas (por seleção)</td> 
   <td>Um relatório de Folha de Horas que exibe Folhas de Horas Enviadas ou Rejeitadas com aprovadores. O relatório exibe os seguintes campos: o Intervalo de datas, Proprietário, Total de horas, Hora extra, Nome do Aprovador e Status das folhas de ponto. O relatório é solicitado por: Data de Início da Folha de Horas, Data de Término da Folha de Horas, Nome do Aprovador da Folha de Horas e Nome de Usuário.</td> 
  </tr> 
  <tr> 
   <td>Projetos em Risco</td> 
   <td>Um relatório de Projeto que exibe os projetos atuais e de planejamento que têm uma condição de Em risco ou Em problema. O relatório exibe os seguintes campos: a Descrição, a Data de Conclusão Planejada, a Data de Conclusão Projetada, a Porcentagem Concluída, o Status e a Prioridade dos projetos. O relatório é agrupado por Portfolio Name.</td> 
  </tr> 
  <tr> 
   <td>Receita faturada por empresa</td> 
   <td>Um relatório de Projeto que exibe a Empresa e a Receita de Faturamento dos projetos. O relatório é agrupado por Nome da empresa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita faturada por grupo</td> 
   <td>Um relatório de Projeto que exibe a Receita de Faturamento e o Grupo dos projetos. O relatório é agrupado por Nome do grupo e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita faturada por mês</td> 
   <td>Um relatório de Registro de Faturamento que exibe o Nome do Projeto, a Receita de Faturamento do Projeto e a Data de Faturamento dos registros de faturamento. O relatório é agrupado pelo mês da Data de Faturamento dos registros de faturamento e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas concluídas por semana</td> 
   <td>Um relatório de Ocorrência que exibe a Data de Conclusão Real dos problemas. O relatório é agrupado pela semana da Data de conclusão real dos problemas e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas concluídas por semana e por usuário</td> 
   <td>Um relatório de Emissão que exibe a Data de Conclusão Real e Atribuições dos problemas. O relatório é agrupado pelo destinatário principal e pela semana da Data de conclusão real dos problemas, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos Atuais</td> 
   <td>Um relatório de Projeto que exibe todos os projetos atuais. O relatório exibe os seguintes campos: a Descrição, a Data de Conclusão Planejada, a Data de Conclusão Projetada, a Porcentagem Concluída, o Status e a Prioridade dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Custos de hora por usuário e por mês</td> 
   <td>Um relatório Matriz Hour que exibe o número de Horas registradas e o Custo real. O relatório é agrupado pelo Nome do Proprietário e o mês da Data de Entrada das horas.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuário</td> 
   <td>Um relatório de Hora que exibe o número de horas registradas. O relatório é agrupado por Nome do Proprietário e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Horas por usuário e por mês</td> 
   <td>Um relatório de Hora da matriz que exibe o número de horas registradas nas últimas quatro semanas e a Data de entrada das horas. O relatório é solicitado pela Data de entrada das horas e é agrupado pelo Nome do proprietário e pelo mês da Data de entrada das horas.</td> 
  </tr> 
  <tr> 
   <td>Problemas por status</td> 
   <td>Um relatório de Ocorrência que exibe o Status dos problemas. O relatório é agrupado por Status dos problemas e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Problemas por status e por projeto</td> 
   <td>Um relatório de Problemas de matriz que exibe o Status dos problemas em Projetos atuais e o Nome do projeto. O relatório é agrupado por Nome do projeto e Status dos problemas.</td> 
  </tr> 
  <tr> 
   <td>Mão de obra v. Custos operacionais por Portfólio</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado da Mão-de-Obra, Custo Real da Mão-de-Obra, Custo Planejado da Despesa e Custo Real da Despesa dos projetos. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Mão de obra v. Custos operacionais por programa</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado da Mão-de-Obra, Custo Real da Mão-de-Obra, Custo Planejado da Despesa e Custo Real da Despesa dos projetos. O relatório é agrupado por Portfolio Name e Program Name, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos mensais planejados do portfolio versus custos atuais por projeto</td> 
   <td>Um relatório de matriz Projeto (Dados Financeiros) que exibe a Data da alocação, Custo total planejado, Custo total real e Variação total do custo dos projetos. O relatório é agrupado por Nome do projeto, o trimestre e o mês da Data de alocação.</td> 
  </tr> 
  <tr> 
   <td>Receita mensal planejada do portfolio versus receita atual por projeto</td> 
   <td>Um relatório de matriz Projeto (Dados Financeiros) que exibe a Data da alocação, Receita total planejada, Receita total real e Variação total da receita dos projetos. O relatório é agrupado por Nome do projeto, o trimestre e o mês da Data de alocação.</td> 
  </tr> 
  <tr> 
   <td>Custos mensais planejados do projeto versus custos atuais</td> 
   <td>Um relatório de matriz Projeto (Dados Financeiros) que exibe a Data da alocação, Custo total planejado, Custo total real e Variação total do custo dos projetos. O relatório é agrupado por Nome do projeto, o trimestre e o mês da Data de alocação e é solicitado pelo Nome do projeto.</td> 
  </tr> 
  <tr> 
   <td>Receita mensal planejada de projeto versus receita atual</td> 
   <td>Um relatório de matriz Projeto (Dados Financeiros) que exibe a Data da alocação, Receita total planejada, Receita total real e Variação total da receita dos projetos. O relatório é agrupado por Nome do projeto, o trimestre e o mês da Data de alocação e é solicitado pelo Nome do projeto.</td> 
  </tr> 
  <tr> 
   <td>Meus documentos</td> 
   <td>Um relatório de Documento que exibe documentos carregados pelo usuário conectado. O relatório exibe os seguintes campos: Nome do Proprietário, Data Modificada, Tamanho, Contagem de Versão, Fonte e Tipo dos documentos.</td> 
  </tr> 
  <tr> 
   <td>Meus favoritos</td> 
   <td>Um relatório de Favoritos que exibe uma lista de objetos marcados como favoritos pelo usuário conectado. O relatório exibe os seguintes campos: o Tipo de objeto e o Nome dos favoritos.</td> 
  </tr> 
  <tr> 
   <td>Meus problemas</td> 
   <td>Um relatório de Problemas que exibe Problemas incompletos atribuídos ao usuário que está conectado. O relatório exibe os seguintes campos: Nome da Fonte, Tipo de Emissão, Destinatário Principal, Data de Entrada, Status e Prioridade dos problemas.</td> 
  </tr> 
  <tr> 
   <td>Meus Portfólios</td> 
   <td>Um relatório de Portfolio que exibe Portfolio ativas, onde o usuário conectado é o Gerenciador de Portfolio.</td> 
  </tr> 
  <tr> 
   <td>Meus Programas</td> 
   <td>Um relatório de Programa que exibe Programas e sua Descrição, onde o usuário conectado é o Gerenciador de Programas.</td> 
  </tr> 
  <tr> 
   <td>Meus Problemas de Projeto Abertos</td> 
   <td>Um relatório de Problemas que exibe problemas incompletos em projetos cuja Equipe de projetos inclui o usuário conectado. O relatório exibe os seguintes campos: Nome da Fonte, Tipo de Emissão, Destinatário Principal, Data de Entrada, Status e Prioridade dos problemas.</td> 
  </tr> 
  <tr> 
   <td>Meus projetos</td> 
   <td>Um relatório de Projeto que mostra projetos Atuais cuja Equipe do Projeto inclui o usuário logado. 
O relatório exibe os seguintes campos: a Descrição, a Data de Conclusão Planejada, a Data de Conclusão Projetada, a Porcentagem Concluída, o Status e a Prioridade dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Meus Problemas Submetidos</td> 
   <td>Um relatório de Problemas que exibe problemas enviados pelo usuário conectado que foram fechados nos últimos três meses ou que estão abertos no momento. O relatório exibe os seguintes campos: Nome da Fonte, Tipo de Emissão, Data de Entrada, Status e Prioridade dos problemas.</td> 
  </tr> 
  <tr> 
   <td>Minhas tarefas</td> 
   <td>Um relatório de Tarefa que exibe tarefas incompletas em Projetos atuais que são atribuídas ao usuário conectado. O relatório exibe os seguintes campos: a Duração planejada, Nome do projeto, Destinatário principal, Início planejado, Conclusão planejada, Porcentagem concluída e Prioridade das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Minhas planilhas de horas</td> 
   <td>Um relatório de Planilha de Horas que mostra todas as planilhas de horas do usuário logado. O relatório exibe os seguintes campos: o Intervalo de datas, Nome do proprietário, Total de horas, Hora extra, Nome do aprovador e Status das folhas de ponto.</td> 
  </tr> 
  <tr> 
   <td>Minhas Problemas não Atribuídos</td> 
   <td>Um relatório de Problemas que exibe problemas em aberto atribuídos a qualquer uma das funções de trabalho do usuário conectado e que não são atribuídas ao usuário. O relatório exibe os seguintes campos: Nome da Fonte, Tipo de Emissão, Data de Entrada, Status e Prioridade dos problemas.</td> 
  </tr> 
  <tr> 
   <td>Minhas Tarefas não Atribuídas</td> 
   <td>Um relatório de Tarefa que exibe tarefas incompletas atribuídas a qualquer uma das funções de trabalho do usuário conectado e que não são atribuídas ao usuário. O relatório exibe os seguintes campos: a Duração planejada, Nome do projeto, Destinatário principal, Data inicial planejada, Data de conclusão planejada, Porcentagem concluída e Prioridade das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Minhas Próximas Tarefas</td> 
   <td>Um relatório de Tarefa que exibe tarefas incompletas que devem começar nas próximas duas semanas, estão em projetos atuais e são atribuídas ao usuário conectado. O relatório exibe os seguintes campos: Nome do projeto, Data de conclusão planejada, Data de conclusão projetada, Porcentagem concluída e Status das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Planilhas de horas abertas (por seleção)</td> 
   <td>Um relatório de Folha de Horas que exibe Folhas de Horas Abertas. O relatório exibe os seguintes campos: o Intervalo de datas, Proprietário, Total de horas, Hora extra, Nome do aprovador, Status das folhas de horas. O relatório é solicitado por: Data de Início da Folha de Horas, Data de Término da Folha de Horas, Nome do Aprovador da Folha de Horas e Nome de Usuário.</td> 
  </tr> 
  <tr> 
   <td>Projetos acima do Orçamento por Portfólio</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado e o Custo Real dos projetos. O relatório é agrupado por Portfolio Name.</td> 
  </tr> 
  <tr> 
   <td>Custo Planejado do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado e o Custo Real dos projetos. O relatório é solicitado pelo Portfolio Name, agrupado por Program Name, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custo Planejado do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado e o Custo Real dos projetos. O relatório é solicitado pelo Nome do Portfolio, agrupado por Nome do projeto, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Planejada do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que exibe a Receita Planejada e a Receita Real dos projetos. O relatório é solicitado pelo Portfolio Name, agrupado por Program Name, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita Planejada do Portfólio por Projeto</td> 
   <td>Um relatório de Projeto que exibe a Receita Planejada e a Receita Real dos projetos. O relatório é solicitado pelo Nome do Portfolio, agrupado por Nome do projeto, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos planejados v. reais por Portfólio</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado e o Custo Real dos projetos por Portfolio. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos planejados v. reais por programa</td> 
   <td>Um relatório de Projeto que exibe o Custo Planejado e o Custo Real dos projetos por Programa. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita planejada v. receita real por Portfólio</td> 
   <td>Um relatório de Projeto que exibe a Receita Planejada e a Receita Real dos projetos. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita planejada v. receita real por programa</td> 
   <td>Um relatório de Projeto que exibe a Receita Planejada e a Receita Real dos projetos. O relatório é agrupado por Nome do programa e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Custos agrupados do Portfolio por programa e por mês</td> 
   <td>Um relatório de Projeto de matriz que exibe o Custo Planejado, Custo Orçado e Custo Real dos projetos. O relatório é agrupado por Portfolio Name, Program Name e the month of the Planned Start Date of the projects.</td> 
  </tr> 
  <tr> 
   <td>Projetos do portfólio por status agrupados por programa</td> 
   <td>Um relatório de Projeto que exibe o Status dos projetos. O relatório é agrupado por Nome do programa e Status do projeto, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos do portfólio agrupados por condição e portfólio</td> 
   <td>Um relatório de Projeto que exibe o Nome do Portfolio e o Status dos projetos. O relatório é agrupado pelo Nome do Portfolio e o Status dos projetos, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita do Portfólio por Programa</td> 
   <td>Um relatório de Projeto que exibe o Portfolio, o Nome do programa, a Receita planejada e a Receita real dos projetos. O relatório é agrupado pelo Nome do Portfolio e Nome do programa, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Receita agrupada do Portfolio por programa e por mês</td> 
   <td>Um relatório de Projeto de matriz que exibe Receita planejada, Receita real, Nome do Portfolio e Nome do programa. O relatório é agrupado pelo Portfolio Name, Program Name e the month of the Planned Start Date of the projects.</td> 
  </tr> 
  <tr> 
   <td>Custos e receitas do projeto por status de tarefa</td> 
   <td>Um relatório de Tarefa de matriz que exibe o Custo Planejado, Custo Real, Receita Planejada, Receita Real e Nome do Projeto das tarefas. O relatório é agrupado por Nome do projeto e Status das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Custos de projetos v. receitas por Portfólio</td> 
   <td>Um relatório de Projeto que exibe o Nome do Portfolio, Custo Real e Receita Real dos projetos. O relatório é agrupado por Nome do Portfolio e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Despesas de projeto por mês e quartil</td> 
   <td>Um relatório de Despesas da matriz que exibe a Data de Entrada, a Quantia Planejada, a Quantia Real e o Projeto das despesas. O relatório é agrupado pelo Nome do Projeto, o trimestre e o mês da Data de Entrada das despesas.</td> 
  </tr> 
  <tr> 
   <td>Custos de hora de projeto por tipo de hora e por mês</td> 
   <td>Um relatório de Hora da matriz que exibe os seguintes campos: Horas, Data de entrada, Custo real dos projetos, Tipo de hora, Nome do projeto. O relatório é agrupado por Nome do projeto, mês da Data de entrada das horas e Tipo de hora.</td> 
  </tr> 
  <tr> 
   <td>Custo do trabalho e despesas do projeto por mês e por quartil</td> 
   <td>Um relatório de matriz Projeto que exibe o Custo Planejado da Mão de obra, Custo Real da Mão de obra, Custo Planejado da Despesa e Custo Real da Despesa dos projetos. O relatório é agrupado pelo Nome do projeto e o trimestre e o mês da Data de início real dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Performance de Projeto</td> 
   <td>Um relatório de Projeto que exibe os seguintes campos de projetos atuais: Data de Vencimento, CPI, SPI, CSI, Custo Planejado, Orçamento, EAC e Despesas dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Solicitações de Projeto</td> 
   <td>Um relatório de Projeto que exibe Projetos solicitados. O relatório exibe os seguintes campos: a Descrição, a Data de Conclusão Planejada, a Data de Conclusão Projetada, a Porcentagem Concluída, o Status e a Prioridade dos projetos.</td> 
  </tr> 
  <tr> 
   <td>Projetos por condição</td> 
   <td>Um relatório de Projeto que exibe a Condição dos projetos. O relatório é agrupado por Condição e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos por condição por grupo</td> 
   <td>Um relatório de Projeto que exibe o Status do Andamento e o Grupo dos projetos. O relatório é agrupado por Nome do grupo e Status do progresso, e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos por Prioridade</td> 
   <td>Um relatório de Projeto que exibe a Prioridade dos projetos. O relatório é agrupado por Prioridade e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Projetos por status de progresso</td> 
   <td>Um relatório de Projeto que exibe o Status de progresso dos projetos. O relatório é agrupado pelo Status do Andamento e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tarefas por status do progresso</td> 
   <td>Um relatório de Tarefa que exibe o Status de Andamento de todas as Tarefas em Projetos Atuais. O relatório é agrupado por Status do Progresso e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Tarefas por status</td> 
   <td>Um relatórios de Tarefa que mostra o Status de todas as tarefas. O relatório é agrupado por Status e inclui um gráfico.</td> 
  </tr> 
  <tr> 
   <td>Planilha de horas para Revisão</td> 
   <td>Um relatório de Folha de Horas que exibe Folhas de Horas Enviadas e Rejeitadas cujo aprovador é o usuário conectado. O relatório exibe os seguintes campos: o Intervalo de datas, Proprietário, Total de horas, Hora extra, Nome do aprovador e Status das folhas de horas.</td> 
  </tr> 
  <tr> 
   <td>Tarefas com Problemas</td> 
   <td>Um relatório de Tarefa que exibe tarefas incompletas com um Status de Andamento Atrasado ou Atrasado, uma Data de Handoff antes de amanhã e onde o usuário conectado faz parte da Equipe de Projeto do projeto em que as tarefas estão. O relatório exibe os seguintes campos: Duração planejada, Nome do projeto, responsável principal, Início planejado, Conclusão planejada, Porcentagem concluída e Prioridade das tarefas.</td> 
  </tr> 
  <tr> 
   <td>Logins de Usuário</td> 
   <td>Um relatório de Usuário que exibe os seguintes campos: a ID exclusiva, a Contagem de logon (o número de vezes que o usuário fez logon desde o início com o Workfront), a Data do último logon dos usuários. O relatório é agrupado pelo Nível de acesso dos usuários.</td> 
  </tr> 
 </tbody> 
 <p><span class="wysiwyg-color-pink"></span> </p> 
</table>

## Acessar relatórios internos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Section directly linked to "Getting Started with Workfront Reporting." Do not change/ rename.) </p>
-->

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.
1. Clique em **Relatórios**.
1. Clique em **Todos os relatórios**.
1. Expanda o **Filtro** e selecione **Novo filtro**.

1. Clique em **Adicionar uma regra de filtro**.
1. No **Iniciar a digitação do nome do campo** , comece a digitar **ID global**.

1. Em **Relatório** objeto, selecione **ID global**.

1. No menu suspenso do modificador de filtro, selecione **Não está em Branco**.\
   ![](assets/qs-global-id-filter-for-system-reports-350x179.png)

1. Clique em **Salvar filtro**.\
   A lista de relatórios exibe somente relatórios internos.\
   Para obter mais informações sobre quais relatórios internos estão disponíveis, consulte [Visão geral dos relatórios internos](#overview-of-built-in-reports).
