---
product-area: requests
navigation-topic: create-requests
title: Excluir uma solicitação enviada ou um rascunho de solicitação
description: Você pode excluir solicitações enviadas ou solicitar rascunhos no Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9098ada7-0e6b-4de2-97ad-5c6e590fbba3
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 9%

---

# Excluir uma solicitação enviada ou um rascunho de solicitação

É possível excluir solicitações enviadas do Adobe Workfront ou do Adobe Workfront Planning ou solicitar rascunhos criados por você ou para os quais você tenha permissões de gerenciamento.

Os administradores do Workfront e os gerentes de espaço de trabalho do Workfront Planning também podem excluir solicitações e solicitar rascunhos que não tenham sido criados.

Não é possível exibir solicitações do Planning na experiência de solicitação herdada.

Este artigo descreve como você pode excluir rascunhos de solicitações na nova experiência de solicitação. A exclusão de solicitações do Workfront e do Planning ou de seus rascunhos é idêntica.

Para obter mais informações, consulte:

* [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md)
* [Criar solicitações a partir de rascunhos](../../../manage-work/requests/create-requests/create-requests-from-drafts.md)
* [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer pacote do Workfront ou Workflow</p>

<p>Qualquer pacote do Workfront Planning para gerenciar solicitações do Planning </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Colaborador ou posterior</p>
   <p>Solicitação ou posterior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront ou um gerenciador de espaço de trabalho do Planning para deletar solicitações que não foram criadas.</p><p>Você deve ter acesso para editar ocorrências.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Você deve ter criado a solicitação ou rascunho para deletá-lo na nova experiência de solicitação ou ser um administrador do Workfront ou gerente do espaço de trabalho do Planning para deletar rascunhos de solicitações que não foram submetidas.
   </p><p>Você deve ter permissões para editar os problemas que estão sendo excluídos.</p>  </td> 
  </tr>

</tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir solicitações ou solicitar rascunhos na nova experiência de solicitação

É possível excluir solicitações e rascunhos nas seguintes áreas:

* Na área Solicitações do Workfront
* No widget Minhas solicitações na página inicial
* De uma página de solicitação

Os seguintes usuários podem excluir rascunhos de solicitações:

* Os administradores do Workfront podem excluir solicitações e rascunhos enviados por eles ou outras pessoas.
* Os gerentes de espaço de trabalho do Workfront Planning podem deletar solicitações e rascunhos no espaço de trabalho do Planning que administram.
* Os usuários podem excluir solicitações e rascunhos enviados.

### Excluir uma solicitação ou um rascunho da área Solicitações ou do widget Minhas solicitações na Página inicial

{{step1-to-requests}}

1. Para acessar o widget **Minhas solicitações** na **Página inicial**:

   {{step1-to-home}}

   1. Localize o widget **Minhas solicitações**.

      Para obter mais informações sobre o widget **Minhas solicitações**, consulte [Usar o widget Minhas solicitações](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Na lista **Solicitações** ou no widget **Minhas Solicitações** na **Página Inicial**, passe o mouse sobre a solicitação ou rascunho que deseja excluir e clique no menu **Mais** ![Mais menu](assets/more-menu.png)

1. Clique em **Excluir**

   Ou

   Clique com o botão direito do mouse na solicitação selecionada e clique em **Excluir**.

   >[!TIP]
   >
   >Quando você não tem acesso para criar problemas, você recebe um aviso de que o administrador restringiu você de criar solicitações.

1. Na caixa de diálogo que é aberta, clique em **Excluir**.

   A solicitação ou o rascunho é excluído.

   As solicitações excluídas são salvas na Lixeira e um administrador do Workfront pode recuperá-las por até 30 dias. Os rascunhos não podem ser recuperados.

### Solicitações de exclusão em massa de uma lista

{{step1-to-requests}}

1. Para acessar o widget **Minhas solicitações** na **Página inicial**:

   {{step1-to-home}}

   1. Localize o widget **Minhas solicitações**.

      Para obter mais informações sobre o widget Minhas solicitações, consulte [Usar o widget Minhas solicitações](/help/quicksilver/workfront-basics/using-home/using-the-home-area/my-requests-widget.md).

1. Na lista **Solicitações** ou no widget **Minhas solicitações**, clique na caixa à esquerda de cada solicitação que você deseja excluir.
1. Na barra azul na parte inferior da página, clique em **Excluir**.

   >[!NOTE]
   >
   >Se a opção **Excluir** não estiver visível na barra azul, você não terá permissão para excluir uma ou mais das solicitações selecionadas.

### Pré-requisitos para excluir rascunhos de solicitações

Você deve fazer o seguinte antes de excluir um rascunho de solicitação:

* Comece a criar uma solicitação. Isso salva a solicitação como rascunho automaticamente na seção Rascunhos.

  Para obter informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

## Excluir rascunhos de solicitação na experiência de solicitação herdada

Você poderá excluir solicitações em rascunho depois que elas forem salvas como rascunhos, se não forem mais relevantes. Não é possível recuperar solicitações de rascunho excluídas.

Não é possível acessar solicitações do Planning ou seus rascunhos da experiência de solicitação herdada.

{{step1-to-requests}}

1. Clique em **Rascunhos** no painel esquerdo.

   Todos os rascunhos de todas as filas de solicitações são exibidos nesta lista.

1. Selecione um rascunho na lista e clique em **Excluir** na parte superior da lista.
1. Clique em **Sim, exclua**.

   O rascunho foi excluído e não pode ser recuperado.






