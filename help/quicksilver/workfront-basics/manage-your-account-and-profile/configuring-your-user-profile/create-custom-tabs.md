---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Criar seções personalizadas
description: As informações que você vê na [!DNL Workfront] o aplicativo web geralmente é exibido nas seções no painel esquerdo por padrão. Cada seção contém informações diferentes sobre um [!DNL Workfront] área ou objeto.
author: Nolan
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 1079f85651ec691280e2cccefaa6e48e0b9d89f8
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 2%

---

# Criar seções personalizadas

## [!DNL Adobe Workfront] seções

As informações que você vê na [!DNL Workfront] o aplicativo web geralmente é exibido nas seções do painel esquerdo por padrão. Cada seção contém informações diferentes sobre um [!DNL Workfront] área ou objeto.\
Para obter mais informações sobre as áreas padrão de [!DNL Workfront], consulte o artigo [Sobre o padrão [!DNL Adobe Workfront] layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

Além das seções que vêm com o [!DNL Workfront] por padrão, é possível adicionar um painel no qual você pode exibir informações relevantes ao seu fluxo de trabalho. Não é possível adicionar um painel a todas as áreas e objetos.

A tabela a seguir lista todas as [!DNL Workfront] áreas e objetos que contêm seções no painel esquerdo e quais deles podem ser personalizados:

| **[!DNL Workfront]área ou objeto** | **Seções padrão do sistema** | **Seções personalizadas** |
|---|---|---|
| [!UICONTROL Projetos] área | ✓ µ | ✓ |
| [!UICONTROL Equipe] | ✓ |   |
| [!UICONTROL Solicitações] área | ✓ |   |
| [!UICONTROL Planilhas de Horas] área | ✓ |   |
| [!UICONTROL Portfólio] | ✓ | ✓ |
| [!UICONTROL Programa] | ✓ | ✓ |
| [!UICONTROL Projeto] | ✓ | ✓ |
| [!UICONTROL Tarefa] | ✓ |  ✓ |
| [!UICONTROL Problema] |  ✓ |  ✓ |
| [!UICONTROL Usuário] |  ✓ |  ✓ |
| [!UICONTROL Documento] |  ✓ |  ✓ |

{style="table-layout:auto"}

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td>[!UICONTROL Reviewer] ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td>Visualizar acesso ao tipo de objeto</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber que tipo de plano ou licença você tem, entre em contato com o [!DNL Workfront] administrador.

## Adicionar um painel no painel esquerdo de um [!DNL Workfront] objeto ou área

Antes de adicionar um painel, você deve criar o painel com todas as informações que deseja exibir nele. Você também pode criar uma página externa.\
Para obter mais informações sobre a criação de painéis, consulte o artigo [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Para obter mais informações sobre a criação de páginas externas, consulte o artigo [Incorporar uma página externa da Web em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Após criar o painel ou a página externa, é possível adicioná-los ao painel esquerdo.

1. Vá para uma das [!DNL Workfront] áreas ou objetos em que você pode adicionar uma seção personalizada no painel esquerdo.\
   Ou
1. Ir para um objeto no qual você pode adicionar um [!UICONTROL painel] no painel esquerdo.\
   Para obter mais informações sobre a quais áreas e objetos você pode adicionar seções personalizadas, consulte [[!DNL Adobe Workfront] seções](#adobe-workfront-sections).
1. Clique em **[!UICONTROL Adicionar painel]** no painel esquerdo.
1. Digite um nome para o painel no campo **[!UICONTROL Nome do link rápido]** campo. Isso é visível apenas para você.
1. Comece digitando o nome de um painel existente ou página externa no **[!UICONTROL Escolher um painel]** e selecione o painel quando ele for exibido na lista.
1. Clique em **[!UICONTROL Adicionar]**.
1. (Opcional) Arraste e solte as seções na ordem em que deseja exibi-las.

   A seção superior é a seção padrão da página.

   As seções criadas para objetos individuais são exibidas quando você acessa todos os objetos do mesmo tipo e só estão disponíveis para você.

## Exibir painéis no painel esquerdo de objetos

Para obter mais informações sobre como adicionar um painel em um objeto, consulte a seção [[!UICONTROL Adicionar um painel] no painel esquerdo de um objeto ou área do Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) neste artigo.

Ao adicionar um painel a uma seção personalizada em um objeto, o objeto atua como um filtro para o painel. Por exemplo, se você adicionar um relatório de tarefa em um painel e adicionar o painel a um projeto, a seção personalizada que contém o painel no projeto exibirá somente tarefas no projeto que você está visualizando.

Os seguintes objetos são filtrados para o objeto sob o qual são exibidos, se esse objeto estiver mais alto em hierarquia do que eles:

* Projeto
* Tarefa
* Problema
* Processo de aprovação
* Nota
* Documento

Para obter mais informações sobre a hierarquia e a interdependência de objetos, consulte a seção [Interdependência e hierarquia de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalizar o painel esquerdo em um modelo de layout

Ao adicionar painéis ao seu [!DNL Workfront] instância, elas só estarão visíveis para você.

Você pode personalizar as seções em [!DNL Workfront] e compartilhar o novo layout com vários usuários em um modelo de layout. Somente um administrador de sistema ou de grupo pode compartilhá-los com outros usuários em um modelo de layout. Para obter mais informações sobre como personalizar o painel esquerdo com um modelo de layout, consulte [Personalizar o painel esquerdo usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
