---
product-area: projects
navigation-topic: financials
title: Gerenciar informações na área de finanças do projeto
description: Gerenciar informações na área de finanças do projeto
author: Alina
feature: Work Management
exl-id: 147f5d55-a827-4cca-9ab0-afb03a4bcd5a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1304'
ht-degree: 2%

---

# Gerenciar informações na área de finanças do projeto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some information in here is duplicated in Edit projects. If you need to update one of the fields in this area, do it in both places.)</p>
-->

Você pode exibir ou editar as informações financeiras de um projeto acessando a área Finanças da seção Detalhes do projeto . Há um número limitado de campos que você pode visualizar ou editar nessa área. Para obter informações sobre como editar todas as informações de um projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

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
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso a Projetos e Dados Financeiros</p> <p>Edite o acesso a Projetos e Dados Financeiros para editar informações financeiras sobre o projeto</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para um projeto ou superior que incluam permissões do View Finance</p> <p>Gerencie permissões do projeto que incluem Gerenciar finanças para editar informações financeiras do projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Visão geral da área de finanças

Considere o seguinte ao exibir ou editar informações na área Financeira:

* As informações financeiras que você pode encontrar na área de finanças de Detalhes do projeto representam valores que são acumulados até o nível do projeto a partir de tarefas, bem como informações inseridas diretamente no projeto. Algumas informações financeiras podem ser gerenciadas no projeto, bem como no nível da tarefa.
* Você deve ter permissões de Exibição no projeto, bem como acesso aos Dados financeiros a partir do nível de acesso para poder visualizar a área de Finanças em um projeto.
* Você deve ter permissões de Gerenciamento no projeto, bem como acesso aos Dados financeiros no nível de acesso para poder editar as informações na área de finanças . No entanto, recomendamos que somente o Proprietário do projeto edite as informações nesta área .

## Exibir informações financeiras em um projeto

1. Vá para um projeto.
1. Clique em **Detalhes do projeto** no painel esquerdo.
1. Clique no botão **Editar** ícone ![](assets/edit-icon.png) no canto superior direito da seção Detalhes e clique em **Finanças**.

   ![](assets/finance-area-in-details-view-only-nwe-350x188.png)

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront configurou o Modelo de layout, a seção Visão geral pode não ser listada primeiro, caso em que é recolhida. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. Exiba os seguintes campos na área de finanças do projeto:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Método Índice de desempenho</td> 
      <td> Controla o método que a Workfront usa para calcular métricas de Valor ganho. Pode ser baseado em horas ou em custos. <br>Para obter mais informações sobre o PIM, consulte o artigo <a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">Definir o PIM (Performance Index Method)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">CPI / SPI / CSI</td> 
      <td> <p>Essas são métricas de desempenho do projeto que mostram o desempenho do seu projeto em um determinado momento. Seus valores são calculados com base no Método de Índice de Desempenho.<br>Para obter mais informações, consulte os seguintes artigos: </p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">Calcular Índice de Desempenho de Custo (CPI)</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">Calcular o Índice de Desempenho da Programação (SPI) </a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">Calcular CSI (Cost Schedule Performance Index, Índice de Desempenho da Programação de Custo)</a> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calcular ao concluir</td> 
      <td> O custo total projetado do seu projeto, representado em horas se o PIM (Performance Index Method) for baseado em horas e for representado em um valor monetário, se o PIM (Performance Index Method) for baseado no custo.<br>Para obter mais informações sobre como calcular a Estimativa na conclusão, consulte o artigo <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">Calcular Estimativa na Conclusão (EAC)</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Orçamento</td> 
      <td>Este é o orçamento definido para o projeto. Isso é especificado manualmente pelo Proprietário do Projeto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo Fixo</td> 
      <td>Trata-se dos custos fixos do projeto, independentemente de outras atividades do projeto. Eles são inseridos manualmente pelo Proprietário do Projeto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo Planejado</td> 
      <td>O custo estimado do projeto, com base nas Horas Planejadas e nas taxas associadas aos destinatários da tarefa (funções de trabalho ou usuários).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Custo Efetivo</td> 
      <td>Todos os custos do projeto. Custo Real é a soma de todos os custos reais: custo da mão de obra (com base nas Horas Reais e nas taxas associadas às funções da tarefa ou aos usuários que as registram), despesas e custos fixos, que podem ser associados a um projeto ou tarefa.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita com Valor Fixo</td> 
      <td>Defina a receita esperada com base no cronograma do projeto. A Receita Fixa é especificada manualmente pelo Proprietário do Projeto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita Planejada</td> 
      <td>A receita projetada era esperada com base nas Horas Planejadas e nas taxas associadas aos destinatários da tarefa (funções de trabalho ou usuários).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita Efetivo</td> 
      <td>Receita real do projeto com base nas Horas Reais e nas taxas associadas aos destinatários da tarefa (funções de trabalho ou usuários).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Receita Faturada</td> 
      <td> <p>Receita faturada a clientes ou outras partes que é capturada nos Registros de Faturamento. Para obter mais informações sobre registros de faturamento, consulte o artigo <a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">Criar registros de faturamento</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

## Editar informações financeiras em um projeto

Como Proprietário do projeto, você pode editar as informações na subguia Finanças de um projeto.

Para editar informações na subguia Financiamento de projeto:

1. Vá para um projeto do qual você é o proprietário.

   >[!NOTE]
   >
   >Você precisa gerenciar permissões no projeto para executar as etapas a seguir. Também recomendamos que somente o Proprietário do projeto faça alterações na subguia Finanças do projeto.

1. Clique em **Detalhes do projeto** no painel esquerdo.
1. Clique no botão **Editar** ícone ![](assets/edit-icon.png) no canto superior direito da seção Detalhes e clique em **Finanças** . Isso abre a área de finanças para edição.
1. Edite qualquer campo disponível para edição, clicando uma vez no campo ou clicando em **+Adicionar** para adicionar informações a um campo vazio.

   >[!TIP]
   >
   >Os campos não estão disponíveis para edição se forem calculados automaticamente pelo Workfront ou se você não tiver permissões de edição neles.

   ![](assets/edit-finance-area-in-project-details-nwe-350x275.png)

1. Atualize qualquer um dos campos abaixo.

   >[!NOTE]
   >
   >Dependendo de como o administrador do Workfront configura nosso Modelo de layout, os campos na seção Detalhes do projeto podem ser diferentes em seu ambiente. Para obter mais informações, consulte [Personalizar a visualização de Detalhes usando um modelo de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Método Índice de desempenho</td> 
      <td> <p>Controla o método que a Workfront usa para calcular métricas de desempenho do projeto. Isso é configurado no nível do sistema pelo seu administrador, mas você também pode editá-lo no nível do projeto. Considere selecionar uma das seguintes opções:</p> 
       <ul> 
        <li><strong>Baseado em hora:</strong>O Workfront usa as Horas Planejadas para calcular o CPI e o EAC do projeto, e o EAC do projeto é exibido como um número, em horas. </li> 
        <li><strong>Baseado em custo:</strong>O Workfront usa o Custo Planejado da Mão de obra para calcular o CPI e o EAC do projeto, e o EAC é exibido como um valor de moeda. Ao selecionar essa opção, verifique se os destinatários da tarefa (funções de trabalho ou usuários) estão associados a taxas de custo.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calcular ao concluir</td> 
      <td> <p>Representa o custo total projetado do projeto ou da tarefa quando ela é concluída. Isso é configurado no nível do sistema pelo seu administrador, mas você também pode editá-lo no nível do projeto. Considere selecionar uma das seguintes opções:</p> 
       <ul> 
        <li><strong>Calcular no nível do projeto</strong>: O EAC para a tarefa-pai e o projeto são determinados inserindo as horas reais/custo real da mão de obra nas Fórmulas do EAC. Esse cálculo inclui Horas/custos e despesas reais adicionados diretamente à tarefa pai ou ao projeto.</li> 
        <li><strong>Rolar de Tarefas/Subtarefas</strong>: EAC para a tarefa pai e o projeto são determinados pela soma do EAC para cada tarefa filho. Esse cálculo exclui Horas/custos e despesas reais adicionados diretamente à tarefa-pai ou ao projeto.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Orçamento</td> 
      <td>Especifique o orçamento para este projeto.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Custo Fixo</strong> </td> 
      <td>Especifique o custo fixo para este projeto. Isso não deve incluir custos de mão de obra ou despesas.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Receita com Valor Fixo</strong> </td> 
      <td> <p>Especifique a receita fixa deste projeto. Tal não deve incluir as receitas provenientes de quaisquer registros de faturação cobrados a parceiros ou a terceiros.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Moeda do projeto</td> 
      <td> <p>Especifique uma moeda para este projeto, se ela for diferente da moeda padrão em seu sistema. A moeda padrão em seu sistema é definida pelo administrador do Workfront. Para obter mais informações sobre como configurar taxas de câmbio no Workfront, consulte o artigo <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Configurar taxas de câmbio</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> </td> 
      <td> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar***Alterações**.
