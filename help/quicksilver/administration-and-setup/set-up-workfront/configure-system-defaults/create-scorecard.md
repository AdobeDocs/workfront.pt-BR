---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Criar um scorecard
description: Um scorecard mede o grau de alinhamento de um projeto aos critérios previamente estabelecidos de um portfólio. Um scorecard geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização. Os gerentes do Portfolio geralmente definem as perguntas e respostas do scorecard para garantir que sejam significativas e valiosas durante a priorização e seleção do projeto. Um [!DNL Adobe Workfront] O administrador cria os scorecards com base nas recomendações dos gerentes do portfólio.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# Criar um scorecard

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Um scorecard mede o grau de alinhamento de um projeto aos critérios previamente estabelecidos de um portfólio. Um scorecard geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.

Geralmente, os gerentes de Portfolio definem as perguntas e respostas do scorecard para garantir que sejam significativas e valiosas durante a priorização e seleção do projeto. Um [!DNL Adobe Workfront] O administrador cria os scorecards com base nas recomendações dos gerentes do portfólio.

As perguntas e respostas escolhidas para um scorecard devem ser quantificáveis para fornecer um valor de alinhamento para comparar diferentes projetos.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>[!UICONTROL Business] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
 </tbody> 
</table>

## Criar um scorecard

1. Clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Scorecards]**, depois clique em **[!UICONTROL Novo Scorecard]** para criar um novo scorecard e iniciar o construtor do scorecard.

1. Especifique um **[!UICONTROL Nome do Scorecard]** e **[!UICONTROL Descrição]**.

   O nome é exibido quando você está associando o scorecard ao projeto. A descrição é exibida ao lado do nome do scorecard na lista de scorecards.

1. Clique no botão **[!UICONTROL Adicionar pergunta]** menu suspenso para abrir o [!UICONTROL pergunta do scorecard] e especifique as seguintes informações para sua pergunta:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pergunta]</td> 
      <td>Digite a pergunta que deseja incluir no scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pontos]</td> 
      <td>Digite os pontos máximos possíveis para esta pergunta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pontos negativos]</td> 
      <td>Selecione esta opção para indicar que [!DNL Workfront] O deve subtrair do total de pontos possíveis. As pontuações negativas não podem ser adicionadas aos pontos máximos possíveis de um scorecard.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Exibir tipo]</td> 
      <td>Selecionar <strong>[!UICONTROL Valor(0-100)]</strong> se desejar exibir um campo numérico no scorecard, onde os usuários podem especificar qualquer valor entre 0 e 100.<p>Ou, selecione <strong>[!UICONTROL Suspenso]</strong> ou <strong>[!UICONTROL Botões de opção]</strong> para criar uma resposta, os usuários podem especificar usando esse controle. Clique em <strong>[!UICONTROL Adicionar resposta]</strong>em seguida, digite o <strong>[!UICONTROL Valor]</strong> em pontos percentuais para esta resposta, caso seja cumprida. Se escolher 100%, o número de pontos atribuído a esta questão é totalmente atingido. Se quiser indicar que essa resposta contém apenas uma parte do total de pontos atribuídos a essa pergunta, selecione um valor de porcentagem menor. Por exemplo, se sua pergunta tem um valor de 10 pontos e você deseja que essa resposta tenha 5 desses pontos, escolha 50% para seu valor.</p>
      <p>Selecionar <strong>[!UICONTROL Padrão]</strong> se você indicar que essa resposta é padrão.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Adicionar pergunta]** para adicionar mais perguntas e respostas ao scorecard, seguindo as mesmas etapas.

   >[!NOTE]
   >
   >Você pode reorganizar as perguntas no scorecard arrastando e soltando as perguntas na ordem correta.

1. Clique em **[!UICONTROL Salvar]** quando terminar de inserir seus dados.

## Aplicar um scorecard a um projeto

Um usuário com [!UICONTROL gerenciar] as permissões para um projeto podem aplicar um scorecard a um projeto, depois que o scorecard for criado pela variável [!DNL Workfront] administrador.

Um scorecard é adicionado a um projeto como parte da criação de um business case para o projeto. Para obter mais informações sobre como adicionar um scorecard a um projeto, consulte [Aplicar um scorecard a um projeto e gerar uma Pontuação de alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para obter mais informações sobre a criação de scorecards, consulte [Criar um scorecard](#create-a-scorecard).

Para obter mais informações sobre permissões de projeto, consulte [Compartilhar um projeto em [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
