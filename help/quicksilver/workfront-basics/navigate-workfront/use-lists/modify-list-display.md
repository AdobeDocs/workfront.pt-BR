---
navigation-topic: use-lists
title: Modificar como uma lista é exibida
description: No  [!DNL Adobe Workfront], você pode personalizar como uma lista é exibida para você. Outros usuários que visualizam a lista não visualizam suas alterações.
feature: Get Started with Workfront
author: Nolan
exl-id: 3ef7ff03-7293-4b56-9481-e89e1a47a904
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '721'
ht-degree: 0%

---

# Modificar como uma lista é exibida

<!--Audited: 11/2024-->

Em [!DNL Adobe Workfront], você pode personalizar como uma lista é exibida para você. Outros usuários que visualizam a lista não visualizam suas alterações.

Você pode fazer as seguintes personalizações:

* O número de itens exibidos
* Largura ou ordem da coluna
* Se os agrupamentos são expandidos ou recolhidos

>[!NOTE]
>
>As alterações feitas na exibição acima são revertidas quando você sai do [!DNL Workfront] ou fecha o navegador. Essas alterações também podem ser revertidas após um período de 8 horas.

Além das personalizações temporárias acima, você também pode ajustar por quais colunas a lista é classificada, quais [!DNL Workfront] são mantidas mesmo depois que você sair ou fechar o navegador. No entanto, se alguém editar as opções de classificação na exibição de uma lista, a seleção de classificação anterior não será mantida.

Para obter informações sobre como modificar as informações exibidas em sua lista, consulte [Elementos de relatório: filtros, exibições e agrupamentos](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador ou superior </p></li>
   </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação ou superior</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso à [!UICONTROL View] para a área em que a lista está</p> <p>Por exemplo, para modificar a exibição em um projeto, você precisa de acesso à [!UICONTROL Exibição] para Projetos.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Permissões de [!UICONTROL View] ou superior para o modo de exibição aplicado à lista</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Modificar uma lista

1. Vá para a lista em [!DNL Workfront] que você deseja modificar.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   By default, groupings are collapsed.
   </MadCap:conditionalText>
   <br> </p>
   -->

1. (Opcional e condicional) Se os agrupamentos na lista forem recolhidos e você quiser exibir mais informações, clique no agrupamento desejado para expandir a lista e exibir as informações listadas nela.

   Ou

   Para expandir todos os agrupamentos, clique na seta à direita da caixa de seleção no cabeçalho da coluna.

   ![expand_groupings__1_.png](assets/expand-groupings--1--350x227.png)

1. (Opcional e condicional) Se quiser mostrar um número específico de itens na tela, clique no menu suspenso **[!UICONTROL Mostrando]** no canto inferior direito da tela e selecione para exibir **100**, **250**, **500**, **[!UICONTROL Todos]** ou **2000** itens.

   ![Listar número na página](assets/list-number-page-350x119.png)

   >[!TIP]
   >
   >Por padrão, 2.000 itens são exibidos para listas atualizadas e 100 itens são exibidos para listas herdadas. Se a lista contiver mais de 2.000 itens, você não poderá exibir todos os itens em uma página.
   >
   >
   >Para obter o melhor desempenho em listas grandes onde objetos contêm campos de texto formatados, recomendamos limitar esse número a 250.
   >
   >
   >Para obter mais informações sobre os dois tipos de lista, consulte a seção [A diferença entre as listas atualizadas e herdadas](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md#updated) no artigo [Introdução a listas em [!DNL Adobe Workfront]](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

   Os resultados da lista são paginados para mostrar o número selecionado de itens por página. Você pode acessar os resultados em outras páginas clicando nas setas para trás e para frente ou selecionando uma página específica.

1. Para redimensionar a largura de uma coluna, passe o mouse sobre a linha que separa duas colunas e clique em para arrastá-la para a largura desejada.

   A coluna é redimensionada até que você limpe o cache no navegador ou até que você a redimensione manualmente novamente.

1. Para reordenar as colunas em uma lista, passe o mouse sobre um cabeçalho de coluna para exibir a ferramenta Mão e, em seguida, clique em para arrastar a coluna para onde deseja exibi-la.

   A posição da coluna é salva até que você atualize a página.

   Para obter mais informações sobre como personalizar a largura e a ordem das colunas em uma lista, consulte o artigo [Modificar a largura e a ordem da coluna](../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).

1. Para ajustar a ordem de classificação de uma lista, clique em um cabeçalho de coluna para selecioná-lo, mantenha pressionada a tecla CMD (em [!DNL Mac]) ou a tecla CTRL (em [!DNL Windows]) no teclado e selecione até 2 cabeçalhos de coluna adicionais para classificar por eles.

   A lista é classificada por cada coluna selecionada na ordem de sua seleção.

   Todas as modificações feitas na lista são salvas instantaneamente.

   >[!NOTE]
   >
   >Se você estiver classificando grupos na área [!UICONTROL Grupos] da [!UICONTROL Configuração], o modo de exibição de hierarquia de grupos e seus subgrupos não será interrompido quando você alterar a forma como a lista é classificada; os subgrupos permanecerão com seus grupos pai. A lista é classificada primeiro por grupos de nível superior. Em seguida, em cada grupo principal, a lista de subgrupos que estão no mesmo nível é classificada juntas.
