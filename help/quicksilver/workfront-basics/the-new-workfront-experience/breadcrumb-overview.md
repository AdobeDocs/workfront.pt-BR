---
content-type: overview
title: Visão geral das navegações estruturais
description: As navegações estruturais exibem a hierarquia de navegação completa para todos os tipos de objetos.
feature: Get Started with Workfront
exl-id: c4103f8e-4c3f-4d4d-a0eb-628c60735ab7
source-git-commit: 0fea13b0a1d8f14c2d601e0ed0a8d15684a3c4d7
workflow-type: tm+mt
source-wordcount: '324'
ht-degree: 1%

---

# Visão geral das navegações estruturais

As navegações estruturais exibem a hierarquia de navegação completa para todos os tipos de objetos. Cada objeto no caminho da navegação estrutural tem um rótulo que exibe o tipo de objeto. A página em que você está no momento é exibida tanto no cabeçalho da página quanto no final do caminho da navegação estrutural em itálico. No exemplo abaixo, este é o &quot;[!UICONTROL Compartilhar com a equipe de marca]&quot; tarefa.

![Caminho de navegação recolhido](assets/NWE-collapsed-breadcrumb.png)

Quando há muitos objetos no caminho da navegação estrutural ou a largura da tela proibir a exibição da hierarquia de navegação completa, o caminho recolhe algumas navegações estruturais e agrupa esses objetos no início do caminho da navegação estrutural. O projeto e a página de objeto atual sempre estão visíveis no caminho da navegação estrutural.

Por exemplo, &quot;mais 3&quot; na imagem acima indica que 3 objetos não estão sendo exibidos. Esses itens podem estar localizados acima do nível do projeto ou entre o projeto e a página atual.

Clicando em &quot;[!UICONTROL more]&quot; permite expandir a hierarquia completa. Você pode clicar em &quot;[!UICONTROL Menos]&quot; para recolher o caminho da navegação estrutural novamente.

![Navegação estrutural expandida](assets/NWE-expanded-breadcrumb.png)

Você também pode usar as seguintes teclas para navegar pelas navegações estruturais:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Guia</strong> </td> 
   <td> <p>Navegar para cada item na navegação estrutural</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Enter</strong> </td> 
   <td> <p>Expanda um caminho de navegação estrutural recolhido, recolha um caminho de navegação estrutural expandido e abre uma nova página quando estiver num link de objeto</p> </td> 
  </tr> 
 </tbody> 
</table>

+++Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

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
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber que plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

+++

<!--drafted: this is no longer possible, since we removed Campaigns, but it might come back as part of Maestro: 

## Multi-object breadcrumbs

>[!NOTE]
>
>The information in this article is available only in the Preview environment when you participate in the [!UICONTROL Campaigns] beta program. The functionality described here might not be fully available yet. For more information about current available features and how to enroll, see [Campaigns beta].

Some objects can belong to multiple parent objects. For example, a project can belong to multiple campaigns. In this case, all the campaigns that the project belongs to display in the breadcrumb.

The multi-object listing in the breadcrumb (for example, the campaigns) displays the number of parent objects which expands into a list to display all the campaigns that the project is associated with. For more information, see [Add objects to a campaign](../../manage-work/campaigns/add-objects-to-a-campaign.md).


![Project with multiple campaigns in the breadcrumb](assets/project-with-multiple-campaigns-in-breadcrumb.png)

-->

## Acessar um objeto pai da navegação estrutural

Para obter informações sobre objetos pai em [!DNL Workfront], consulte [Entender objetos em [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Condicional) Se você não vir o objeto para o qual deseja navegar em um caminho de navegação estrutural recolhido, clique em **[!UICONTROL more]** e localize o objeto.

   >[!NOTE]
   >
   >Se você não tiver permissão para um objeto, ele não estará visível na navegação estrutural.

1. Clique em qualquer objeto no caminho da navegação estrutural para acessar esse objeto.

   A página de objetos é aberta.
