---
product-area: projects
navigation-topic: approvals
title: Aprovar um documento no Workfront
description: Se você estiver atribuído como aprovador de um documento, há várias maneiras de tomar sua decisão de aprovação.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 1f7a17206ca77442b501f121f3333d4b60aa85f1
workflow-type: tm+mt
source-wordcount: '1247'
ht-degree: 0%

---

# Aprovar um documento no Workfront

Se você estiver atribuído como aprovador de um documento, há várias maneiras de tomar sua decisão de aprovação.

Para obter informações sobre como criar uma nova aprovação de documento, consulte [Criar uma revisão de documento ou solicitação de aprovação](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>O conteúdo deste artigo se refere à funcionalidade atualizada de aprovação de documentos, disponível somente para contas específicas. Para obter informações sobre processos de aprovação padrão, consulte os artigos listados em [Aprovações de trabalho](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou ter maior acesso aos objetos associados às aprovações</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou mais altas para os objetos associados às aprovações</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Aprovar um documento da Página inicial

1. Clique no ícone **Página inicial** ![Ícone da página inicial](../assets/home-icon-30x29.png), no canto superior esquerdo do Adobe Workfront.

   >[!NOTE]
   >
   >O administrador do Workfront pode fazer as seguintes alterações no ícone Início do ambiente:
   >
   >* Substitua-a por uma imagem personalizada para ilustrar sua organização. Nesse caso, o ícone será diferente do mostrado neste artigo.
   >
   >* Substituir a página vinculada a ela por uma página diferente. Nesse caso, clique no **Ícone do** ![Menu principal](../assets/main-menu-icon.png), no canto superior direito da página, e clique em **Página inicial**.

1. Clique em **Filtros** na parte superior esquerda da página e verifique se **Aprovações** está marcado.

   Todos os itens de trabalho que exigem aprovação são exibidos na lista.

   >[!NOTE]
   >
   >* As aprovações atribuídas a Funções ou Grupos de trabalho não são listadas na Página inicial.
   >* As aprovações atribuídas às equipes são exibidas no widget Minhas aprovações de cada membro da equipe na Página inicial.

1. Clique na aprovação do documento na lista para a qual deseja tomar uma decisão de aprovação. As informações relativas à aprovação serão exibidas no lado direito da página.

1. Clique em uma das duas seguintes opções de aprovação no canto superior direito da página:

   * A lista suspensa **Aprovar** contém duas opções:

      * **Aprovar** indica que nenhuma alteração é necessária para esta versão do documento e que a aprovação é fornecida.

      * **Aprovar com alterações** indica que algumas pequenas alterações ainda são necessárias no documento, mas a aprovação é dada com a condição de que essas alterações sejam feitas. Se você selecionar essa opção, será exibida uma janela contendo uma caixa de texto denominada **Próximas etapas**, na qual você pode especificar quais alterações são necessárias para que o documento seja aprovado. Você pode inserir essas informações e clicar em **Adicionar mensagem** ou clicar em **Ignorar** para enviar a decisão de aprovação sem informações adicionais.

   * **Precisa do trabalho** indica que a versão do documento não foi aprovada e requer alterações significativas.

   Considere o seguinte ao exibir aprovações de documentos na Página inicial:

   * O nome do usuário que solicitou a aprovação é exibido acima do nome do documento na Página inicial com o texto &quot;*O usuário A* gostaria de obter sua aprovação em...&quot;, bem como em **Enviado por** nas informações de aprovação que são exibidas à direita depois que uma aprovação é selecionada.

   * Depois que uma decisão é tomada em uma aprovação, ela permanece na guia Minhas aprovações com o texto &quot;Tomada de decisão&quot; até que você clique no botão **Atualizar** ou até que você atualize a página do navegador.

## Aprovar um documento na página de documento

1. Vá para a página do documento clicando no nome do documento.

1. Selecione a versão do documento que está aguardando sua aprovação na lista suspensa de versões ao lado do nome do documento. A versão mais recente será selecionada por padrão.

   Se a versão selecionada atualmente do documento tiver uma aprovação pendente para você, os botões de decisão de aprovação serão exibidos no canto superior direito da página; se outras versões do documento tiverem aprovações pendentes para você, o menu suspenso da versão exibirá um ponto vermelho.

   <!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Clique em uma das duas seguintes opções de aprovação no canto superior direito da página:

   * A lista suspensa **Aprovar** contém duas opções:

      * **Aprovar** indica que nenhuma alteração é necessária para esta versão do documento e que a aprovação é fornecida.

      * **Aprovar com alterações** indica que algumas pequenas alterações ainda são necessárias no documento, mas a aprovação é dada com a condição de que essas alterações sejam feitas. Se você selecionar essa opção, será exibida uma janela contendo uma caixa de texto denominada **Próximas etapas**, na qual você pode especificar quais alterações são necessárias para que o documento seja aprovado. Você pode inserir essas informações e clicar em **Adicionar mensagem** ou clicar em **Ignorar** para enviar a decisão de aprovação sem informações adicionais.

   * **Precisa do trabalho** indica que a versão do documento não foi aprovada e requer alterações significativas.

## Aprovar um documento no painel Resumo do documento

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.

1. Clique no documento que precisa de sua aprovação e o painel Resumo do documento será aberto.

1. Selecione a versão do documento que deseja revisar na lista suspensa de versões. A versão mais recente será selecionada por padrão.

   Se a versão selecionada atualmente do documento tiver uma aprovação pendente para você, os botões de decisão de aprovação serão exibidos no canto superior direito do painel Resumo do documento; se outras versões do documento tiverem aprovações pendentes para você, o menu suspenso da versão exibirá um ponto vermelho.
<!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
 -->
1. Clique em uma das duas opções de aprovação a seguir no canto superior direito do painel Resumo do documento:

   * A lista suspensa **Aprovar** contém duas opções:

      * **Aprovar** indica que nenhuma alteração é necessária para esta versão do documento e que a aprovação é fornecida.

      * **Aprovar com alterações** indica que algumas pequenas alterações ainda são necessárias no documento, mas a aprovação é dada com a condição de que essas alterações sejam feitas. Se você selecionar essa opção, será exibida uma janela contendo uma caixa de texto denominada **Próximas etapas**, na qual você pode especificar quais alterações são necessárias para que o documento seja aprovado. Você pode inserir essas informações e clicar em **Adicionar mensagem** ou clicar em **Ignorar** para enviar a decisão de aprovação sem informações adicionais.

   * **Precisa do trabalho** indica que a versão do documento não foi aprovada e requer alterações significativas.


## Aprovar um documento do visualizador de prova

Para revisar e aprovar um documento:

1. Vá para a notificação por email de revisão e clique em **Ir para revisão**.

1. Depois de entrar no Workfront, clique em **Ir para prova**.

1. Revise o conteúdo e adicione comentários ou marcações. Para obter mais informações sobre como usar o visualizador de provas, consulte [Revisar provas no Adobe Workfront: índice do artigo](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Escolha uma das seguintes decisões:

   * **Aprovar**: o documento não precisa de alterações e está pronto para uso.
   * **Aprovar com alterações**: o documento precisa de alterações e está pronto para uso quando elas forem feitas. Aprovação adicional não é necessária.
   * **Precisa do trabalho**: o documento precisa de alterações e não está pronto para uso. Depois que as alterações especificadas forem feitas, o documento deverá ser carregado como uma nova versão e passar por outra rodada de aprovações. Para obter mais informações sobre como carregar uma nova versão, consulte [Criar uma nova versão conforme necessário](#create-a-new-version-as-needed) neste artigo.

Depois de tomar uma decisão, o proprietário do documento é notificado por email.


