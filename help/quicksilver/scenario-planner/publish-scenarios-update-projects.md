---
product-area: enterprise-scenario-planner-product-area
keywords: publicar,planos,projetos,cenário,cenários
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Atualize ou crie projetos publicando iniciativas no Planejador de Cenários
description: Você pode criar projetos a partir de iniciativas existentes, bem como atualizar projetos vinculados anteriormente a iniciativas, publicando cenários no Adobe Workfront Scenario Planner.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '1694'
ht-degree: 0%

---

# Atualize ou crie projetos publicando iniciativas no [!DNL Scenario Planner]

Publicar um cenário do [!DNL Adobe Workfront Scenario Planner] realiza o seguinte:

* Cria projetos a partir das iniciativas no cenário e os vincula.
* Atualiza projetos já vinculados a iniciativas no cenário com informações da iniciativa vinculada. Os projetos também podem ser vinculados a iniciativas quando você os importa para um plano. Para obter mais informações, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td>[!UICONTROL Business] ou superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto </td> 
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">O acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>Nível de acesso*</p> </td> 
   <td> 
    <ul> 
    <li>Acesso à [!UICONTROL Editar] para [!DNL Scenario Planner] e projetos</li></ul>

<p><b>Nota</b>

Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto</p> </td> 
   <td> 
    <ul> 
     <li>Permissões do [!UICONTROL Manager] para o plano </li> 
     <li>Permissões do [!UICONTROL Manager] para projetos publicados</li> 
    </ul> <p>Para obter informações sobre como solicitar acesso adicional a projetos, consulte <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano na [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter mais informações sobre o acesso ao [!DNL Workfront Scenario Planner], consulte [O acesso necessário para usar o [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## Pré-requisitos

Antes de começar:

* Você deve criar e salvar um plano antes de poder publicar iniciativas dele.

## Considerações sobre a publicação de iniciativas em projetos

* Você pode publicar apenas um cenário de um plano.
* Uma iniciativa só pode ser vinculada a um projeto.
* Um projeto pode estar ligado a mais de uma iniciativa quando as iniciativas pertencerem a planos diferentes.

   >[!TIP]
   >
   >Quando um projeto existe em vários planos e você publica informações no projeto a partir de todos os planos, a publicação mais recente substitui as [!DNL Scenario Planner] informações sobre o projeto.

* Se iniciativas foram criadas no plano importando projetos para o plano, a publicação da iniciativa também atualiza os projetos vinculados com informações de iniciativa.

   >[!TIP]
   >
   >Você pode importar o mesmo projeto em vários planos. A publicação pode substituir as informações da iniciativa em um projeto vinculado a várias iniciativas.

   Para obter informações sobre como criar iniciativas importando projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Quaisquer alterações efetuadas ao projeto não são transferidas para a iniciativa ligada.



## Publicar iniciativas

>[!IMPORTANT]
>
>Se você fizer alterações em iniciativas no plano, incluindo resolução de conflitos, deverá republicar a iniciativa para que as novas informações sejam visíveis no projeto. Essas informações são exibidas nos projetos vinculados às iniciativas somente quando você publica a iniciativa correspondente. Para obter informações sobre como resolver conflitos entre iniciativas, consulte [Resolver conflitos de iniciativa na [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **[!UICONTROL Cenários]**
1. (Opcional e condicional) Se desejar publicar de um plano existente, clique no link **[!UICONTROL Filtro]** ícone ![](assets/filter-nwepng.png) no canto superior direito do plano e selecione uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tudo]</td> 
      <td>Exibe todos os planos que você possui ou que são compartilhados com você. Este é o padrão. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Meus planos]</td> 
      <td>Exibe planos que você criou.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Compartilhado comigo]</td> 
      <td> <p>Exibe planos que você não criou, mas que foram compartilhados com você.</p> <p>Importante: Você deve ter permissões do [!UICONTROL Manager] para que os planos compartilhados com você possam publicá-los. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Opcional) Clique no botão **[!UICONTROL Pesquisar]** ícone ![](assets/search-icon.png) e comece a digitar o nome de um plano para encontrá-lo rapidamente na lista.
1. (Condicional) Para publicar de um novo plano, crie um plano.

   Para obter informações sobre como criar planos, consulte [Crie e edite planos na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (Opcional) Clique no nome de um plano existente e crie novos cenários para o plano.

   Para obter informações sobre como criar cenários para um plano, consulte [Crie e compare cenários de plano na [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Opcional) Atualize as iniciativas de um plano existente ou novo ou crie novos planos.

   Para obter informações sobre como criar iniciativas, consulte [Crie e edite iniciativas na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Clique em **[!UICONTROL Salvar plano]**.
1. Selecione o cenário que deseja publicar no **[!UICONTROL Cenário inicial]** menu suspenso e, em seguida, clique em **[!UICONTROL Ir para Publicar]** ![](assets/go-to-publish-button-icon.png) no canto superior direito.

   Ou

   Clique em **[!UICONTROL Comparar cenários]**, passe o mouse sobre o cartão de cenário do qual deseja publicar e clique em **[!UICONTROL Ir para Publicar]** ![](assets/go-to-publish-button-icon.png).

   O [!UICONTROL Publicar iniciativas] página é exibida, mostrando uma lista de todas as iniciativas no cenário. Se alguma das iniciativas foi publicada anteriormente, o ícone do projeto ![](assets/project-icon-sp.png) é exibido após o nome e a variável **[!UICONTROL Última publicação]** é preenchida na lista.

   >[!TIP]
   >
   >Iniciativas que foram criadas importando projetos também exibem o ícone do projeto ![](assets/project-icon-sp.png) à direita do seu nome

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Opcional e condicional) Se desejar publicar de um plano existente, clique no link **[!UICONTROL Filtro]** ícone ![](assets/filter-nwepng.png) no canto superior direito do plano e selecione uma das seguintes opções:

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
      <td>Exibe as iniciativas que você ou outro usuário publicou anteriormente. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Não publicado]</td> 
      <td> <p>Exibe iniciativas não publicadas. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Opcional) Clique no botão **[!UICONTROL Pesquisar]** ícone ![](assets/search-icon.png) e comece a digitar o nome de uma iniciativa para encontrá-la rapidamente na lista.
1. Selecione uma ou várias iniciativas para publicar e criar ou atualizar projetos a partir delas, em seguida, clique em **[!UICONTROL Publicar iniciativas]**.

   Isso cria um novo projeto a partir de cada iniciativa selecionada ou atualiza os projetos conectados existentes, caso as iniciativas publicadas já estivessem vinculadas a um projeto.

   >[!TIP]
   >
   >Novos projetos têm o mesmo nome das iniciativas publicadas.

1. (Condicional) Siga um destes procedimentos:

   * Se você publicou uma iniciativa, clique em **[!UICONTROL Consulte projeto associado]** para abrir o projeto criado ou atualizado da iniciativa.
   * Se você publicou mais de uma iniciativa, clique em **[!UICONTROL Consulte projetos associados]** abrir uma lista de projetos publicados a partir de iniciativas. [!DNL Workfront] aplica a variável [!DNL Scenario Planner] Por padrão, os projetos filtram a lista de projetos. Os projetos publicados mais recentemente são exibidos no topo da lista.

      ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Acesse as seguintes áreas para exibir as informações da iniciativa sobre o projeto:

   * **O [!UICONTROL Atualizações] seção**: Uma atualização é publicada para indicar que o projeto foi criado ou atualizado a partir da iniciativa. A atualização contém o nome da iniciativa que criou ou atualizou o projeto e o nome vinculado do plano que contém a iniciativa. Você pode clicar no nome do plano na atualização para abrir o plano na [!DNL Scenario Planner].

      ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **O [!UICONTROL Visão geral] área do [!UICONTROL Detalhes do projeto] seção**: Um novo [!DNL Scenario Planner] é criada nessa área que contém informações da iniciativa vinculada.

      ![](assets/scenario-planner-on-project-details-350x135.png)

      As seguintes informações de iniciativa são publicadas no [!DNL Scenario Planner] área do [!UICONTROL Detalhes do projeto] seção:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>A duração da iniciativa correspondente quando o projeto está ligado a uma iniciativa. Este campo não é editável.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data da última publicação]</span> </td> 
        <td><span>A data em que o projeto foi publicado pela última vez a partir de uma iniciativa correspondente.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data de início da iniciativa]</span> </td> 
        <td><span>Primeiro dia do início do mês da iniciativa, quando o projeto está vinculado a uma iniciativa.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Data de término da iniciativa]</span> </td> 
        <td><span>O último dia do mês final da iniciativa, quando o projeto está vinculado a uma iniciativa. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Funções de trabalho da iniciativa em FTEs e Horas]</span> </td> 
        <td> <p>Informações sobre as funções associadas e as respectivas atribuições de tempo para a iniciativa. Isso inclui:</p> 
         <ul> 
          <li>Nome da Função de Trabalho</li> 
          <li>Número de ETI</li> 
          <li> <p>Número de horas para todos os FTEs</p> <p>Você pode estimar a quantidade de funções de cargo necessárias para seu plano ou iniciativa usando horas ou FTEs.</p> <p>Para obter mais informações, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no Planejador de Cenário</a>. </p> </li> 
         </ul> 
      <p><b>DICA</b>

      Se o número de funções de trabalho for diferente para cada mês na iniciativa, esse campo exibirá a quantidade máxima de funções necessárias para a iniciativa. Por exemplo, se você precisar de 1 consultor para janeiro e 2 para fevereiro, a coluna exibirá 2FTE e a quantidade correspondente de horas para 2 FTEs para todos os meses.</p> </td>
      </tr> 
      </tbody> 
     </table>

      >[!NOTE]
      >
      >Todos os usuários com [!UICONTROL Exibir] o acesso ao projeto pode visualizar o [!DNL Scenario Planner] na seção [!UICONTROL Visão geral] área. É possível controlar se essa área é exibida na variável [!UICONTROL Detalhes] usando um modelo de layout. Se os usuários não tiverem um modelo de layout associado a eles, essa área será exibida por padrão.
      >
      >   
      >   
      >   * Para obter informações sobre como adicionar ou remover áreas na [!UICONTROL Detalhes] seção usando um modelo de layout, consulte [Personalize o [!UICONTROL Detalhes] exibir usando um modelo de layout](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
      >   * Para obter mais informações sobre a exibição de informações no [!UICONTROL Visão geral] área do [!UICONTROL Detalhes do projeto], consulte [[!UICONTROL Gerenciar] informações no projeto [!UICONTROL Visão geral] area](../manage-work/projects/manage-projects/understand-project-overview-area.md).


   * **O [!UICONTROL Alocação de função] no painel [!UICONTROL Balanceador de Carga de Trabalho] ou a lista de tarefas do projeto**: As informações sobre a atribuição de funções na iniciativa povoam esta área, para além das atribuições de funções no projeto.

      Para obter mais informações, consulte [Visão geral da reconciliação das alocações de recursos entre projetos e iniciativas](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

      ![](assets/role-allocation-panel-350x174.png)

      Quaisquer alterações nas datas ou recursos do projeto não afetam a iniciativa correspondente nem qualquer uma das áreas do projeto que contenham informações de iniciativa.

   * **O [!UICONTROL Orçamentação de Recursos] área do [!UICONTROL Caso de negócios] do projeto**: Uma nova opção para gerenciar recursos do projeto usando [!DNL Scenario Planner] são adicionadas no [!UICONTROL Orçamentação de Recursos] área do [!UICONTROL Caso de negócios] do projeto.

      Para obter mais informações, consulte [Recursos orçamentais na [!UICONTROL Caso de negócios] usando o [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      ![](assets/sp-in-business-case-selected-350x110.png)

1. (Opcional) Revise as seguintes informações na [!DNL Scenario Planner] depois de publicar um cenário:

   * O cenário publicado se torna o primeiro cenário após publicar iniciativas a partir dele.
   * Não é possível publicar de nenhum outro cenário depois de publicar um cenário pelo menos uma vez.
   * O [!UICONTROL Ir para Publicar] é removida de todos os outros cenários depois de pelo menos uma iniciativa ter sido publicada em um cenário.
   * Um indicador verde é exibido ao lado dos ícones do projeto das iniciativas publicadas no plano.

      ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * Um indicador verde &quot;Publicado&quot; é exibido na parte superior do cenário, no cartão do cenário e o campo Publicado é preenchido no cartão do cenário, indicando o número de iniciativas no cenário que foram publicadas.

      ![](assets/published-scenario-highlighted-350x632.png)

      >[!TIP]
      >
      >Se todos os projetos publicados nas iniciativas do cenário forem excluídos, a indicação de que o cenário foi publicado será removida. Para obter mais informações, consulte [Excluir projetos](../manage-work/projects/manage-projects/delete-projects.md).

1. (Opcional) Atualize as informações sobre a iniciativa e repita o processo descrito acima para republicar as informações da iniciativa e atualizar as informações sobre o projeto vinculado.

   Para obter informações sobre como editar iniciativas, consulte [Crie e edite iniciativas na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


