---
product-area: projects
navigation-topic: use-the-home-area
title: Usar o widget Minhas solicitações
description: Você pode enviar solicitações no widget Minhas solicitações. Você também pode personalizar o widget com filtros e colunas.
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 2fe55f61bd24ebb3ecfe09fff29c4aad2ca33608
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 3%

---

# Usar o widget Minhas solicitações

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

>[!IMPORTANT]
>
>Este artigo descreve o novo widget Minhas solicitações. Você deve ter a nova experiência de solicitação habilitada para ver o novo widget.
>&#x200B;>Você pode ativar a nova experiência de solicitação na área Solicitações.

O widget Minhas solicitações exibe solicitações que foram enviadas para sua organização. Você pode filtrar as solicitações, pesquisar solicitações específicas ou ajustar a ordem e a visibilidade da coluna. Você também pode criar uma nova solicitação no widget Minhas solicitações.

>[!NOTE]
>
>* Quando o widget Minhas solicitações é carregado, ele exibe até 50 solicitações. Para exibir mais solicitações, role para baixo na lista.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Product]</strong></td> 
   <td> <ul><li>Adobe Workfront</li><li>Você precisa ter o Adobe Workfront Planning para exibir solicitações ou formulários de solicitação do Planning</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>Novo: Colaborador ou superior</p>
   Ou   
   <p>Atual: [!UICONTROL Request] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuração do nível de acesso</strong></td> 
   <td> <p>Acesso de visualização ou superior a qualquer objeto para o qual você esteja marcado em uma conversa ou precise resolver uma aprovação (Projetos, Tarefas, Problemas, Documentos)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Permissões [!UICONTROL View] ou superior para projetos, tarefas, problemas, documentos nos quais você está marcado em uma conversa ou precisa resolver uma aprovação</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront]. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar uma solicitação

Você pode criar uma solicitação diretamente do widget Minhas solicitações.

Para obter instruções, consulte [Criar uma solicitação](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) no artigo Criar itens de trabalho e projetos da área Página inicial.

## Filtrar solicitações

O widget Minhas solicitações apresenta um filtro personalizável que permite controlar quais solicitações aparecem no widget. Você pode configurar esse filtro para diferentes campos e valores e pode empilhar condições usando AND e OR.

Para configurar o filtro no widget Minhas solicitações:

1. Clique no **[!UICONTROL Menu Principal]** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **[!UICONTROL Página Inicial]**.
1. (Condicional) Para adicionar o widget **Minhas solicitações** à sua tela inicial. Clique em **Personalizar** e localize **Minhas Solicitações**.
1. No widget Minhas solicitações, clique em **Filtro**.
1. No campo mais à esquerda, selecione pelo qual deseja filtrar. As opções disponíveis são:

   * Espaço de trabalho
   * Tipo de objeto
   * Data de entrada
   * Formulário de solicitação
   * Status
   * Inserido por

1. No campo seguinte, selecione o operador que deseja usar para essa condição de filtro. Os operadores disponíveis dependem do campo escolhido.
1. (Condicional) Se um campo aparecer à direita do operador, selecione o valor pelo qual deseja filtrar.
1. (Opcional) Para adicionar outra condição de filtro, clique em **Adicionar condição** e repita as etapas 4 a 6.
1. (Opcional e condicional) Se você tiver várias condições, alterne o valor And ou Or clicando em **And** ou **Or** à esquerda da condição.

O filtro é salvo automaticamente.

>[!TIP]
>
>Se sua organização tiver comprado o Workfront Planning, o widget Minhas solicitações incluirá as solicitações do Workfront e do Workfront Planning.
> 
>* Para filtrar apenas por solicitações Workfront, defina o filtro como **Tipo de objeto** > **Tem qualquer um dos** > **Problemas**.
>* Para filtrar apenas por solicitações do Workfront Planning, defina o filtro como **Tipo de objeto** > **Não tem nenhum de** > **Problemas**.

## Ajustar colunas

Você pode escolher quais das colunas disponíveis aparecem no widget Minhas solicitações e definir sua ordem.

As colunas disponíveis incluem:

* Assunto
* Objeto criado
* Tipo de objeto
* Status
* Formulário de solicitação
* Data de entrada
* Inserido por

Para ajustar as colunas no widget Minhas solicitações:

1. Clique no **[!UICONTROL Menu Principal]** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **[!UICONTROL Página Inicial]**.
1. (Condicional) Para adicionar o widget **Minhas solicitações** à sua tela inicial. Clique em **Personalizar** e localize **Minhas Solicitações**.
1. No widget Minhas solicitações, clique em **Colunas**.
1. (Opcional) Para reordenar colunas, clique na alça de arrastar ![alça de arrastar](assets/drag-handle.png) da coluna que você deseja mover e arraste-a para os locais desejados. A coluna na parte superior da lista aparece no widget Minhas solicitações como a coluna mais à esquerda.
1. (Opcional) Use o botão para controlar se uma coluna é exibida no widget Minhas solicitações.

As preferências de coluna são salvas automaticamente.

## Pesquisar solicitações

Para pesquisar solicitações específicas no widget Minhas solicitações:

1. Clique no **[!UICONTROL Menu Principal]** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **[!UICONTROL Página Inicial]**.
1. (Condicional) Para adicionar o widget **Minhas solicitações** à sua tela inicial. Clique em **Personalizar** e localize **Minhas Solicitações**.
1. Na barra de pesquisa próxima ao canto superior direito do widget Minhas solicitações, digite o termo que você deseja pesquisar.

   As solicitações que contêm o termo são realçadas em laranja.

1. (Opcional) Para ir para as solicitações destacadas, clique nas setas para cima ou para baixo na barra de pesquisa.
