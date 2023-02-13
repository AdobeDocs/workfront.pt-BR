---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copie módulos ou cenários em [!DNL Adobe Workfront Fusion]
description: Copie módulos ou cenários em [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 59941ea1ce523a0d1036138a83f771b058049b34
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Copie módulos ou cenários em [!DNL Adobe Workfront Fusion]

Você pode copiar módulos, grupos de módulos ou cenários inteiros em [!DNL Adobe Workfront Fusion]. Essa capacidade permite reutilizar cenários ou partes de cenários sem precisar criá-los novamente

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p><p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr>
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Você deve adicionar módulos a um cenário antes de copiá-los.

## Copiar um módulo ou um grupo de módulos

Ao copiar um módulo, a cópia retém todos os valores e configurações de campo do módulo original.

Você pode colar o(s) módulo(s) em outra área do mesmo cenário ou em um cenário diferente.

Considere o seguinte ao colar módulos em um cenário diferente.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Qualquer valor de campo que extraia informações de outro módulo que você não copiou não poderá mais acessar essas informações. Você deve definir esses campos para obter informações do novo cenário.
* Se você colar os módulos em um cenário pertencente a outra equipe ou organização, todas as conexões deverão ser atualizadas para as conexões pertencentes ao grupo ou à organização proprietária do novo cenário.

### Copiar módulos

A cópia de um grupo de módulos é semelhante à cópia de um único módulo.

1. Clique com o botão direito do mouse no módulo que deseja copiar.

   >[!NOTE]
   >
   >Você pode selecionar mais de um módulo mantendo pressionada [!UICONTROL shift] e clicando nos módulos que deseja copiar. Copiar um grupo de módulos também copia linhas de conexão, filtros ou lógica de roteamento entre eles.

1. Selecionar **[!UICONTROL Módulo de cópia]**.
1. Mova o cursor para a área do cenário na qual deseja inserir a cópia do cenário.
1. Clique com o botão direito do mouse e selecione **[!UICONTROL Colar]**.
1. Conecte os módulos colados ao cenário, arrastando-os para o local apropriado no cenário.

   Também é possível usar atalhos de teclado para copiar e colar.

## Copiar um cenário por clonagem

Clonar um cenário cria uma cópia do cenário, que pode ser editada.

1. Abra a página de detalhes do cenário:

   1. Clique no botão **[!UICONTROL Cenário]** no painel esquerdo, em seguida, clique em um cenário no qual deseja obter detalhes.

      Ou

      Se você estiver trabalhando no cenário na [O editor de cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próximo ao canto superior esquerdo da janela.

1. Clique com o botão direito **[!UICONTROL Opções]** no canto superior direito da página.
1. Selecionar **[!UICONTROL Clonar]**.
1. (Opcional) Insira um nome para o novo cenário.
1. (Opcional) Ativar **[!UICONTROL Mantenha os estados de qualquer novo módulo iguais aos que estão sendo duplicados]** para garantir que o cenário copiado também inclua informações sobre os registros mais recentes processados pelo cenário original.
1. Clique em **[!UICONTROL Salvar]** para criar o cenário.

## Copie um cenário usando blueprints

Os esquemas de cenário representam a disposição, o mapeamento e os valores de campo de um determinado cenário em um determinado momento. Você pode exportar um blueprint de cenário para um arquivo JSON em seu computador e depois importá-lo ao criar um novo cenário. Os cenários importados de um blueprint de cenário podem ser editados.

Um blueprint do cenário representa o cenário inteiro. Se quiser copiar apenas determinados módulos de um cenário, consulte [Copiar um módulo ou um grupo de módulos](#copy-a-module-or-a-group-of-modules) neste artigo.

>[!NOTE]
>
>Para obter informações sobre blueprints no contexto de [!DNL Adobe Workfront], consulte [Visão geral do Blueprints](../../administration-and-setup/blueprints/blueprints-overview.md).

### Exportar um blueprint de cenário

1. No cenário, clique no botão **[!UICONTROL Mais]** na área de configurações do cenário.
1. Clique em **[!UICONTROL Exportar Blueprint]**.

   Um arquivo JSON é criado e é baixado no computador. Você pode localizar esse arquivo em [!DNL Downloads] pasta.

### Importar um blueprint

>[!IMPORTANT]
>
>Se você importar um blueprint para um cenário existente, o blueprint substituirá o cenário existente. Não é possível anexar um blueprint a um cenário existente.

1. Comece a criar um novo cenário.
1. No cenário, clique no botão **[!UICONTROL Mais]** na área de configurações do cenário.
1. Clique em **[!UICONTROL Importar Blueprint]**.
1. Na caixa de diálogo exibida, clique em **[!UICONTROL Procurar]**
1. Navegue até o blueprint que deseja importar e clique em **[!UICONTROL Abrir]**.
1. Clique em **[!UICONTROL Salvar]**.

   Um arquivo JSON é criado e é baixado no computador. Você pode localizar esse arquivo em [!UICONTROL Downloads] pasta.

## Copiar e reutilizar cenários usando modelos

Você pode criar modelos como ponto de partida para [!DNL Workfront Fusion] cenários. Ao criar um cenário a partir de um modelo, você pode modificar o cenário sem modificar o modelo. Os valores de campo não são salvos em modelos.

Para obter mais informações sobre como criar e usar modelos, consulte [Modelos de cenário](../../workfront-fusion/scenarios/templates/fusion-templates.md).
