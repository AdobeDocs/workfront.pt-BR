---
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adicionar resultados às metas no Adobe Workfront Goals
description: Os resultados medem o progresso de uma meta. Sem associar resultados, atividades ou metas alinhadas a uma meta, você não pode ativar a meta e não pode registrar o progresso nela.
author: Alina
feature: Workfront Goals
exl-id: 30e22482-22e2-432d-bb73-7f9a9160aba2
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 3%

---

# Adicionar resultados às metas no Adobe Workfront Goals

<!--Audited for P&P only: 10/2025-->

Os resultados medem o progresso de uma meta. Sem associar resultados, atividades ou metas alinhadas a uma meta, você não pode ativar a meta e não pode registrar o progresso nela.

## Requisitos de acesso

>[!NOTE]
>
>Sua empresa pode optar por continuar usando o Adobe Workfront Goals se ele comprou esse pacote no passado. Você precisa falar com o seu representante de conta para obter mais detalhes.
>
>O Adobe Workfront Goals não está mais disponível para compra.

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Pacote do Adobe Workfront</p> </td> 
   <td> 
   <p>Adobe Workfront Ultimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Licença do Adobe Workfront</td>
 <td>
 <p>Colaborador ou superior</p>
<p>Solicitação ou superior</p></td>
 </tr>
  <tr>
 <td role="rowheader">Configuração do nível de acesso</td>
 <td> <p>Editar acesso às Metas</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Permissões de objeto</td>
 <td>
  <div>
  <p>Exibir permissões ou mais altas para a meta para exibi-la</p>
  <p>Gerenciar permissões para a meta para editá-la</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Todos os usuários, incluindo Administradores do sistema, devem receber um modelo de layout que inclua a área Metas no Menu principal. </p>  
</td>
  </tr>
</tbody>
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader"><p>Access level</p></td>
 <td> <p>Edit access to Goals</p>  </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## Pré-requisitos

Você deve ter o seguinte antes de iniciar:

* Um Modelo de layout que inclui a área Metas no Menu principal.
* Uma meta existente.

  Para obter informações sobre como criar metas, consulte [Criar metas nas Metas do Adobe Workfront](../../workfront-goals/goal-management/create-goals.md).

>[!IMPORTANT]
>Uma meta não pode ter mais de 1.000 atividades, resultados, projetos ou metas alinhadas.

## Adicionar um resultado a uma meta

<!--

Adding results to goals differs depending on which environment you use.

### Add a result to a goal in the Production environment

1. Go to the goal for which you want to add a result and click the name to open the **Goal Details** panel.
1. Click **Add results**.

   ![Add result inside goal](assets/add-result-inside-goal-details-highlighted-350x145.png)

1. Start typing the result you want to achieve in the **Result** field. This is the name of the result and it displays wherever the goal displays. 
1. (Optional) If you want to set the Result Owner as someone other than yourself, click your name in the **Owner** field and start typing the name of the user that you want to assign as the owner of the result, then click it when it appears in the drop-down list.

   >[!NOTE]
   >
   >You cannot assign a team or group as a result owner.

1. In the Value drop-down menu, select the type of value that you want to measure your success by.

   ![Results value](assets/results-value-initial-target-boxes-350x49.png)

   Select from the following options:

   |Option|Value type|
   |---|---|
   | # |Number value |
   | % |Percentage value |
   |$, CN¥, DKK, KR, Mex$, R, R$, zł, £ , ¥ , &euro; , ₹, ฿, MYR, ₪  |Currency values |

   For example, if you want to increase profit to 8%, and profit is currently at 4%, you can select % as the Measured Value.

   >[!TIP]
   >
   >The result Type is always Metric and cannot be edited.

1. In the Initial field, indicate the value that the result has in the beginning, before any progress on it has been recorded. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 4 as the Starting At value. 
1. In the Target field, indicate the value that the result aims to achieve. For example, if you want to increase profit to 8%, and profit is currently at 4%, you can enter 8 as the Ending At value.
1. Click **Save**.

   The result is saved for the selected goal. The progress of the goal automatically updates when you update the progress of a result.

-->

1. Clique no ![ícone do Menu Principal](assets/main-menu-icon.png) e depois em **Metas**.

1. Na **Lista de Metas**, clique no nome de uma meta para abrir a página de metas.
1. Clique em **Indicadores de progresso** no painel esquerdo.
1. Expanda o menu suspenso **Novo indicador de progresso** e clique em **Criar resultado**.

   A caixa Novo resultado é aberta.

   ![Nova caixa de resultados](assets/new-result-box-unshimmed.png)

1. Insira um nome para o resultado no campo **Nome do resultado**. Este campo é obrigatório.
1. (Opcional) Remova seu nome do campo **Proprietário do resultado** se desejar atribuir o resultado a outro usuário. Por padrão, você é o proprietário de uma atividade criada.

   >[!NOTE]
   >
   >Não é possível atribuir uma equipe, grupo ou empresa como proprietário do resultado.

1. Na **Como você deseja medir o resultado?área**, especifique as seguintes informações:
   * **Tipo de valor**: isso indica como você deseja medir o progresso no resultado. Você pode medir o progresso numericamente, com um valor percentual ou usando um valor de moeda.

     Selecione um tipo de valor nas opções listadas na tabela a seguir:

     | Tipo de valor | Descrição |
     |---------------------------------------------------------|------------------|
     | Número | Valor numérico |
     | % | Valor percentual |
     | CN¥,DKK,KR,Mex$, R, R$, zł, £ , ¥ , € , Rt, ฿, MYR, Novo, $ | Valores de moeda |

   * **Valor Inicial**: o valor que o resultado tem no início, antes que qualquer progresso tenha sido registrado.
   * **Valor de Destino**: o valor que o resultado pretende atingir quando é considerado concluído.
1. Clique em **Criar resultado**.

   O resultado é exibido na seção Indicadores de progresso da página de meta, no Agrupamento de resultados.

   Após ativar a meta, o progresso da meta é atualizado automaticamente ao atualizar o progresso de um resultado. Para obter informações sobre como ativar uma meta, consulte [Ativar metas no Adobe Workfront Goals](../goal-management/activate-goals.md).
