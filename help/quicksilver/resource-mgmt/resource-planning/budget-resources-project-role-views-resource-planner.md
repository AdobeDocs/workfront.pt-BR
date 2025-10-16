---
product-area: resource-management
navigation-topic: resource-planning
title: Recursos orçados no planejador de recursos usando as visualizações de projeto e função
description: Você pode estimar recursos no Planejador de recursos do Adobe Workfront usando as visualizações Projeto e Função. Não é possível estimar recursos usando a exibição Usuário no Planejador de Recursos.
author: Lisa
feature: Resource Management
exl-id: b1b48529-68e7-4aee-aaa1-d78e91fbb39c
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '2098'
ht-degree: 0%

---

# Recursos de orçamento no Planejador de recursos usando as visualizações Projeto e Função

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: broken off of another larger article (Planning in the RP); reformat, restructure, relink)</p>
-->

A principal função do Planejador de recursos é planejar o orçamento de seus recursos para o trabalho que deve ser concluído nos projetos.

>[!IMPORTANT]
>
>Você pode estimar seus recursos somente se aplicar as visualizações **Visualizar por Projeto** ou **Visualizar por Função** ao Planejador de Recursos.

Antes de começar a orçar as informações no Planejador de recursos, consulte os seguintes artigos:

* [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md)
* [Acesso necessário para estimar recursos no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)
* [Visão geral de horas, FTE e informações de custo nas visualizações Projeto e Função do Planejador de recursos](../../resource-mgmt/resource-planning/overview-of-planner-hour-fte-cost-information-in-role-project-views.md)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td>
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso ao Gerenciamento de recursos que inclui acesso a Editar prioridades e horas de orçamento no Planejador de recursos</p> <p>Editar acesso a Dados Financeiros para recursos de orçamento por Custo</p> <p>Editar acesso a projetos e usuários</p></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para os projetos para os quais você deseja orçar informações</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Recursos de orçamento no Planejador de recursos

* [Recursos de orçamento na Exibição do Projeto](#budget-resources-in-the-project-view)
* [Recursos de orçamento na Exibição de Função](#budget-resources-in-the-role-view)
* [Recursos de orçamento em massa](#budget-resources-in-bulk)

### Recursos de orçamento na Exibição do Projeto {#budget-resources-in-the-project-view}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this section is linked to the Budgeting Project Resources in the Business Case article)</p>
-->

{{step1-to-resourcing}}

1. O **Planejador** é exibido por padrão.
1. (Condicional) Selecione a visualização **Visualizar por projeto**.
1. Expanda os projetos e as funções de trabalho para gerenciar a alocação do projeto, das funções de trabalho ou dos usuários.
1. Para alocação de orçamento para usuários, siga um destes procedimentos:

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para os usuários.

   * Clique no menu **Mais** da função de trabalho do usuário e em **Definir as horas planejadas dos usuários como orçadas**.\
     As horas orçadas de cada usuário são calculadas usando a seguinte fórmula:

     `User Budgeted Hours = User Planned Hours`

1. Para alocar orçamento para funções de trabalho, siga um destes procedimentos:

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para a função de trabalho.

     >[!NOTE]
     >
     >As horas orçadas da função são adicionadas às horas orçadas do projeto.

   * (Condicional) Se você tiver orçado horas para usuários, clique no menu **Mais** para a função de trabalho e, em seguida, clique em **Total de horas orçadas dos usuários para a função**.\
     As horas orçadas para cada função são calculadas usando a seguinte fórmula:

     `Role Budgeted Hours = SUM(User Budgeted Hours)`

   * Clique no menu **Mais** do projeto e em **Definir as horas planejadas das funções como orçadas**.\
     As horas orçadas para cada função são calculadas usando a seguinte fórmula:\
     &#x200B;*

     `Role Budgeted Hours = Role Planned Hours`

     >[!NOTE]
     >   
     >* As horas orçadas da função são adicionadas às horas orçadas do projeto.
     >* Os usuários podem ser orçados para funções principais e outras (ou secundárias).
     >* O **Percentual de Disponibilidade de FTE** das funções do usuário deve ser um número diferente de 0% para que as Horas Disponíveis exibam um valor no Planejador de Recursos para uma função de trabalho. Se um usuário estiver associado a uma função com 0% **Percentual de Disponibilidade de FTE**, o valor de Horas Disponíveis será zero para essa função de trabalho. Nesse caso, a função pode mostrar um **Valor Líquido** negativo.\
     >Para obter mais informações sobre a **Porcentagem de Disponibilidade de FTE** para funções de trabalho, consulte o artigo [Editar perfil de usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para o projeto. Isso distribui o número de Horas Orçadas do Projeto para cada função no projeto. Existem os seguintes cenários:

      * Se o número de Horas orçadas do projeto especificado for igual às Horas planejadas do projeto, as Horas orçadas da função corresponderão às Horas planejadas da função.
      * Se o número de Horas Orçadas do Projeto especificado não for igual às Horas Planejadas do Projeto, as Horas Orçadas da Função serão distribuídas de acordo com a porcentagem de Horas Planejadas necessárias para cada função.\
        Por exemplo, se um projeto tiver 20 Horas planejadas e elas estiverem distribuídas entre duas funções de trabalho (o Consultor exige 12 Horas planejadas e o Engenheiro requer 8 Horas planejadas) e você fizer um orçamento de 30 horas para o Projeto, as horas serão distribuídas da seguinte maneira: a função Consultor recebe 18 Horas orçadas e a função Engenheiro recebe 12 Horas orçadas.

1. Para alocar orçamento para o projeto, siga um destes procedimentos:

   * Estime as funções no projeto, conforme descrito na Etapa 7.\
     As horas orçadas do projeto são calculadas pela seguinte fórmula:

     `Project Budgeted Hours = SUM(Role Budgeted Hours)`

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para o projeto.\
     Isso atualiza as horas orçadas da função, conforme descrito na Etapa 7.\
     ![budget_for_project.png](assets/budget-for-project-350x182.png)

1. Clique em **Salvar**.\
   Depois de fazer o orçamento dos recursos no Planejador de recursos, as horas orçadas dos recursos e qualquer custo associado a eles são listados no Business Case de cada projeto.\
   Para obter mais informações sobre como entender a área Orçamento de Recursos do Business Case, consulte a seção &quot;Orçamento de Recursos&quot; no artigo [Visão Geral das Áreas do Business Case](../../manage-work/projects/define-a-business-case/areas-of-business-case.md).

1. (Opcional) Selecione a view Usuário para observar qualquer superalocação ou subutilização de usuário entre as Horas Disponíveis e Planejadas de cada usuário. As horas orçadas não estão visíveis na visualização Usuário.

   Para obter informações sobre como o Workfront calcula a disponibilidade de um usuário, consulte [Configurar preferências de gerenciamento de recursos](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### Recursos de orçamento na Visualização de função {#budget-resources-in-the-role-view}

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: THIS IS WRONG - I LOGGED A BUG TO FIX THIS LINK - IT SHOULD GO TO"ACCESS NEEDED TO BUDGET IN THE RP":</p>
<p>Planning in the resource planner has links to the UI - ensure Flare notes are there for this: https://workfront.zendesk.com/hc/en-us/articles/115006356928 - the "Budgeting resources in the role view" is linked to this tooltip: ***This is linked to the product in the RP when the user does not have Manage rights on one of the projects under the role. This tool tip is linked here: "You don't have Manage permissions for all projects. Budget hours by individual project instead. Learn more...")</p>
</div>
-->

Você deve ter acesso de Edição a Gerenciamento de Recursos e a Dados Financeiros e ter permissões de Gerenciamento Financeiro nos projetos para fazer o orçamento de recursos no Planejador de Recursos. Se você tiver acesso de Visualização somente a pelo menos um projeto listado em uma função de trabalho, não poderá prever alocações para a função na visualização Função. Você ainda pode fazer a alocação de orçamento para os projetos para os quais tem permissões de gerenciamento.

Para obter informações sobre o acesso necessário para recursos de orçamento, consulte o artigo [Acesso necessário para recursos de orçamento no Adobe Workfront](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

Para alocações de orçamento no Planejador de recursos na visualização de função **&#x200B;**:

1. Clique no ícone **Menu principal** ![Ícone do menu principal](assets/main-menu-icon.png), no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**.
1. O **Planejador** é exibido por padrão.
1. (Condicional) Selecione a exibição **Exibir por função**.
1. Expanda as funções de trabalho e os projetos para gerenciar a alocação do projeto, das funções de trabalho ou dos usuários.
1. Para alocar orçamento para usuários, siga um destes procedimentos:

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para os usuários.
   * Clique no menu **Mais** do projeto e em **Definir as horas planejadas dos usuários como orçadas**.\
     As horas orçadas de cada usuário são calculadas usando a seguinte fórmula:

     `User Budgeted Hours = User Planned Hours`

1. Para alocar orçamento para funções de trabalho, siga um destes procedimentos:

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para as funções de trabalho.\
     Isso distribui as Horas orçadas da função para as Horas orçadas do projeto para os projetos que você tem acesso para gerenciar.

   * Clique no menu **Mais** da função de trabalho e clique em **Definir as horas planejadas dos projetos como orçadas.**&#x200B;As horas orçadas da função são calculadas usando a seguinte fórmula:\
     &#x200B;*

     `Role Budgeted Hours = SUM(Project Budgeted Hours)`

     *As Horas Orçadas do Projeto são calculadas usando a seguinte fórmula:

     `Project Budgeted Hours = Project Planned Hours`

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para os projetos listados na função de trabalho.\
     Isso adiciona o número de Horas orçadas do projeto à função.

   >[!NOTE]
   >
   >Os usuários podem ser orçados para funções principais e outras (ou secundárias). O **Percentual de Disponibilidade de FTE** das funções do usuário deve ser um número diferente de 0% para que as Horas Disponíveis exibam um valor no Planejador de Recursos para uma função de trabalho. Se um usuário estiver associado a uma função com 0% **Percentual de Disponibilidade de FTE**, o valor de Horas Disponíveis será zero para essa função de trabalho. Nesse caso, a função pode mostrar um **Valor Líquido** negativo.\
   >Para obter mais informações sobre a **Porcentagem de Disponibilidade de FTE** para funções de trabalho, consulte o artigo [Editar perfil de usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Para alocar orçamento para o projeto, siga um destes procedimentos:

   * Na coluna **BDG**, especifique manualmente um número de horas orçadas, FTE ou custo para os projetos.\
     Isso também atualiza as Horas orçadas das funções sob as quais o projeto está listado.

   * Clique no menu **Mais** da função de trabalho e em **Definir as horas planejadas dos projetos como orçadas**.\
     As horas orçadas do projeto são calculadas pela seguinte fórmula:

     `Project Budgeted Hours = Project Planned Hours`

     As horas orçadas do projeto são adicionadas às horas orçadas da função.

   * (Condicional) Se tiver orçado as horas para os usuários, clique no menu **Mais** para o projeto e, em seguida, clique em **Total de Horas Orçadas dos Usuários para o Projeto**.\
     As Horas Orçadas do Projeto são calculadas usando a seguinte fórmula:

     `Project Budgeted Hours = SUM(User Budgeted Hours)`

     ![budget_by_role.png](assets/budget-by-role-350x181.png)

1. Clique em **Salvar**.\
   Depois de fazer o orçamento dos recursos no Planejador de recursos, as horas orçadas dos recursos e qualquer custo associado a eles são listados no Business Case de cada projeto.
Para obter mais informações sobre como entender a área Orçamento de Recursos do Business Case, consulte o artigo [Recursos de orçamento no Business Case](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

1. (Opcional) Selecione a visualização **Visualizar por Usuário** para observar qualquer superalocação ou subutilização de usuário entre as Horas Disponíveis e Planejadas para cada usuário. As horas orçadas não estão visíveis na visualização Visualizar por usuário.

### Recursos de orçamento em massa {#budget-resources-in-bulk}

Você pode estimar alocações para seus recursos em massa ao usar links rápidos. Os links rápidos estão disponíveis somente para as Visualizações de projeto e função.

![Opções de orçamento automáticas](assets/rp-project-view-with-automatic-budgeting-options-on-project-350x173.png)

>[!NOTE]
>
>Ao usar os links rápidos para alocações de orçamento para recursos, o orçamento é aplicado automaticamente apenas aos períodos exibidos na tela. Se a linha do tempo de um projeto se estender por um período maior que o exibido na tela, você deverá rolar da esquerda para a direita e usar os links rápidos para fazer o orçamento dos recursos automaticamente.

Para fazer um orçamento de recursos em massa:

1. Vá para o .\
   Para obter mais informações sobre como acessar o Planejador de recursos, consulte a seção &quot;Acessar o Planejador de recursos&quot; no artigo [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   Uma lista de projetos que você pode gerenciar é exibida na lista.

1. (Opcional) Expanda cada projeto para ver uma lista de funções de trabalho associadas a ele.\
   Ou
1. (Opcional) Selecione **Exibir por função** e expanda cada função para ver uma lista de projetos associados a ela.
1. Passe o mouse sobre o nome de um projeto ou de uma função de trabalho.
1. Clique no ícone **Mais** ![ícone_opções_ícone_recurso_planejador.png](assets/options-icon-resource-planner.png)que é exibido na extremidade direita do nome do projeto ou da função.

1. Clique em uma das opções disponíveis para especificar automaticamente a quantidade de horas orçadas (BDG) para outros objetos.

   Dependendo de você ter clicado no ícone Mais em um projeto ou em uma função, as opções para orçamento em massa serão diferentes. A tabela abaixo ilustra as opções disponíveis para projetos e funções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td> </td> 
      <td><strong>Exibição do projeto</strong> </td> 
      <td><strong>Exibição de função</strong> </td> 
     </tr> 
     <tr> 
      <td>Opções de projeto</td> 
      <td> 
       <ul> 
        <li><strong>Definir as horas planejadas das funções como orçadas</strong>: selecione esta opção para fazer com que as horas orçadas da função se tornem idênticas às suas horas planejadas. O total de Horas Orçadas para as funções será exibido para as Horas Orçadas do Projeto. </li> 
        <li><strong>Ajustar Datas de Orçamento</strong> : selecione esta opção para mover as Horas Orçadas para um período diferente.<br>Para obter mais informações sobre como ajustar datas de orçamento, consulte <a href="../../resource-mgmt/resource-planning/adjust-budgeting-dates.md" class="MCXref xref">Ajustar datas de orçamento no Planejador de Recursos</a>.</li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Definir as horas planejadas dos usuários como orçadas</strong>: selecione esta opção para tornar as horas orçadas do usuário idênticas às horas planejadas. </li> 
        <li><strong>Total de Horas Orçadas dos Usuários para o Projeto</strong>: selecione essa opção para adicionar todas as Horas Orçadas dos usuários e exibir o total como as Horas Orçadas do projeto e da função. Recomendamos que você use essa opção depois de ter feito o orçamento manualmente dos usuários ou de ter usado a opção anterior primeiro. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>Opções de Função</td> 
      <td> 
       <ul> 
        <li><strong>Definir as horas planejadas dos usuários como orçadas</strong>: selecione esta opção para tornar as horas orçadas do usuário idênticas às horas planejadas. </li> 
        <li><strong>Total de horas orçadas dos usuários para a função</strong>: selecione esta opção para adicionar todas as horas orçadas do usuário juntas e exibir o total como as horas orçadas para a função e o projeto. Recomendamos que você use essa opção depois de ter feito o orçamento manualmente dos usuários ou de ter usado a opção anterior primeiro. </li> 
       </ul> </td> 
      <td> 
       <ul> 
        <li><strong>Definir as horas planejadas dos projetos como orçadas</strong>: selecione esta opção para tornar as horas orçadas do projeto idênticas às horas planejadas do projeto. </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Algumas das opções podem não ser exibidas se alguns dos pré-requisitos de trabalho no Planejador de recursos estiverem ausentes.
   >
   >
   >Para obter mais informações sobre os pré-requisitos que devem ser atendidos para um orçamento preciso no Planejador de recursos, consulte a seção &quot;Pré-requisitos para trabalhar no Planejador de recursos&quot; no artigo [Visão geral do Planejador de recursos](../../resource-mgmt/resource-planning/get-started-resource-planner.md).\
   >Por exemplo, algumas das opções podem não ser exibidas nos seguintes cenários:
   >
   >   
   >   
   >   * Quando os projetos não estão associados ao Conjunto de recursos
   >   * Quando os Conjuntos de recursos associados aos projetos não contêm usuários
   >   * Quando os Conjuntos de recursos associados a projetos contêm usuários sem função de trabalho associada a eles.
   >   
   >
