---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Incorporar uma fila de solicitações em um painel
description: Você pode incorporar uma nova fila de solicitações em um painel para fornecer acesso direto à fila de solicitações aos usuários, sem ter que acessar a área Solicitações.
author: Courtney
feature: Reports and Dashboards
exl-id: 2d129095-c7ee-45b1-94ce-055d1d91e2fe
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1143'
ht-degree: 6%

---

# Incorporar uma fila de solicitações em um painel

<!-- Audited: 1/2025 -->

Você pode incorporar uma nova fila de solicitações em um painel para fornecer acesso direto à fila de solicitações aos usuários, sem ter que acessar a área Solicitações.

Por exemplo, se você tiver uma fila de solicitações aberta para toda a organização, como uma fila de Help Desk ou uma fila de solicitações PTO que todos devem acessar regularmente, pode ser conveniente inserir a fila de solicitações diretamente em um de seus painéis para acesso rápido e fácil. O processo de configuração é semelhante ao de criar uma página externa em um painel.

Primeiro, você precisa obter um URL para a fila de solicitações. Em segundo lugar, você pode incorporar o URL a um painel adicionando uma página externa.

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
   <td> 
      <p>Padrão</p>
      <p>Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para o painel</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


+++

## Pré-requisitos

Ambas as opções a seguir devem ser criadas antes que você possa incorporar uma fila de solicitações em um painel:

* **O painel**: para obter informações sobre como criar painéis, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

* **A fila de solicitações**: para obter informações sobre como criar filas de solicitações, consulte [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)

## Obter o URL da fila de solicitações {#obtain-the-url-of-the-request-queue}

Você pode obter o URL de uma fila de solicitações de várias maneiras, dependendo de qual parte da fila de solicitações você deseja expor aos usuários quando eles acessam-na de um painel.

* [Obter um link para um tópico de fila específico com capacidade para alterar o tipo de solicitação](#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type)

* [Obter um link para uma fila de solicitações e capacidade de alterar o tipo de solicitação](#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type)

* [Obter um link para uma fila de solicitações sem capacidade de alterar o tipo de solicitação](#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type)

### Obter um link para um tópico de fila específico com capacidade de alterar o tipo de solicitação {#obtain-a-link-to-a-specific-queue-topic-with-ability-to-change-the-request-type}

Quando você compartilha um link para um tópico de fila específico com outros usuários, o formulário de solicitação é aberto no tópico de fila exato que eles precisam usar para enviar a solicitação. Isso é útil quando os usuários podem não ter certeza de qual tópico de fila escolher ao registrar solicitações para uma fila de solicitações específica.

Os usuários podem alterar o tipo de solicitação ou escolher outro tópico se precisarem. A navegação da área Solicitações também é exibida.

1. Clique no **Menu Principal** > **Solicitações** > **Nova Solicitação**.
1. Continue selecionando grupos de tópicos e tópicos de fila até chegar à fila que deseja compartilhar no painel, se desejar compartilhar uma fila específica. Para obter informações sobre como enviar solicitações, consulte [Criar e enviar solicitações do Adobe Workfront](../../../manage-work/requests/create-requests/create-submit-requests.md).

   >[!TIP]
   >
   >A seleção de grupos de tópicos e tópicos de filas é opcional.

1. Clique em **Caminho de compartilhamento** no canto superior direito da área Nova solicitação.

   Isso copia o link para a fila de solicitação ou para o tópico da fila conforme você o exibe na tela. Os usuários podem atualizar o Tipo de solicitação ou qualquer um dos grupos de tópicos e tópicos da fila disponíveis.

   ![Fila de solicitações com caminho de compartilhamento](assets/share-request-queue-with-share-path-link-embedded-in-dashboard-nwe-350x116.png)

### Obter um link para uma fila de solicitações e capacidade de alterar o tipo de solicitação {#obtain-a-link-to-a-request-queue-and-ability-to-change-the-request-type}

Quando você compartilha um link para um tipo de solicitação, o tipo de solicitação é selecionado para o usuário. Isso é útil quando os usuários precisam escolher entre vários grupos de tópicos ou tópicos de fila para o mesmo tipo de solicitação. Os usuários podem alterar o tipo de solicitação e escolher outro. A navegação da área Solicitações também é exibida.

1. Vá para um projeto designado como uma fila de solicitações.

   Para obter informações sobre como criar uma fila de solicitações a partir de um projeto, vá para [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vá para **Detalhes da Fila**.
1. Copie o código encontrado no campo **URL de Acesso Direto**.

   O código deve ser semelhante ao seguinte:

   `https://<yourdomain>.my.workfront.com/requests/new?activeTab=tab-new-helpRequest&projectID=50062d6f000849c95ab3513c0e84a51e&path=`

   Este é o link para a fila de solicitações associada ao projeto selecionado. O Tipo de solicitação é pré-selecionado.

   Os usuários podem selecionar qualquer grupo de tópicos ou tópico de fila de que precisem ou podem escolher outro tipo de solicitação.

   ![URL da fila de solicitações](assets/share-request-queue-with-direct-url-embedded-in-dashboard-nwe-350x118.png)

### Obter um link para uma fila de solicitações sem capacidade de alterar o tipo de solicitação {#obtain-a-link-to-a-request-queue-with-no-ability-to-change-the-request-type}

Quando você compartilha um link para um tipo de solicitação pré-selecionado, o tipo de solicitação é selecionado para o usuário e não pode ser alterado (ele fica esmaecido). Os usuários podem escolher os grupos de tópicos ou tópicos de fila de que precisam. Isso é útil quando você não deseja que os usuários exibam e selecionem outros tipos de solicitação. A navegação da área Solicitações não é exibida.

1. Vá para um projeto designado como uma fila de solicitações.

   Para obter informações sobre como criar uma fila de solicitações a partir de um projeto, vá para [Criar uma Fila de Solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

1. Vá para **Detalhes da Fila**.
1. Copie o código encontrado no campo **Código incorporado**.

   O código deve ser semelhante ao seguinte:

   `<iframe src="https://<yourdomain>my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71" frameborder="0" width="500" height="600"></iframe>`

1. Edite o código para preservar apenas as informações abaixo:

   `https://<yourdomain>.my.workfront.com/requests/newRequestEmbedded?projectID=612518c7000404462d3bc9a0bc09fa71`

   >[!TIP]
   >
   >Você pode adicionar uma tag `<samp>iframe </samp>` ao incorporar o código em um aplicativo diferente do Workfront.

   Este é o link para a fila de solicitações associada ao projeto selecionado. O Tipo de Solicitação é pré-selecionado e não pode ser alterado.

   Os usuários podem selecionar qualquer grupo de tópicos ou tópico de fila necessário para o tipo de solicitação selecionado. Os usuários não podem selecionar outro tipo de solicitação.

   ![Solicitar código de fila](assets/share-request-queue-with-embedded-code-embedded-in-dashboard-nwe-350x210.png)

## Incorporar uma fila de solicitações em um painel

Você pode incorporar um link para a fila de solicitações ou para um tópico de fila aninhado em uma fila de solicitações em um painel para fornecer aos usuários acesso direto às solicitações de inserção.

1. Obtenha uma URL da fila de solicitações usando um dos métodos descritos na seção [Obter a URL da fila de solicitações](#obtain-the-url-of-the-request-queue) deste artigo.

1. Clique no **Menu Principal** > **Painéis** > **Novo Painel**.

1. Digite um **Nome** para o painel. Este campo é obrigatório.

1. Clique em **Adicionar Página Externa**.

   ![Página externa](assets/add-external-page-highlighted---nwe-350x214.png)

1. Na caixa **Adicionar página externa**, edite os seguintes campos:

   * **Nome**: insira o nome da fila de solicitações como deseja que apareça no painel. Este campo é obrigatório.

   * **Descrição**: insira uma descrição sobre a exibição desta página externa. Esse não é um campo obrigatório e é importante apenas para fins de relatório. Ele não é exibido no painel.

   * **URL**: cole a URL obtida usando um dos métodos descritos na Etapa 1.

   * **Altura**: insira a altura da página externa. Isso define quanto espaço a página externa que contém a fila de solicitações ocupa no painel. Esse é um campo obrigatório e o valor padrão é 500.

1. Clique em **Salvar**.

1. Clique em **Salvar + Fechar**.

   A fila de solicitações é exibida no painel como um componente separado do painel.

1. (Opcional) Clique em **Ações do Painel** e depois em **Editar** para adicionar relatórios, calendários ou páginas externas adicionais ao mesmo painel.

   Para obter informações sobre como adicionar componentes a um painel, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1"> <p class="preview" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>Main Menu</strong> > Requests >&nbsp;<strong>New Request</strong>. </p> </li>
<li class="preview" value="2" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Continue entering the request.&nbsp;For information about submitting requests, see <a href="../../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Create and submit Adobe Workfront requests</a>. </p> </li>
<li value="3"> <p>Select the <strong>Request Type</strong> for the queue you would like added to the dashboard.</p> </li>
<li value="4"> <p>(Optional) Select a Queue Topic and a Topic Group. Depending on how the project manager set up the request queue, the names of these fields are different in each Workfront instance.</p> </li>
<li class="preview" value="5" data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <p>Click <strong>Share path</strong> to obtain a shared link from the request queue you want to embed on a dashboard.</p> <p>For information about sharing a request queue, see <a href="../../../manage-work/requests/create-requests/share-link-to-request-queue.md" class="MCXref xref">Share a link to a request queue</a></p> </li>
<li value="6"> <p>For example, enter a URL similar to one of the following: </p> </li>
</ol>
-->
