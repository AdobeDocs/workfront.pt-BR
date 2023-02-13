---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Criar e editar iniciativas no Planejador de Cenário
description: Ao usar o Adobe Workfront Scenario Planner, você pode criar iniciativas em um plano que você criou ou que foi compartilhado com você. Ao criar iniciativas, você pode mostrar como unidades organizacionais menores contribuem para a conclusão do plano. Por exemplo, se sua organização tiver um plano para os próximos três anos se expandir para um novo mercado, você poderá criar iniciativas dentro desse plano para cada departamento para estimar a necessidade de pessoas e orçamento de cada departamento para realizar esse plano.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1623'
ht-degree: 0%

---

# Crie e edite iniciativas na [!DNL Scenario Planner]

Ao usar a variável [!UICONTROL Planejador de cenário do Adobe Workfront], é possível criar iniciativas em um plano que você criou ou que foi compartilhado com você. Ao criar iniciativas, você pode mostrar como unidades organizacionais menores contribuem para a conclusão do plano. Por exemplo, se sua organização tiver um plano para os próximos três anos se expandir para um novo mercado, você poderá criar iniciativas dentro desse plano para cada departamento para estimar a necessidade de pessoas e orçamento de cada departamento para realizar esse plano.

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
   <td> <p>[!DNL Adobe Workfront] licença* </p> </td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td>Produto </td> 
   <td> <p>Você deve comprar uma licença adicional para a [!DNL Adobe Workfront Scenario Planner] para acessar a funcionalidade descrita neste artigo. </p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">O acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Configurações de nível de acesso* </td> 
   <td> <p>Acesso à [!UICONTROL Editar] ou superior à [!DNL Scenario Planner]</p> <p>Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Permissões de objeto </p> </td> 
   <td> <p>Permissões do [!UICONTROL Manager] para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano na [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Você deve criar um plano ou outro usuário deve compartilhar um plano com você antes que você possa criar uma iniciativa dentro desse plano. Para obter informações sobre como criar planos, consulte [Crie e edite planos na [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Para obter mais informações sobre as iniciativas, consulte [Visão geral das iniciativas na [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Criar iniciativas

Você pode criar iniciativas das seguintes maneiras:

* Do zero.
* Importando projetos em um plano

   Para obter informações sobre como importar projetos como iniciativas em um plano, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Copiando iniciativas existentes.

   Para obter informações sobre cópia de iniciativas, consulte [Copie iniciativas no [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

Para criar iniciativas do zero:

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png), depois clique em [!UICONTROL Cenários].

1. Clique no nome do plano para o qual deseja criar uma iniciativa.
1. Clique no botão **ícone +** à esquerda de **[!UICONTROL Nova iniciativa]**

   Ou

   Clique no botão **[!UICONTROL Nova iniciativa]** e selecione **[!UICONTROL Nova iniciativa]** ou **[!UICONTROL Importar projetos].**

1. Digite um nome para sua iniciativa no **[!UICONTROL Iniciativa sem título]** e pressione Enter ou clique em qualquer outro lugar na página.

   A iniciativa é exibida na linha do tempo do plano, como uma barra azul. Por padrão, a duração de uma iniciativa é de um mês e sempre começa no primeiro mês do plano.

1. (Opcional) Arraste a barra de separação entre o painel esquerdo e a linha do tempo para redimensionar o painel esquerdo.

1. (Opcional) Arraste o final da barra de iniciativa para estender sua duração para mais de um mês e solte-a onde deseja que o mês final da iniciativa seja.
1. (Opcional e condicional) Se a duração da iniciativa for inferior à do plano, arraste e solte a barra de iniciativa em uma posição diferente na linha do tempo do plano, para movê-la para outro período de tempo.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Você só pode selecionar uma duração em meses. A duração de uma iniciativa criada do zero nunca pode exceder a Duração do plano.

1. (Opcional) Na **[!UICONTROL Mês]** selecione uma das seguintes opções para alterar a linha do tempo do plano:

   | Opção de menu suspenso | Descrição |
   |---|---|
   | [!UICONTROL Mês] | Exibe a linha do tempo por mês. Esta é a opção padrão para um plano de um ano. |
   | [!UICONTROL Trimestre] | Exibe a linha do tempo por trimestre. Essa opção só estará disponível quando a variável [!UICONTROL Duração] do plano é de 3 ou 5 anos. Esta é a opção padrão para um plano de 3 anos. |
   | [!UICONTROL Ano] | Exibe a linha do tempo por ano. Essa opção só estará disponível quando a variável [!UICONTROL Duração] do plano é de 5 anos. Esta é a opção padrão para um plano de 5 anos. |


1. (Opcional) Role da esquerda para a direita para ver toda a duração da iniciativa.
1. (Opcional) Clique no botão **[!UICONTROL Hoje]** linha de indicador a retornar à data atual.

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
      <td role="rowheader">Datas de início e fim</td> 
      <td>As datas de início e término da iniciativa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seção Funções de Trabalho Obrigatórias </td> 
      <td> <p>Clique no botão <strong>[!UICONTROL Iniciar a digitação da função de trabalho]</strong> e selecione uma função na lista ou comece a digitar o nome de um<span>n ativo</span> função profissional. </p> <p><span>Dependendo se o plano está configurado para usar FTEs ou horas,</span> adicionar o número de funções necessárias para esta iniciativa em FTE <span><span>ou horas</span></span><span> para cada mês na iniciativa</span>. <span>Os três primeiros meses da iniciativa são exibidos por padrão.</span></p> <p><span>Atualizar as informações de função de cargo para a iniciativa também atualiza as informações de função de cargo Obrigatório para o plano.</span> </p> <p>Para obter informações sobre como configurar o plano para usar FTE ou horas, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crie e edite planos na [!DNL Scenario Planner]</a>. </p> <p>Dica:  
        <ul> 
         <li> <p><span>Use a tecla [!UICONTROL Tab] para ir para o mês seguinte.</span> </p> </li> 
         <li> <p> Todos <span>ative</span> as funções de trabalho no sistema são listadas ao clicar neste campo. </p> </li> 
         <li> <p>As funções de job que já foram adicionadas às funções de job Disponíveis do plano são exibidas primeiro. Para obter informações sobre como adicionar funções de job disponíveis a um plano, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no Planejador de Cenário</a>. </p> </li> 
         <li> <p>[!DNL Workfront] considera que um equivalente a tempo inteiro é de 160 horas por mês. </p> </li> 
        </ul> </p> <p>Você pode inserir um número menor que 1 FTE ou números decimais para FTE <span>ou</span> <span data-mc-edit-date="2021-04-22T16:51:21.5923499-04:00" data-mc-editor="alinawilson" data-mc-comment=" yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:00.3159349-04:00">horas</span>. Por exemplo, uma função de consultor de 0,5 significaria que um consultor dedicaria metade de seu FTE (normalmente, 4 horas, onde 8 horas é 1 FTE) a trabalhar nesta iniciativa. </p> <p>Para todos os cálculos no Planejador de Cenário, o Workfront usa o seguinte valor: 1 FTE = 8 Horas. </p> </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Seção Custos</td> 
      <td> <p>Os custos totais da iniciativa são exibidos à direita da seção [!UICONTROL Custos]. [!DNL Workfront] O calcula os custos de uma iniciativa usando a seguinte fórmula:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>No <strong>[!UICONTROL Custos fixos]</strong> , insira manualmente uma quantia aproximada da estimativa de custo para concluir esta iniciativa. Tal não deve incluir os custos associados às funções de emprego estimadas para a iniciativa.</p> <p><span>Insira um valor para cada mês da iniciativa, movendo-se de um mês para o próximo, conforme você usa a tecla Tab.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>Dependendo de o plano estar configurado para usar FTEs ou horas, a [!UICONTROL Workfront] usa as seguintes fórmulas para calcular o [!UICONTROL Custo de Pessoas]:</p> 
        <ul> 
         <li> <p>Ao usar FTEs: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, sendo 160 o número total de horas de trabalho por mês. </p> </li> 
         <li> <p style="font-weight: normal;">Ao usar horas: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Para obter informações sobre como configurar o plano para usar horas ou FTE, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Criar e editar planos no Planejador de Cenário</a>.</p> </li> 
        </ul> 
        <p>Os custos de Pessoas são calculados na moeda base selecionada nas preferências de Taxas de Câmbio. Para obter informações sobre Taxas de Câmbio, consulte <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> 
        <p>A atualização das informações de custo de uma iniciativa também atualiza a área [!UICONTROL Custos] do plano. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">Depois de definir a função de cargo e os valores de custo necessários para sua iniciativa e modificar a duração da iniciativa, um dos seguintes cenários pode ocorrer:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Se encurtar a iniciativa, [!DNL Workfront] remove a quantia Necessária de recursos e os custos associados ao tempo removido do Plano. As funções de trabalho permanecem no plano, mas não têm FTE Obrigatório ou <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">horas</span>. Os recursos disponíveis para o plano e o orçamento permanecem inalterados.<br>Para atualizar informações sobre o plano, consulte <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Crie e edite planos na [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Se tornar a iniciativa mais longa, você deve especificar a quantidade de funções e custos do emprego para os meses recém-adicionados na iniciativa. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] seção</td> 
      <td>No <strong>[!DNL Net Value]</strong> informe manualmente uma quantia aproximada de estimativa no <strong>[!UICONTROL Benefício planejado]</strong> campo. É isso que os senhores deputados acreditam que será benéfico alcançar esta iniciativa. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Se já tiver definido o número de funções de emprego e o orçamento para o seu plano, o número de funções de emprego e os custos da iniciativa que está a editar e de todas as iniciativas acima e todas excederem os montantes especificados para o plano, [!DNL Workfront] Talvez você não tenha recursos suficientes para terminar a iniciativa. [!DNL Workfront] O marca esse fato como um conflito ao tentar alcançar essa iniciativa e o exibe como uma barra vermelha. Todas as iniciativas que se seguem à iniciativa conflitante são apresentadas em vermelho. Talvez seja necessário ajustar algumas das necessidades de suas iniciativas, começando pela primeira que tem recursos insuficientes. Para obter informações sobre como ajustar iniciativas conflitantes, consulte [Resolver conflitos de iniciativa na [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Opcional) Passe o mouse sobre o nome de uma função de trabalho e clique no botão **[!UICONTROL ícone da lixeira]** ![](assets/delete.png) retirar da iniciativa.

1. (Condicional) Se você fez alterações na iniciativa, clique em **[!UICONTROL Aplicar]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Condicional) Se você não fez alterações, clique no botão **X** ícone no canto superior direito do painel de detalhes da iniciativa para fechá-lo.
1. (Opcional) Atualize a prioridade de suas iniciativas.

   Para obter informações sobre como priorizar iniciativas, consulte [Atualizar as prioridades da iniciativa no Planejador de Cenário](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >As iniciativas listadas primeiro na lista têm prioridade mais alta e obtêm recursos antes das iniciativas listadas abaixo na lista.

1. Clique em **[!UICONTROL Salvar plano]**.

   A iniciativa está agora incluída no seu plano.

   Para obter informações sobre como excluir iniciativas de um plano, consulte [Exclua iniciativas no [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
