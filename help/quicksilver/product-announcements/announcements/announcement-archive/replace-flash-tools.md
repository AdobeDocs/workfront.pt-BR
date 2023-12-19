---
title: Substituição de ferramentas baseadas em Flashes no Adobe Workfront
description: Substituição de ferramentas baseadas em Flashes no Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '2702'
ht-degree: 0%

---

# Substituição de ferramentas baseadas em Flashes no Adobe Workfront

Removemos todas as ferramentas baseadas em Flashes do Adobe Workfront Classic.

As ferramentas de substituição baseadas nos padrões atuais estão disponíveis agora no Workfront. Essas mudanças estão de acordo com o fim do suporte aos produtos de Flash, conforme anunciado pela Adobe.

## Datas importantes

As seguintes datas são importantes para o processo de remoção de todas as ferramentas baseadas em Flashes no Workfront:

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 de novembro de 2020**: todas as ferramentas baseadas em Flashes foram removidas de todos os produtos da Workfront.

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Ferramentas herdadas baseadas em Flashes

As ferramentas listadas nas seções a seguir foram removidas do sistema Workfront e substituídas por novas soluções.

Para obter informações sobre as ferramentas de substituição, consulte [Ferramentas herdadas baseadas em Flashes e suas substituições](#legacy-flash-based-tools-and-their-replacements) neste artigo.

### Gerenciamento de recursos

* A guia Planejamento de recursos herdados na área Pessoas e todas as ferramentas contidas na guia, que inclui o seguinte:

   * Gerenciador de Estimativa de Recursos
   * Planejador de Capacidade
   * Estimativas de Recursos
   * Grade de Recursos\
     Para obter mais informações, consulte [Planejamento de recursos no Adobe Workfront](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* A área Estimativas de recursos legados no Business Case de um projeto

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

  .

* A subguia Grade de Recursos na guia Equipe de um projeto
* A opção Usar nova área de agendamento na subguia Agendamento da guia Equipe de um projeto que remove a área de agendamento herdada ou o Criador de equipe. Nesse caso, a linha do tempo Scheduling agora é exibida por padrão.
* A guia Alocação no perfil do usuário

### Relatórios

Os seguintes recursos e relatórios de relatórios foram removidos:

* Recursos de relatórios removidos:

   * A opção Grade de Recursos em um relatório do usuário
   * A opção Gantt herdado em um relatório de projeto ou tarefa\
     Para obter mais informações, consulte [Exibir informações no Gráfico de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Relatórios removidos:

   * O relatório Conjunto de recursos herdados
   * O relatório Estimativas de recursos

  >[!NOTE]
  >
  >Todos os campos herdados acessados por meio de relatórios ou pela API (Conjunto de recursos herdados, Custo orçado herdado, Custo herdado, Horas orçadas herdadas, Custo do trabalho orçado herdado etc.) são exibidos em vários relatórios, mas não são preenchidos com novas informações.

### Diagrama de Gantt antigo

* Todas as exibições de Gantt herdadas das listas de projetos e tarefas, bem como relatórios e opções de relatórios
* As subguias do Diagrama de Gantt herdado em Portfolio e Programas
* A subguia Gantt Herdado em uma lista de Tarefas de Modelo em um Modelo, a exibição Gantt Herdado na guia Subtarefas de uma Tarefa de Modelo e em um relatório de Tarefa de Modelo

### Prova

O visualizador de provas herdadas foi substituído pelo novo Visualizador de provas da Web e Visualizador de provas de desktop para a maioria dos clientes e foi removido para todos os clientes em novembro de 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Para obter mais informações, consulte os seguintes recursos:

* [Revisar provas no Visualizador de provas da Web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Revisar provas no Visualizador de provas da área de trabalho](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## Ferramentas herdadas baseadas em Flashes e suas substituições {#legacy-flash-based-tools-and-their-replacements}

Salvo especificação em contrário, todos os recursos herdados foram substituídos por novos, conforme mostrado na tabela a seguir.

>[!CAUTION]
>
>As ferramentas herdadas baseadas em Flashes foram removidas de todos os ambientes.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Ferramentas herdadas</strong> </p> </th> 
   <th> <p><strong>Novas ferramentas</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Conjuntos de recursos legados</strong> </p> <p>Conjuntos de recursos legados eram grupos ou coleções de funções de trabalho necessárias ao mesmo tempo para a conclusão de um projeto. Os Conjuntos de recursos legados apresentavam várias deficiências:</p> 
    <ul> 
     <li> Você poderia associar um usuário a um Conjunto de recursos herdados, mas ele só era usado para fins de relatório. Como os Conjuntos de Recursos Legados estavam operando com entidades de função de trabalho abstratas, nenhuma das exceções de agendamento e folga dos usuários foi considerada, resultando em dados imprecisos sobre a disponibilidade de recursos. </li> 
    </ul> 
    <ul> 
     <li>Você pode especificar apenas um Conjunto de Recursos Legados por projeto, o que resultou em vários Conjuntos de Recursos Legados que dão suporte apenas ao fluxo de grupos separados que trabalham independentemente uns dos outros e que nunca compartilham recursos. Em todos os outros casos, foi recomendado manter um Conjunto de recursos herdados que incluísse todos os recursos no sistema, o que resultava em problemas de desempenho com grandes quantidades de projetos e dados.</li> 
    </ul> </td> 
   <td> <p><strong>Conjunto de recursos</strong> </p> <p>Os novos Conjuntos de recursos são uma coleção de usuários necessários ao mesmo tempo para a conclusão do projeto. A Workfront também percebe que há casos em que usuários especializados precisam ter o trabalho alocado a eles separadamente. Por esse motivo, agora você pode estimar usuários em vez de funções de trabalho. </p> As vantagens do Conjunto de recursos em relação aos Conjuntos de recursos legados incluem: 
    <ul>
     <li>Como os Conjuntos de recursos são baseados nos usuários, suas exceções de folga e agendamento já são consideradas para os cálculos de disponibilidade de usuário e função. Isso resulta em dados precisos e atualizados, permitindo decisões orçamentárias corretas e minimizando a probabilidade de alterações quando o projeto está em andamento.</li>
     <li>Como agora há mais controle sobre a disponibilidade de recursos e a precisão dos dados, o Workfront permite associar vários Conjuntos de recursos a um projeto. Um usuário também pode pertencer a mais de um Conjunto de recursos, caso tenha várias habilidades que podem ser usadas em vários projetos ao mesmo tempo. </li>
    </ul><p>Com esse controle sobre os dados, não é mais necessário ter um Conjunto de recursos que inclua todos os recursos para distribuir o orçamento disponível. Na verdade, não recomendamos isso. Em vez disso, recomendamos diversificar seus Conjuntos de recursos e associar apenas Conjuntos de recursos relevantes aos projetos.</p><p> Para obter mais informações sobre Conjuntos de recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos conjuntos de recursos </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gerenciador de Estimativa de Recursos</strong> </p> <p>Você pode usar o Gerenciador de Estimativa de Recursos para especificar a disponibilidade dos recursos da função de trabalho em vários Conjuntos de Recursos. No entanto, devido às deficiências do Conjunto de recursos herdados, essa funcionalidade raramente era usada. Quando era usado, forçava os usuários a inserir manualmente a disponibilidade de funções de trabalho para tornar o orçamento mais preciso. As exceções de agendamento e o tempo de folga dos usuários não foram considerados.</p> </td> 
   <td> <p>Com o cálculo automático da disponibilidade baseado nos usuários nos Conjuntos de Recursos, o Gerenciador de Estimativa de Recursos não é mais necessário. A ferramenta foi eliminada, juntamente com todo o trabalho manual para calcular a disponibilidade.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimativas de Recursos</strong> </p> <p>A guia Estimativas de Recursos em cada Conjunto de Recursos Legados atendia à mesma finalidade do Gerenciador de Orçamento de Recursos, somente no contexto de um Conjunto de Recursos Legados. Essa ferramenta apresentou as mesmas limitações que o Gerenciador de Estimativa de Recursos e os Conjuntos de Recursos Legados: dados imprecisos e entrada manual de disponibilidade. </p> </td> 
   <td> <p>Com o cálculo automático da disponibilidade de usuários, as Estimativas de Recursos se tornaram obsoletas e foram removidas.</p> <p>A ferramenta é eliminada nos Conjuntos de recursos legados e nas Estimativas de recursos legados no Business Case de um projeto. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Planejador de Capacidade</strong> </p> <p>O Planejador de Capacidade era uma ferramenta do Workfront para orçar recursos e priorizar projetos dentro de um Conjunto de Recursos Legados, de acordo com a disponibilidade dos recursos. Dada a incompletude dos dados das estimativas de recursos e do gestor de orçamento de recursos que forneceram as informações para o Planejador de capacidade, a priorização dos projetos teve de ser verificada em função da disponibilidade dos utilizadores.</p> <p>O uso de um único Conjunto de recursos herdados que incluía todas as funções de trabalho no sistema era o cenário mais comum, o que resultava em problemas de desempenho com o Planejador de Capacidade tentando carregar um grande número de projetos.</p> </td> 
   <td> <p><strong>A Visão do Projeto do Planejador de Recursos</strong> </p> <p>Na visualização baseada em projeto do Planejador de recursos, você pode orçar recursos e priorizar projetos de forma semelhante a como fazia no Planejador de capacidade herdado. Diferentemente da ferramenta herdada, agora há suporte para mais dados, com as informações disponíveis mais precisas, levando em conta as exceções de tempo de folga e de agendamento dos usuários.</p> <p>As informações disponíveis, planejadas e orçadas são visíveis rapidamente para que os Gerentes de recursos possam ver se há pessoas suficientes para fazer o trabalho e se os planos de projeto excedem as estimativas de orçamento iniciais.</p> <p> Para obter informações sobre como usar a Visualização Projeto no Planejador de recursos, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a></p> <p><strong>O Planejador de cenários</strong> </p> <p>Para o planejamento de capacidade de longo prazo, modelagem e priorização de cenários hipotéticos, também introduzimos o Planejador de cenários da Workfront. </p> <p>O Planejador de cenários está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de cenários do Workfront, consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">A visão geral do Planejador de cenários</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimativas de recursos legados (Business Case)</strong> </p> <p>Você pode usar a área Estimativas de recursos legados do Business Case para orçar uma certa quantidade de horas e custos de mão de obra como parte do planejamento do projeto e da solicitação de recursos. Essa visualização não dava visibilidade à disponibilidade de recursos, o que resultava em solicitações aproximadas de recursos e uma maior chance de trabalho de projeto rejeitado.</p> </td> 
   <td> <p><strong>Estimativa de recursos (Business Case)</strong> </p> <p>A seção Orçamento de recursos no Business Case traz os recursos do Planejador de recursos para o Business Case, fornecendo visibilidade sobre a disponibilidade de usuários e funções, bem como a capacidade de orçar no nível do usuário. </p> <p> Para obter informações sobre a área Orçamento de recursos do Business Case, consulte <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Visão geral das áreas do business case</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Relatórios de Estimativa de Recursos</strong> </p> <p>Ao usar as ferramentas herdadas para o Gerenciamento de recursos, você pode relatar as horas orçadas e planejadas do Business Case. Isso permitiu criar relatórios de matriz mostrando o trabalho total Orçado e Planejado para cada função de trabalho em um intervalo de tempo específico. Este relatório não era editável e você não podia fazer alterações no orçamento de seus recursos com base nos resultados do relatório. </p> </td> 
   <td> <p><strong>Relatório de Utilização</strong> </p> <p>O relatório de Utilização interna exibe lado a lado as Horas Planejadas, Orçadas e Reais, o Custo e a Receita. </p> <p>Para obter informações sobre o uso do relatório de Utilização, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações de utilização de recursos </a>. </p> 
    <div> 
     <p><strong>Horas Orçadas Relatáveis</strong> </p> 
     <p>Crie um relatório para Horas orçadas para revisar as horas orçadas no Planejador de recursos em um formulário de relatório. </p> 
     <p>Para obter informações sobre horas orçadas, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossário da terminologia do Adobe Workfront</a>.</p> 
     <p>Para obter informações sobre como criar um relatório, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> 
    </div> <p><strong>A Visão da Função do Planejador de Recursos</strong> </p> <p>As horas orçadas e planejadas do Business Case nas ferramentas de Gerenciamento de recursos legados agora estão disponíveis em uma nova visualização nativa: a visualização baseada em função do Planejador de recursos. Essa exibição fornece informações sobre Horas Disponíveis, Planejadas e Orçadas rapidamente e permite controlar e alterar o orçamento no mesmo local. Isso garante uma melhor tomada de decisões durante o planejamento de funções de trabalho de alto nível. </p> <p> Para obter informações sobre recursos de orçamento na Exibição Função do Planejador de Recursos, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Usar as Exibições de Projeto e Função para orçar recursos </a> seção em <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Grade de Recursos</strong> </p> <p>A Grade de Recursos forneceu visibilidade sobre a alocação de usuários específicos à medida que um projeto avançava até a conclusão. </p> <p>Por exemplo, você pode ver facilmente quando alguém em sua equipe de projeto fez o trabalho antecipadamente e quando alguém ficou para trás, bem como se ele estava superalocado ou subalocado para um período específico. </p> <p>Infelizmente, você não pôde agir de acordo com as informações na mesma visão. Para corrigir problemas de excesso de alocação, você tinha que ir aos projetos e ajustar manualmente as informações lá, sem qualquer visibilidade sobre o resultado de suas ações.</p> </td> 
   <td> <p>A Grade de Recursos foi substituída por duas novas ferramentas. É possível usar as seguintes ferramentas, dependendo da fase do planejamento de recursos em que você estiver:</p> 
    <ul> 
     <li> <p><strong>Para a fase analítica:</strong> </p> 
      <ul> 
       <li> <p><strong>O Balanceador de carga de trabalho</strong>: use o Balanceador de carga de trabalho para exibir a carga de trabalho dos usuários em um nível mais granular. Ao usar o Balanceador de carga de trabalho, você pode visualizar quais usuários têm disponibilidade em sua carga de trabalho para concluir a tarefa no prazo. Isso inclui os detalhes de folga e exceções da programação. </p> <p>Para obter informações sobre o Balanceador de carga de trabalho, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Visão geral do Balanceador de carga de trabalho</a>.</p> </li> 
       <li> <p><strong>A Visão de Usuário do Planejador de Recursos</strong><strong>:</strong> Ao tentar entender em um nível superior a quais projetos seus usuários estão alocados, use a Exibição de usuário do Planejador de recursos. Isso permite que você veja em quais usuários estão trabalhando, bem como seus superalocações e subalocações para um intervalo de tempo específico. O Planejador de recursos também fornece visualização da alocação geral de usuários como um todo, bem como visibilidade das Horas Reais registradas, o que é útil para analisar o progresso do trabalho feito. </p> <p>Para obter informações sobre como usar a Visualização Usuário no Planejador de recursos, consulte a <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Use a Exibição de Usuário para exibir Horas Disponíveis, Planejadas e Reais ou FTE </a> seção em <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a></p> </li> 
      </ul> </li> 
     <li><strong>Para a fase tática:</strong> 
      <ul> 
       <li><strong>O Balanceador de carga de trabalho</strong> Você pode fazer o seguinte usando o Balanceador de carga de trabalho: 
        <ul>
         <li>Atribuir trabalho aos usuários.</li>
         <li>Gerenciar alocações de usuários para itens de trabalho. </li>
         <li>Compartilhe o Balanceador de carga de trabalho com outros usuários que podem não ter visibilidade sobre a área Pessoas. Use a funcionalidade Link compartilhável para compartilhar um link para o Balanceador de carga de trabalho e incorporá-lo aos painéis personalizados. Qualquer usuário com acesso a Exibir usuários pode exibir esses painéis quando você os compartilha.</li>
        </ul><p>O Balanceador de carga de trabalho está disponível na área Pessoas. </p><p>Para obter informações sobre o Balanceador de carga de trabalho, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Visão geral do Balanceador de carga de trabalho</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gráfico de Gantt legado, Lista de tarefas</strong> </p> <p> O gráfico de Gantt Herdado na lista de tarefas forneceu aos usuários a capacidade de visualizar a linha do tempo do projeto e executar o planejamento do cenário hipotético sem confirmar as alterações no banco de dados. O gráfico de Gantt herdado era baseado na tecnologia Flash, que apresentava riscos de segurança. </p> </td> 
   <td> <p><strong>Gráfico de Gantt,</strong> <strong>Lista de tarefas</strong></p> <p> O novo Gráfico de Gantt baseado em HTML está atendendo à mesma finalidade do Gantt herdado. Os usuários podem visualizar a linha do tempo do projeto e executar o planejamento de cenário hipotético sem confirmar as alterações no banco de dados, alterando para a opção Salvar manual na barra de ferramentas da lista de tarefas. </p> <p>O novo Gráfico de Gantt é interativo ao usar a opção de Salvamento automático que você pode usar quando quiser salvar automaticamente as alterações à medida que elas ocorrerem. </p> <p>O novo Diagrama de Gantt da Lista de Tarefas foi criado com base na tecnologia mais recente e é confiável. Este novo Gráfico de Gantt está localizado diretamente na lista de tarefas e é facilmente acessado enquanto trabalha na lista de tarefas sem alternar guias ou alterar a exibição. </p> <p>Embora o novo Diagrama de Gantt ofereça a mesma funcionalidade do Diagrama anterior, há algumas diferenças nos recursos em comparação com o Diagrama de Gantt herdado. </p> <p> A subguia Gantt Herdado em uma lista de Tarefas de Modelo em um Modelo, a exibição Gantt Herdado na guia Subtarefas de uma Tarefa de Modelo e o gráfico Gantt Herdado em um relatório de Tarefa de Modelo também foram substituídos pelo gráfico Gantt baseado em HTML. </p> <p>Se você usar o Gráfico de Gantt herdado principalmente para a exibição simples e edições rápidas e não usar o gráfico real, a nova opção Planejamento de linha do tempo permitirá fazer alterações rápidas nos principais campos de planejamento. Você pode selecionar Planejamento de linha do tempo em vez de Salvar automaticamente na barra de ferramentas da lista de tarefas.</p> <p>Para obter mais informações sobre como salvar uma lista de tarefas usando a opção Planejamento de linha do tempo, consulte a seção "Salvar alterações em uma lista de tarefas manualmente ao selecionar a opção Planejamento de linha do tempo" no artigo <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tarefas em uma lista</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gráfico de Gantt legado para uma lista de projetos</strong> </p> <p>O gráfico de Gantt herdado na lista de projetos fornecia aos usuários a capacidade de ver projetos e suas tarefas em uma única visualização. Sem sair do contexto da lista de projetos, os usuários poderiam ver detalhes sobre as tarefas em um projeto, bem como as dependências entre os projetos. O gráfico de Gantt herdado na lista de projetos era baseado na tecnologia Flash, que apresentava riscos de segurança. </p> </td> 
   <td> <p><strong>Gráfico de Gantt, Lista de Projetos</strong> </p> <p>O Gráfico de Gantt baseado em HTML tem o mesmo objetivo que o Gráfico de Gantt herdado. Os usuários podem exibir projetos e suas tarefas em uma única exibição para identificar visualmente as dependências entre projetos e tarefas. O Diagrama de Gantt da Lista de Projetos está localizado diretamente na lista de projetos. O novo Diagrama de Gantt tem uma interface moderna e é construído com base na tecnologia mais recente.</p> <p>Para obter informações sobre o gráfico de Gantt da lista de projetos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Exibir informações no Gráfico de Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Compartilhamento de caixas de diálogo para relatórios, calendários e documentos</strong> </p> <p>Ao compartilhar relatórios, calendários e documentos, as caixas de diálogo usadas se baseavam na tecnologia do Flash.</p> </td> 
   <td> <p>A experiência ao compartilhar relatórios, calendários e documentos no Workfront não foi alterada. No entanto, a experiência não depende mais do Flash.</p> <p>Para obter mais informações sobre o compartilhamento desses itens, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral das permissões de compartilhamento em objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visualizador de provas herdadas</strong> </p> <p>O visualizador de provas herdadas era um visualizador de provas baseado na Web que fornecia recursos de provas para provas estáticas, de vídeo e interativas.</p> </td> 
   <td> <p><strong>Visualizador de provas da web e visualizador de provas da área de trabalho</strong> </p> <p>O Visualizador de provas da Web fornece recursos de provas para provas estáticas e de vídeo.</p> <p>O Visualizador de provas de desktop fornece recursos de prova para provas interativas, além de oferecer suporte completo para provas estáticas e de vídeo.</p> <p>O formato de arquivo SWF não é mais suportado por nenhum dos principais provedores e foi substituído por banners HTML5 para prova. </p> <p>Para obter informações mais detalhadas sobre as diferenças entre os revisores de prova disponíveis, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Diferenças entre o Visualizador de provas da Web e a visão geral do Visualizador de provas do desktop</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
