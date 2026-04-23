---
title: Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning
description: Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '929'
ht-degree: 3%

---

# Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.

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
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e qualquer pacote do Planning</p>
Ou
<p>Qualquer pacote de fluxo de trabalho e qualquer pacote de planejamento</p>

<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p> 
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

* Você pode adicionar um ou vários aprovadores a um formulário de solicitação. Você pode adicionar usuários e equipes como aprovadores.
* Você pode exibir informações de aprovação em um registro criado submetendo um formulário de solicitação nos campos Aprovado por e Data de aprovação. Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).
* Quando você adiciona vários aprovadores a um formulário de solicitação, todos os aprovadores devem aceitar a solicitação antes que um registro seja criado no Workfront Planning.
* Se todos os aprovadores aprovarem a solicitação, um registro será criado para o tipo de registro associado ao formulário de solicitação.
* Se pelo menos um aprovador rejeitar a solicitação e todos os outros aprovarem, uma solicitação será criada para a área Solicitações no Workfront, mas nenhum registro será criado para o tipo de registro associado ao formulário de solicitação.
* Adicionar aprovações a um formulário de solicitação é opcional. O Workfront Planning cria imediatamente um registro quando uma solicitação é submetida, se o form de solicitação não estiver associado a uma aprovação.

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

## Adicionar regras de aprovação a um formulário de solicitação

As regras de aprovação definem o processo de aprovação com base nos valores dos campos nas solicitações enviadas.

Por exemplo, se um formulário de solicitação tiver o campo &quot;Tipo de campanha&quot;, poderá ser criada uma regra que envia a solicitação para uma pessoa quando o campo tem o valor &quot;Digital&quot; e outra pessoa quando ele tem o valor &quot;Imprimir&quot;.

Considere o seguinte ao adicionar regras de aprovação:

* Você pode adicionar um ou vários aprovadores a uma regra de aprovação.
* Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o registro não será criado. A solicitação permanece na área Solicitações do Workfront.
* Se você adicionar mais de um aprovador e a opção Somente uma decisão é obrigatória não estiver ativada, todos os aprovadores deverão tomar uma decisão antes que uma solicitação seja aprovada ou rejeitada.
* Se uma equipe for definida como um aprovador, somente uma decisão será necessária para um membro da equipe.

Para definir regras de aprovação para um formulário de solicitação:

1. Comece a criar um formulário de solicitação para um tipo de registro, conforme descrito no artigo [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Quando o formulário de solicitação for aberto, clique em **Configurações**.

   A guia **Configurações** é aberta.

1. Para começar a configurar as regras de aprovação, clique em **Aprovações** ![ícone Aprovações](assets/approvals-icon-on-form.png) no painel esquerdo.

1. (Opcional) Se quiser definir um processo de aprovação padrão, adicione pelo menos um usuário ou equipe ao campo **Aprovadores** da área **Regra de aprovação padrão** e clique na caixa de seleção **Somente uma decisão é necessária** se quiser que o registro seja criado depois que qualquer um dos aprovadores padrão o aprovar.

   ![Área de regra de aprovação padrão](assets/default-approvers.png)

1. (Opcional) Comece a adicionar regras de aprovação. Para cada regra de aprovação personalizada, faça o seguinte:

   1. Clique em **Adicionar regra de aprovação**
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

1. Clique em **Salvar** para salvar as regras de aprovação.
1. (Opcional) Clique em **Publicar** se você nunca compartilhou o formulário de solicitação antes.
