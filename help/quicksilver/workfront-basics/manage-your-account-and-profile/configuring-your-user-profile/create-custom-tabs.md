---
product-area: user-management
navigation-topic: configure-your-user-profile
title: Criar seções personalizadas
description: Por padrão, as informações que você vê no aplicativo Web  [!DNL Workfront]  são exibidas com frequência nas seções no painel esquerdo. Cada seção contém informações diferentes sobre uma área ou objeto  [!DNL Workfront] .
author: Courtney
feature: Get Started with Workfront
exl-id: 68f4b83b-a8b4-4304-930f-62551cb06a92
source-git-commit: 8b1c7f4fa96a6d5f1bc7fbc7ef11e57fa9ff4bff
workflow-type: tm+mt
source-wordcount: '697'
ht-degree: 1%

---

# Criar seções personalizadas

## [!DNL Adobe Workfront] seções

As informações que você vê no aplicativo Web [!DNL Workfront] são frequentemente exibidas nas seções do painel esquerdo por padrão. Cada seção contém informações diferentes sobre uma área ou objeto [!DNL Workfront].\
Para obter mais informações sobre as áreas padrão de [!DNL Workfront], consulte o artigo [Sobre o  [!DNL Adobe Workfront] layout](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md) padrão.

Além das seções que vêm com o [!DNL Workfront] por padrão, você pode adicionar um painel no qual pode exibir informações relevantes ao seu fluxo de trabalho. Não é possível adicionar um painel a todas as áreas e objetos.

A tabela a seguir lista todas as áreas e objetos do [!DNL Workfront] que contêm seções no painel esquerdo e quais deles podem ser personalizados:

| Área ou objeto **[!DNL Workfront]** | **Seções padrão do sistema** | **Seções personalizadas** |
|---|---|---|
| Área [!UICONTROL Projetos] | ✓ µ | ✓ µ |
| [!UICONTROL Equipe] | ✓ µ |   |
| Área [!UICONTROL Solicitações] | ✓ µ |   |
| Área [!UICONTROL Planilhas de Horas] | ✓ µ |   |
| [!UICONTROL Portfolio] | ✓ µ | ✓ µ |
| [!UICONTROL Programa] | ✓ µ | ✓ µ |
| [!UICONTROL Projeto] | ✓ µ | ✓ µ |
| [!UICONTROL Tarefa] | ✓ µ |  ✓ µ |
| [!UICONTROL Problema] |  ✓ µ |  ✓ µ |
| [!UICONTROL Usuário] |  ✓ µ |  ✓ µ |
| [!UICONTROL Documento] |  ✓ µ |  ✓ µ |

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
   <td> <p>Qualquer</p> </td> 
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

&#42;Para saber que tipo de plano ou licença você tem, contate o administrador do [!DNL Workfront].

## Adicionar um painel no painel esquerdo de um objeto ou área [!DNL Workfront]

Antes de adicionar um painel, você deve criar o painel com todas as informações que deseja exibir nele. Você também pode criar uma página externa.\
Para obter mais informações sobre a criação de painéis, consulte o artigo [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).\
Para obter mais informações sobre a criação de páginas externas, consulte o artigo [Incorporar uma página da Web externa em um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

Após criar o painel ou a página externa, é possível adicioná-los ao painel esquerdo.

1. Vá para uma das áreas ou objetos [!DNL Workfront] onde você pode adicionar uma seção personalizada no painel esquerdo.\
   Ou
1. Vá para um objeto onde você pode adicionar um [!UICONTROL painel] no painel esquerdo.\
   Para obter mais informações sobre a quais áreas e objetos você pode adicionar seções personalizadas, consulte [[!DNL Adobe Workfront] seções](#adobe-workfront-sections).
1. Clique em **[!UICONTROL Adicionar painel]** no painel esquerdo.
1. Digite um nome para o painel no campo **[!UICONTROL Nome do link rápido]**. Isso é visível apenas para você.
1. Comece digitando o nome de um painel existente ou página externa no campo **[!UICONTROL Escolha um painel]** e selecione o painel quando ele for exibido na lista.
1. Clique em **[!UICONTROL Adicionar]**.
1. (Opcional) Arraste e solte as seções na ordem em que deseja exibi-las.

   A seção superior é a seção padrão da página.

   As seções criadas para objetos individuais são exibidas quando você acessa todos os objetos do mesmo tipo e só estão disponíveis para você.

## Exibir painéis no painel esquerdo de objetos

Para obter mais informações sobre como adicionar um painel sob um objeto, consulte a seção [[!UICONTROL Adicionar um painel] no painel esquerdo de um objeto ou área do Workfront](#add-a-dashboard-in-the-left-panel-of-a-workfront-object-or-area) neste artigo.

Ao adicionar um painel a uma seção personalizada em um objeto, o objeto atua como um filtro para o painel. Por exemplo, se você adicionar um relatório de tarefa em um painel e adicionar o painel a um projeto, a seção personalizada que contém o painel no projeto exibirá somente tarefas no projeto que você está visualizando.

Os seguintes objetos são filtrados para o objeto sob o qual são exibidos, se esse objeto estiver mais alto em hierarquia do que eles:

* Projeto
* Tarefa
* Problema
* Processo de aprovação
* Nota
* Documento

Para obter mais informações sobre a hierarquia e interdependência de objetos, consulte a seção [Interdependência e hierarquia de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Personalizar o painel esquerdo em um modelo de layout

Ao adicionar painéis à instância do [!DNL Workfront], eles só ficam visíveis para você.

Você pode personalizar as seções em [!DNL Workfront] e compartilhar o novo layout com vários usuários em um modelo de layout. Somente um administrador de sistema ou de grupo pode compartilhá-los com outros usuários em um modelo de layout. Para obter mais informações sobre como personalizar o painel esquerdo com um modelo de layout, consulte [Personalizar o painel esquerdo usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).
