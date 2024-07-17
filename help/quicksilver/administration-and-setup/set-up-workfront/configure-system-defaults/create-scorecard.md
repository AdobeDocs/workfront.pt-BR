---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Criar um cartão de pontuação
description: Um scorecard mede o alinhamento de um projeto com os critérios estabelecidos anteriormente de um portfólio. Um scorecard geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.Os gerentes de Portfolio geralmente definem as perguntas e respostas do scorecard para garantir que sejam significativas e valiosas durante a priorização e a seleção do projeto. Um administrador do  [!DNL Adobe Workfront]  cria os scorecards com base nas recomendações dos gerentes de portfólio.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 84c5772d130be78d9f9b9aef342c57183d5ec985
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 0%

---

# Criar um cartão de pontuação

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Um scorecard mede o alinhamento de um projeto com os critérios estabelecidos anteriormente de um portfólio. Um cartão de pontuação geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.

Os gerentes de Portfolio geralmente definem as perguntas e respostas do cartão de pontuação para garantir que sejam significativas e valiosas durante a priorização e a seleção do projeto. Um administrador do [!DNL Adobe Workfront] cria os scorecards com base nas recomendações dos gerentes de portfólio.

As perguntas e respostas escolhidas para um cartão de pontuação devem ser quantificáveis para fornecer um valor de alinhamento para comparar projetos diferentes.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Atual: [!UICONTROL Business] ou superior</p> 
   Ou
   <p>Novo: [!UICONTROL Prime] ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td><p>Atual: [!UICONTROL Plano]</p>
   Ou
   <p>Novo: [!UICONTROL Padrão]</p>
   </td> 
  </tr> 
 </tbody> 
</table>

+++

## Criar um cartão de pontuação

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Scorecards]** e em **[!UICONTROL Novo Scorecard]** para iniciar o construtor de scorecards e criar um scorecard.

1. Especifique um **[!UICONTROL Nome do Scorecard]** e uma **[!UICONTROL Descrição]**.

   O nome é exibido ao associar o cartão de pontuação ao projeto. A descrição é exibida ao lado do nome do cartão de pontuação na lista do cartão de pontuação.

1. Clique no menu suspenso **[!UICONTROL Adicionar pergunta]** para abrir a seção [!UICONTROL pergunta de scorecard] e especifique as seguintes informações para a pergunta:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pergunta]</td> 
      <td>Digite a pergunta que deseja incluir no cartão de pontuação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pontos]</td> 
      <td>Digite o máximo de pontos possível para esta pergunta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Pontos Negativos]</td> 
      <td>Selecione esta opção para indicar que [!DNL Workfront] deve subtrair do total de pontos possíveis. Pontuações negativas não podem ser adicionadas ao máximo de pontos possível de um cartão de pontuação.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Tipo de Exibição]</td> 
      <td>Selecione <strong>[!UICONTROL Value(0-100)]</strong> se desejar exibir um campo numérico no scorecard onde os usuários podem especificar qualquer valor entre 0-100.<p>Ou selecione <strong>[!UICONTROL Suspenso]</strong> ou <strong>[!UICONTROL Botões de Opção]</strong> para criar uma resposta que os usuários possam especificar usando esse controle. Clique em <strong>[!UICONTROL Adicionar resposta]</strong> e digite o <strong>[!UICONTROL Valor]</strong> em pontos percentuais para esta resposta, caso ela seja atendida. Se você escolher 100%, o número de pontos atribuídos para essa pergunta será totalmente atingido. Se você quiser indicar que esta resposta contém apenas uma parte do total de pontos atribuídos a esta pergunta, selecione um valor percentual mais baixo. Por exemplo, se a sua pergunta for avaliada em 10 pontos e você quiser que essa resposta tenha 5 desses pontos, escolha 50% para o seu valor.</p>
      <p>Selecione <strong>[!UICONTROL Padrão]</strong> para indicar que esta é a resposta padrão.</strong></p>
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Adicionar pergunta]** para adicionar mais perguntas e respostas ao cartão de pontuação, seguindo as mesmas etapas.

   >[!NOTE]
   >
   >Você pode reordenar as perguntas no cartão de pontuação arrastando e soltando as perguntas na ordem correta.

1. Clique em **[!UICONTROL Salvar]** quando terminar de inserir todas as informações.

   Isso cria o cartão de pontuação e os gerentes de projeto agora podem anexá-lo ao business case do projeto.

## Aplicar um cartão de pontuação a um projeto

Um usuário com permissões de [!UICONTROL gerenciar] para um projeto pode aplicar um scorecard a um projeto depois que o scorecard tiver sido criado pelo administrador [!DNL Workfront].

Um cartão de pontuação é adicionado a um projeto como parte da criação de um business case para o projeto. Para obter mais informações sobre como adicionar um cartão de pontuação a um projeto, consulte [Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de Alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para obter mais informações sobre permissões de projeto, consulte [Compartilhar um projeto em [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
