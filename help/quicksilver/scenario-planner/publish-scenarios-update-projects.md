---
product-area: enterprise-scenario-planner-product-area
keywords: publicar,planos,projetos,cenário,cenários
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Atualizar ou criar projetos publicando iniciativas no Planejador de cenários
description: Você pode criar projetos a partir de iniciativas existentes, bem como atualizar projetos anteriormente vinculados a iniciativas, publicando cenários no Planejador de cenários do Adobe Workfront.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '1729'
ht-degree: 0%

---

# Atualizar ou criar projetos publicando iniciativas no [!DNL Scenario Planner]

A publicação de um cenário a partir do [!DNL Adobe Workfront Scenario Planner] realiza o seguinte:

* Cria projetos das iniciativas no cenário e os vincula.
* Atualiza projetos já vinculados a iniciativas no cenário com informações da iniciativa vinculada. Os projetos também podem ser vinculados às iniciativas quando você os importa para um plano. Para obter informações, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td> <ul></li>
   <li><p>Novo: Ultimate </p></li>
   <p>O Planejador de cenários não está disponível para os novos planos Select ou Prime do Workfront Workfront. </p>
   <li><p>Atual: [!UICONTROL Business] ou superior</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>Novo: Claro ou superior</p> 
   <p>Atual: [!UICONTROL Review] ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto* </td> 
   <td> <ul><li><p>Para os novos planos do Workfront:</p><p> Adobe Workfront</li></p>
   <li><p>Para os planos atuais do Workfront: </p>
   <p>Adobe Workfront</p> <p>Planejador de cenários do Adobe Workfront</p></li></ul>

<p>Para obter mais informações, consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nível de acesso </td> 
   <td> <p>Acesso a [!UICONTROL Editar] para [!DNL Scenario Planner] e [!UICONTROL Projetos]</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td>  <ul> 
     <li>Permissões de [!UICONTROL Manager] para o plano </li> 
     <li>Permissões de [!UICONTROL Manage] para projetos publicados</li> 
    </ul> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar:

* Você deve criar e salvar um plano antes de publicar iniciativas dele.
* A configuração Permitir que usuários criem projetos sem usar um modelo deve estar ativada em sua área Preferências do projeto da Configuração. Para obter informações, consulte [Configurar preferências de projeto do sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Considerações sobre a publicação de iniciativas em projetos

* Você pode publicar somente um cenário de um plano.
* Uma iniciativa pode ser vinculada a apenas um projeto.
* Um projeto pode estar vinculado a mais de uma iniciativa quando as iniciativas pertencerem a planos diferentes.

  >[!TIP]
  >
  >Quando um projeto existe em vários planos e você publica informações de todos os planos no projeto, a publicação mais recente substitui as informações existentes [!DNL Scenario Planner] sobre o projeto.

* Se iniciativas foram criadas no plano importando projetos para o plano, a publicação da iniciativa também atualiza os projetos vinculados com as informações da iniciativa.

  >[!TIP]
  >
  >Você pode importar o mesmo projeto para vários planos. A publicação pode substituir informações da iniciativa em um projeto vinculado a várias iniciativas.

  Para obter informações sobre como criar iniciativas importando projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* As alterações feitas no projeto não são transferidas para a iniciativa vinculada.



## Publicar iniciativas

>[!IMPORTANT]
>
>Se você fizer alterações nas iniciativas do plano, inclusive resolver conflitos, deverá republicar a iniciativa para que as novas informações fiquem visíveis no projeto. Essas informações são exibidas nos projetos vinculados às iniciativas somente quando você publica a iniciativa correspondente. Para obter informações sobre como resolver conflitos entre iniciativas, consulte [Resolver conflitos de iniciativa no [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

{{step1-to-scenario-planner}}

1. (Opcional e condicional) Se quiser publicar de um plano existente, clique no ícone **[!UICONTROL Filtro]** ![Ícone Filtro](assets/filter-nwepng.png) no canto superior direito do plano e selecione uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tudo]</td> 
      <td>Exibe todos os planos que você possui ou que estão compartilhados com você. Este é o padrão. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Meus planos]</td> 
      <td>Exibe os planos que você criou.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Compartilhado comigo]</td> 
      <td> <p>Exibe os planos que você não criou, mas que são compartilhados com você.</p> <p>Importante: você deve ter permissões de [!UICONTROL Manage] para planos compartilhados com você para poder publicá-los. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Opções da lista suspensa de filtros](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Opcional) Clique no ícone **[!UICONTROL Pesquisar]** ![ícone pesquisar](assets/search-icon.png) e comece a digitar o nome de um plano para localizá-lo rapidamente na lista.
1. (Condicional) Para publicar a partir de um novo plano, crie um plano.

   Para obter informações sobre como criar planos, consulte [Criar e editar planos no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. (Opcional) Clique no nome de um plano existente e crie novos cenários para o plano.

   Para obter informações sobre como criar cenários para um plano, consulte [Criar e comparar cenários de plano em [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Opcional) Atualize as iniciativas de um plano existente ou novo ou crie novos.

   Para obter informações sobre como criar iniciativas, consulte [Criar e editar iniciativas no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Clique em **[!UICONTROL Salvar plano]**.
1. Selecione o cenário que deseja publicar no menu suspenso **[!UICONTROL Cenário inicial]** e clique em **[!UICONTROL Ir para publicação]** ![Ir para publicação](assets/go-to-publish-button-icon.png) no canto superior direito.

   Ou

   Clique em **[!UICONTROL Comparar cenários]**, passe o mouse sobre o cartão de cenário do qual deseja publicar e clique em **[!UICONTROL Ir para Publicação]** ![Ir para publicação](assets/go-to-publish-button-icon.png).

   A página [!UICONTROL Publicar iniciativas] é exibida, mostrando uma lista de todas as iniciativas no cenário. Se alguma das iniciativas foi publicada anteriormente, o ícone do projeto ![Ícone do projeto](assets/project-icon-sp.png) será exibido depois que seu nome e a data **[!UICONTROL Última publicação]** forem preenchidos na lista.

   >[!TIP]
   >
   >As iniciativas criadas com a importação de projetos também exibem o ícone do projeto ![Ícone do projeto](assets/project-icon-sp.png) à direita do nome

   ![Ícone do projeto e última data de publicação](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Opcional e condicional) Se quiser publicar de um plano existente, clique no ícone **[!UICONTROL Filtro]** ![Ícone Filtro](assets/filter-nwepng.png) no canto superior direito do plano e selecione uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tudo]</td> 
      <td>Exibe todas as iniciativas do cenário selecionado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Publicado]</td> 
      <td>Exibe as iniciativas que você ou outro usuário publicou antes. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Não Publicado]</td> 
      <td> <p>Exibe iniciativas não publicadas. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Filtro de iniciativas](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Opcional) Clique no ícone **[!UICONTROL Pesquisar]** ![Ícone Pesquisar](assets/search-icon.png) e comece a digitar o nome de uma iniciativa para localizá-la rapidamente na lista.
1. Selecione uma ou várias iniciativas para publicar e criar ou atualizar projetos a partir delas, em seguida, clique em **[!UICONTROL Publicar iniciativas]**.

   Isso criará um novo projeto a partir de cada iniciativa selecionada ou atualizará os projetos conectados existentes, se as iniciativas publicadas já estiverem vinculadas a um projeto.

   >[!TIP]
   >
   >Novos projetos têm o mesmo nome das iniciativas publicadas.

1. (Condicional) Siga um destes procedimentos:

   * Se você publicou uma iniciativa, clique em **[!UICONTROL Ver projeto associado]** para abrir o projeto criado ou atualizado da iniciativa.
   * Se você publicou mais de uma iniciativa, clique em **[!UICONTROL Ver projetos associados]** para abrir uma lista de projetos publicados de iniciativas. [!DNL Workfront] aplica o filtro de Projetos [!DNL Scenario Planner] à lista de projetos por padrão. Os projetos publicados mais recentemente são exibidos no topo da lista.

     ![Planejador de cenários após a publicação das iniciativas](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Acesse as seguintes áreas para exibir informações de iniciativa do projeto:

   * **A [!UICONTROL Seção Atualizações]**: uma atualização é publicada para indicar que o projeto foi criado ou atualizado a partir da iniciativa. A atualização contém o nome da iniciativa que criou ou atualizou o projeto e o nome vinculado do plano que contém a iniciativa. Você pode clicar no nome do plano na atualização para abrir o plano no [!DNL Scenario Planner].

     ![Atualizar confirmação de fluxo de publicação](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **A área [!UICONTROL Visão Geral] da [!UICONTROL seção Detalhes do Projeto]**: uma nova seção [!DNL Scenario Planner] é criada nesta área que contém informações da iniciativa vinculada.

     ![Planejador de cenários nos detalhes do projeto](assets/scenario-planner-on-project-details-350x135.png)

     As seguintes informações de iniciativa estão publicadas na área [!DNL Scenario Planner] da seção [!UICONTROL Detalhes do Projeto]:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Duração da iniciativa]</span> </td> 
        <td><span>A duração da iniciativa correspondente quando o projeto está vinculado a uma iniciativa. Este campo não é editável.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data da Última Publicação]</span> </td> 
        <td><span>A data em que o projeto foi publicado pela última vez em uma iniciativa correspondente.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data de Início da Iniciativa]</span> </td> 
        <td><span>O primeiro dia do mês de início da iniciativa, quando o projeto está vinculado a uma iniciativa.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data de término da iniciativa]</span> </td> 
        <td><span>O último dia do mês final da iniciativa, quando o projeto está vinculado a uma iniciativa. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Funções de Trabalho da Iniciativa em FTEs e Horas]</span> </td> 
        <td> <p>Informações sobre as funções de trabalho associadas e suas alocações de tempo para a iniciativa. Isso inclui:</p> 
         <ul> 
          <li>Nome Função</li> 
          <li>Número de FTEs</li> 
          <li> <p>Número de horas para todos os FTEs</p> <p>Você pode estimar a quantidade de funções de trabalho necessárias para seu plano ou iniciativa usando horas ou FTEs.</p> <p>Para obter mais informações, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no Planejador de cenários</a>. </p> </li> 
         </ul> 
      <p><b>DICA</b>

     Se o número de funções de trabalho for diferente para cada mês na iniciativa, este campo exibirá a quantidade máxima de funções necessárias para a iniciativa. Por exemplo, se você precisar de um Consultor para janeiro e de dois para fevereiro, a coluna exibirá dois FTEs e a quantidade correspondente de horas para dois FTEs para todos os meses.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Todos os usuários com acesso de [!UICONTROL Visualização] ao projeto podem ver a seção [!DNL Scenario Planner] na área [!UICONTROL Visão geral]. Você pode controlar se esta área é exibida na seção [!UICONTROL Detalhes] usando um modelo de layout. Se os usuários não tiverem um modelo de layout associado a eles, essa área será exibida por padrão.
     >
     >   
     >   
     >   * Para obter informações sobre como adicionar ou remover áreas na seção [!UICONTROL Detalhes] usando um modelo de layout, consulte [Personalizar a exibição [!UICONTROL Detalhes] usando um modelo de layout](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Para obter mais informações sobre como exibir informações na área [!UICONTROL Visão Geral] dos [!UICONTROL Detalhes do Projeto], consulte [[!UICONTROL Gerenciar] informações na área [!UICONTROL Visão Geral] do projeto](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **O painel [!UICONTROL Alocação de Função] no [!UICONTROL Balanceador de Carga de Trabalho] ou a lista de tarefas do projeto**: Informações sobre a alocação de funções na iniciativa são preenchidas nesta área, além das alocações de funções no projeto.

     Para obter mais informações, consulte [Visão geral da reconciliação de alocações de recursos entre projetos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![Painel de alocação de funções](assets/role-allocation-panel-350x174.png)

     Quaisquer alterações nas datas ou nos recursos do projeto não afetam a iniciativa correspondente nem nenhuma das áreas do projeto que contêm informações da iniciativa.

   * **A área [!UICONTROL Orçamento de Recursos] do [!UICONTROL Business Case] do projeto**: uma nova opção para gerenciar recursos de projeto usando informações de [!DNL Scenario Planner] foi adicionada na área [!UICONTROL Orçamento de Recursos] do [!UICONTROL Business Case] do projeto.

     Para obter mais informações, consulte [Recursos de orçamento no [!UICONTROL Business Case] usando o [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![Planejador de cenários no business case](assets/sp-in-business-case-selected-350x110.png)

1. (Opcional) Revise as seguintes informações no [!DNL Scenario Planner] depois de publicar um cenário:

   * O cenário publicado se torna o primeiro cenário depois de publicar iniciativas dele.
   * Não é possível publicar a partir de nenhum outro cenário depois de publicar um cenário pelo menos uma vez.
   * A opção [!UICONTROL Ir para a Publicação] é removida de todos os outros cenários depois que pelo menos uma iniciativa tiver sido publicada de um cenário.
   * Um indicador verde é exibido ao lado dos ícones de projeto das iniciativas publicadas no plano.

     ![Indicador para iniciativa publicada](assets/indicator-for-published-initiative-icon-350x119.png)

   * Um indicador verde &quot;Publicado&quot; é exibido na parte superior do cenário e no cartão de cenário, e o campo Publicado é preenchido no cartão de cenário, indicando o número de iniciativas no cenário que foram publicadas.

     ![Cenário publicado](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Se todos os projetos publicados das iniciativas do cenário forem excluídos, a indicação de que o cenário foi publicado será removida. Para obter informações, consulte [Excluir projetos](../manage-work/projects/manage-projects/delete-projects.md).

1. (Opcional) Atualize as informações sobre a iniciativa e repita o processo descrito acima para republicar a iniciativa e atualizar as informações sobre a iniciativa no projeto vinculado.

   Para obter informações sobre como editar iniciativas, consulte [Criar e editar iniciativas no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


