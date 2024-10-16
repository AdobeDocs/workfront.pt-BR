---
product-area: projects
navigation-topic: use-the-home-area
title: Exibir itens na [!UICONTROL Lista de Trabalho] na área Página Inicial
description: A [!UICONTROL Lista de Trabalho] na área [!UICONTROL Página Inicial] exibe todos os itens de trabalho atribuídos a você. Você pode controlar quais itens são exibidos na sua [!UICONTROL Lista de Trabalho], usando filtros e agrupando e classificando seus itens de trabalho.
author: Nolan
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1840'
ht-degree: 0%

---

# Exibir itens na [!UICONTROL Lista de Trabalho] na área [!UICONTROL Página Inicial]

<!-- Audited: 1/2024 -->


A [!UICONTROL Lista de Trabalho] na área [!UICONTROL Página Inicial] exibe todos os itens de trabalho atribuídos a você. Você pode controlar quais itens são exibidos na sua [!UICONTROL Lista de Trabalho], usando filtros e agrupando e classificando seus itens de trabalho.

>[!NOTE]
>
>* Ao converter um problema em uma tarefa ou um projeto, o problema é removido da área da página inicial do usuário atribuído ao problema.
>
>* Ao converter uma tarefa em um projeto, a tarefa é excluída e removida da área da página inicial do usuário atribuído à tarefa.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença</strong></td> 
   <td> <p>Novo:</p><ul><li>[!UICONTROL Contributor] somente para aprovações</li> <li>[!UICONTROL Padrão] ou superior para todos os outros objetos</li> <p>Ou</p> 
  </ul><p>Atual:</p><ul><li>[!UICONTROL Review] somente para aprovações</li> <li>[!UICONTROL Trabalho] ou superior para todos os outros objetos</li> </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso a Projetos, Tarefas, Problemas e Documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>permissões do Contribute ou superior para as tarefas e problemas que você precisa para trabalhar</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar a [!UICONTROL Lista de Trabalho]

Você pode filtrar itens na [!UICONTROL Lista de Trabalho] para ver apenas tipos específicos de itens. Por exemplo, você pode filtrar a [!UICONTROL Lista de Trabalho] para exibir somente problemas ou solicitações.

>[!NOTE]
>
>As opções de filtro são armazenadas no navegador. Se você usar consistentemente o mesmo navegador no mesmo computador (e não limpar os dados do site), os filtros selecionados não serão alterados. Se você alternar navegadores ou computadores, os filtros serão revertidos para a opção padrão, que é com todos os filtros desmarcados.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Início]**.
1. Clique no menu suspenso **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png). Se você tiver algum filtro selecionado, o número de filtros selecionados será exibido no lugar do ícone.
1. Selecione entre as seguintes opções de filtro para especificar o tipo de itens que deseja exibir:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tudo]</strong></td> 
      <td>Exibe e seleciona todos os itens. Isso inclui tarefas, problemas, aprovações, tarefas pessoais e tarefas e problemas concluídas. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tarefas: Trabalhando]</strong></td> 
      <td> <p>Exibe somente as tarefas nas quais você está trabalhando ativamente. São tarefas atribuídas a você para as quais você clicou no botão [!UICONTROL Trabalhar Nele].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tarefas: Prontas para Iniciar]</strong></td> 
      <td> 
       <div> 
        <p>Exibe somente as tarefas que estão prontas para você iniciar. Ambas as declarações a seguir devem ser verdadeiras:</p> 
        <ul> 
         <li> <p>As tarefas e seus pais não têm predecessores ou restrições de tarefa que as impeçam de ser trabalhadas.</p> </li> 
         <li> <p>Todas as tarefas predecessoras foram concluídas.</p> </li> 
         <li> <p>A [!UICONTROL Data de Início Planejada] das tarefas está no passado ou em até duas semanas no futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tarefas: Não Está Pronto]</strong></td> 
      <td> 
       <div> 
        <p>Exibe somente as tarefas que ainda não estão prontas para serem iniciadas. Qualquer uma das seguintes declarações deve ser verdadeira:</p> 
        <ul> 
         <li> <p>As tarefas e seus pais podem ter predecessores ou restrições de tarefa que impedem seu trabalho.</p> </li> 
         <li> <p>As tarefas têm uma [!UICONTROL Data de Início Planejada] que é mais de duas semanas no futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas: Trabalhando]</strong></td> 
      <td> <p>Exibe somente os problemas nos quais você está trabalhando ativamente. Esses são problemas atribuídos a você para os quais você clicou no botão [!UICONTROL Trabalhar Nele].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas: Solicitado]</strong></td> 
      <td>Exibe apenas os problemas aos quais você está atribuído, mas para os quais você não clicou no botão [!UICONTROL Trabalhar nisto].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Pessoal</strong></td> 
      <td>Exibe somente tarefas pessoais. Estas são tarefas que você cria como uma tarefa [!UICONTROL Para Fazer], conforme descrito na seção <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-personal-task">Criar uma tarefa pessoal</a> no artigo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Criar itens de trabalho da área [!UICONTROL Início]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Aprovações]</strong></td> 
      <td> 
       <div> 
        <p>Exibe somente as aprovações atribuídas ou delegadas a você e as aprovações submetidas. As aprovações incluem aprovações de itens de trabalho (projetos, tarefas e problemas) e aprovações de documentos, provas, solicitações de acesso e folhas de horas. Para obter mais informações sobre aprovações, consulte os seguintes artigos:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Exibir aprovações</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Aprovações de trabalho</a> </p> </li> 
        </ul> 
        <p>Nota: As aprovações que você submeteu e das quais você também é um dos aprovadores são contadas duas vezes.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegado: Delegado por mim]</strong></td> 
      <td> 
       <div> 
        <p>Exibe somente os itens de trabalho que você delegou a outro usuário.</p> 
        <p>Para obter mais informações sobre como delegar tarefas, consulte <a href="/help/quicksilver/manage-work/delegate-work/how-to-delegate-work.md#delegate-tasks-and-issues-to-another-user" class="MCXref xref">Delegar tarefas e problemas</a>.
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Delegado: Delegado a mim]</strong></td> 
      <td> 
       <div> 
        <p>Exibe somente itens de trabalho que foram temporariamente delegados a você por outro usuário.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Concluído]</strong></td> 
      <td> <p>Exibe somente tarefas concluídas, problemas e tarefas pessoais. O trabalho concluído é exibido nas duas semanas anteriores e é agrupado na Lista de trabalho de acordo com a semana em que foi concluído. As aprovações não estão incluídas.</p> <p>O trabalho concluído fica oculto na [!UICONTROL Lista de Trabalho] a menos que você selecione esse filtro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* As opções de filtro são baseadas em objetos (Tarefas, Problemas, Aprovações, tarefas Pessoais).
   >* Tarefas e problemas são filtrados ainda mais pelo seu estado em relação à nossa prontidão para trabalhar neles ([!UICONTROL Trabalhando Em], [!UICONTROL Pronto para Iniciar], [!UICONTROL Não Está Pronto] para tarefas e [!UICONTROL Trabalhando Em] e [!UICONTROL Solicitado] para problemas). Você pode optar por exibir tarefas ou problemas em um estado específico ou clicar em Tarefas ou Problemas para selecionar e exibir todos os estados.
   >* Há um filtro separado para itens concluídos e inclui tarefas e problemas. Isso não inclui aprovações. O filtro [!UICONTROL Concluído] inclui tarefas Pessoais.
   >* Você pode optar por exibir apenas um estado por vez. Por exemplo, você pode exibir somente [!UICONTROL Trabalhando em] tarefas e somente [!UICONTROL Solicitados] problemas. Você também pode selecionar vários estados de uma vez.
   >* Não é possível aplicar filtros a itens atribuídos a uma de suas equipes, e as atribuições de equipe não estão incluídas nos itens atribuídos diretamente a você.


1. (Opcional) Organize ainda mais a [!UICONTROL Lista de Trabalho], conforme descrito na seção [Agrupar e classificar por Data, Projeto e Prioridade](#group-and-sort-by-date-project-and-priority) deste artigo.

## Agrupar e classificar por [!UICONTROL Data], [!UICONTROL Projeto] e [!UICONTROL Prioridade]

Você pode agrupar e classificar a [!UICONTROL Lista de Trabalho] por [!UICONTROL Data de Término Planejada], [!UICONTROL Data de Confirmação], [!UICONTROL Projeto] ou [!UICONTROL Minha Prioridade]. A opção escolhida determina como os itens são agrupados na [!UICONTROL Lista de Trabalho].

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Início]**.
1. Clique no menu suspenso **[!UICONTROL Agrupar por]** ![Agrupar por](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/grouping-28x19.png).

   <!--
   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)
   -->

1. Selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Término Planejado]</strong></td> 
      <td> <p> Os itens são exibidos nos seguintes agrupamentos na [!UICONTROL Lista de Trabalho], dependendo da [!UICONTROL Data de Conclusão Planejada] (o número de itens contidos em cada agrupamento é exibido entre parênteses ao lado do título do cabeçalho):</p> 
       <ul> 
        <li> <p>[!UICONTROL Atrasado]</p> </li> 
        <li> <p>[!UICONTROL Sem Data de Término Planejada]</p> </li> 
        <li> <p>[!UICONTROL Esta Semana]</p> <p>Esse agrupamento é expandido por padrão.</p> </li> 
        <li> <p>[!UICONTROL Próxima Semana]</p> </li> 
        <li> <p>[!UICONTROL Planejado], seguido por várias [!UICONTROL Datas de Término Planejadas] (vários agrupamentos)</p> </li> 
        <li> <p>[!UICONTROL Concluído]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Início Planejado]</strong></td> 
      <td> <p>Os itens são exibidos nos seguintes agrupamentos na [!UICONTROL Lista de Trabalho], dependendo da [!UICONTROL Data de Início Planejada] (o número de itens contidos em cada agrupamento é exibido entre parênteses ao lado do título do cabeçalho):</p> 
       <ul> 
        <li> <p>[!UICONTROL Atrasado]</p> </li> 
        <li> <p>[!UICONTROL Esta Semana] </p> <p>Esse agrupamento é expandido por padrão.</p> </li> 
        <li> <p>[!UICONTROL Próxima Semana]</p> </li> 
        <li> <p>[!UICONTROL Planejado], seguido por várias [!UICONTROL Datas de Início Planejadas] (vários agrupamentos)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data de Confirmação]</strong></td> 
      <td> <p>Os itens são exibidos nos seguintes agrupamentos na [!UICONTROL Lista de Trabalho] (o número de itens contidos em cada agrupamento é exibido entre parênteses ao lado do título do cabeçalho):</p> 
       <ul> 
        <li> <p>[!UICONTROL Sem Data de Confirmação]</p> </li> 
        <li> <p>[!UICONTROL Comprometido para a Próxima Semana]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Projeto]</strong></td> 
      <td>Os itens são agrupados de acordo com o projeto e os projetos são exibidos em ordem alfabética na [!UICONTROL Lista de Trabalho]. (O número de itens contidos em cada agrupamento é exibido entre parênteses ao lado do título do cabeçalho.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Minha Prioridade]</strong></td> 
      <td>Os itens são exibidos em uma ordem escolhida. Para obter mais informações, consulte <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Priorizar trabalho na área [!UICONTROL Home]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>A classificação padrão é crescente. Se você alterar a classificação para decrescente, as opções de classificação selecionadas serão armazenadas no navegador. Se você usar consistentemente o mesmo navegador no mesmo computador (e não limpar os dados do site), a classificação não será alterada, mas se você alternar navegadores ou computadores, a classificação será alterada para a classificação padrão.

## Exibir itens atrasados

[!DNL Adobe Workfront] usa as seguintes datas para determinar se as solicitações de trabalho estão atrasadas:

* **Tarefas**: [!UICONTROL Data de Término Planejada]
* **Problemas**: [!UICONTROL Data de Término Planejada]
* **Documentos**: [!UICONTROL Data de envio]
* **Folhas de horas**: [!UICONTROL Data de envio]
* **Aprovações**: [!UICONTROL Data de envio]
* **Aprovações de provas**: [!UICONTROL Prazo da prova]

## Pesquisar a [!UICONTROL Lista de Trabalho]

Quando você pesquisa a [!UICONTROL Lista de Trabalho], todos os itens atribuídos a você são retornados na pesquisa (até mesmo itens que não estão carregados na tela). Se a opção [!UICONTROL Mostrar concluídos] estiver selecionada, todos os itens marcados como concluídos nas últimas duas semanas também serão retornados.

Além disso, somente os nomes dos itens de trabalho são pesquisados (as informações contidas no item de trabalho não são pesquisadas, nem os nomes dos projetos em que o item de trabalho reside).

Para pesquisar a [!UICONTROL Lista de Trabalho]:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Início]**.
1. (Opcional) Filtre e agrupe a [!UICONTROL Lista de Trabalho], conforme descrito em [Filtrar a [!UICONTROL Lista de Trabalho]](#filter-the-work-list) e [Agrupar e classificar por Data, Projeto e Prioridade](#group-and-sort-by-date-project-and-priority).

1. (Opcional) Se você estiver procurando um item de trabalho que já está concluído, configure a [!UICONTROL Lista de Trabalho] para exibir os itens concluídos antes de pesquisar.

1. Clique no ícone de Pesquisa ![Pesquisa](/help/quicksilver/workfront-basics/using-home/using-the-home-area/assets/search-icon.png).
1. Comece a digitar o nome do item que você está procurando.\
   A [!UICONTROL Lista de Trabalho] é automaticamente filtrada para incluir itens com um nome correspondente.

## Alterar o tamanho da Lista de trabalho

Você pode alterar o tamanho da [!UICONTROL Lista de Trabalho] para que ela seja consumida em qualquer lugar entre aproximadamente um quarto da área da Página Inicial para aproximadamente metade da área [!UICONTROL Página Inicial].

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Início]**.
1. Passe o mouse sobre a borda direita da [!UICONTROL Lista de Trabalho], em seguida, arraste para a esquerda ou para a direita até que a Lista de Trabalho esteja no tamanho desejado.

## Recolher e expandir agrupamentos

Os itens na [!UICONTROL Lista de Trabalho] são exibidos em agrupamentos. Você pode recolher e expandir agrupamentos para controlar quanta informação é exibida na página em um determinado momento.

Você pode recolher e expandir agrupamentos na [!UICONTROL Lista de Trabalho] para controlar melhor quais informações estão visíveis.\
Por padrão, o agrupamento [!UICONTROL Esta Semana] é expandido e todos os outros agrupamentos são recolhidos. Quaisquer alterações feitas serão lembradas na próxima vez que você acessar a área da página inicial.

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Início]**.
1. Clique na seta **[!UICONTROL Expandir]** ou **[!UICONTROL Recolher]** ao lado de qualquer agrupamento que você deseja expandir ou recolher.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Ou\
   Para expandir ou recolher todos os agrupamentos simultaneamente, clique na seta **[!UICONTROL Expandir]** ou **[!UICONTROL Recolher]** ao lado de qualquer agrupamento enquanto mantém pressionada a tecla [!UICONTROL Shift].
