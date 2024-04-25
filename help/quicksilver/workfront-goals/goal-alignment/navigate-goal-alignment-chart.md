---
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Navegar pela seção Alinhamento de metas no Adobe Workfront Goals
description: Use a seção Alinhamento de metas para exibir uma visualização integral do alinhamento de metas em toda a organização em um fluxograma. Metas alinhadas são exibidas em cartões que se interconectam em uma árvore hierárquica.
author: Alina
feature: Workfront Goals
exl-id: e79ced31-4680-4af7-b083-3d615c747af8
source-git-commit: 09e34ecdfeec531ebbaaba4fb8682496c53d86bf
workflow-type: tm+mt
source-wordcount: '921'
ht-degree: 1%

---

# Navegar pela seção Alinhamento de metas no Adobe Workfront Goals

Use a seção Alinhamento de metas para exibir uma visualização integral do alinhamento de metas em toda a organização em um fluxograma. Metas alinhadas são exibidas em cartões que se interconectam em uma árvore hierárquica.

Para obter informações sobre o alinhamento da meta e como atingi-lo, consulte também os seguintes artigos:

* [Visão geral do alinhamento de metas no Adobe Workfront Goals](../../workfront-goals/goal-alignment/goal-alignment-overview.md)
* [Alinhar metas ao conectá-las às Metas do Adobe Workfront](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)

## Requisitos de acesso

Você deve ter o seguinte para executar as atividades descritas neste artigo:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
<tr>
<td role="rowheader">plano do Adobe Workfront</td>
<td>
<p>Qualquer</p>

</td>
</tr>
<tr>
<td role="rowheader">Licença da Adobe Workfront*</td>
<td>
<p>Nova licença: Contributor ou superior</p>
Ou
<p>Licença atual: Solicitação ou superior</p>  </td>
</tr>
<tr>
<td role="rowheader">Produto*</td>
<td>
<p> Novo requisito de produto, um dos seguintes: </p>
<ul>
<li>Um plano Select ou Prime do Adobe Workfront e uma licença adicional do Adobe Workfront Goals.</li>
<li>Um plano do Ultimate Workfront que inclui o Workfront Goals por padrão. </li></ul>
<p>Ou</p>
<p>Requisito atual do produto: um plano do Workfront e uma licença adicional para o Adobe Workfront Goals. </p> <p>Para obter informações, consulte <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requisitos para usar as metas do Workfront</a>. </p> </td>
</tr>
<tr>
<td role="rowheader">Nível de acesso</td>
<td> <p>Editar acesso às Metas</p> </td>
</tr>
<tr data-mc-conditions="">
<td role="rowheader">Permissões de objeto</td>
<td>
<div>
<p>Exibir permissões ou mais altas para a meta para exibi-la</p>
<p>Gerenciar permissões para a meta para editá-la</p>
<p>Para obter informações sobre como compartilhar metas, consulte <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Compartilhar uma meta no Workfront Goals</a>. </p>
</div> </td>
</tr>
<tr>
<td role="rowheader"><p>Modelo de layout</p></td>
<td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Metas no Menu principal. </p>  
</td>
</tr>
</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Navegar pela seção Alinhamento de metas

1. Clique em **Menu principal** ícone ![Ícone do menu principal](../goal-alignment/assets/dots-main-menu-icon.png) no canto superior direito da tela e clique em **Metas**.
   <!-- Add this when Shell is available to all: or (if available), click the **Main Menu** icon ![Main menu icon](../goal-alignment/assets/three-line-main-menu-icon.png) in the upper-left corner)
   -->
1. Clique em **Alinhamento de metas** no painel esquerdo.
1. Use os filtros no canto superior direito do gráfico de alinhamento para selecionar apenas as metas que são importantes para você. Para obter informações sobre como usar filtros no Workfront Goals, consulte [Filtrar informações nos Adobe Workfront Goals](../../workfront-goals/goal-management/filter-information-wf-goals.md).

   As metas que correspondem aos filtros são exibidas no gráfico de alinhamento nos cartões.

   As seguintes informações são exibidas em um cartão de meta:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Datas do período de tempo </td> 
      <td> <p>Este é o período para o qual a meta está aberta. A meta deve ser alcançada até a data final do período. As Metas do Workfront calculam o progresso na meta com base na duração do período da meta e na data atual.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Indicadores de progresso</td> 
      <td>O número de indicadores de progresso para a meta. Os indicadores de progresso podem estar alinhados a metas, resultados ou atividades. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome do proprietário</td> 
      <td>O nome do usuário, da equipe, do grupo ou da organização designada como Proprietário da meta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nome da meta</td> 
      <td>O nome da meta. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Barra de progresso da meta <span>e Progresso</span></td> 
      <td> <p>O progresso da meta indica quanto da meta foi alcançado no momento. Este é um cálculo automático da média do progresso de todas as metas, resultados e atividades alinhados para a meta com base no tempo decorrido desde o início do período da meta. Para obter informações sobre como calcular o progresso das metas, consulte <a href="../../workfront-goals/goal-management/calculate-goal-progress.md" class="MCXref xref">Visão geral do progresso e da condição da meta no Adobe Workfront Goals</a>. </p> 
       <div> 
        <p>O progresso real da meta na data atual. Os seguintes valores de progresso e cores indicam a probabilidade de a meta ser alcançada no prazo: </p> 
        <ul> 
         <li><span>No Destino</span> (indicador verde): a meta está no prazo e será alcançada no prazo.</li> 
         <li> <span>Em Risco</span> (indicador amarelo): a meta é atrasada e pode não ser alcançada a tempo.</li> 
         <li> <span>Com Problemas</span> (indicador vermelho): a meta corre o risco de não ser alcançada no prazo. </li> 
        </ul> 
       </div> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Updated on date </td> 
       <td> <p>The date when the goal was last updated</p> <p>(NOTE: drafted because I think this was removed with the alignment chart redesign - 21.1) </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">Status</td> 
      <td><span>Metas em todos os status são exibidas na seção Alinhamento de metas.</span> </td> 
     </tr> 
    </tbody> 
   </table>

   Metas alinhadas a outras metas exibem o número de metas alinhadas no cartão de metas.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

1. Clique em **seta apontando para baixo** ícone em uma meta para expandir e exibir ainda mais as metas secundárias.

   ![](assets/alignment-chart-arrow-for-aligned-goals-highlighted-350x241.png)

   >[!TIP]
   >
   >Metas que têm metas secundárias alinhadas a elas exibem o número de metas alinhadas em seus respectivos cartões.

1. (Condicional) Se o filtro atual excluir algumas metas que participam de um alinhamento, uma mensagem de aviso será exibida para indicar que nem todas as metas são exibidas.

   ![](assets/parent-goal-excluded-by-filter-alignment-section-350x230.png)

1. Clique em **Mostre-lhes** para exibir as metas eliminadas no momento pelo filtro.

   Observe as seguintes alterações no gráfico de alinhamento:

   * As metas conectadas anteriormente eliminadas pelo filtro agora são exibidas no gráfico de alinhamento.
   * O filtro no canto superior direito é contornado em amarelo para indicar que não está aplicado no momento.

     ![](assets/reapply-filter-link-and-yellow-filter-highlight-350x120.png)

     Um link Reapply filter é exibido à esquerda do nome do filtro.

1. (Opcional) Clique em **Reaplicar filtro** para retornar aos resultados originais e exibir a hierarquia de metas.
1. (Opcional) Passe o mouse sobre o indicador de progresso para entender onde o progresso da meta deve estar para o dia atual.

   ![](assets/progress-mouse-over-alignment-chart-350x163.png)

   As seguintes informações são exibidas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">A partir de hoje</td> 
      <td>O status do progresso é sempre atual. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><span>Efetivo</span> </td> 
      <td>O progresso real (uma porcentagem) da meta até a data atual, conforme calculado levando em conta todos os indicadores de progresso na meta. Os indicadores de progresso da meta são metas, atividades e resultados alinhados. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Esperado</td> 
      <td> <p>O progresso esperado (uma porcentagem) da meta até a data atual, supondo que você atinja a meta no prazo.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em um cartão de meta para abrir a página de metas. Para obter informações sobre edição de metas existentes, consulte [Editar metas nas Metas do Adobe Workfront](../../workfront-goals/goal-management/edit-goals.md). Para obter informações sobre como atualizar o progresso das metas, consulte [Atualizar progresso da meta nas Metas do Adobe Workfront](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

1. Clique na seta apontando para cima da meta de nível atual para retornar ao nível anterior na hierarquia do gráfico.

   Ou

   (Opcional) Clique em **Sair da hierarquia de metas** para exibir os cartões de todas as metas que correspondem ao filtro atual, sem exibir a conexão entre elas.


