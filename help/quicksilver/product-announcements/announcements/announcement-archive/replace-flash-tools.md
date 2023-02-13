---
title: Substituição de ferramentas baseadas em Flashes no Adobe Workfront
description: Substituição de ferramentas baseadas em Flashes no Adobe Workfront
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '2705'
ht-degree: 1%

---

# Substituição de ferramentas baseadas em Flashes no Adobe Workfront

Removemos todas as ferramentas baseadas em Flashes do Adobe Workfront Classic.

As ferramentas de substituição baseadas nos padrões atuais estão disponíveis no Workfront. Essas alterações estão alinhadas com o fim do suporte para produtos Flash, conforme anunciado pelo Adobe.

## Datas importantes

As datas a seguir são importantes para o processo de remoção de todas as ferramentas baseadas em Flashes no Workfront:

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **19 de novembro de 2020**: Todas as ferramentas baseadas em Flashes foram removidas de todos os produtos da Workfront.

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## Ferramentas herdadas baseadas em Flashes

As ferramentas listadas nas seções a seguir foram removidas do sistema Workfront e substituídas por novas soluções.

Para obter informações sobre ferramentas de substituição, consulte [Ferramentas herdadas baseadas em Flashes e suas substituições](#legacy-flash-based-tools-and-their-replacements) neste artigo.

### Gerenciamento de recursos

* A guia Planejamento de recursos herdados na área Pessoas e todas as ferramentas contidas na guia , que inclui o seguinte:

   * Gerenciador de Estimativa de Recursos
   * Planejador de Capacidade
   * Estimativas de Recursos
   * Grade de Recursos\
      Para obter mais informações, consulte [Planejamento de recursos no Adobe Workfront](../../../resource-mgmt/resource-planning/resource-planning-overview.md).

* A área Estimativas de recursos herdados no Caso de negócios de um projeto

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

* A subguia Grade de Recurso na guia Pessoal de um projeto
* A opção Usar nova área de agendamento na subguia Agendamento da guia Pessoal de um projeto que remove a área de Agendamento herdada ou o Construtor de equipe. Nesse caso, a linha do tempo de Agendamento agora é exibida por padrão.
* A guia Alocação no perfil do usuário

### Relatórios

Os seguintes recursos de relatórios e relatórios foram removidos:

* Remoção dos recursos de relatório:

   * A opção Grade de Recurso em um relatório de usuário
   * A opção Gantt herdado em um relatório de projeto ou tarefa\
      Para obter mais informações, consulte [Exibir informações no Gráfico de Gantt](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

* Relatórios removidos:

   * O relatório do Pool de Recursos Herdado
   * O relatório Estimativas de recursos

   >[!NOTE]
   >
   >Todos os campos herdados acessados por meio de relatórios ou pela API (Pool de Recursos Herdados, Custo Previsto Orçado, Custo Herdado, Horas Orçadas Herdadas, Custo Herdado da Mão de Obra Orçada etc.) são exibidos em vários relatórios, mas não são preenchidos com novas informações.

### Diagrama de Gantt antigo

* Todas as exibições de Gantt herdadas das listas de projetos e tarefas, bem como relatórios e opções de relatórios
* As sub-guias de Gantt herdado em Portfolio e programas
* A subguia Gantt herdado em uma lista de Tarefas de modelo em um modelo, a exibição Gantt herdado na guia Subtarefas de uma Tarefa de modelo e em um relatório de Tarefa de modelo

###  Prova

O Visualizador de prova de digital herdado foi substituído pelo novo Visualizador de prova de web e Visualizador de prova de desktop para a maioria dos clientes e foi removido para todos os clientes em novembro de 2020.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

Para obter mais informações, consulte os seguintes recursos:

* [Revisar provas no Visualizador de Provas da Web](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [Revisar provas no Visualizador de prova de desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

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

Exceto quando especificado de outra forma, todos os recursos herdados foram substituídos por novos, conforme mostrado na tabela a seguir.

>[!CAUTION]
>
>As ferramentas herdadas, baseadas em Flashes, foram removidas de todos os ambientes.

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
   <td> <p><strong>Conjuntos de recursos legados</strong> </p> <p>Os Pools de Recursos Herdados eram grupos ou coleções de funções de trabalho necessárias ao mesmo tempo para a conclusão de um projeto. Os pools de recursos herdados apresentavam várias falhas:</p> 
    <ul> 
     <li> Você poderia associar um usuário a um Pool de Recursos Herdados, mas ele era usado apenas para fins de relatório. Como os Pools de Recursos Herdados estavam operando com entidades abstratas de função de trabalho, nenhuma das exceções de programação e tempo de folga dos usuários foram consideradas, resultando em dados imprecisos sobre a disponibilidade de recursos. </li> 
    </ul> 
    <ul> 
     <li>Você poderia especificar apenas um Pool de Recursos Herdados por projeto, o que resultava em vários Pools de Recursos Herdados que ofereciam suporte somente ao fluxo de grupos separados que trabalhavam independentemente uns dos outros e nunca compartilhavam recursos. Em todos os outros casos, foi recomendável manter um Pool de Recursos Herdados que incluísse todos os recursos no sistema, o que levou a problemas de desempenho com grandes quantidades de projetos e dados.</li> 
    </ul> </td> 
   <td> <p><strong>Conjunto de Recursos</strong> </p> <p>Novos Pools de Recursos são uma coleção de usuários que são necessários ao mesmo tempo para a conclusão do projeto. A Workfront também sabe que há casos em que usuários especializados precisam ter trabalho alocado para eles separadamente. Por isso, agora você pode orçar usuários em vez de funções de trabalho. </p> As vantagens do Pool de Recursos sobre os Pools de Recursos Legados incluem o seguinte: 
    <ul>
     <li>Como os Pools de Recursos são baseados nos usuários, suas exceções de tempo limite e programação já são consideradas para os cálculos de disponibilidade de função e usuário. Isso resulta em dados precisos e atualizados, permitindo decisões corretas de orçamento e minimizando a probabilidade de alterações quando o projeto estiver em andamento.</li>
     <li>Como agora há mais controle sobre a disponibilidade de recursos e a precisão dos dados, o Workfront permite associar vários Pools de Recursos a um projeto. Um usuário também pode pertencer a mais de um pool de recursos, caso tenha várias habilidades que podem ser usadas em vários projetos ao mesmo tempo. </li>
    </ul><p>Com esse controle sobre os dados, não é mais necessário ter um pool de recursos que inclua todos os recursos para distribuir o orçamento disponível. Na verdade, não recomendamos isso. Em vez disso, recomendamos diversificar seus Conjuntos de Recursos e associar apenas os Conjuntos de Recursos relevantes aos projetos.</p><p> Para obter mais informações sobre Pools de Recursos, consulte <a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref"> Visão geral dos pools de recursos </a></p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gerenciador de Estimativa de Recursos</strong> </p> <p>Você poderia usar o Gerenciador de Orçamento de Recursos para especificar a disponibilidade de recursos de função de cargo em vários Pools de Recursos. No entanto, devido às deficiências do Pool de Recursos Herdados, essa funcionalidade raramente foi usada. Quando foi usado, isso forçou os usuários a inserir manualmente a disponibilidade de funções de trabalho para tornar o orçamento mais preciso. As exceções de agendamento e o tempo de folga dos usuários não foram considerados.</p> </td> 
   <td> <p>Com o cálculo automático da disponibilidade com base nos usuários nos Pools de Recursos, o Gerenciador de Orçamento de Recursos não é mais necessário. A ferramenta foi eliminada, juntamente com todo o trabalho manual para calcular a disponibilidade.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimativas de Recursos</strong> </p> <p>A guia Estimativas de Recursos em cada Pool de Recursos Herdados tinha a mesma finalidade que o Gerenciador de Orçamento de Recursos, somente no contexto de um Pool de Recursos Herdados. Esta ferramenta apresentou as mesmas limitações que o Gerenciador de Orçamento de Recursos e os Pools de Recursos Legados: dados imprecisos e entrada manual de disponibilidade. </p> </td> 
   <td> <p>Com o cálculo automático da disponibilidade do usuário, as Estimativas de Recursos tornaram-se obsoletas e foram removidas.</p> <p>A ferramenta é eliminada nos Pools de Recursos Herdados e nas Estimativas de Recursos Herdados no Caso de Negócios de um projeto. <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Planejador de Capacidade</strong> </p> <p>O Planejador de Capacidade era uma ferramenta da Workfront para orçar recursos e priorizar projetos dentro de um Pool de Recursos Herdados, de acordo com a disponibilidade dos recursos. Dada a insuficiência de dados provenientes das estimativas de recursos e do gestor de orçamento de recursos que forneceram as informações para o plano de capacidade, a priorização do projeto teve de ser verificada duas vezes em relação à disponibilidade dos utilizadores.</p> <p>Usar um único Pool de Recursos Herdados que incluísse todas as funções de trabalho no sistema foi o cenário mais comum, o que levou a problemas de desempenho com o Capacity Planner tentando carregar um grande número de projetos.</p> </td> 
   <td> <p><strong>A Visualização de Projeto do Planejador de Recursos</strong> </p> <p>Na exibição baseada em projeto do Planejador de Recursos, é possível orçar recursos e priorizar projetos de forma semelhante à forma como você costumava fazer isso no Planejador de Capacidade Herdado. Ao contrário da ferramenta herdada, agora há suporte para mais dados, com as informações disponíveis mais precisas levando em conta as exceções de tempo limite e agendamento dos usuários.</p> <p>As informações disponíveis, programadas e orçadas são visíveis rapidamente para que os Gerentes de Recursos possam ver se há pessoas suficientes para fazer o trabalho e se os planos do projeto excedem as estimativas iniciais do orçamento.</p> <p> Para obter informações sobre o uso da Visualização de projeto no Planejador de Recursos, consulte <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a></p> <p><strong>O Planejador de Cenário</strong> </p> <p>Para o planejamento de capacidade de longo prazo, modelagem de cenário de hipóteses e priorização, também introduzimos o Workfront Scenario Planner . </p> <p>O Planejador de cenário está disponível somente na nova experiência do Adobe Workfront e requer uma licença adicional. Para obter informações sobre o Planejador de Cenário do Workfront, consulte <a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">A visão geral do Planejador de cenário</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Estimativas de recursos herdados (Caso de negócios)</strong> </p> <p>Você poderia usar a área Estimativas de recursos herdados do Caso de negócios para orçar uma determinada quantidade de horas e custos de mão de obra como parte do planejamento do projeto e da solicitação de recursos. Esta exibição não forneceu visibilidade sobre a disponibilidade de recursos, o que resultou em solicitações aproximadas de recursos e em uma maior chance de trabalho de projeto rejeitado.</p> </td> 
   <td> <p><strong>Orçamentação de Recursos (Caso Comercial)</strong> </p> <p>A seção Orçamento de Recursos no Caso de Negócios traz os recursos do Planejador de Recursos ao Caso de Negócios, fornecendo visibilidade sobre a disponibilidade do usuário e da função, bem como sobre a capacidade de orçar no nível do usuário. </p> <p> Para obter informações sobre a área Orçamento de Recursos do Caso de Negócios, consulte <a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">Visão geral das áreas do caso comercial</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Relatórios de Estimativa de Recursos</strong> </p> <p>Ao usar as ferramentas herdadas para o Gerenciamento de Recursos, você pode gerar relatórios sobre as horas orçadas e Planejadas do Caso de Negócios. Isso permitia criar relatórios de matriz mostrando o trabalho total orçado e planejado para cada função de cargo em um período específico. Este relatório não era editável e não era possível fazer alterações no orçamento de seus recursos com base nas conclusões do relatório. </p> </td> 
   <td> <p><strong>Relatório de utilização</strong> </p> <p>O relatório integrado de Utilização exibe as Horas Planejadas, Orçadas e Reais, o Custo e a Receita lado a lado. </p> <p>Para obter informações sobre como usar o relatório Utilização, consulte <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">Exibir informações de utilização de recursos </a>. </p> 
    <div> 
     <p><strong>Horas Orçamentadas Reportáveis</strong> </p> 
     <p>Crie um relatório para Horas Orçadas para revisar as horas orçadas no Planejador de Recursos em um formulário de relatório. </p> 
     <p>Para obter informações sobre Horas Orçadas, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Glossário da terminologia do Adobe Workfront</a>.</p> 
     <p>Para obter informações sobre como criar um relatório, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Criar um relatório personalizado</a>.</p> 
    </div> <p><strong>A Exibição de Função do Planejador de Recursos</strong> </p> <p>As horas orçadas e planejadas do Business case nas ferramentas de Gerenciamento de Recursos Herdados agora estão disponíveis em uma nova exibição nativa - a exibição baseada em Função do Planejador de Recursos. Esta exibição fornece informações sobre Horas Disponíveis, Planejadas e Orçadas imediatamente e permite que você controle e altere o orçamento tudo no mesmo lugar. Isso garante uma melhor tomada de decisões durante o planejamento de funções de alto nível. </p> <p> Para obter informações sobre como orçar recursos na Exibição de Função do Planejador de Recursos, consulte o <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">Usar as Exibições de Projeto e Função para recursos do orçamento </a> seção em <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Grade de Recursos</strong> </p> <p>A Grade de Recurso deu visibilidade à alocação de usuários específicos conforme um projeto avançava para a conclusão. </p> <p>Por exemplo, você pode ver facilmente quando alguém em sua equipe de projeto fez o trabalho adiantado e quando alguém ficou para trás, bem como se eles foram realocados ou sub-alocados por um período específico. </p> <p>Infelizmente, não foi capaz de agir com base nas informações do mesmo ponto de vista. Para corrigir problemas de atribuição excessiva, você tinha que ir para os projetos e ajustar manualmente as informações lá, sem nenhuma visibilidade do resultado de suas ações.</p> </td> 
   <td> <p>A Grade de Recurso foi substituída por duas novas ferramentas. Você pode usar as seguintes ferramentas, dependendo de qual fase do planejamento de recursos você se encontra:</p> 
    <ul> 
     <li> <p><strong>Para a fase analítica:</strong> </p> 
      <ul> 
       <li> <p><strong>O Balanceador de Carga de Trabalho</strong>: Use o Balanceador de Carga de Trabalho para exibir a carga de trabalho dos usuários em um nível mais granular. Ao usar o Balanceador de Carga de Trabalho, você pode visualizar quais usuários têm disponibilidade em sua carga de trabalho para concluir a tarefa a tempo. Isso inclui os detalhes de tempo limite e de exceções de programação. </p> <p>Para obter informações sobre o Balanceador de Carga de Trabalho, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Visão Geral do Balanceador de Carga de Trabalho</a>.</p> </li> 
       <li> <p><strong>A Visualização de Usuário do Planejador de Recursos</strong><strong>:</strong> Ao tentar entender em um nível superior quais projetos seus usuários estão alocados, use a Visualização de usuário do Planejador de Recursos. Isso permite ver no que os usuários estão trabalhando, bem como sua alocação excessiva e insuficiente para um período específico. O Planejador de Recursos também fornece visualização da alocação geral de usuários como um todo, bem como visibilidade sobre as Horas Reais registradas, o que é útil para analisar o progresso do trabalho feito. </p> <p>Para obter informações sobre como usar a Visualização de usuário no Planejador de Recursos, consulte o <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">Use a Visualização de usuário para exibir as Horas Disponíveis, Planejadas e Reais ou FTE </a> seção em <a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">Visão geral do Planejador de recursos</a></p> </li> 
      </ul> </li> 
     <li><strong>Para a Fase Tática:</strong> 
      <ul> 
       <li><strong>O Balanceador de Carga de Trabalho</strong> Você pode fazer o seguinte usando o Balanceador de Carga de Trabalho: 
        <ul>
         <li>Atribuir trabalho aos usuários.</li>
         <li>Gerencie alocações de usuários para itens de trabalho. </li>
         <li>Compartilhe o Balanceador de Carga de Trabalho com outros usuários que podem não ter visibilidade na área Pessoas. Use a funcionalidade de link Compartilhável para compartilhar um link para o Balanceador de carga de trabalho e incorporá-lo a painéis personalizados. Qualquer usuário com acesso a Exibir usuários poderá visualizar esses painéis ao compartilhá-los.</li>
        </ul><p>O Balanceador de Carga de Trabalho está disponível na área Pessoas. </p><p>Para obter informações sobre o Balanceador de Carga de Trabalho, consulte <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">Visão Geral do Balanceador de Carga de Trabalho</a>.</p></li> 
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
   <td> <p><strong>Gráfico Gantt Herdado, Lista de Tarefas</strong> </p> <p> O gráfico Gantt herdado na lista de tarefas forneceu aos usuários a capacidade de visualizar a linha do tempo do projeto e executar o planejamento de cenário de hipóteses sem confirmar as alterações no banco de dados. O Gráfico de Gantt Herdado foi baseado na tecnologia de Flash, que apresentava riscos de segurança. </p> </td> 
   <td> <p><strong>Gráfico de Gantt,</strong> <strong>Lista de tarefas</strong></p> <p> O novo Gráfico de Gantt baseado em HTML está servindo o mesmo propósito do Gantt Herdado. Os usuários podem visualizar a linha do tempo do projeto e executar o planejamento de cenário de hipóteses sem confirmar as alterações no banco de dados, alterando para a opção Salvar manual na barra de ferramentas da lista de tarefas. </p> <p>O novo Gráfico de Gantt é interativo ao usar a opção de Salvamento automático , que você pode usar quando quiser salvar automaticamente suas alterações conforme elas ocorrerem. </p> <p>O novo Gráfico de Gantt da Lista de Tarefas é baseado na tecnologia mais recente e é confiável. Esse novo gráfico de Gantt está localizado diretamente na lista de tarefas e é facilmente acessado ao trabalhar na lista de tarefas sem trocar guias ou alterar a exibição. </p> <p>Embora o novo gráfico de Gantt ofereça a mesma funcionalidade que o gráfico anterior, há algumas diferenças nos recursos em comparação com o Gantt herdado. </p> <p> A subguia Gantt herdado em uma lista de Tarefas de modelo em um modelo, a exibição Gantt herdada na guia Subtarefas de uma tarefa de modelo e o gráfico Gantt herdado em um relatório de Tarefa de modelo também foram substituídos pelo gráfico Gantt baseado em HTML. </p> <p>Se você usar o Gráfico de Gantt Herdado principalmente para a visualização simples e edições rápidas e não usar o gráfico real, a nova opção Planejamento de Linha do Tempo permitirá fazer alterações rápidas nos campos de planejamento principais. Você pode selecionar Planejamento de Linha do Tempo em vez de Salvar automaticamente na barra de ferramentas da lista de tarefas.</p> <p>Para obter mais informações sobre como salvar uma lista de tarefas usando a opção Planejamento de Linha do Tempo, consulte a seção "Salvar alterações em uma lista de tarefas manualmente ao selecionar a opção Planejamento de Linha do Tempo" no artigo <a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">Editar tarefas em uma lista</a>. </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Gráfico de Gantt Herdado para uma Lista de Projetos</strong> </p> <p>O gráfico de Gantt herdado na lista de projetos forneceu aos usuários a capacidade de visualizar projetos e suas tarefas em uma única visualização. Sem deixar o contexto da lista de projetos, os usuários poderiam ver detalhes sobre as tarefas em um projeto, bem como as dependências entre os projetos. O Gráfico de Gantt herdado na lista de projetos era baseado na tecnologia Flash, que apresentava riscos de segurança. </p> </td> 
   <td> <p><strong>Gráfico de Gantt, Lista de Projetos</strong> </p> <p>O gráfico de Gantt baseado em HTML serve a mesma finalidade do gráfico de Gantt herdado. Os usuários podem visualizar projetos e suas tarefas em uma única visualização para identificar visualmente dependências entre projetos e tarefas. O gráfico Gantt da lista de projetos está localizado diretamente na lista de projetos. O novo gráfico de Gantt tem uma interface moderna e é construído com base na tecnologia mais recente.</p> <p>Para obter informações sobre o gráfico de Gantt da lista de projetos, consulte <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Exibir informações no Gráfico de Gantt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Caixas de diálogo de compartilhamento para relatórios, calendários e documentos</strong> </p> <p>Ao compartilhar relatórios, calendários e documentos, as caixas de diálogo usadas eram baseadas na tecnologia do Flash.</p> </td> 
   <td> <p>A experiência ao compartilhar relatórios, calendários e documentos no Workfront não foi alterada. No entanto, a experiência não depende mais do Flash.</p> <p>Para obter mais informações sobre como compartilhar esses itens, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral do compartilhamento de permissões em objetos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Visualizador de prova herdado</strong> </p> <p>O Visualizador de prova herdado era um visualizador de prova baseado na Web que fornecia recursos de revisão de tela para provas estáticas, de vídeo e interativas.</p> </td> 
   <td> <p><strong>Visualizador de prova de web e visualizador de prova de desktop</strong> </p> <p>O Web Proofing Viewer fornece recursos de prova para provas estáticas e de vídeo.</p> <p>O Desktop Proofing Viewer fornece recursos de prova para provas interativas, além de fornecer suporte total para provas estáticas e de vídeo.</p> <p>O formato de arquivo SWF não é mais compatível com nenhum dos principais provedores e foi substituído por banners de HTML5 para prova. </p> <p>Para obter informações mais detalhadas sobre as diferenças entre os visualizadores de prova disponíveis, consulte <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Diferenças entre o Visualizador de Provas da Web e a visão geral do Visualizador de Provas de Desktop</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
