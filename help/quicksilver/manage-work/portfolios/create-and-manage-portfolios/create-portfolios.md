---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Criar um portfólio
description: Uma Portfolio é uma coleção de projetos que competem pelos mesmos recursos, orçamento e agendamento. Os projetos em uma Portfolio são semelhantes o suficiente para usarem o mesmo Conjunto de recursos e serem medidos com base no mesmo cartão de pontuação.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '671'
ht-degree: 1%

---

# Criar um portfólio

<!--Audited: 7/2024-->

Uma Portfolio é uma coleção de projetos que competem pelos mesmos recursos, orçamento e agendamento. Os projetos em uma Portfolio são semelhantes o suficiente para usarem o mesmo Conjunto de recursos e serem medidos com base no mesmo cartão de pontuação.

Você pode usar Portfólios para agrupar projetos que pertencem às mesmas linhas de produtos, divisões, departamentos, empresas ou outras unidades de negócios.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p>
   <p>Atual:[!UICONTROL Plano] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de [!UICONTROL Editar] a Portfólios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Após criar um portfólio, você tem Gerenciar permissões para ele, por padrão</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Maneiras de criar portfólios

Você pode criar portfólios no Workfront usando um dos seguintes métodos:

* Crie um portfólio do zero, começando pela área Portfólios do menu principal. Este artigo descreve como criar um portfólio do zero.

* Importe um portfólio usando o kick-starts.

  Como administrador do Workfront, você pode importar portfólios usando um início.

  Para obter informações sobre como importar dados usando o kick-starts no Workfront, consulte [Importar dados para o Adobe Workfront usando um modelo de Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

* Adicione portfólios à medida que você os conecta a partir de um tipo de registro no Workfront Planning.

  Você deve ter uma nova licença do Workfront e uma licença adicional do Workfront Planning para o Workfront Planning.

  Para obter informações sobre o acesso ao Workfront Planning, consulte [Visão geral do acesso](/help/quicksilver/planning/access/access-overview.md).

  Para obter informações sobre como criar portfólios adicionando-os a registros, consulte a seção &quot;Criar registros conforme você os conecta&quot; no artigo [Criar registros](/help/quicksilver/planning/records/create-records.md).


## Criar um portfólio

{{step1-click-main-menu}}

1. Clique em **[!UICONTROL Portfólios]**.
1. Clique em **[!UICONTROL Novo Portfolio]**.
1. Substitua **[!UICONTROL Portfolio]** sem título pelo nome desejado para o portfólio.

   O nome pode conter até 255 caracteres.

1. (Opcional) Clique no nome em **[!UICONTROL Portfolio Manager]** no cabeçalho na parte superior da página para atribuir um gerente diferente para o portfólio.

   ![Nome do gerente do Portfolio](assets/portfolio-manager-name-350x51.jpg)

   Como criador do portfólio, você é designado como gerente do portfólio por padrão.

1. Clique em **[!UICONTROL Detalhes do Portfolio]** no painel esquerdo.
1. Na área **[!UICONTROL Visão geral]**, altere qualquer uma das seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td> <p>Digite uma descrição para o Portfolio para indicar o que é exclusivo sobre ele. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>Comece digitando o nome de um usuário que deseja indicar como gerente de portfólio e, em seguida, selecione-o quando ele aparecer na lista. É o mesmo que [!UICONTROL Proprietário do Portfolio]. Essa é a pessoa que pode supervisionar o trabalho definido nos projetos do portfólio e aprovar o Business Case.</p> <p>Importante: quando você designa alguém como o [!UICONTROL Portfolio Manager], ele automaticamente obtém permissões do [!UICONTROL Manager] para o portfólio, os programas e os projetos no portfólio. </p> <p>Dica: você também pode atualizar o [!UICONTROL Portfolio Manager] no cabeçalho na parte superior da página.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Grupo </td> 
      <td> <p>Adicione o nome de um único grupo se o grupo for proprietário do portfólio ou tiver responsabilidade de concluí-lo. </p> <p>Você pode verificar se está selecionando o grupo correto passando o mouse sobre ele e clicando no ícone [!UICONTROL information] <img src="assets/info-icon.png"> que é exibido ao lado dele. Uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e seus administradores.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Clique dentro da caixa **[!UICONTROL Adicionar formulário personalizado]** no canto superior direito da página [!UICONTROL Detalhes do Portfolio] para selecionar um formulário personalizado para o portfólio e atualizar os campos personalizados.

   >[!TIP]
   >
   >Você deve ter formulários personalizados de portfólio já criados antes de anexá-los a portfólios.

1. Clique em **[!UICONTROL Salvar alterações]**.
1. (Opcional) Clique em **[!UICONTROL Programas]** no painel esquerdo e em **[!UICONTROL Adicionar Programas]** para adicionar programas ao portfólio.

   Para obter mais informações sobre como criar Programas, consulte [Criar um programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Opcional) Clique em **[!UICONTROL Projetos]** no painel esquerdo e em **[!UICONTROL Adicionar projetos]** para adicionar projetos ao portfólio.

   Para obter mais informações sobre como adicionar projetos a uma Portfolio, consulte [Adicionar projetos a um portfólio](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
