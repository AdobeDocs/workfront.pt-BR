---
product-area: documents
navigation-topic: approvals
title: Criar um modelo de fluxo de trabalho de aprovação para documentos
description: Você pode criar Modelos de aprovação para simplificar seu processo de aprovação.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: c18d6c6d-1a09-47c5-af4e-027f7cc48cd7
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 11%

---

# Criar um modelo de fluxo de trabalho de aprovação para documentos

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Na área Configuração do Workfront, os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis. Depois de criados, os Modelos de aprovação podem ser aplicados a ativos na área Documentos de um projeto, tarefa ou problema.

>[!IMPORTANT]
>
>O conteúdo deste artigo se refere à funcionalidade atualizada de aprovação de documentos, disponível somente para contas específicas. Para obter informações sobre processos de aprovação padrão, consulte os artigos listados em [Aprovações de trabalho](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> 
   <p>Plano</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++




## Criar um modelo de aprovação no seu ambiente de produção

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Revisar e aprovar** > **Modelos de Aprovação**.
1. Clique em **Novo modelo** no lado direito da página.
1. Especifique as seguintes informações:

   | Nome do modelo | Comece a digitar um nome para este modelo. |
   |----------------------------|---|
   | **(Opcional) Cronograma** | Insira o período em dias. O prazo de aprovação é calculado a partir desse campo assim que o modelo é aplicado a um ativo. |
   | **Adicionar aprovadores ou revisores** | Comece a digitar o nome de usuários ou equipes e, em seguida, designe-os como revisores ou aprovadores. |

1. Clique em **Salvar**.



<div class="preview">

## Criar um modelo de aprovação no seu ambiente de visualização

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Revisar e aprovar** > **Modelos de Aprovação**.
1. Clique em **Novo modelo** no lado direito da página.

1. Preencha os seguintes detalhes:

   <table>
     <tr>
   <td><strong>Nome do modelo</strong></td>
   <td>Adicione um nome de template. </td>
   </tr>
   <tr>
   <td><strong>Nome do estágio</strong></td>
   <td>Adicione um nome de estágio. Você pode alterar o nome para algo mais descritivo, como <em>Revisão inicial</em> ou <em>Aprovação final</em>.</td>
   </tr>
   <tr>
   <td><strong>Adicionar nomes ou emails</strong></td>
   <td>Comece a digitar um nome de usuário ou de equipe para adicionar como aprovador ou revisor. Se você tiver apenas revisores, eles serão notificados e terão a opção de concluir a revisão, mas nenhuma decisão será necessária ou tomada.</td>
   </tr>
   <tr>
   <td><strong>É necessária uma decisão (opcional)</strong></td>
   <td>A primeira pessoa que toma uma decisão completa a etapa.</td>
   </tr>
   <tr>
   <td><strong>Dias úteis até a data de vencimento</strong></td>
   <td>Escolha quantos dias úteis até a aprovação vence depois que um estágio é ativado.</td>
   </tr>
   </table>

1. (Opcional) Repita a etapa anterior para adicionar etapas adicionais, conforme necessário.

   >[!NOTE]
   >
   >Se você adicionar vários estágios, o workflow de aprovação continuará na ordem em que os estágios são listados. Quando todas as decisões necessárias forem tomadas, o próximo estágio será iniciado e o estágio anterior será bloqueado.

   ![Detalhes do documento](assets/new-stage.png)

1. Clique em **Salvar**.

Depois que o modelo é criado, ele pode ser aplicado a documentos na área Documentos de um projeto, tarefa ou problema para iniciar o processo formal de revisão e aprovação no Workfront.

</div>


<!--
 Once a template is created, it can be applied to assets sent from Frame.io to begin the formal review and approval process in Workfront.
![Assign template](assets/assign-template.png)
-->
