---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Copiar módulos ou cenários em  [!DNL Adobe Workfront Fusion]
description: Copiar módulos ou cenários em  [!DNL Adobe Workfront Fusion]
author: Becky
feature: Workfront Fusion
exl-id: 24e77a56-d676-4cf1-a801-1c328ffd0c4e
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# Copiar módulos ou cenários em [!DNL Adobe Workfront Fusion]

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
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
  <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Pré-requisitos

Você deve adicionar módulos a um cenário antes de copiá-los.

## Copiar um módulo ou um grupo de módulos

Ao copiar um módulo, a cópia retém todos os valores de campo e configurações do módulo original.

Você pode colar o módulo ou os módulos em outra área do mesmo cenário ou em um cenário diferente.

Considere o seguinte ao colar módulos em um cenário diferente.

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>If you paste the modules into another scenario, any fields that pull information from a module that you did not copy must be set to pull information from a module in the new scenario.</p> </li>
  -->

* Quaisquer valores de campo que extraem informações de outro módulo que você não copiou não poderão mais acessar essas informações. Você deve definir esses campos para obter informações do novo cenário.
* Se você colar os módulos em um cenário de propriedade de outra equipe ou organização, todas as conexões deverão ser atualizadas para conexões de propriedade do grupo ou organização proprietária do novo cenário.

### Copiar módulos

Copiar um grupo de módulos é semelhante a copiar um único módulo.

1. Clique com o botão direito do mouse no módulo que deseja copiar.

   >[!NOTE]
   >
   >Você pode selecionar mais de um módulo, mantendo pressionado o [!UICONTROL shift] e clicando nos módulos que deseja copiar. Copiar um grupo de módulos também copia quaisquer linhas de conexão, filtros ou lógica de roteamento entre eles.

1. Selecione **[!UICONTROL Copiar módulo]**.
1. Mova o cursor para a área do cenário em que deseja copiar o cenário.
1. Clique com o botão direito e selecione **[!UICONTROL Colar]**.
1. Conecte os módulos colados ao cenário arrastando-os para o local apropriado no cenário.

   Você também pode usar atalhos de teclado para copiar e colar.

## Copiar um cenário por clonagem

A clonagem de um cenário cria uma cópia do cenário, que pode ser editada.

1. Abra a página de detalhes do cenário:

   1. Clique na guia **[!UICONTROL Cenário]** no painel esquerdo e, em seguida, clique no cenário sobre o qual deseja obter detalhes.

      Ou

      Se você estiver trabalhando no cenário no [Editor de cenários no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md), clique na seta para a esquerda ![](assets/exit-editing-arrow.png) próxima ao canto superior esquerdo da janela.

1. Clique com o botão direito do mouse em **[!UICONTROL Opções]** no canto superior direito da página.
1. Selecione **[!UICONTROL Clone]**.
1. (Opcional) Insira um nome para o novo cenário.
1. (Opcional) Habilite **[!UICONTROL Manter os estados de qualquer módulo novo iguais aos que estão sendo duplicados]** para garantir que o cenário copiado também inclua informações sobre os registros mais recentes processados pelo cenário original.
1. Clique em **[!UICONTROL Salvar]** para criar o cenário.

## Copiar um cenário usando blueprints

Os blueprints de cenário representam a organização, o mapeamento e os valores de campo de um determinado cenário em um determinado momento. Você pode exportar um blueprint de cenário para um arquivo JSON em seu computador e, em seguida, importá-lo ao criar um novo cenário. Os cenários importados de um blueprint de cenário podem ser editados.

Um blueprint de cenário representa todo o cenário. Para copiar apenas determinados módulos de um cenário, consulte [Copiar um módulo ou um grupo de módulos](#copy-a-module-or-a-group-of-modules) neste artigo.

>[!NOTE]
>
>Para obter informações sobre blueprints no contexto de [!DNL Adobe Workfront], consulte [Visão geral de blueprints](../../administration-and-setup/blueprints/blueprints-overview.md).

### Exportar um blueprint de cenário

1. No cenário, clique no menu **[!UICONTROL Mais]** na área de configurações de cenário.
1. Clique em **[!UICONTROL Exportar blueprint]**.

   Um arquivo JSON é criado e baixado no computador. Você pode localizar este arquivo na pasta [!DNL Downloads].

### Importar um blueprint

>[!IMPORTANT]
>
>Se você importar um blueprint para um cenário existente, o blueprint do cenário substituirá o existente. Não é possível anexar um blueprint a um cenário existente.

1. Comece a criar um novo cenário.
1. No cenário, clique no menu **[!UICONTROL Mais]** na área de configurações de cenário.
1. Clique em **[!UICONTROL Importar blueprint]**.
1. Na caixa de diálogo exibida, clique em **[!UICONTROL Procurar]**
1. Navegue até o blueprint que você deseja importar e clique em **[!UICONTROL Abrir]**.
1. Clique em **[!UICONTROL Salvar]**.

   Um arquivo JSON é criado e baixado no computador. Você pode localizar este arquivo na pasta [!UICONTROL Downloads].

## Copiar e reutilizar cenários usando modelos

Você pode criar modelos como ponto de partida para seus cenários [!DNL Workfront Fusion]. Ao criar um cenário a partir de um modelo, você pode modificar o cenário sem modificar o modelo. Os valores de campo não são salvos em modelos.

Para obter mais informações sobre como criar e usar modelos, consulte [Modelos de Cenário](../../workfront-fusion/scenarios/templates/fusion-templates.md).
