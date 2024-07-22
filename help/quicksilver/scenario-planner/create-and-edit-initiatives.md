---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Criar e editar iniciativas no Planejador de cenários
description: Ao usar o Planejador de cenários do Adobe Workfront, você pode criar iniciativas em um plano que você criou ou que foi compartilhado com você. Ao criar iniciativas, você pode mostrar como as unidades organizacionais menores contribuem para a conclusão do plano. Por exemplo, se sua organização tiver um plano para os próximos três anos para expandir para um novo mercado, você poderá criar iniciativas dentro desse plano para cada departamento a fim de estimar a necessidade de pessoal e orçamento de cada departamento para realizar esse plano.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '1618'
ht-degree: 0%

---

# Criar e editar iniciativas no [!DNL Scenario Planner]

<!--Audited: 07/2024-->

Ao usar o [!UICONTROL Planejador de cenários do Adobe Workfront], você pode criar iniciativas em um plano que você criou ou que foi compartilhado com você. Ao criar iniciativas, você pode mostrar como as unidades organizacionais menores contribuem para a conclusão do plano. Por exemplo, se sua organização tiver um plano para os próximos três anos para expandir para um novo mercado, você poderá criar iniciativas dentro desse plano para cada departamento a fim de estimar a necessidade de pessoal e orçamento de cada departamento para realizar esse plano.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plano*</p> </td> 
   <td> <p>Atual: [!UICONTROL Business] ou superior</p>
   <p>Novo: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licença*</p> </td> 
   <td> <p>Novo: Claro ou superior</p> 
   <p>Atual: [!UICONTROL Review] ou posterior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto*</td> 
   <td> 
   <p>Para os planos atuais do Workfront: </p>
   <p>Você deve comprar uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre acesso e permissões para o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Nível de acesso </td> 
   <td> <p>[!UICONTROL Editar] acesso à [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso à documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve criar um plano ou outro usuário deve compartilhar um plano com você antes de criar uma iniciativa dentro desse plano. Para obter informações sobre como criar planos, consulte [Criar e editar planos no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obter mais informações sobre o que são iniciativas, consulte [Visão geral das iniciativas no [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Criar iniciativas

É possível criar iniciativas das seguintes maneiras:

* Do zero.
* Importando projetos para um plano

  Para obter informações sobre como importar projetos como iniciativas em um plano, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Copiando iniciativas existentes.

  Para obter informações sobre como copiar iniciativas, consulte [Copiar iniciativas na [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

Para criar iniciativas do zero:

{{step1-to-scenario-planner}}

1. Clique no nome do plano para o qual deseja criar uma iniciativa.
1. Clique no ícone **+** à esquerda de **[!UICONTROL Nova iniciativa]**

   Ou

   Clique no menu suspenso **[!UICONTROL Nova iniciativa]** e selecione **[!UICONTROL Nova iniciativa]** ou **[!UICONTROL Importar Projetos].**

1. Digite um nome para a iniciativa no campo **[!UICONTROL Iniciativa sem título]** e pressione Enter ou clique em qualquer outro lugar da página.

   A iniciativa é exibida na linha do tempo do plano, como uma barra azul. Por padrão, a duração de uma iniciativa é de um mês e sempre começa no primeiro mês do plano.

1. (Opcional) Arraste a barra de separação entre o painel esquerdo e a linha do tempo para redimensionar o painel esquerdo.

1. (Opcional) Arraste o final da barra de iniciativas para estender sua duração para mais de um mês e solte-a onde deseja que o mês final da iniciativa seja.
1. (Opcional e condicional) Se a duração da iniciativa for menor do que a do plano, arraste e solte a barra da iniciativa em uma posição diferente na linha do tempo do plano para movê-la para outro intervalo de tempo.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Você só pode selecionar uma duração em meses. A duração de uma iniciativa criada do zero nunca pode exceder a Duração do plano.

1. (Opcional) No menu suspenso **[!UICONTROL Mês]**, selecione uma das seguintes opções para alterar a linha do tempo do plano:

   | Opção de menu suspenso | Descrição |
   |---|---|
   | [!UICONTROL Mês] | Exibe a linha do tempo por mês. Essa é a opção padrão para um plano anual. |
   | [!UICONTROL Trimestre] | Exibe a linha do tempo por trimestre. Esta opção está disponível somente quando a [!UICONTROL Duração] do plano é de 3 ou 5 anos. Essa é a opção padrão para um plano de 3 anos. |
   | [!UICONTROL Ano] | Exibe a linha do tempo por ano. Esta opção está disponível somente quando a [!UICONTROL Duração] do plano é de 5 anos. Essa é a opção padrão para um plano de 5 anos. |


1. (Opcional) Role da esquerda para a direita para ver toda a duração da iniciativa.
1. (Opcional) Clique na linha de indicador **[!UICONTROL Hoje]** para voltar à data atual.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Se o seu plano estiver no futuro ou no passado e não incluir a data atual, o indicador Hoje não será exibido.

1. Clique na barra de uma iniciativa. O painel de detalhes da iniciativa é aberto à direita.

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

   Especifique ou revise as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Duração da iniciativa</td> 
      <td>A duração da iniciativa em meses. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Datas inicial e final</td> 
      <td>As datas inicial e final da iniciativa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seção Funções de Trabalho Necessárias </td> 
      <td> <p>Clique no campo <strong>[!UICONTROL Comece a digitar a função de trabalho]</strong> e selecione uma função na lista ou comece a digitar o nome de uma função de trabalho<span>n ativa</span>. </p> <p><span>Se o plano estiver configurado para usar FTEs ou horas,</span> adicione o número de funções de trabalho necessárias para esta iniciativa no FTE <span><span>ou horas</span></span><span> para cada mês na iniciativa</span>. <span>Os primeiros três meses da iniciativa são exibidos por padrão.</span></p> <p><span>Atualizar as informações de função de trabalho para a iniciativa também atualiza as informações de função de trabalho necessárias para o plano.</span> </p> <p>Para obter informações sobre como configurar o plano para usar FTE ou horas, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no [!DNL Scenario Planner]</a>. </p>
      <p><b>IMPORTANTE</b></p>  
      <p>Para todos os cálculos no [!DNL Scenario Planner], [!DNL Workfront] usa o seguinte valor: 1 FTE = 8 Horas. </p>

   <p><b>DICA</b></p>

   <ul> 
       <li> <p><span>Use a tecla [!UICONTROL Tab] para passar para o próximo mês.</span> </p> </li> 
      <li> <p> Todas as funções de trabalho <span>ativas</span> no sistema são listadas quando você clica neste campo. </p> </li> 
       <li> <p>As funções de trabalho que já foram adicionadas às funções de trabalho Disponíveis do plano são exibidas primeiro. Para obter informações sobre como adicionar funções de trabalho disponíveis a um plano, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no Planejador de Cenários</a>. </p> </li> 
       <li> <p>[!DNL Workfront] considera que um equivalente a tempo inteiro é de 160 horas por mês. </p> <p>Para todos os cálculos no Planejador de cenários, o Workfront usa o seguinte valor: 1 FTE = 8 Horas. </p></li> 
      </ul> </p> <p>Você pode inserir um número menor que 1 FTE ou números decimais para FTE <span>ou</span> <span>horas</span>. Por exemplo, uma função de trabalho de consultor de 0,5 significa que um consultor dedicaria metade de seu FTE (normalmente, 4 horas, onde 8 horas é 1 FTE) para trabalhar nessa iniciativa. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Seção Custos</td> 
      <td> <p>Os custos totais da iniciativa são exibidos à direita da seção [!UICONTROL Custos]. [!DNL Workfront] calcula os custos de uma iniciativa usando a seguinte fórmula:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>No campo <strong>[!UICONTROL Custos Fixos]</strong>, insira manualmente uma quantia aproximada estimada do que você acredita que custará para concluir esta iniciativa. Isso não deve incluir os custos associados às funções de trabalho estimadas para a iniciativa.</p> <p><span>Insira um valor para cada mês da iniciativa movendo de um mês para o próximo ao usar a tecla Tab.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>Dependendo de o plano estar configurado para usar FTEs ou horas, a [!UICONTROL Workfront] usa as seguintes fórmulas para calcular o [!UICONTROL Custo de Pessoas]:</p> 
        <ul> 
         <li> <p>Ao usar FTEs: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, onde 160 é o número total de horas de trabalho por mês. </p> </li> 
         <li> <p style="font-weight: normal;">Ao usar horas: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Para obter informações sobre como configurar o plano para usar horas ou FTE, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no Planejador de Cenários</a>.</p> </li> 
        </ul> 
        <p>Os custos de pessoas são calculados na moeda base selecionada nas preferências de Taxas de câmbio. Para obter informações sobre Taxas de Câmbio, consulte <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> 
        <p>Atualizar as informações de custo de uma iniciativa também atualiza a área [!UICONTROL Custos] do plano. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">Depois de definir a função de trabalho e os valores de custo necessários para sua iniciativa e modificar a duração da iniciativa, pode ocorrer um dos seguintes cenários:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Se você encurtar a iniciativa, o [!DNL Workfront] removerá a quantidade Necessária de recursos e os custos associados ao tempo removido do Plano. As funções de trabalho permanecem no plano, mas não têm FTE necessário ou <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">horas</span>. Os recursos disponíveis para o plano e o orçamento permanecem inalterados.<br>Para atualizar informações sobre o plano, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos na [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Se você tornar a iniciativa mais longa, deverá especificar a quantidade de funções de trabalho e custos para os meses adicionados recentemente na iniciativa. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] seção</td> 
      <td>Na seção <strong>[!DNL Net Value]</strong>, insira manualmente um valor aproximado de estimativa no campo <strong>[!UICONTROL Benefício Planejado]</strong>. É isso que o senhor acredita que será o benefício de se alcançar essa iniciativa. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se você já tiver definido o número de funções de trabalho e o orçamento para o seu plano, bem como o número de funções de trabalho e os custos da iniciativa que você está editando e de todas as iniciativas acima dela, e todas excederem os valores especificados para o plano, [!DNL Workfront] poderá descobrir que você não tem recursos suficientes para concluir a iniciativa. [!DNL Workfront] marca isso como um conflito ao tentar alcançar essa iniciativa e a exibe como uma barra vermelha. Todas as iniciativas que seguem a iniciativa conflitante são exibidas em um fundo vermelho. Talvez seja necessário ajustar algumas das necessidades de suas iniciativas, começando pela primeira que tem recursos insuficientes. Para obter informações sobre como ajustar iniciativas conflitantes, consulte [Resolver conflitos de iniciativa no [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Opcional) Passe o mouse sobre o nome de uma função de trabalho, em seguida, clique no **[!UICONTROL ícone da lixeira]** ![](assets/delete.png) para removê-la da iniciativa.

1. (Condicional) Se você fez alterações na iniciativa, clique em **[!UICONTROL Aplicar]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Condicional) Se não tiver feito alterações, clique no ícone **X** no canto superior direito do painel de detalhes da iniciativa para fechá-lo.
1. (Opcional) Atualize a prioridade de suas iniciativas.

   Para obter informações sobre como priorizar iniciativas, consulte [Atualizar prioridades de iniciativa no Planejador de Cenários](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >As iniciativas listadas primeiro na lista têm uma prioridade mais alta e obtêm recursos antes das iniciativas listadas abaixo na lista.

1. Clique em **[!UICONTROL Salvar plano]**.

   A iniciativa agora está incluída em seu plano.

   Para obter informações sobre como excluir iniciativas de um plano, consulte [Excluir iniciativas no [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
