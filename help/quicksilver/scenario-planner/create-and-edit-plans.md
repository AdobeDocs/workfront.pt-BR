---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Criar e editar planos no Planejador de cenários
description: Você pode criar planos como parte do uso do Planejador de cenários da Workfront, ao priorizar a estratégia de nível superior de sua empresa. Para obter mais informações sobre planos, consulte Visão geral dos planos no Planejador de cenários.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '2434'
ht-degree: 0%

---

# Criar e editar planos no [!DNL Scenario Planner]

Você pode criar planos como parte do uso do [!DNL Workfront Scenario Planner], ao priorizar a estratégia de nível superior da sua empresa. Para obter mais informações sobre planos, consulte [Visão geral dos planos no [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

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

## Criar ou editar planos

É possível criar um plano do zero ou editar um plano existente que tenha sido compartilhado com você.

>[!NOTE]
>
>Depois de criar um plano, você é considerado o criador e o proprietário do plano. Quando um usuário é desativado, o plano não tem proprietário e não fica visível para ninguém, a menos que compartilhado anteriormente com um link.

Este artigo descreve como criar um plano do zero ou editar um plano existente.

Para todas as considerações sobre planos, incluindo as informações disponíveis para um plano, consulte [Visão geral dos planos no [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Para obter informações sobre como excluir planos, consulte [Excluir planos na [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Para criar ou editar um plano:

{{step1-to-scenario-planner}}

Uma lista de planos existentes que você criou é exibida no [!DNL Workfront Scenario Planner].

1. (Opcional) Clique no ícone **[!UICONTROL Filtro]** ![Ícone Filtro](assets/filter-icon-34x37.png)no canto superior direito da lista de planos e selecione uma das seguintes opções:

   | Filtro | Descrição |
   |---|---|
   | [!UICONTROL Tudo] | Exibe todos os planos criados ou que foram compartilhados com você. |
   | [!UICONTROL Meus planos] | Exibe os planos que você criou. |
   | [!UICONTROL Compartilhado(s) comigo] | Exibe planos compartilhados com você. |

   ![Opções da lista suspensa de filtros de planos](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Opcional) Clique no ícone **[!UICONTROL Pesquisar]** ![Ícone Pesquisar](assets/search-icon.png) para digitar uma palavra-chave e localizar rapidamente um plano na lista.

1. Clique no nome de um plano existente para editá-lo e continue com a etapa 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   Ou

   Clique em **[!UICONTROL Novo Plano]** no canto superior esquerdo para criar um plano e continue com a etapa 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![Botão Novo plano](assets/new-plan-button.png)

   A caixa [!UICONTROL Novo Plano] é exibida.

   ![Nova caixa de plano](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Condicional) Ao criar um novo plano, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Digite um nome para o plano. Este campo é obrigatório.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Importante: <span style="font-weight: normal;">Você não poderá modificar as seguintes seleções depois de criar e salvar o plano.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Equivalente em Tempo Integral]) ou [!UICONTROL Horas]</span> </td> 
      <td> <p><span>Selecione uma das seguintes opções para indicar como você deseja estimar as informações de função de trabalho para este plano:</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>. Este é o </span> padrão </p> 
      <p><b>IMPORTANTE</b></p>  
      <p>Para todos os cálculos no [!DNL Scenario Planner], [!DNL Workfront] usa o seguinte valor: 1 FTE = 8 Horas. </p> </li> 
      <li> <p><strong>[!UICONTROL Horas]</strong> </p> </li> 
       </ul> <p><b>IMPORTANTE</b></p>

   A opção selecionada aqui determina como as informações de função de trabalho são exibidas para o plano, os cenários do plano e as iniciativas</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Data de início]</td> 
      <td> <p>Selecione o mês e o ano em que deseja que o plano seja iniciado. Você pode selecionar apenas meses nesse campo. [!DNL Workfront] presume que a data de início do plano é o primeiro dia do mês selecionado e a data de término é o último dia do fim do mês em sua duração. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duração]</td> 
      <td> <p>No menu suspenso, selecione uma das seguintes durações:</p> 
       <ul> 
        <li>1 ano. Esta é a duração padrão. </li> 
        <li>3 anos</li> 
        <li> <p>5 anos</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. (Condicional) Clique em **[!UICONTROL Avançar]**.

   A linha do tempo do plano é exibida como o **[!UICONTROL Cenário inicial]**.

   Para obter informações sobre como criar cenários adicionais, consulte [Criar e comparar cenários de planejamento em [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Opcional) No menu suspenso da linha do tempo, selecione uma das opções na tabela a seguir para alterar a forma como você exibe a linha do tempo do plano.

   ![Lista suspensa de meses](assets/month-dropdown-with-all-options.png)

   | Opção de menu suspenso | Descrição |
   |---|---|
   | [!UICONTROL Mês] | Exibe a linha do tempo por mês. Esta é a opção padrão e única para um plano de um ano. |
   | [!UICONTROL Trimestre] | Exibe a linha do tempo por trimestre. Esta opção está disponível somente quando a [!UICONTROL Duração] do plano é de 3 ou 5 anos. Essa é a opção padrão para um plano de 3 anos. |
   | [!UICONTROL Ano] | Exibe a linha do tempo por ano. Esta opção está disponível somente quando a [!UICONTROL Duração] do plano é de 5 anos. Essa é a opção padrão para um plano de 5 anos. |

1. (Opcional) Role da esquerda para a direita para exibir toda a duração do plano.
1. (Opcional) Clique na linha de indicador **[!UICONTROL Hoje]** para retornar ao dia atual.

   ![Indicador de hoje](assets/today-indicator-350x160.png)

1. Clique na caixa **[!UICONTROL Funções de Trabalho]** no cabeçalho do plano para adicionar funções de trabalho que estarão disponíveis para executar o plano.

   Os detalhes da caixa [!UICONTROL Funções de trabalho] são exibidos.

   >[!TIP]
   >
   >A unidade de alocação de função (FTE ou horas) que [!DNL Workfront] usa para este plano é exibida entre parênteses no título da caixa.

   ![Adicionando pessoas ao plano](assets/adding-people-to-plan-350x206.png)

1. Clique no campo **[!UICONTROL Comece a digitar a função de trabalho]** e selecione uma função na lista ou comece a digitar o nome de uma função de trabalho ativa.

   Todas as funções de trabalho ativas no sistema são listadas ao clicar neste campo.

   Isso adiciona a função de trabalho à coluna Funções de trabalho.

1. Atualize ou revise as seguintes informações para a função de trabalho:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Máx. disponível] (para FTE) </p> <p role="rowheader">ou </p> <p role="rowheader"><span>[!UICONTROL Total disponível] (para horas)</span> </p> </td> 
      <td> <p><span>Se você optou por usar horas ou FTE para o plano, digite</span> o número de FTEs de funções de trabalho <span>ou horas</span> disponíveis para executar o trabalho no plano nos seguintes campos: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total disponível]</strong> (para horas): Indique o número total de horas de todos os meses durante a duração do cenário. Por padrão, [!DNL Workfront] divide o número Total disponível igualmente entre todos os meses na duração do cenário. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se você inserir 1200 horas para uma Designer, isso significa que a Designer estará disponível por 100 horas para cada mês durante a duração do plano, quando o plano [!UICONTROL Duration] for de 1 ano. </p> </li> 
        <li> <p><b>[!UICONTROL Máx. disponível]</b> (para FTE): Indique o número de FTEs em que a função de trabalho está disponível para cada mês durante a duração do plano. Por padrão, o <strong>Workfront</strong> atribui o número máximo de [!UICONTROL disponível] a cada mês na duração do cenário.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se você inserir 1 FTE para um Consultor, isso significa que o Consultor estará disponível para 1 FTE para cada mês durante a duração do plano. </p> <p>Você pode informar um número menor que 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Uma função de trabalho de consultor 0,5 significaria que um consultor dedicaria metade de seu FTE (normalmente, 4 horas, onde 8 horas é 1 FTE) para trabalhar neste plano. Para todos os cálculos no Planejador de cenários, o Workfront usa o seguinte valor: 1 FTE = 8 Horas. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Máx. necessário] (para FTE)</p> <p role="rowheader">ou </p> <p role="rowheader"><span>[!UICONTROL Total necessário] (para horas)</span> </p> </td> 
      <td> <p><span>Se você optou por usar horas ou FTE para o seu plano, revise</span> o número de FTEs de funções de trabalho <span>ou horas</span> necessários para concluir as iniciativas no cenário. Revise os seguintes campos:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total necessário]</strong> (para horas): O número total de horas necessárias para todos os meses durante a duração do plano.</p> </li> 
        <li> <p><strong>[!UICONTROL Máx. necessário]</strong> (para FTE): o número máximo de FTEs necessários para qualquer um dos meses durante a duração do plano. </p> </li> 
       </ul> <p>Dica: o <span>número máximo</span> de FTEs <span>ou o número total de horas</span> necessário para essa função de trabalho é exibido após você começar a adicionar iniciativas. Para obter informações sobre como adicionar iniciativas a um plano, consulte <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Criar e editar iniciativas na [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL Taxa horária]</td> 
      <td> <p>Esta é a taxa de [!UICONTROL Hora de Custo] para a função de trabalho. A taxa horária é exibida na moeda do sistema. Para obter informações sobre como configurar Taxas de Câmbio para o seu sistema, consulte <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Passe o mouse sobre o nome de uma função de trabalho ou clique na guia depois de atualizar as informações da função, em seguida, clique no **[!UICONTROL ícone da lixeira]** ![ícone Excluir](assets/delete.png) para removê-lo do plano.
1. Clique em **[!UICONTROL Distribuição da função do trabalho]**.

   O painel Distribuição de funções de trabalho é exibido para todos os meses na duração do cenário.

   ![Distribuição mensal da função de trabalho](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Digite o nome de uma função de trabalho para adicioná-la ao plano no **[!UICONTROL Comece a digitar o campo de função de trabalho]**, em seguida, clique em Inserir quando ele aparecer na lista. Isso adiciona a função de trabalho à coluna [!UICONTROL Funções de trabalho].
1. Atualize ou revise as seguintes informações para cada mês do cenário:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Funções de Trabalho] (FTE ou Horas)</td> 
      <td>Tanto a função de trabalho disponível para o cenário quanto as necessárias para as iniciativas no cenário são exibidas no painel de distribuição de funções de trabalho. Há uma indicação se as estimativas de função de trabalho estão em FTEs ou horas no cabeçalho da coluna. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Disponível] (número máximo &lt;número de FTEs&gt;) </p> 
       <div> 
        <p>ou</p> 
        <p>[!UICONTROL Disponível] (total &lt;número de horas&gt;) </p> 
       </div> </td> 
      <td> <p><span>Se você optou por usar horas ou FTE para o seu plano, revise ou atualize</span> o número mensal de FTEs de funções de trabalho <span>ou horas</span> disponíveis para o cenário nos seguintes campos:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Disponível] (número máximo &lt;número de FTEs&gt;)</strong>: o número entre parênteses exibe o número máximo de funções disponíveis para qualquer um dos meses do cenário. Revise ou atualize o número de FTEs para cada mês do cenário. Alterar a alocação mensal pode atualizar o número de FTEs nos parênteses. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Disponível] (total &lt;número de horas&gt;)</strong>: o número entre parênteses exibe o número total de horas disponíveis para todos os meses no cenário. Revise ou atualize o número de horas para cada mês do cenário. Alterar a alocação mensal atualiza o número de horas entre parênteses.</span> </p> </li> 
       </ul> <p>A atualização manual das alocações mensais de funções de trabalho é outra maneira de resolver conflitos de funções de trabalho entre iniciativas no cenário. </p> <p>Dica:   <p><span>Para atualizar a disponibilidade mensal de função por vários meses, digite o número de horas ou FTEs no campo [!UICONTROL Disponível] de qualquer mês e, em seguida, arraste o canto do campo sobre os meses adjacentes para copiar o mesmo valor para cada mês. Solte-o para atualizar todos os meses.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Necessário] (máx &lt;número&gt;)</p> 
       <div> 
        <p role="rowheader">ou</p> 
        <p role="rowheader">[!UICONTROL Necessário] (total &lt;número&gt;)</p> 
       </div> </td> 
      <td> <p><span>Se você optou por usar horas ou FTE para o plano, revise</span> o número mensal de FTEs de funções de trabalho ou as horas necessárias para o cenário nos seguintes campos: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Necessário] (máximo &lt;número de FTEs&gt;)</strong>: o número entre parênteses exibe o número máximo de funções necessárias para qualquer um dos meses do cenário. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Necessário] (total &lt;número de horas&gt;)</strong>: o número entre parênteses exibe o número total de horas necessárias para todos os meses no cenário.</span> </p> </li> 
       </ul> <p>Dica: não é possível modificar o número necessário de FTEs <span>ou horas</span> para a função de trabalho. Esse número é preenchido para o cenário depois que você começa a adicionar iniciativas e seus requisitos de função de trabalho. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Diferença]</td> 
      <td> 
       <div> 
        <p>A diferença mensal entre os valores das funções de trabalho necessárias e disponíveis para o cenário. [!DNL Workfront] calcula a diferença para cada função de trabalho para cada mês usando a seguinte fórmula:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (em FTEs ou horas) </p> 
        <p>Dica: quando a diferença exibe um número negativo, o cenário requer mais funções de trabalho do que o plano tem disponível. Seus recursos estão superalocados. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilização] %</td> 
      <td> 
       <div> 
        <p>A porcentagem de utilização exibe quantas das funções de trabalho disponíveis são realmente usadas (ou necessárias) nas iniciativas do cenário. </p> 
        <p>[!DNL Workfront] calcula a utilização por função de trabalho por mês usando a seguinte fórmula: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>A porcentagem de utilização pode ser exibida nas seguintes cores, dependendo da alocação dos recursos:</p> 
        <ul> 
         <li> <p><b>Verde</b>: os números disponíveis e necessários de funções de trabalho correspondem. Os recursos estão totalmente alocados e a porcentagem de utilização é de 100%. </p> </li> 
         <li> <p><b>Vermelho</b>: há mais funções de trabalho necessárias do que o plano tem disponível. Os recursos estão superalocados e a porcentagem de utilização é superior a 100%.</p> </li> 
         <li> <p><b>Azul</b>: há mais funções de trabalho disponíveis do que o necessário. Os recursos estão subalocados e a porcentagem de utilização é inferior a 100%. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Aplicar]** para salvar a distribuição mensal de funções de trabalho

   Ou

   Clique em **[!UICONTROL Cancelar]** para fechar a lista de distribuição de funções de trabalho e retornar ao cenário.

1. Clique na caixa **[!UICONTROL Financeiro]** no cabeçalho do plano para adicionar o orçamento a este plano.

   Os detalhes da caixa [!UICONTROL Financial] são exibidos.

   >[!TIP]
   >
   >A moeda que [!DNL Workfront] usa para este plano é exibida entre parênteses no título da caixa.

1. Especifique o **[!UICONTROL Orçamento anual]**.

   >[!NOTE]
   >
   >Se o seu plano abranger vários anos, você deverá especificar uma quantia de orçamento para cada ano.

1. Pressione Enter para salvar o orçamento anual e, em seguida, [!UICONTROL Tab] para mover para o ano seguinte.

   O orçamento anual é distribuído automaticamente de forma igual para cada mês do ano selecionado.

1. Clique em **[!UICONTROL Avançado]** para ver a distribuição mensal do orçamento. Os orçamentos anuais e mensais são sempre números arredondados. Quando o valor do orçamento não pode ser distribuído igualmente para todos os meses em um ano devido a decimais, um indicador **[!UICONTROL Restante]** é exibido abaixo da distribuição do orçamento anual.

   ![Links avançados e restantes](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Ajuste manualmente os orçamentos mensais para eliminar os valores excedentes.

   Quando o total de todos os valores de orçamento mensais for maior que o orçamento anual, um indicador de aviso **[!UICONTROL Excedendo]** será exibido abaixo da distribuição do orçamento anual. Ajuste manualmente as quantias de orçamento mensais até que sejam iguais ou inferiores ao orçamento disponível para o plano.

   ![Aviso de orçamento excedido](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Desabilite a configuração **[!UICONTROL Incluir custos de pessoas]** para excluir da contagem os custos associados a funções de trabalho para o custo geral do plano. Os Custos Fixos estão sempre contando para o custo geral do plano. Essa configuração é ativada por padrão e afeta todos os cenários do plano.
1. Clique em qualquer lugar fora da caixa [!UICONTROL Financeiro] para fechá-la. As informações inseridas são salvas automaticamente.

   Agora você pode começar a criar as iniciativas no plano e adicionar cenários.

1. (Recomendado) Clique em **[!UICONTROL Nova iniciativa]** para adicionar uma nova iniciativa.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Para obter informações sobre como adicionar iniciativas, consulte o artigo [Criar e editar iniciativas no [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Opcional) Faça uma cópia do cenário existente para criar um novo cenário do mesmo plano. Para obter mais informações sobre como criar e trabalhar com vários cenários, consulte [Criar e comparar cenários de plano em [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Clique em **[!UICONTROL Salvar Plano]**.

   Seu plano foi criado ou atualizado.

1. (Opcional) Clique no **[!UICONTROL ícone Favoritos]** ![ícone Favoritos](assets/favorites-icon-small.png) à direita do nome do plano para adicionar o plano à sua lista de Favoritos.

1. (Opcional) Copie o URL do plano e envie-o para qualquer outro usuário que precise revisá-lo ou atualizá-lo. Ele deve ter pelo menos o acesso [!UICONTROL Visualização] em seu nível de acesso para poder visualizar o plano. Eles devem ter acesso de [!UICONTROL Edição] para editá-lo. Se eles precisarem revisar informações financeiras sobre o plano, como orçamentos, custos e taxas de funções de trabalho, eles também deverão ter acesso a [!UICONTROL Dados Financeiros] em seus respectivos Níveis de Acesso. Para obter informações sobre o acesso necessário para o [!DNL Scenario Planner], consulte [Acesso necessário para usar o [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
