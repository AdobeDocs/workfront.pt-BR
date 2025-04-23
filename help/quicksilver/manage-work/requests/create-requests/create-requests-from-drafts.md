---
product-area: requests
navigation-topic: create-requests
title: Criar solicitações a partir de rascunhos
description: Além de usar os rascunhos disponíveis que o Workfront sugere quando você informa uma nova solicitação, também é possível acessar um rascunho de solicitação na seção Rascunhos e finalizar a submissão a partir daí.
author: Alina
feature: Work Management
exl-id: 664004e7-04c8-4a1f-b682-7b82d349643d
source-git-commit: 6311526ddf9143c4a979d8bbac96312a3b0e8151
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 1%

---

# Criar solicitações a partir de rascunhos

Além de usar os rascunhos disponíveis que o Workfront sugere quando você informa uma nova solicitação, também é possível acessar um rascunho de solicitação na seção Rascunhos e finalizar a submissão a partir daí.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Colaborador ou superior</p>
   Ou
   <p>Atual: solicitação ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos para criar solicitações a partir de rascunhos

Você deve fazer o seguinte antes de criar uma solicitação a partir de um rascunho: 

* Comece a criar uma solicitação. Isso salva a solicitação como rascunho automaticamente na seção Rascunhos.

  Para obter informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Criar solicitações a partir de rascunhos

{{step1-to-requests}}

1. Selecione **Rascunhos** no painel esquerdo.

   Um rascunho para cada tópico da fila de cada fila de solicitações é exibido nesta lista.

   ![](assets/nwe-drafts-section-with-list-of-drafts-350x169.png)

1. (Opcional) Clique em um cabeçalho de coluna para classificar a lista por essa coluna.

1. Revise as informações sobre cada rascunho nas seguintes colunas da lista Rascunhos:

   | Assunto | Esse é o nome que você deu à solicitação quando ela começou a ser criada. |
   |---|---|
   | Caminho | O nome da fila de solicitações, dos grupos de tópicos e dos tópicos da fila em que você originalmente pretendia submeter a solicitação. |
   | Data de Entrada | A data em que você iniciou a criação da solicitação. |
   | Última data de atualização | A última de sua última atualização. Se você não a atualizou desde que iniciou a solicitação pela primeira vez, a Data de Entrada e a Data da Última Atualização devem ser iguais. |

   {style="table-layout:auto"}

1. (Opcional) Usando o filtro rápido no canto superior direito da lista Rascunhos, comece digitando o nome de uma solicitação em rascunho, fila de solicitações, tópico da fila ou grupo de tópicos e, em seguida, clique no nome de um rascunho para abri-lo.

   >[!TIP]
   >
   >Não é possível aplicar filtros permanentes na seção Rascunhos da área Solicitações. Além disso, não há opções para modificar ou alterar a exibição da lista de rascunhos.

1. Atualize as informações da solicitação conforme descrito em [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).
1. (Opcional e condicional) A qualquer momento durante a inserção da solicitação, clique em **Descartar** rascunho se desejar excluir o rascunho. Isso exclui o rascunho que não pode ser recuperado. Para obter mais informações sobre como excluir rascunhos, consulte [Excluir um rascunho de solicitação](../../../manage-work/requests/create-requests/delete-request-draft.md).

1. (Opcional) Clique em **Cancelar** no canto inferior esquerdo da página se desejar reverter sua ação e manter o rascunho.

1. Após concluir as informações da solicitação, siga um destes procedimentos:

   * Clique em **Enviar** se estiver pronto para enviar a solicitação. A solicitação é salva na seção Enviada. Dependendo da Regra de Encaminhamento da Fila de Solicitações, essa solicitação pode ser encaminhada para um projeto diferente daquele designado como Fila de Solicitações. Para obter informações sobre regras de roteamento, consulte [Criar Regras de Roteamento](../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md).

     Ou

     Clique em **Fechar** se não estiver pronto para enviá-lo e você poderá voltar e concluí-lo mais tarde. Sua solicitação é salva na seção Rascunhos e estará disponível para você na próxima vez que enviar uma solicitação para essa fila de solicitações.

     ![](assets/nwe-submit-close-discard-draft-buttons-on-new-request-350x340.png)

     Quando você envia a solicitação, o rascunho é excluído e não pode ser restaurado.
