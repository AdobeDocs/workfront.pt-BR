---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Navegar pelo Balanceador de Carga de Trabalho
description: Use o Balanceador de Carga de Trabalho para entender a disponibilidade de seus recursos e para atribuir trabalho aos usuários. Este artigo aborda o uso de ícones e configurações disponíveis para atualizar a exibição e navegar no Balanceador de carga de trabalho.
author: Alina
feature: Resource Management
exl-id: 60dabfc5-6a2e-4368-9dac-db48d0307895
source-git-commit: f150c57e8b83e73734b1cbeded7ef4c16d65097c
workflow-type: tm+mt
source-wordcount: '4050'
ht-degree: 0%

---

# Navegar pelo Balanceador de Carga de Trabalho

Use o Balanceador de Carga de Trabalho no Adobe Workfront para atribuir trabalho aos usuários com base em sua disponibilidade. Este artigo descreve como você pode usar configurações e opções para navegar no Balanceador de carga de trabalho e exibir as informações relevantes para você. Artigos adicionais listados aqui descrevem como você pode usar o Balanceador de Carga de Trabalho para gerenciar seus recursos e sua alocação para funcionar.

O Balanceador de carga de trabalho está disponível em várias áreas do Adobe Workfront. Navegá-la é semelhante em todas as áreas.

Para obter mais informações sobre onde o Balanceador de Carga de Trabalho está localizado, consulte [Localizar o Balanceador de Carga de Trabalho](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/locate-workload-balancer.html?lang=en).


## Requisitos de acesso

<!--drafted - replace table for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
<td><p>Current license: Standard </p>
    Or 
<p>Legacy license:</p>
    <ul>
    <li><p>Plan, when using the Workload Balancer for a team or in the Resourcing area </p></li>
    <li><p>Work, when using the Workload Balancer of a project </p></li>
    </ul>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Planejar, ao usar o Balanceador de Carga de Trabalho para uma equipe ou na área Recursos </p>
   <p>Trabalhe, ao usar o Balanceador de Carga de Trabalho de um projeto </p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Tarefas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p>Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar ou exibir permissões mais altas para projetos, tarefas e problemas </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.


## Considerações para exibir itens no Balanceador de Carga de Trabalho

Considere o seguinte ao exibir o Balanceador de Carga de Trabalho:

* O Balanceador de Carga de Trabalho exibe itens de trabalho em duas áreas separadas, dependendo de suas atribuições. Itens de trabalho e usuários são exibidos nas seguintes áreas:

   * **Trabalho Não Atribuído**: Itens que não têm atribuições ou são atribuídos somente a funções ou equipes de trabalho.
   * **Trabalho Atribuído**: Itens que são atribuídos a pelo menos um usuário. Os itens atribuídos são exibidos sob o nome do usuário atribuído.

   >[!NOTE]
   >
   >* Os itens atribuídos a uma função de trabalho ou a uma equipe que também são atribuídos a um usuário que é o destinatário principal não são exibidos na área Trabalho não atribuído.
   >
   >* Os itens atribuídos a um usuário e uma função de trabalho na qual a função de trabalho é selecionada como o destinatário principal do item são exibidos na área Trabalho Não Atribuído.
   >* Itens atribuídos a mais de um usuário são exibidos em todos os nomes de usuários na área de Trabalho atribuído.


* Quando um projeto não tem tarefas durante um período de tempo, a barra no nível do projeto se torna uma cor esmaecida.

   ![](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* Quando você não tem permissões para ver determinados itens, eles são exibidos como **Itens de trabalho inacessíveis** ou **Projetos inacessíveis**.

   ![](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* Os nomes dos itens de trabalho são exibidos à esquerda e sua linha do tempo é exibida à direita.
* O total de Horas Planejadas para cada item de trabalho é exibido à direita do nome do item de trabalho e à esquerda da barra que representa a linha do tempo do item de trabalho.
* O total de Horas Planejadas para cada projeto é exibido à direita do nome do projeto e à esquerda da barra que representa a linha do tempo do projeto.

   As informações de Horas Planejadas do projeto são um total de Horas Planejadas de todos os itens listados no Balanceador de Carga de Trabalho, e não um total de Horas Planejadas no projeto.

Para obter mais informações sobre a exibição de informações no Balanceador de Carga de Trabalho, consulte também os seguintes artigos:

* [Localizar o Balanceador de Carga de Trabalho](../workload-balancer/locate-workload-balancer.md)
* [Filtrar informações no Balanceador de Carga de Trabalho](../workload-balancer/filter-information-workload-balancer.md)
* [Compartilhar o Balanceador de Carga de Trabalho com um link](../workload-balancer/share-link-for-workload-balancer.md)
* [Atualizar itens de trabalho no Balanceador de Carga de Trabalho usando o Resumo](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md)

Para obter informações sobre como gerenciar recursos usando o Balanceador de Carga de Trabalho, consulte também os seguintes artigos:

* [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/assign-work-in-workload-balancer.html?lang=en)
* [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](https://experienceleague.adobe.com/docs/workfront/using/manage-resources/the-workload-balancer/manage-user-allocations-workload-balancer.html?lang=en)


## Navegue pelo Balanceador de Carga de Trabalho para vários projetos na área Recursos

Navegar pelo Balanceador de Carga de Trabalho é semelhante em todas as áreas de onde você o acessa.

As subseções a seguir descrevem como visualizar as informações no Balanceador de Carga de Trabalho para vários projetos.

É possível ajustar várias configurações e opções no Balanceador de Carga de Trabalho para exibir as informações em que você precisa se concentrar no período que faz mais sentido para você.

Após selecionar as configurações que deseja aplicar à sua exibição, o Balanceador de Carga de Trabalho lembra dessas configurações toda vez que você o acessa de qualquer navegador ou dispositivo.

### Acesse o Balanceador de Carga de Trabalho para vários projetos na área Recursos

Para navegar pelo Balanceador de Carga de Trabalho para vários projetos:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Recursos**.
1. Clique em **Balanceador de Carga de Trabalho** no painel esquerdo.

   ![](assets/nwe-balancer-global.png)

   O Balanceador de Carga de Trabalho exibe informações de atribuição de trabalho começando com a semana atual nas duas áreas a seguir:

   * O **Trabalho Não Atribuído** exibe os seguintes itens de trabalho:

      * Itens de trabalho (tarefas e problemas) atribuídos a funções, equipes ou que não estão atribuídos são exibidos após a aplicação de filtros.
A Área de Trabalho Não Atribuído não exibe nenhum item de trabalho por padrão. Recomendamos usar filtros para exibir informações relevantes para você nessa área.

         Para obter informações sobre como usar filtros, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../workload-balancer/filter-information-workload-balancer.md).

      * Os projetos são exibidos somente quando você ativa a configuração Agrupar por projeto . Para obter mais informações, consulte a seção [Personalizar a visualização](#customize-the-view) neste artigo.
   * O **Trabalho Atribuído** exibe os seguintes itens de trabalho:

      * Todos os usuários ativos no sistema são exibidos nessa área por padrão. Recomendamos o uso de filtros para limitar a quantidade de informações nessa área. Se os usuários forem atribuídos a itens, os itens de trabalho também serão exibidos sob seu nome.

      * Tarefas e problemas atribuídos a pelo menos um usuário são exibidos sob o nome do usuário.

         Os itens de trabalho em nomes de usuários na área de Trabalho Atribuído são classificados de acordo com os seguintes critérios, nesta ordem:

         1. Data de início planejada (mais antiga primeiro)
         1. Data de conclusão planejada (mais antiga primeiro)
         1. Alfabético por projeto (somente quando os dois primeiros critérios são idênticos para vários itens de trabalho)

            >[!TIP]
            >
            >* Você pode personalizar a classificação do projeto selecionando uma opção na configuração &quot;Classificar projetos por&quot;.
            >
            >* Os projetos são exibidos somente quando a configuração &quot;Agrupar por projeto&quot; é ativada.

            > 
            >Para obter informações sobre como personalizar configurações, consulte a seção [Personalizar a visualização](#customize-the-view) neste artigo.


1. (Opcional) Clique no botão **Filtro** ícone ![](assets/filter-icon.png) no **Trabalho Atribuído** e selecione a **Filtro padrão** no **Sugerido** área da caixa de filtro.

   Ao aplicar o filtro Padrão, os usuários que pertencem a qualquer uma das equipes e seus itens de trabalho são exibidos. Você pode editar uma cópia deste filtro.

   >[!TIP]
   >
   >O filtro Padrão está disponível somente no Balanceador de Carga de Trabalho na área Recursos.

1. Continue com as etapas a seguir para navegar pelo Balanceador de carga de trabalho:

   * [Selecione um período no Balanceador de Carga de Trabalho](#select-a-time-frame-in-the-workload-balancer)
   * [Personalizar a visualização](#customize-the-view)
   * [Atribuir itens de trabalho e ajustar alocações de usuário](#assign-work-items-and-adjust-user-allocations)
   * [Exibir alocações em um gráfico](#view-allocations-in-a-chart)

### Selecione um período no Balanceador de Carga de Trabalho

1. Acesse o Balanceador de Carga de Trabalho na **Recursos** , conforme descrito na seção [Acesse o Balanceador de Carga de Trabalho para vários projetos na área Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) neste artigo.

   O Balanceador de Carga de Trabalho exibe informações de atribuição de trabalho começando com a semana atual.

1. Use a rolagem horizontal para exibir a linha do tempo de itens de trabalho que se estendem além dos limites da tela.
1. Clique no botão **para trás ou para frente** ícones ![](assets/back-and-forward-icons.png) no canto superior esquerdo para navegar pela linha do tempo, em seguida, clique em **Hoje** para retornar à semana atual.
1. Clique no botão **menu suspenso de período** na barra de ferramentas, clique na data de início do período que deseja exibir. Por padrão, a primeira semana selecionada no calendário é a semana na qual você navegou.

   ![](assets/calendar-date-picker-wb.png)

1. Selecione o número de semanas que deseja exibir de uma vez no Balanceador de Carga de Trabalho das seguintes opções:
   * 1 semana
   * 2 semanas
   * 4 semanas. Esta é a configuração padrão.
   * 6 semanas
   * 3 meses

   ![](assets/3-months-12-weeks-drop-down-wb.png)

1. Clique em uma das seguintes opções na barra de ferramentas para exibir as informações por diferentes intervalos de tempo:
   * **Dia**: Exibe informações por dia durante quatro semanas, começando pela data de hoje, por padrão.
   * **Semana**: Exibe informações por semana durante quatro semanas.
   * **Mês**: Exibe informações por mês durante três meses.

1. Continue navegando no Balanceador de Carga de Trabalho conforme descrito nas seções a seguir.

### Personalizar a visualização

1. Acesse o Balanceador de Carga de Trabalho na **Recursos** , conforme descrito na seção [Acesse o Balanceador de Carga de Trabalho para vários projetos na área Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) neste artigo.

   Os nomes dos itens de trabalho são listados no lado esquerdo e são representados por barras no lado direito do Balanceador de Carga de Trabalho. O comprimento da barra representa a linha do tempo de um item de trabalho.

1. (Opcional e recomendado) Use filtros nas áreas de Trabalho não atribuído e atribuído para exibir somente itens de trabalho ou usuários relevantes para você.

   Para obter mais informações, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../workload-balancer/filter-information-workload-balancer.md).

   Por padrão, as barras azuis representam as linhas do tempo de projetos e tarefas, e as barras de maron representam problemas.

   Você pode alterar a cor das barras para projetos e tarefas ao selecionar seu tema de cores para corresponder ao projeto. Para obter mais informações, continue lendo este procedimento.

   Os itens de trabalho na área de Trabalho Atribuído são classificados por projetos de acordo com os seguintes critérios, nesta ordem:
   1. Data de início planejada (mais antiga primeiro)
   1. Data de conclusão planejada (mais antiga primeiro)
   1. Alfabético por projeto (somente quando os dois primeiros critérios são idênticos para vários itens de trabalho)

1. Clique no botão **seta apontando para a direita** à esquerda das áreas Não atribuído ou Atribuído para expandir todos os itens sob os nomes do projeto (na área Não atribuído) e sob os nomes de usuário (na área Atribuído).

   >[!TIP]
   >
   >Os itens de trabalho são listados em nomes de projeto na área Não atribuído somente quando você ativa a configuração &quot;Agrupar por projeto&quot;.


1. Clique no botão **seta para baixo** à esquerda das áreas Não atribuídas ou Atribuídas para recolher todos os itens sob os nomes do projeto (na área Não Atribuído) e sob os nomes de usuário (na área Atribuído).

1. Arraste e solte a **linha divisória** entre o painel esquerdo e a área da linha do tempo para ajustar o tamanho do painel esquerdo.

   ![](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. Clique no botão **Configurações** ícone ![](assets/settings-gear-icon.png).

   O painel Configurações é exibido à direita.

   ![](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Selecione uma das opções listadas abaixo para atualizar as informações exibidas no Balanceador de Carga de Trabalho e clique no botão **Ícone X** no canto superior direito da caixa Configurações para fechá-la.

   * **Agrupar por projeto**: Quando essa opção é selecionada, os itens nas áreas de Trabalho não atribuído e Atribuído são agrupados por projeto. Isso é selecionado por padrão.

   * **Incluir horas de problemas**: Quando essa opção é selecionada, os problemas atribuídos aos usuários são exibidos sob o nome do usuário na área de Trabalho atribuído e os problemas que não são atribuídos aos usuários são exibidos na área de Trabalho não atribuído. As Horas Planejadas dos problemas contam para as Horas Planejadas do projeto e para o usuário na área de Trabalho Atribuído.
   * **Mostrar datas previstas**: Quando essa opção é selecionada, a linha do tempo projetada dos itens de trabalho é exibida além da linha do tempo planejada. Observe o seguinte:
      * A linha do tempo projetada para projetos, tarefas e problemas é exibida como uma linha azul escura acima das barras de tarefa, problema e projeto.
      * A linha do tempo projetada fora da linha do tempo planejada é exibida em azul claro, mesmo quando você atualiza o tema da cor, conforme descrito abaixo.
      * A linha do tempo projetada para os itens que você não tem acesso para exibir é exibida em cinza-claro com uma linha embaixo.
      * Quando uma tarefa ou um problema é concluído antes da Data de Conclusão Planejada devida, os números de alocação dos dias restantes são atingidos e não contam na alocação do usuário. Isso é exibido somente quando a configuração Mostrar datas projetadas e o ícone Mostrar alocação estão ativados.

      >[!TIP]
      >
      >Observe que os itens de trabalho são exibidos no Balanceador de Carga de Trabalho quando as linhas do tempo planejadas ou projetadas (não necessariamente ambas ao mesmo tempo) ocorrem durante o período selecionado.

   * **Mostrar trabalho concluído**: Quando isso está ativado, as tarefas concluídas e os problemas são exibidos na área de Trabalho atribuído. Isso é ativado por padrão.

      Um ícone de marca de seleção verde é exibido no canto superior direito de uma barra de tarefas ou de ocorrências quando elas são concluídas. O mesmo ícone é exibido para um projeto quando as tarefas ou os problemas para o período selecionado do projeto são concluídos.
   * **Mostrar tempo restante**: Quando ativado, o Workfront exibe a diferença entre o tempo diário para o qual o usuário está disponível para trabalhar com base em suas programações e as horas para as quais ele está alocado na área de Trabalho atribuído para os usuários. Isso é desativado por padrão e o tempo alocado é exibido por padrão.
   * No **Selecionar tema de cor** selecione a cor desejada para as barras de projeto e tarefa.

      >[!TIP]
      >
      >A configuração para selecionar o tema de cor não afeta a cor das barras de problema. Os problemas sempre são exibidos em uma barra de cores do maron.

      Selecione uma das opções a seguir:
      * **Padrão**: As barras para todos os projetos e seus itens de trabalho são exibidas em azul.
      * **Projeto**: As barras associadas a cada projeto e suas tarefas são alteradas de acordo com o nome do projeto. Todas as tarefas que pertencem ao projeto são exibidas em barras que correspondem à cor do projeto. As barras do projeto são exibidas em um tom mais claro para diferenciá-las das tarefas. As barras de projeto também incluem um ícone de projeto ao escolher não exibir alocações.
      * **Status do projeto**: As barras associadas a cada projeto e seus itens de trabalho mudam para a cor do status do projeto.

         O status do projeto é o associado ao Grupo do projeto. Se o Grupo não tiver status específicos do grupo, a cor das barras do item de trabalho será a do status do projeto no nível do sistema. Tanto o sistema quanto os status personalizados são exibidos. Para obter informações sobre status de grupo, consulte [Criar ou editar um status de grupo](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
   * No **Exibir alocação de usuário em** selecione uma das seguintes opções:
      * **Horas**: Exibe o tempo alocado como horas. Este é o padrão.
      * **Porcentagem**: Exibe o tempo alocado como uma porcentagem do tempo total disponível
   * No **Preferências de classificação** selecione como deseja que os itens sejam classificados no Balanceador de Carga de Trabalho. Selecione dentre as seguintes opções:
      * **Classificar usuários por Função Principal**: Os usuários são exibidos na ordem alfabética de suas Funções primárias na área de Trabalho atribuído.
      * **Classificar usuários alfabeticamente**: Os usuários são exibidos na ordem alfabética de seus nomes na área de Trabalho atribuído.
      * **Classificar projetos por**: Selecione um campo de projeto no menu suspenso para classificar projetos alfabeticamente por esse campo nas áreas de Trabalho Atribuído ou Não Atribuído.

   >[!TIP]
   >
   >Você pode classificar por projetos somente quando a configuração Agrupar por projeto estiver ativada. Caso contrário, essa configuração ficará esmaecida.

1. (Opcional e condicional) Ao alterar o tema de cor para Status do projeto, passe o mouse sobre o nome de um projeto à esquerda para visualizar o status do projeto.

   ![](assets/hover-over-project-status-tooltip-350x115.png)

### Atribuir itens de trabalho e ajustar alocações de usuário

1. Acesse o Balanceador de Carga de Trabalho na área Recursos, conforme descrito na seção [Acesse o Balanceador de Carga de Trabalho para vários projetos na área Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) neste artigo.
1. Clique no botão **Ícone Mostrar alocações** ![](assets/show-allocations-icon-small.png) para visualizar as Horas Planejadas diárias ou semanais para itens de trabalho.

   Isso substitui o nome nas barras dos itens de trabalho pela quantidade de Horas Planejadas diárias ou semanais nas áreas de Trabalho Não Atribuído e Atribuído. Esta configuração é desativada por padrão.

   Os dias que mostram sobrealocações são exibidos em vermelho.

   >[!TIP]
   >
   >* A opção Mostrar alocações afeta apenas o que é exibido para projetos, tarefas, problemas e itens inacessíveis. As Horas Planejadas Diárias para usuários são exibidas por padrão e não podem ser ocultas.
   >* Você deve ativar a configuração Agrupar por projeto para exibir as Horas Planejadas diárias dos projetos.
   >* Quando você exibe o Balanceador de Carga de Trabalho por semana, as horas exibidas são as Horas Planejadas semanais.



1. (Opcional) Passe o mouse sobre o tempo alocado na linha de usuário para entender a capacidade e a alocação do usuário. A capacidade é a disponibilidade do usuário de acordo com seu cronograma.

   ![](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Opcional) Clique no botão **Ícone Ocultar alocações** ![](assets/show-allocations-icon-small.png) para exibir o nome das tarefas e problemas nas barras dos itens de trabalho.
1. Clique no botão **Menu Mais** ícone ![](assets/more-icon.png) à direita de uma tarefa ou nome de ocorrência, clique em uma das opções abaixo.

   ![](assets/more-menu-right-of-task-350x104.png)

   * **Atribua isso a** em seguida, comece a digitar o nome de um usuário, função ou equipe ao qual deseja atribuir o item de trabalho na **Pesquisar pessoas, funções ou equipes** campo.

      Você também pode usar os seguintes atalhos para atribuir tarefas ou problemas:

      * No Windows: Clique com a tecla CTRL pressionada na barra de tarefas ou problemas.
      * No Mac: Clique com a tecla CMD na barra de tarefas ou problemas.

      Para obter mais informações sobre como atribuir itens de trabalho a usuários no Balanceador de Carga de Trabalho, consulte [Visão Geral da atribuição de trabalho no Balanceador de Carga de Trabalho](../workload-balancer/assign-work-in-workload-balancer.md).

      >[!TIP]
      >
      >Se o administrador do Workfront ou do grupo ativou delegações em seu ambiente, use a guia Atribuições para atribuir usuários à tarefa ou problema. Para obter informações sobre delegação de trabalho, consulte [Gerenciar delegação de tarefa e emissão](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Editar alocações**, em seguida, edite as alocações diárias ou semanais para o usuário. Para obter informações sobre como gerenciar alocações de usuários, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../workload-balancer/manage-user-allocations-workload-balancer.md).

   * **Abrir resumo**. O painel Resumo é aberto à direita, em seguida, clique no campo Atribuições e comece a digitar o nome de um usuário, função ou equipe no **Pesquisar pessoas, funções ou equipes** para atribuir o item. Para obter mais informações, consulte a seção [Exibir mais informações sobre tarefas e problemas](#display-more-information-about-tasks-and-issues) neste artigo.


1. (Opcional) Clique duas vezes em uma alocação diária ou semanal para um usuário dentro da barra de um item de trabalho para editar o número de horas alocadas e clique no botão **Salvar** ícone ![](assets/save-allocations-wb.png) para salvar as alocações ou o **Cancelar** ícone  ![](assets/cancel-allocations-wb.png) para remover as alocações que você ajustou.

   >[!TIP]
   >
   >Os ícones Salvar e Cancelar são exibidos no final de uma tarefa ou na barra da linha do tempo de um problema.
   >
   >![](assets/cancel-and-save-icon-on-adjust-allocation-bar-wb-highlighted.png)

   Para obter informações sobre como gerenciar alocações de usuários, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../workload-balancer/manage-user-allocations-workload-balancer.md).

1. Clique em **Atribuições em massa** para atribuir itens de trabalho em massa.

   Para obter mais informações, consulte [Atribua trabalho em massa usando o Balanceador de Carga de Trabalho](../workload-balancer/assign-work-in-workload-balancer-in-bulk.md).
1. Arraste itens do **Trabalho Não Atribuído** ou de um usuário e solte-os em outro usuário para atribuí-los.

   Para obter mais informações, consulte [Atribua trabalho ao Balanceador de Carga de Trabalho arrastando e soltando](../workload-balancer/assign-work-in-workload-balancer-by-drag-and-drop.md).


### Exibir alocações em um gráfico

Em vez de exibir alocações em números diários ou semanais, você pode exibi-las em um gráfico.

1. Acesse o Balanceador de Carga de Trabalho na área Recursos, conforme descrito na seção [Acesse o Balanceador de Carga de Trabalho para vários projetos na área Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) neste artigo.
1. Clique no botão **Ícone do gráfico** ![](assets/user-allocation-chart-icon.png) para exibir a alocação de usuários em um formato de gráfico.

   Os dias em que o usuário tem alocação excessiva são exibidos como blocos vermelhos e os dias em que o usuário está sub-alocado ou na capacidade são exibidos como blocos azuis.

   O tamanho dos blocos indica a quantidade da alocação: quanto maior a caixa, mais tempo o usuário é alocado para itens de trabalho para esse dia ou semana.

   ![](assets/user-allocation-chart-350x237.png)



### Exibir mais informações sobre tarefas e problemas

Você pode exibir mais informações sobre as tarefas e os problemas no Balanceador de Carga de Trabalho.


1. Acesse o Balanceador de Carga de Trabalho na área Recursos, conforme descrito na seção [Acesse o Balanceador de Carga de Trabalho para vários projetos na área Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) neste artigo.
1. Para exibir mais informações no painel Resumo, siga um destes procedimentos:

   * Clique na barra de uma tarefa ou problema para abrir o painel Resumo à direita.
   * Clique no botão **Abrir resumo** ícone ![](assets/summary-panel-icon.png), em seguida, clique na barra de uma tarefa ou problema para abrir o painel Resumo.
   * Clique no botão **Mais** à direita de uma tarefa ou problema e clique em **Abrir resumo**.

   Para obter informações sobre como atualizar informações de tarefa no Resumo no Balanceador de Carga de Trabalho, consulte [Atualizar itens de trabalho no Balanceador de Carga de Trabalho usando o Resumo](../workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

1. Passe o mouse sobre o nome de uma tarefa ou problema para exibir mais informações sobre ela. Uma caixa é exibida acima da tarefa ou do problema com as seguintes informações:

   * O nome da tarefa ou problema.
   * O nome do projeto.
   * As datas de início e conclusão previstas.
   * O número de Horas Planejadas.
   * Para tarefas, o número do antecessor.
   * Para tarefas, um indicador no canto superior da caixa que indica se a tarefa está pronta para ser trabalhada ou não.

   ![](assets/task-bar-hover-over-detail-wb.png)

1. Clique no nome de um item de trabalho à esquerda para acessá-lo. O item de trabalho é aberto em uma nova guia do navegador.


### Exibir o Balanceador de Carga de Trabalho em tela cheia

1. Acesse o Balanceador de Carga de Trabalho na área Recursos, conforme descrito na seção [Acesse o Balanceador de Carga de Trabalho para vários projetos na área Recursos](#access-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) neste artigo.

1. Clique no botão **Tela cheia** ícone ![](assets/full-screen.png) para exibir o Balanceador de Carga de Trabalho em tela cheia.

   O Balanceador de carga de trabalho ocupa a tela inteira. As janelas e guias do navegador são excluídas da visualização.

1. Clique no botão **Sair de tela cheia** ícone ![](assets/exit-full-screen.png) para retornar à tela padrão e exibir o Balanceador de carga de trabalho dentro da guia do navegador.


## Navegar pelo Balanceador de Carga de Trabalho de uma equipe

Navegar pelo Balanceador de Carga de Trabalho de uma equipe é semelhante à forma como você navega pelo Balanceador de Carga de Trabalho para vários projetos. Para obter mais informações, consulte a seção [Navegar pelo Balanceador de Carga de Trabalho para vários projetos](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) neste artigo.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Equipes**.
A página da Equipe inicial é exibida por padrão.
1. Clique em **Balanceador de Carga de Trabalho** no painel esquerdo. O Balanceador de Carga de Trabalho de uma equipe deve ser exibido por padrão.

   ![](assets/nwe-balancer-team-350x172.png)

   O Balanceador de Carga de Trabalho de uma equipe exibe as seguintes informações, por padrão:

   * No **Trabalho Não Atribuído** Área: Itens de trabalho atribuídos à equipe ou à equipe e funções de trabalho e que não são atribuídos a usuários.
   * No **Trabalho Atribuído** Área: Os itens de trabalho atribuídos aos usuários são exibidos sob os nomes dos usuários.

1. Continue navegando no Balanceador de carga de trabalho de uma equipe, conforme descrito na seção [Navegue pelo Balanceador de Carga de Trabalho para vários projetos na área Recursos](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) seção deste artigo.

## Navegar pelo Balanceador de Carga de Trabalho de um único projeto

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Projetos**.
1. Clique no nome de um projeto para abrir a página do projeto.
1. Clique em **Balanceador de Carga de Trabalho** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Balanceador de Carga de Trabalho**.

   ![](assets/nwe-balancer-project-350x152.png)

   O Balanceador de Carga de Trabalho do projeto exibe as seguintes informações, por padrão:

   * No **Trabalho Não Atribuído** Área: Itens de trabalho no projeto que são atribuídos a funções ou equipes e não são atribuídos a usuários.
   * No **Trabalho Atribuído** Área: Itens de trabalho no projeto que são atribuídos a pelo menos um usuário.

   Recomendamos usar filtros para mostrar somente os usuários que são importantes para você.

   Por exemplo, você pode considerar a exibição de somente usuários que pertencem a suas equipes ou grupos. Para obter mais informações, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../workload-balancer/filter-information-workload-balancer.md).

1. (Opcional) Clique no botão **Filtro** ícone ![](assets/filter-icon.png) na área Trabalho atribuído e selecione o **Itens de trabalho deste projeto** da **Sugerido** área do painel de filtro. Esse filtro é desmarcado por padrão.

   Quando essa opção é selecionada, somente os itens atribuídos aos usuários no projeto selecionado são exibidos.

   Quando a opção não está selecionada, todos os itens atribuídos aos usuários no projeto são exibidos, independentemente de a que projetos os itens pertencem.

1. (Opcional e recomendado) Aplique um filtro na área de Trabalho atribuído para exibir usuários importantes para você, mas que talvez não sejam atribuídos a itens no projeto, em seguida, clique no botão **Mostrar todos os usuários** ícone ![](assets/show-all-users-icon-project-workload-balancer.png).

   Ao mostrar todos os usuários, você pode exibir todos os usuários no Workfront que ainda não foram atribuídos a funções ou outras funções no projeto.

   Você pode aplicar um filtro primeiro, para reduzir o número de usuários exibidos.

   Por exemplo, você pode querer filtrar primeiro os usuários que pertencem a suas equipes ou grupos e, em seguida, exibir todos esses usuários.

   Para obter informações sobre como criar um filtro, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../workload-balancer/filter-information-workload-balancer.md).

   >[!NOTE]
   >
   > A opção Mostrar todos os usuários está disponível somente para o Balanceador de Carga de Trabalho de um projeto.


1. (Opcional) Clique no botão **Mostrar alocações de função** ícone ![](assets/show-role-allocation-icon.png).

   O painel Alocação de função é exibido.

   Você pode exibir informações sobre Horas Planejadas associadas às funções de cargo no projeto e aquelas funções de cargo associadas a iniciativas vinculadas aos projetos do Planejador de Cenário.

   Para obter mais informações, consulte [Visão geral da reconciliação das alocações de recursos entre projetos e iniciativas](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).


   >[!NOTE]
   >
   >Não é possível exibir informações de função de trabalho de iniciativa se a organização não tiver comprado uma licença para o Workfront Scenario Planner. Nesse caso, você só poderá visualizar as horas planejadas associadas às funções de cargo no projeto. Para obter mais informações, consulte [Acesso necessário para usar o Planejador de cenário](../../scenario-planner/access-needed-to-use-sp.md).


1. Continue navegando no Balanceador de carga de trabalho de um projeto, conforme descrito na seção [Navegar pelo Balanceador de Carga de Trabalho para vários projetos](#navigate-the-workload-balancer-for-multiple-projects-in-the-resourcing-area) seção deste artigo.

<!--old content below - this used to be a one-large-procedure article - outdated, and rewrote it above with several smaller procedures: 

# Navigate the Workload Balancer

<!-drafted note for 22.4 release: remove all production/ preview references at Prod release>

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

Use the Workload Balancer to understand the availability of your resources as well as to assign work to your users. This article walks you through using the icons and settings available to update the view for and navigate the Workload Balancer.

>[!NOTE]
>
>The Workload Balancer is a resource scheduling tool that will eventually replace the current resource scheduling tools which are currently deprecated. 
>
>For more information about removing the resource scheduling tools and replacing them with the Workload Balancer, see [Deprecation of Resource Scheduling tools in Adobe Workfront](../../resource-mgmt/resource-mgmt-overview/deprecate-resource-scheduling.md).
>
>We recommend that you use the Workload Balancer for scheduling your resources.

The Workload Balancer is available in multiple areas of Adobe Workfront. Navigating it is similar in all areas. This article describes how to navigate the Workload Balancer for multiple projects in the Resourcing area. For more information about where the Workload Balancer is located, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

For information about managing resources using the Workload Balancer, also consider reading the following articles:

* [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
* [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)

## Access requirements

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan, when using the Workload Balancer in all areas in the Production environment</p>
   <p><span class="preview">Work, when using the Workload Balancer of a project, in the Preview environment</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to the following:</p> 
    <ul> 
     <li> <p>Resource Management</p> </li> 
     <li> <p>Projects</p> </li> 
     <li> <p>Tasks</p> </li> 
     <li> <p>Issues</p> </li> 
    </ul> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the projects, tasks, and issues </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Considerations for viewing items in the Workload Balancer

Consider the following when viewing the Workload Balancer:

* Projects display in the Workload Balancer only when the Group by Project setting is enabled. This setting is enabled by default.
* Mousing over a task or an issue displays the following additional information about the task or issue:

  * Project name

  * Task or issue name

  * Parent task

  * Planned Start and Completion Dates

  * Number of Planned Hours

  * Ready to start or Not ready status

  ![task-pop-up-with-additional-info-in-workload-balancer](assets/task-pop-up-with-additional-info-in-global-wb.png)

* When a project has no tasks during a period of time, the bar at the project level becomes a dimmed color.

  ![](assets/wb-break-in-project-timeline-with-no-tasks-highlight-350x80.png)

* When you don't have permissions to see certain items, they display as **Inaccessible work items** or **Inaccessible projects**.

  ![](assets/balancer-inaccessible-items-and-projects-highlighted-350x108.png)

* The names of the work items display on the left and within the timeline selected on the right. 
* The total of Planned Hours for each work item displays to the right of the name of the work items on the left. 
* The total of the Planned Hours for each project displays to the right of the name of the project on the left.

  The Planned Hours information for the project is a total of Planned Hours from all items listed in the Workload Balancer, and not a total of Planned Hours on the project.

## Overview of the Unassigned Work and Assigned Work areas

The Workload Balancer displays work items in two separate areas, depending on their assignments.

The two areas of the Workload Balancer display the following information:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Unassigned Work</td> 
   <td> <p>This area displays tasks <span class="preview">and issues</span> unassigned to users. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>This area does not display any work items by default. We recommend using filters to display relevant information for you in this area.</p> <p>After you apply a filter, this area displays the following work items:</p> 
    <ul> 
     <li>unassigned</li> 
     <li>assigned to a team </li> 
     <li>assigned to a job role</li> 
     <li> <p>assigned to a team and a role at the same time</p> </li> 
    </ul> <p>Tip: Items assigned to a user as the primary assignee do not display in the Unassigned Work area. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Assigned Work</td> 
   <td> <p> All active users in the system display in this area by default. We recommend using filters to limit the amount of information in this area.  </p> <p>Both tasks and issues display in the Assigned Work area. </p> <p>Projects display when the Group by Project setting is enabled.</p> <p>The work items that the users are assigned to display under their names. </p> <p>If a work item is assigned to multiple users, the item displays under each assigned user. </p> </td> 
  </tr> 
 </tbody> 
</table>

For information about applying a filter in the Workload Balancer, see [Filter information in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

![](assets/balancer-empty-unassiged-area-350x179.png)

## Navigate the Workload Balancer

You can update the view in the Workload Balancer to display exactly the information you need to focus on in the time frame that makes the most sense to you.

After selecting the settings you want to apply to your view, the Workload Balancer remembers these settings every time you access it from any browser or device.

1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Workfront, then click **Resourcing**.
1. Click **Workload Balancer** in the left panel.

   The Workload Balancer displays work assignment information starting with the current week. The names of work items are listed on the left side as well as represented by bars on the right side of the of the Workload Balancer within their respective timelines. By default, blue bars represent the timelines of projects and tasks and maroon bars represent issues.

   >[!TIP]
   >
   >You can change the color of the bars for projects and tasks when you select your color scheme to match the project. For more information, continue reading this procedure.

   The work items that display under the name of users in the Workload Balancer are sorted by the following criteria, in this order:

   1. Planned Start Date (oldest first)
   1. Planned Completion Date (oldest first)
   1. Alphabetical by project (only when the first two criteria are identical for multiple work items)

1. Click the right-pointing arrow to the left of the Unassigned or Assigned areas to expand all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Click the down-pointing arrow to the left of the Unassigned or Assigned areas to collapse all items under the project names (in the Unassigned area) and under the user names (in the Assigned area).
1. Use the horizontal scroll to navigate the timelines of work items that extends beyond the limits of the screen. 
1. Use the vertical scroll to display additional users and work items. 
1. Drag and drop the separation line between the left panel and the timeline areas to adjust the size of the left panel.

   ![](assets/separation-line-between-left-panel-and-timeline-highlighted-nwe-350x174.png)

1. Click the **Filter icon** ![](assets/filter-icon.png) in the upper-right corner of the **Unassigned Work** or the **Assigned Work** areas to select the type of information to display in the Workload Balancer.

   For information about filtering information in the Workload Balancer, see [Manage filters in the Workload Balancer](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md). 

1. Click the right-pointing arrow next to **Unassigned Work** to expand this area or the down-pointing arrow to collapse it.

   >[!TIP]
   >
   >No items display in this area by default. You must apply a filter to view unassigned work items.

1. Drag and drop the separation line between the **Unassigned Work** and **Assigned Work** areas to adjust their size.

   ![](assets/modern-scheduler-separation-line-between-areas-350x278.png)

1. Click the back or forward icons ![](assets/back-and-forward-icons.png) to navigate the timeline, then click **Today** to return to the current week. 

1. Click the **time frame drop-down menu** on the toolbar, then click the beginning date of the period you want to display. By default, the first week selected on the calendar is the week you navigated to.

   ![](assets/calendar-date-picker-wb.png)


1. Click one of the following options in the toolbar to display information by different time frames:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Day</td> 
      <td>Displays information by day for four weeks starting with today's date, by default. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Week</td> 
      <td>Displays information by week for four weeks. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Month</td> 
      <td> <p><span>Displays information by month for three months.</span> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Select the number of weeks you want to display at one time in the Workload Balancer from the following options:

   * 1 week
   * 2 weeks
   * 4 weeks. This is the default setting.
   * 6 weeks
   * 3 months
   ![](assets/3-months-12-weeks-drop-down-wb.png)     

1. Click the **Settings** icon ![](assets/settings-gear-icon.png).

   The Settings panel displays.

   ![](assets/settings-box-options-global-with-color-theme-and-percentage-wb-nwe.png)

   Select from the options listed below to update the information you view in the Workload Balancer, then click the **X icon** in the upper-right of the Settings box to close it.

   * **Group by Project**: When this is selected, the items in the Unassigned and Assigned Work areas are grouped by project. This is selected by default.

     ![](assets/group-by-project-350x530.png)

   * **Include hours from issues**: When this is selected, issues assigned to users display under the user's name in the Assigned Work area <span class="preview">and issues that are not assigned to users display in the Unassigned Work area</span>. The Planned Hours from the issues count towards the Planned Hours for the project and for the user in the Assigned Work area. 

        ![](assets/issue-on-workload-balancer-350x20.png)

   
      * **Show Projected Dates**: When this is selected, the projected timeline of work items displays in addition to the planned timeline. Notice the following:

         * The projected timeline of project, tasks, and issues displays as a dark blue line above the task, issue, and project bars.
         * The projected timeline that is outside of the planned timeline displays in light blue, even when you update the color theme, as described below.
         * The projected timeline for the items that you have no access to view displays in light gray with a line underneath.
         * When a task or issue completes before the due Planned Completion Date the allocation numbers for the remaining days are struck through and do not count towards the user's allocation. This displays only when both the Show Projected Dates setting and the Show allocation icon are enabled.

         ![](assets/task-issue-projected-timelines-350x91.png)

         >[!TIP]
         >
         >Notice that work items display in the Workload Balancer when either their planned or the projected timelines (not necessarily both at the same time) occur during the timeframe selected.

   * **Show completed work**: When this is enabled, tasks and issues that are completed display in the Assigned Work area. This is enabled by default.

     A green checkmark icon ![](assets/green-checkmark-icon.png) displays to the upper-right corner of a task or issue bar when they are completed. The same icon displays for a project when the tasks or issues for the selected time frame of the project are completed. 
   
   * **Show remaining time**: When this is enabled, Workfront displays the difference between the daily time for which the user is available to work based on their schedules and the hours for which they are allocated in the Assigned Work area for the users. This is disabled by default and allocated time displays by default.

   * In the **Select color theme** section, select the color that you want for the project and task bars.  

      >[!NOTE]
      >
      >The setting for selecting the color theme  does not affect the color of the issue bars. Issues always display in a maroon-color bar. 


      Select from the following:

      * **Default**: The bars for all projects and their work items display in blue.  
      * **Project**: The bars associated with each project and its tasks change according to the name of the project. All tasks that belong to the project display in bars that match the color of the project. The project bars display in a lighter shade to distinguish them from the tasks. The project bars also include a project icon when choosing not to display allocations.
      * **Project Status**: The bars associated with each project and its work items change to the color of the status of the project.

        >[!TIP]
        >
        >* The project status is that associated with the Group of the project. If the Group does not have group-specific statuses, the color of the work item bars is that of the system-level project status. Both system as well as custom statuses display. For information about group statuses, see [Create or edit a group status](../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
        
   * In the **Display user allocation in** section, select from the following:

      * **Hours**: Displays allocated time as hours. This is the default. 
      * **Percentage**: Displays allocated time as a percentage of the total available time

   * In the **Sorting preferences** section, select how you want the items to be sorted in the Workload Balancer. Select from the following options: 

      * **Sort users by Primary Role**: Users display in the alphabetical order of their Primary Roles in the Assigned Work area.

      * **Sort users alphabetically**: Users display in the alphabetical order of their first names in the Assigned Work area.

      * **Sort projects by**: Select a project field from the drop-down menu to sort projects alphabetically by that field in the Unassigned or Assigned Work areas. 

      >[!TIP]
      >
      >You can sort by projects only when the Group by Project setting is enabled. Otherwise, this setting is dimmed.


1. (Optional and conditional) If you changed the color theme to Project Status, hover over the name of a project on the left to view the status of the project.

   ![](assets/hover-over-project-status-tooltip-350x115.png)

1. <span class="preview">(Conditional and recommended) In the Workload Balancer of a project, apply a filter in the Assigned Work area to display users that are important to you but might not be assigned to items on the project, then click the **Show all users** icon ![](assets/show-all-users-icon-project-workload-balancer.png). This displays other users in the system that are not yet assigned on the project. For information about how to build a filter, see [Manage filters in the Workload Balancer](../workload-balancer/filter-information-workload-balancer.md).</span>

 
   >[!TIP]
   >
   ><span class="preview">The Show all users icon is available only for the Workload Balancer of a project.</span> 

1. Click the **Chart icon** ![](assets/user-allocation-chart-icon.png) to display the user allocation in a chart format. Days where the user is overallocated display as red blocks, and days where the user is underallocated or at capacity display as blue blocks. The size of the blocks indicates the amount of the allocation: the larger the box, the more time the user is allocated to work items for that day or week.

   ![](assets/user-allocation-chart-350x237.png)

1. Click the **Show allocations icon** ![](assets/show-allocations-icon-small.png) to view the daily or weekly Planned Hours for work items.

   This replaces the name in the bars of the work items with the amount of daily or weekly Planned Hours in the Unassigned and Assigned Work areas. This setting is disabled by default.

   >[!TIP]
   >
   >* The Show allocations setting only affects what displays for projects, tasks, issues and inaccessible items. Daily Planned Hours for users display by default and cannot be hidden.
   >* You must enable the Group by Project setting to display daily Planned Hours for projects. 
   >* When you view the Workload Balancer by week, the hours displayed are the weekly Planned Hours. 

   Days that show overallocations display in red. 

1. (Optional) Hover over the allocated time in the user line to understand what the capacity and allocation of the user. The capacity is the availability of the user according to their schedule.

   ![](assets/overallocation-vs-capacity-tooltip-wb-nwe.png)

1. (Optional) Click the **Hide allocations icon** ![](assets/show-allocations-icon-small.png) to display the name of the tasks in the bars of the work items. 
1. Click the **More menu** icon ![](assets/more-icon.png) to the right of a task or issue name, then click one of options below. 

   ![](assets/more-menu-right-of-task-350x104.png)

      * **Assign this to**, then start typing the name of a user, role, or team you want to assign the work item to in the **Search people, role, or teams** field.
    
      >[!TIP]
      >
      >You can also use the following shortcuts to assign tasks or issues:
      >
      >* In Windows: CTRL+click the task or issue bar.
      >* In Mac: CMD+click the task or issue bar.

      For more information about assigning work items to users in the Workload Balancer, see [Overview of assigning work in the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md). 

      >[!TIP]
      >
      >If your Workfront or group administrator enabled delegations in your environment, use the Assignments tab to assign users to the task or issue. For information about delegating work, see [Manage task and issue delegation](../../manage-work/delegate-work/how-to-delegate-work.md).

   * **Edit allocations**, then edit the daily or weekly allocations for the user. For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

1. Click the bar of a task or issue to open the Summary panel on the right

   Or

   Click **Open Summary** icon ![](assets/summary-panel-icon.png), then click the bar of a task or issue to open the Summary panel

   Or

   Click the **More** menu ![](assets/more-icon.png) to the right of a task or issue, then click **Open Summary**.

   For information about updating task information in the Summary in the Workload Balancer, see [Update work items in the Workload Balancer using the Summary](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

    The Summary panel opens on the right. 

1. Click **Bulk Assignments** to assign work items in bulk.

   For more information, see [Assign work in bulk using the Workload Balancer](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md). 

1. Click the **Full screen** icon ![](assets/full-screen.png) to display the Workload Balancer in full screen, then click the **Exit full screen** icon ![](assets/exit-full-screen.png) to return to the default screen. 
1. (Optional) Double-click a daily or weekly allocation for a user inside the bar of a work item to edit the number of allocated hours, then click the **Save** icon ![](assets/save-allocations-wb.png) to save the allocations or the **Cancel** icon ![](assets/cancel-allocations-wb.png) to remove the allocations you adjusted.

   >[!TIP]
   >
   >The Save and Cancel icons display towards the end of a task or an issue's timeline bar.

   For information about managing user allocations, see [Manage user allocations in the Workload Balancer](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md). 

1. Click the name of a work item on the left to access it. 
1. Click the **Shareable link icon** ![](assets/wb-shearable-link-icon-small.png) to copy the direct URL for the Workload Balancer to your clipboard. 
1. (Optional) Share the link with any user who does not have direct access to the Workload Balancer.

   For information about sharing the Workload Balancer with a link, see [Share the Workload Balancer with a link](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md). 

1. (Conditional) From the Workload Balancer of a project, click the **Show role allocations** icon ![](assets/show-role-allocation-icon.png).

   The Role Allocation panel displays. You can view information about Planned Hours associated with job roles on the project and job roles associated with initiatives from the Scenario Planner. For more information, see [Overview of reconciling resource allocations between projects and initiatives](../../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

   >[!TIP]
   >
   >You cannot view initiative job role information if your organization has not purchased a license for the Workfront Scenario Planner. In this case, you can only view the planned hours associated with job roles on the project. For more information, see [Access needed to use the Scenario Planner](../../scenario-planner/access-needed-to-use-sp.md).

-->