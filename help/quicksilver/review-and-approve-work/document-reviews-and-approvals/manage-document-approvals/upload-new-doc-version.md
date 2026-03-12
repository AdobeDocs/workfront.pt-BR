---
product-area: documents
navigation-topic: approvals
title: Fazer upload de uma nova versão do documento e solicitar uma aprovação
description: Você pode fazer upload de uma nova versão do documento e solicitar aprovação de outros usuários no Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '902'
ht-degree: 7%

---

# Fazer upload de uma nova versão do documento e solicitar uma aprovação

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ele está disponível somente no ambiente de Pré-visualização da Sandbox.</span>

Se um documento estiver marcado como &quot;Precisa de trabalho&quot; em uma revisão anterior, você poderá fazer upload de uma nova versão para o documento original e iniciar outra rodada de aprovações. Após carregar uma nova versão do documento, as versões anteriores serão bloqueadas.

Se o nome do arquivo da nova versão for diferente do nome do arquivo da versão anterior, o Workfront exibirá o documento com o nome de arquivo mais recente.

Quando uma nova versão é adicionada a um documento com aprovações pendentes, a aprovação da versão anterior é exibida como &quot;Retirada&quot;. O processo de aprovação anterior é encerrado, mesmo que alguns participantes ainda não tenham tomado uma decisão.

Se a versão mais recente do documento for excluída, as versões anteriores permanecerão bloqueadas. Se precisar editar uma versão anterior, desbloqueie-a manualmente.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> <p>Solicitação ou posterior</p>
   <p>Colaborador ou posterior</p>
   <p>Se você estiver usando a integração Frame.io, é necessário ter uma licença Standard para criar workflows de aprovação.</p>
    </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar acesso ao objeto associado ao documento</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Use o arrastar e soltar para adicionar uma nova versão no ambiente de produção

>[!NOTE]
>
>Arrastar e soltar não funciona com o Internet Explorer.


Se você precisar de outra rodada de revisão e aprovação em um documento, poderá criar uma nova versão do documento no Workfront.

Você pode adicionar os participantes anteriores, novos participantes ou uma combinação de ambos. Você pode exibir informações sobre versões anteriores e participantes na página Detalhes do documento.

Para adicionar uma nova versão:

1. Navegue até o documento no Workfront.
1. Arraste e solte o novo arquivo sobre o documento anterior. Isso cria uma nova versão automaticamente.

1. Quando o documento terminar de carregar, selecione-o e clique em **Detalhes do Documento**.
   ![Abrir a página de detalhes do documento](assets/open-doc-details.png)


1. No painel esquerdo, clique em **Aprovações** e em **Adicionar**.

1. Para adicionar todos os participantes anteriores, clique em **Adicionar todos**. Você também pode adicionar novos participantes ou remover participantes anteriores, conforme necessário.


1. Para adicionar um modelo de aprovação existente, clique no botão Modelo e comece a digitar um nome de modelo.

   >[!TIP]
   >
   >   Os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis na área Configuração. Para obter mais informações, consulte [Criar um modelo de fluxo de trabalho de aprovação para documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).


1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Depois de adicionar todos os revisores e aprovadores, clique em **Enviar solicitação**. Os participantes são notificados por email.

   ![enviar nova versão para aprovação](assets/add-previous-participants.png)





<div class="preview">

## Use arrastar e soltar para adicionar uma nova versão no ambiente de visualização na área de documentos herdados

Se sua organização estiver no armazenamento da Workfront, você verá a área de documentos herdados ao acessar documentos no Workfront. Para obter mais informações sobre o armazenamento da Workfront, consulte [Armazenamento da Workfront vs. armazenamento corporativo da Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

>[!NOTE]
>
>Arrastar e soltar não funciona com o Internet Explorer.


Se você precisar de outra rodada de revisão e aprovação em um documento, poderá criar uma nova versão do documento no Workfront.

Você pode adicionar os participantes anteriores, novos participantes ou uma combinação de ambos. Você pode exibir informações sobre versões anteriores e participantes na página Detalhes do documento.

Para adicionar uma nova versão:

1. Navegue até o documento no Workfront.
1. Arraste e solte o novo arquivo sobre o documento anterior. Isso cria uma nova versão automaticamente.

1. Quando o documento terminar de ser carregado, selecione-o para abrir o painel Resumo do documento. Aqui você verá o número da versão na parte superior do painel.
   ![Abrir a página de detalhes do documento](assets/open-doc-details.png)


1. Role até a seção **Aprovações**.

1. Clique em **Criar fluxo de trabalho** e preencha os seguintes detalhes:

   <table>
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
   <td><strong>Data de vencimento (opcional)</strong></td>
   <td>Defina uma data de vencimento para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes da data de vencimento especificada.</td>
   </tr>
   </table>

1. (Opcional) Repita a etapa anterior para adicionar etapas adicionais, conforme necessário.

   >[!NOTE]
   >
   >Se você adicionar vários estágios, o workflow de aprovação continuará na ordem em que os estágios são listados. Quando todas as decisões necessárias forem tomadas, o próximo estágio será iniciado e o estágio anterior será bloqueado.



1. (Opcional) Para adicionar um modelo de aprovação existente, selecione um modelo no lado esquerdo da caixa de diálogo.

   >[!TIP]
   >
   >   Os usuários com uma licença Standard podem criar Modelos de aprovação reutilizáveis na área Configuração. Para obter mais informações, consulte [Criar um modelo de fluxo de trabalho de aprovação para documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md).



1. Depois de adicionar todos os estágios e participantes necessários, clique em **Solicitar aprovação**.

   O fluxo de trabalho de aprovação é iniciado e os aprovadores recebem uma notificação de que sua aprovação é necessária na nova versão do documento. A versão anterior do documento está bloqueada e todas as aprovações pendentes na versão anterior são retiradas.

   ![solicitar aprovação](assets/request-approval.png)
   <!--1. To add all previous participants, click **Add all**. You can also add new participants or remove previous participants as needed.-->



</div>

