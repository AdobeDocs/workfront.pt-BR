---
title: Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning
description: Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/E9LEGJ8T822JuvIO3s8nn6UkLbX-j4ffwaKSviKxl0o
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: e147ce9d-7675-49bd-8a32-44f27d865560
    internal-label: Get started
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 3b3d455ded251b06084249cf9df12c1f112f05e9
workflow-type: tm+mt
source-wordcount: '1171'
ht-degree: 2%
---
# Adicionar uma aprovação a um formulário de solicitação no Planejamento do Adobe Workfront

<!--update the metadata with real information when making this available in TOC and in the left nav-->


<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Após o lançamento para Pré-visualização, os mesmos recursos também estarão disponíveis mensalmente no ambiente de Produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.

<!--<span class="preview">Multiple stages are supported in the approval process. When all required decisions in a stage are made, the next stage begins and the new stage's approvers receive an email notification.</span>-->

Este artigo descreve como um gerente de espaço de trabalho pode adicionar uma aprovação a um formulário de solicitação associado a um tipo de registro.

Para obter informações sobre como criar um formulário de solicitação no Workfront Planning, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Para obter informações sobre como enviar uma solicitação a um tipo de registro para criar um registro, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p></li>
Ou
<li><p>Qualquer pacote do Planning quando adquirido como um produto independente</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>licença do Adobe Planning</p></td> 
   <td><p>Planejamento padrão</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Você deve adicionar um Workflow e um tipo de licença do Planning ao nível de acesso quando tiver um Workflow e um pacote do Planning</p>   
</td> 
  </tr>  
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e tipo de registro</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre a adição de aprovações a um formulário de solicitação

* Você pode adicionar um ou vários aprovadores (usuários ou equipes) a um formulário de solicitação ou a uma regra de aprovação.
* As regras de aprovação roteiam solicitações com base em valores de campo na solicitação enviada (por exemplo, aprovadores diferentes para valores diferentes de um campo &quot;Tipo de campanha&quot;).
* É possível exibir informações de aprovação no registro criado por meio dos campos Approved by e Approved date. Consulte Criar campos.
* Se todos os aprovadores aprovarem, um registro será criado para o tipo de registro associado ao formulário de solicitação.
* Se pelo menos um aprovador for rejeitado, nenhum registro será criado para o tipo de registro; em vez disso, a solicitação permanecerá/chegará à área Solicitações do Workfront. (Esse ponto aparece em ambas as seções com textos ligeiramente diferentes — mesclados aqui como uma declaração.)
* Quando vários aprovadores são necessários, todos eles devem tomar uma decisão antes que a solicitação seja aprovada ou rejeitada, a menos que a opção Only one decision is required esteja habilitada.
* Se uma equipe for definida como um aprovador, somente uma decisão será necessária de um membro dessa equipe.
* As aprovações são opcionais — se um formulário de solicitação não tiver nenhuma aprovação anexada, o Workfront Planning criará o registro imediatamente após a submissão.
* <span class="preview">Você pode adicionar um ou mais estágios às aprovações.</span>

## Adicionar regras de aprovação a um formulário de solicitação

As regras de aprovação definem o processo de aprovação com base nos valores dos campos nas solicitações enviadas.

Por exemplo, se um formulário de solicitação tiver o campo &quot;Tipo de campanha&quot;, poderá ser criada uma regra que envia a solicitação para uma pessoa quando o campo tem o valor &quot;Digital&quot; e outra pessoa quando ele tem o valor &quot;Imprimir&quot;.

Para definir regras de aprovação para um formulário de solicitação:

1. Comece a criar um formulário de solicitação para um tipo de registro, conforme descrito no artigo [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Quando o formulário de solicitação for aberto, clique em **Configurações**.

   A guia **Configurações** é aberta.

1. Para começar a configurar as regras de aprovação, clique em **Aprovações** ![ícone Aprovações](assets/approvals-icon-on-form.png) no painel esquerdo.

1. (Opcional) Se quiser definir um processo de aprovação padrão, adicione pelo menos um usuário ou equipe ao campo **Aprovadores** da área **Regra de aprovação padrão** e clique na caixa de seleção **Somente uma decisão é necessária** se quiser que o registro seja criado depois que qualquer um dos aprovadores padrão o aprovar.

   ![Área de regra de aprovação padrão](assets/default-approvers.png)

1. (Opcional) Comece a adicionar regras de aprovação. Para cada regra de aprovação personalizada, faça o seguinte:

   1. Clique em **Adicionar regra de aprovação**.
   1. Clique no título do espaço reservado **Regra de aprovação sem título** e insira um nome para a regra de aprovação.
   1. Clique em **Selecionar um campo** e selecione o campo que ativa a regra.
   1. Selecione o operador para a regra. Os operadores variam de acordo com o tipo de campo.
   1. Se o operador selecionado exigir um valor, clique no ícone de adição e adicione um ou mais valores.
   1. (Opcional) Clique em **Adicionar condição** para adicionar mais condições e conectá-las por instruções **And** ou **Or** configurando as condições adicionais como nas etapas C-E.
   1. Na área **Ações** da regra de aprovação, no campo **Aprovadores**, adicione pelo menos um usuário ou equipe a ser definido como aprovador quando a condição for atendida.
   1. (Condicional e opcional) Se quiser que o registro seja criado depois que qualquer um dos aprovadores o aprovar, marque a caixa de seleção **Somente uma decisão é necessária**. Caso contrário, todos os aprovadores devem decidir sobre a aprovação antes que a solicitação seja aceita ou rejeitada.

   >[!NOTE]
   >
   >   Considere o seguinte ao adicionar regras de aprovação:
   >
   >   * Se apenas uma regra padrão estiver configurada, ela se aplica a todas as solicitações enviadas.
   >   * Se uma regra personalizada for atendida, o padrão não será aplicado ao fluxo de trabalho de solicitação de aprovação. Somente as regras personalizadas correspondentes se aplicam às aprovações e a regra padrão é ignorada.
   >   * Se várias regras personalizadas forem atendidas, a primeira regra na ordem será aplicada. Nesse caso, a aprovação padrão não se aplica, se houver.

1. <span class="preview">(Opcional) Clique em **Adicionar estágio** para adicionar outro estágio à aprovação.</span>

1. Clique em **Salvar** para salvar as regras de aprovação.

1. <span class="preview">(Opcional) Para adicionar mais estágios à aprovação, faça o seguinte:</span>

   1. <span class="preview">Clique em **Adicionar estágio**.</span>

      <span class="preview">A caixa **Aprovação de vários estágios** é exibida. Se você já criou uma ação de aprovação padrão, esses aprovadores serão adicionados automaticamente ao Estágio 1.</span>

   1. <span class="preview">No campo **Adicionar pessoas ou equipes**, adicione pelo menos um usuário ou equipe a ser definido como aprovador para o estágio.</span>
   1. <span class="preview">(Condicional e opcional) Se quiser que o registro avance para o próximo estágio depois que qualquer um dos aprovadores o aprovar, marque a caixa de seleção **Somente uma decisão é necessária**. Caso contrário, todos os aprovadores devem decidir sobre a aprovação antes que a solicitação seja movida para o próximo estágio.</span>
   1. <span class="preview">Clique em **Adicionar estágio** e repita da etapa B para adicionar mais estágios à aprovação.</span>

      <span class="preview">Quando existirem dois ou mais estágios, você poderá clicar no ícone **Arrastar** ![Ícone Arrastar](assets/drag-icon.png) para arrastá-los e soltá-los em ordem.</span>

      <span class="preview">Clique em **Excluir este estágio** para excluir um estágio da aprovação ou clique no **ícone Excluir** ![ícone Excluir](assets/delete.png) ao lado de um aprovador para excluir o usuário ou a equipe da lista de aprovadores em um estágio.</span>

      ![Caixa de aprovação de vários estágios](assets/planning-request-multi-stage-approval-box.png)

   1. <span class="preview">Quando terminar de criar o fluxo de trabalho de aprovação, clique em **Salvar**.</span>

      <span class="preview">Você pode editar ou excluir a aprovação de vários estágios da página Aprovações.</span>

1. (Opcional) Clique em **Publicar** se você nunca compartilhou o formulário de solicitação antes.



<!--

## Add an approval to a request form in the Production environment

1. Start creating a request form for a record type, as described in [Create and manage a request form in Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Click **Configuration**.

    The **Configuration** area displays.

    ![Configuration tab](assets/configuration-tab.png)
1. In the **Approvers** field, start typing the name of a user or team that you want to set as an approver, then select it when it displays in the list. 
1. (Optional and conditional) If you have set more than one approver, and only need one approver to make a decision, enable the **Only one decision is required** option.

    (****most of the Note below is duplicated in the Create a request form article***)

      >[!NOTE]
      >
      >
      >* You can add one or several approvers to a request form.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must approve the request before Workfront Planning creates a record.
      >
      >* If at least one approver rejects the request, the request is rejected and the record is not created. The request remains in the Requests area of Workfront.
      >
      >* If you add more than one approver, and the Only one decision is required option is not enabled, all approvers must make a decision before a request is either approved or rejected.
      >
      >* If a team is set as an approver, only one decision is required from the team.


1. (Optional) Click **Publish** if you have never shared the request form before.

    Or

    Click **Share** to share the form, then **Copy link**. 
1. (Optional) After a user uses the link you share and submits a request, Workfront Planning sends an approval in-app notification and an email to the approvers.

   For information about approving requests, see [Approve a request](/help/quicksilver/planning/requests/approve-request.md).

-->