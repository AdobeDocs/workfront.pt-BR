---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Criar relatórios de dados financeiros com taxas de câmbio exclusivas
description: Se várias taxas de câmbio tiverem sido configuradas no Adobe Workfront, você poderá definir valores financeiros em relatórios e listas para serem exibidos em uma moeda diferente da moeda padrão.
author: Nolan
feature: Reports and Dashboards
exl-id: a0837c70-8330-4c38-98dc-8cf2e7e2e4bd
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1028'
ht-degree: 0%

---

# Criar relatórios de dados financeiros com taxas de câmbio exclusivas

Se várias taxas de câmbio tiverem sido configuradas no Adobe Workfront, você poderá definir valores financeiros em relatórios e listas para serem exibidos em uma moeda diferente da moeda padrão.

>[!IMPORTANT]
>
>Se você selecionar uma moeda diferente da moeda padrão em uma Exibição, os links não serão mais exibidos **Adicionar mais tarefas** e **Adicionar mais problemas** na parte inferior de uma lista de projetos.

Para obter informações sobre como alterar a moeda padrão de um determinado projeto, consulte [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

Se houver projetos com uma moeda única no relatório, as somas em agrupamentos também serão exibidas na moeda padrão do sistema.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de visualizar moedas alternativas, conforme descrito nesta seção, o administrador do Workfront deve primeiro ativar e configurar várias moedas na área Configurar do Workfront. Para obter mais informações, consulte [Configurar taxas de câmbio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

## Aplicar valores financeiros a um relatório {#apply-financial-values-to-a-report}

Para converter valores financeiros entre moedas ao trabalhar com relatórios:

1. Vá para o relatório onde deseja converter valores financeiros em uma moeda diferente.
1. Clique no botão **Exibir** lista suspensa, clique em **Alterar Moeda**, selecione uma das seguintes moedas nas quais deseja exibir valores financeiros:

   * Moeda original do projeto
   * Qualquer uma das outras moedas

      >[!TIP]
      >
      >Você pode escolher somente as moedas selecionadas anteriormente em Configurar.
   Usar essa opção permite converter rapidamente valores financeiros em um relatório entre valores de taxa.

   ![Alterar moeda](assets/qs-change-currency-2022-350x257.png)

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: drafted this tip because I think this is confusing; this is in the step above.)</p>
   -->

   <!--
   <note type="tip">
   You can also select the Change Currency option to convert financial values in other lists.
   <br>
   <img src="assets/nwe-change-currency-new-lists-350x219.png" style="width: 350;height: 219;" data-mc-conditions="QuicksilverOrClassic.Quicksilver">
   <br>
   <br>
   </note>
   -->

## Exibir a moeda padrão em vários projetos com moedas diferentes

Quando você personaliza a moeda no nível do projeto e deseja exibir informações de todos os projetos no mesmo relatório, os seguintes cenários existem:

* Se você criar um relatório que traz informações financeiras de dois ou mais projetos com moedas diferentes aplicadas, por padrão, o resumo do agrupamento reflete a moeda padrão do sistema, conforme selecionada pelo administrador do Workfront.
* Se você criar um relatório para dois ou mais projetos que tenham a mesma moeda, mas que sejam diferentes da moeda padrão do sistema, as somas nos agrupamentos serão exibidas usando a moeda padrão do sistema.
* Se você criar um relatório para dois ou mais projetos que tenham atribuições de função de cargo associadas a uma substituição de moeda, o Workfront converterá as informações financeiras das taxas de moeda substituídas da função de cargo para a moeda do projeto (quando você selecionar a Moeda Original do Projeto na exibição) ou para qualquer moeda diferente que você selecionar ao exibir o relatório. Para obter informações sobre a substituição da moeda de uma função de cargo, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

Para exibir dois projetos com moedas personalizadas em um relatório:

1. Crie dois projetos com moedas diferentes aplicadas.

   ![](assets/qs-currency-350x217.png)

1. Registre as horas em ambos os projetos.

   Para obter mais informações sobre tempo de registro, consulte [Tempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Relatório**.
1. Clique em **Novo relatório**, em seguida **Relatório de projeto**.
1. No **Colunas (Exibir)** , adicione uma **Custo real** e resumi-la por **Soma**.

   Para obter informações sobre como criar uma coluna, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

1. No **Agrupamentos** aplique uma **Data de Conclusão Planejada** agrupamento.

   Para obter informações sobre como criar um agrupamento, consulte [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

1. No **Filtros** , adicione um filtro para **Nome do projeto** e selecione os dois projetos com moedas diferentes.

   Para obter informações sobre como criar um filtro, consulte [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Clique em **Salvar + Fechar**.

   O total da variável **Custo real** é exibida no Grouping usando a moeda padrão do sistema, independentemente da moeda dos projetos no relatório.

   ![Moeda exibida no agrupamento](assets/qs-currency-displayed-in-groupings-2022-350x292.png)

   Se os dois projetos tiverem moedas diferentes umas das outras, a moeda padrão do sistema também será exibida no Agrupamento do relatório.

## Exibir a Moeda do projeto em um relatório no nível do projeto

Se um agrupamento for aplicado em uma tarefa ou lista de horas em um projeto, os totais no agrupamento serão exibidos na moeda do projeto.

1. Crie um projeto com uma moeda personalizada diferente da moeda padrão do sistema.
1. Vá para o projeto e verifique se ele inclui horas que foram registradas para tarefas.

   Para obter mais informações sobre tempo de registro, consulte [Tempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

   >[!NOTE]
   >
   >As tarefas devem ser atribuídas a usuários ou funções de trabalho com taxas de custo por hora.

1. Clique em **Tarefas**.
1. Expanda o **Exibir** e selecione **Nova exibição**.
1. Adicionar **Custo real** na nova coluna Exibir como uma nova coluna, e resumi-la por **Soma**.
1. Clique em **Concluído**, depois clique em **Salvar exibição**.
1. Expanda o **Agrupamento** e selecione **Novo agrupamento**.
1. Adicionar **Data de conclusão real** no novo agrupamento como um novo campo, em seguida, clique em **Salvar Agrupamento**.

   O **Custo real** resume o novo agrupamento e exibe o total na moeda do projeto.

## Editar relatórios com moedas exclusivas

Os campos financeiros em um relatório não são editáveis até que você altere a configuração do relatório para mostrar a moeda original dos projetos.

Para editar um campo financeiro em um relatório em linha:

1. Navegue até um relatório.

   >[!NOTE]
   >
   >Se a moeda padrão não for exibida em uma lista em qualquer outra área, você poderá editar a Exibição para exibir a moeda padrão.\
   >Para obter informações sobre como alterar a moeda em uma Exibição, consulte a seção neste artigo [Aplicar valores financeiros a um relatório](#apply-financial-values-to-a-report).

1. Clique em **Ações de Relatório**, em seguida selecione **Editar**.
1. Clique em **Configurações do relatório**.
1. Clique no botão **Moeda padrão** , em seguida, selecione **Moeda original do projeto**.

   ![](assets/qs-report-settings-default-currency-350x370.png)

1. Clique em **Concluído**.
