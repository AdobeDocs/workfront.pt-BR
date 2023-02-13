---
product-area: projects
navigation-topic: use-the-home-area
title: Exibir itens no [!UICONTROL Lista de Trabalho] na área de residência
description: O [!UICONTROL Lista de Trabalho] no [!UICONTROL Início] exibe todos os itens de trabalho atribuídos a você. Você pode controlar quais itens são exibidos na variável [!UICONTROL Trabalho] Lista conforme descrito abaixo.
author: Lisa
feature: Get Started with Workfront, Work Management
exl-id: eac2e065-9e32-43c1-90ff-0f841b508c35
source-git-commit: c111ae72da39fc1637320d993906ae9451e17e99
workflow-type: tm+mt
source-wordcount: '1602'
ht-degree: 0%

---

# Exibir itens no [!UICONTROL Lista de Trabalho] na área de residência

O [!UICONTROL Lista de Trabalho] no [!UICONTROL Início] exibe todos os itens de trabalho atribuídos a você. Você pode controlar quais itens são exibidos na variável [!UICONTROL Trabalho] Lista conforme descrito abaixo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Review] somente para aprovações</p> <p>[!UICONTROL Trabalho] ou superior para todos os outros objetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>[!UICONTROL View] ou acesso superior a Projetos, Tarefas, Problemas e Documentos</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Contribua com permissões ou mais para as tarefas e problemas necessários para trabalhar</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Filtre o [!UICONTROL Lista de Trabalho]

Você pode filtrar os itens no [!UICONTROL Lista de Trabalho] para ver apenas tipos específicos de itens. Por exemplo, você pode filtrar a variável [!UICONTROL Lista de Trabalho] para exibir somente problemas ou solicitações.

>[!NOTE]
>
>As opções de filtro são armazenadas no navegador. Se você usar consistentemente o mesmo navegador no mesmo computador (e não apagar os dados do site), os filtros selecionados não serão alterados. Se você alternar entre navegadores ou computadores, os filtros serão revertidos para a opção padrão , que é com todos os filtros desmarcados.

1. Clique no botão **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **[!UICONTROL Início]**.
1. Clique no botão **[!UICONTROL Filtro]** ![](assets/filter-nwepng.png) menu suspenso.
1. Selecione dentre as seguintes opções de filtro para especificar o tipo de itens que deseja exibir:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tudo]</strong></td> 
      <td>Exibe e seleciona todos os itens. Isso inclui tarefas, emissões, aprovações, tarefas pessoais e tarefas e problemas concluídos. </td>
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tarefas Em Execução]</strong></td> 
      <td> <p>Exibe apenas as tarefas nas quais você está trabalhando ativamente. Essas são tarefas atribuídas a você para as quais você clicou no botão [!UICONTROL Trabalhar nela].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tarefas prontas para iniciar]</strong></td> 
      <td> 
       <div> 
        <p>Exibe apenas as tarefas que estão prontas para você iniciar. Ambas as declarações a seguir devem ser verdadeiras:</p> 
        <ul> 
         <li> <p>As tarefas e seus pais não têm predecessores nem limitações de tarefas que os impeçam de ser trabalhadas.</p> </li> 
         <li> <p>A [!UICONTROL Data de início planejada] das tarefas está nas últimas ou até duas semanas no futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tarefas não prontas]</strong></td> 
      <td> 
       <div> 
        <p>Exibe apenas tarefas que ainda não estão prontas para iniciar. Uma das seguintes declarações deve ser verdadeira:</p> 
        <ul> 
         <li> <p>As tarefas e seus pais podem ter antecessores ou restrições de tarefas que as impedem de ser trabalhadas.</p> </li> 
         <li> <p>As tarefas têm uma [!UICONTROL Data de início planejada] que é superior a duas semanas no futuro.</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas trabalhando]</strong></td> 
      <td> <p>Exibe apenas os problemas em que você está trabalhando ativamente. Esses são problemas atribuídos a você, para os quais você clicou no botão [!UICONTROL Trabalhar nele].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Problemas solicitados]</strong></td> 
      <td>Exibe apenas os problemas atribuídos, mas para os quais você não clicou no botão [!UICONTROL Trabalhar nela].</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Pessoal</strong></td> 
      <td>Exibe apenas tarefas pessoais. Essas são tarefas criadas como uma tarefa [!UICONTROL To Do], conforme descrito na seção <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#creating-a-personal-task">Criar uma tarefa pessoal</a> no artigo <a href="../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md">Criar itens de trabalho na área [!UICONTROL Início]</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Aprovações]</strong></td> 
      <td> 
       <div> 
        <p>Exibe apenas aprovações atribuídas ou delegadas a você e aprovações enviadas. As aprovações incluem aprovações em itens de trabalho (projetos, tarefas e emissões) e aprovações de documentos, provas, solicitações de acesso e folhas de horas. Para obter mais informações sobre aprovações, consulte os seguintes artigos:</p> 
        <ul> 
         <li><a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">Exibir aprovações</a> </li> 
        </ul> 
        <ul> 
         <li> <p><a href="../../../review-and-approve-work/manage-approvals/manage-approvals.md" class="MCXref xref">Aprovações de trabalho</a> </p> </li> 
        </ul> 
        <p>Observação: As aprovações enviadas e em que você também é um dos aprovadores são contadas duas vezes.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Concluído]</strong></td> 
      <td> <p>Exibe apenas tarefas concluídas, problemas e tarefas pessoais. O trabalho concluído é exibido nas duas semanas anteriores e é agrupado na Lista de trabalho de acordo com a semana em que foi concluído. As aprovações não são incluídas.</p> <p>O trabalho concluído fica oculto na [!UICONTROL Work List], a menos que você selecione esse filtro.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

   >[!TIP]
   >
   >* As opções de filtro são baseadas em objetos (Tarefas, Problemas, Aprovações, Tarefas pessoais).
   >* Tarefas e problemas são ainda mais filtrados pelo estado em relação à nossa disponibilidade para trabalhar com elas ([!UICONTROL Trabalhando em], [!UICONTROL Pronto para começar], [!UICONTROL Não pronto] para tarefas, e [!UICONTROL Trabalhando em] e [!UICONTROL Solicitado] para problemas). Você pode selecionar para exibir tarefas ou problemas em um estado específico ou clicar em Tarefas ou Problemas para selecionar e exibir todos os estados.
   >* Há um filtro separado para itens concluídos e ele inclui tarefas e problemas. Isso não inclui aprovações. O [!UICONTROL Concluído] O filtro inclui tarefas Pessoais.
   >* Você pode selecionar apenas um estado por vez. Por exemplo, você pode exibir somente [!UICONTROL Trabalhando em] tarefas e somente [!UICONTROL Solicitado] problemas.
   >* Não é possível aplicar filtros para itens atribuídos a uma de suas equipes e eles não são incluídos nos itens atribuídos diretamente a você.



1. (Opcional) Organize ainda mais a [!UICONTROL Lista de Trabalho], conforme descrito na seção [Agrupar e classificar por data, projeto e prioridade](#group-and-sort-by-date-project-and-priority) neste artigo.

## Agrupar e classificar por [!UICONTROL Data], [!UICONTROL Projeto]e [!UICONTROL Prioridade]

É possível agrupar e classificar a variável [!UICONTROL Lista de Trabalho] por [!UICONTROL Data de Conclusão Planejada], [!UICONTROL Data de confirmação], [!UICONTROL Projeto]ou [!UICONTROL Minha prioridade]. A opção escolhida determina como os itens são agrupados na variável [!UICONTROL Lista de Trabalho].

1. Clique no botão **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **[!UICONTROL Início]**.
1. Clique no botão **[!UICONTROL Agrupar por]** menu suspenso.

   ![](assets/group-by-drop-down-expanded-in-home-with-planned-start-date-nwe-350x273.png)

1. Selecione dentre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Conclusão planejada]</strong></td> 
      <td> <p> Os itens são exibidos nos seguintes agrupamentos na [!UICONTROL Work List], dependendo de sua [!UICONTROL Planned Completion Date] (a quantidade de itens contidos em cada agrupamento é exibida entre parênteses ao lado do título do cabeçalho):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Sem data de conclusão planejada]</p> </li> 
        <li> <p>[!UICONTROL Esta Semana]</p> <p>Esse agrupamento é expandido por padrão.</p> </li> 
        <li> <p>[!UICONTROL Próxima Semana]</p> </li> 
        <li> <p>[!UICONTROL Planejado], seguido por várias [!UICONTROL Datas de conclusão planejadas] (vários agrupamentos)</p> </li> 
        <li> <p>[!UICONTROL concluído]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Início planejado]</strong></td> 
      <td> <p>Os itens são exibidos nos seguintes agrupamentos na [!UICONTROL Work List], dependendo da [!UICONTROL Data de início planejada] (o número de itens contidos em cada agrupamento é exibido entre parênteses ao lado do título do cabeçalho):</p> 
       <ul> 
        <li> <p>[!UICONTROL Late]</p> </li> 
        <li> <p>[!UICONTROL Esta Semana] </p> <p>Esse agrupamento é expandido por padrão.</p> </li> 
        <li> <p>[!UICONTROL Próxima Semana]</p> </li> 
        <li> <p>[!UICONTROL Planejado], seguido por várias [!UICONTROL Datas de início planejadas] (vários agrupamentos)</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Data da confirmação]</strong></td> 
      <td> <p>Os itens são exibidos nos seguintes agrupamentos na [!UICONTROL Work List] (o número de itens contidos em cada agrupamento é exibido entre parênteses ao lado do título do cabeçalho):</p> 
       <ul> 
        <li> <p>[!UICONTROL Sem data de confirmação]</p> </li> 
        <li> <p>[!UICONTROL Confirmado na próxima semana]</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Project]</strong></td> 
      <td>Os itens são agrupados de acordo com o projeto, e os projetos são exibidos em ordem alfabética na [!UICONTROL Work List]. (O número de itens contidos em cada agrupamento é exibido entre parênteses ao lado do título do cabeçalho.)</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Minha prioridade]</strong></td> 
      <td>Os itens são exibidos na ordem escolhida. Para obter mais informações, consulte <a href="../../../workfront-basics/using-home/using-the-home-area/prioritize-work-in-home.md" class="MCXref xref">Priorizar o trabalho na área [!UICONTROL Início]</a>.</td> 
     </tr> 
    </tbody> 
   </table>

>[!NOTE]
>
>A classificação padrão é crescente. Se você alterar a classificação para decrescente , as opções de classificação selecionadas serão armazenadas no navegador. Se você usar consistentemente o mesmo navegador no mesmo computador (e não limpar os dados do site) a classificação não é alterada, mas se você alternar navegadores ou computadores, a classificação será alterada para a classificação padrão.

## Exibir itens atrasados

[!DNL Adobe Workfront] O usa as seguintes datas para determinar se as solicitações de trabalho estão atrasadas:

* **Tarefas**: [!UICONTROL Data de Conclusão Planejada]
* **Problemas**: [!UICONTROL Data de Conclusão Planejada]
* **Documentos**: [!UICONTROL Data de envio]
* **Folhas de Horas**: [!UICONTROL Data de envio]
* **Aprovações**: [!UICONTROL Data de envio]
* **Aprovações de prova**: [!UICONTROL Prazo da prova]

## Pesquise no [!UICONTROL Lista de Trabalho]

Quando você pesquisa a variável [!UICONTROL Lista de Trabalho], todos os itens atribuídos a você são retornados na pesquisa (mesmo itens que não estão carregados na tela no momento). Se a variável [!UICONTROL Mostrar concluído] for selecionada, todos os itens marcados como concluídos nas últimas duas semanas também serão retornados.

Além disso, somente os nomes dos itens de trabalho são pesquisados (as informações dentro do item de trabalho não são pesquisadas, nem os nomes dos projetos em que o item de trabalho reside).

Para pesquisar o [!UICONTROL Lista de Trabalho]:

1. Clique no botão **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **[!UICONTROL Início]**.
1. (Opcional) Filtre o [!UICONTROL Lista de Trabalho], conforme descrito em [Filtre o [!UICONTROL Lista de Trabalho]](#filter-the-work-list) e [Agrupar e classificar por data, projeto e prioridade](#group-and-sort-by-date-project-and-priority).

1. (Opcional) Se você estiver pesquisando um item de trabalho que já esteja concluído, deverá configurar a variável [!UICONTROL Lista de Trabalho] para exibir itens concluídos antes de pesquisar.
1. ![](assets/search-icon-highlighted-home-new-filters-and-sorting-nwe-350x238.png)

1. Comece a digitar o nome do item que está procurando.\
   O [!UICONTROL Lista de Trabalho] O é automaticamente filtrado para incluir itens com um nome correspondente.

## Alterar o tamanho da lista de trabalho

Você pode alterar o tamanho da variável [!UICONTROL Lista de Trabalho] de forma que consome em qualquer ponto entre cerca de um quarto da área residencial para cerca de metade da [!UICONTROL Início] área.

1. Clique no botão **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **[!UICONTROL Início]**.
1. Passe o mouse sobre a borda direita do [!UICONTROL Lista de Trabalho], em seguida, arraste para a esquerda ou para a direita até que Lista de trabalho tenha o tamanho desejado.

## Recolher e expandir agrupamentos

Os itens na [!UICONTROL Lista de Trabalho] são exibidos em agrupamentos. Você pode recolher e expandir agrupamentos para controlar quantas informações são exibidas na página em um determinado momento.

Você pode recolher e expandir agrupamentos dentro do [!UICONTROL Lista de Trabalho] para controlar melhor quais informações são visíveis.\
Por padrão, a variável [!UICONTROL Nesta Semana] o agrupamento é expandido e todos os outros agrupamentos são recolhidos. Todas as alterações feitas serão lembradas na próxima vez que você acessar a área inicial.

1. Clique no botão **[!UICONTROL Menu principal]** ![](assets/main-menu-icon.png) no canto superior direito, em seguida, clique em **[!UICONTROL Início]**.
1. Clique no botão **[!UICONTROL Expandir]** ou **[!UICONTROL Recolher]** seta ao lado de qualquer agrupamento que desejar expandir ou recolher.

   ![](assets/expand-section-icon-highlighted-home-new-filters-and-sorting-nwe-350x268.png)

   Ou\
   Para expandir ou recolher todos os agrupamentos simultaneamente, clique no botão **[!UICONTROL Expandir]** ou **[!UICONTROL Recolher]** seta ao lado de qualquer agrupamento enquanto mantém pressionada a tecla [!UICONTROL Shift] chave.
