---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Criar um Scorecard
description: Um scorecard mede o alinhamento de um projeto com os critérios estabelecidos anteriormente de um portfólio. Um scorecard geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.Os gerentes do Portfolio geralmente definem as perguntas e respostas do scorecard para garantir que elas sejam significativas e valiosas durante a priorização e a seleção do projeto. Um administrador do  [!DNL Adobe Workfront]  cria os scorecards com base nas recomendações dos gerentes de portfólio.
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: f97c989f57d864252adf6e24f8e6b03f56d26901
workflow-type: tm+mt
source-wordcount: '718'
ht-degree: 1%

---

# Criar um cartão de pontuação

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

Um scorecard mede o alinhamento de um projeto com os critérios estabelecidos anteriormente de um portfólio. Um cartão de pontuação geralmente reflete a missão, os valores e os objetivos estratégicos de uma organização.

Como gerente de portfólio, você pode definir as perguntas e respostas do cartão de pontuação para garantir que sejam significativas e valiosas durante a priorização e a seleção do projeto.

Como administrador do [!DNL Adobe Workfront], você pode criar scorecards com base nas recomendações dos gerentes de portfólio.

As perguntas e respostas escolhidas para um cartão de pontuação devem ser quantificáveis para fornecer um valor de alinhamento para comparar projetos diferentes.

Você pode criar um cartão de pontuação da seguinte maneira:

* Do zero
* Copiando um existente

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Novo: Ultimate</p>
   <p>Atual: [!UICONTROL Business] ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr> 
   <tr> 
   <td role="rowheader"><p>Nível de acesso</p></td> 
   <td><p>Administrador de Sistema</p>
   </td> 
  </tr>
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar um cartão de pontuação do zero

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Scorecards]** e em **[!UICONTROL Novo Scorecard]**.

   A caixa **Novo cartão de pontuação** é aberta.

   ![Nova caixa de scorecard](assets/new-scorecard-350x173.png)

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

1. Clique em **[!UICONTROL Salvar]**.

   Isso cria o cartão de pontuação e os gerentes de projeto agora podem anexá-lo ao business case do projeto.

## Copiar um scorecard existente

Você pode criar um cartão de pontuação copiando e editando um existente.

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Scorecards]** no painel esquerdo.
1. Selecione um scorecard na lista e clique no ícone **Copiar** ![Ícone Copiar scorecard](assets/copy-scorecard-icon.png) na parte superior da lista de scorecards.

   A caixa **Copiar Scorecard** é aberta.

   ![Copiar caixa de scorecard](assets/copy-scorecard-box.png)

1. Especifique as seguintes informações:

   * **Scorecard**: atualize o nome do scorecard.  Por padrão, o nome é atualizado automaticamente de acordo com o seguinte formato:

     `Original scorecard name (Copy)`
   * **Descrição**: digite informações adicionais sobre o cartão de pontuação.
1. Clique em **Salvar**.

   Isso cria um novo cartão de pontuação com as mesmas informações que o original. Os gerentes de projeto agora podem anexá-lo ao seu caso de negócios de projeto.

## Aplicar um cartão de pontuação a um projeto

Um usuário com permissões de [!UICONTROL gerenciar] para um projeto pode aplicar um scorecard a um projeto depois que o scorecard tiver sido criado pelo administrador [!DNL Workfront].

Um cartão de pontuação é adicionado a um projeto como parte da criação de um business case para o projeto. Para obter mais informações sobre como adicionar um cartão de pontuação a um projeto, consulte [Aplicar um cartão de pontuação a um projeto e gerar uma Pontuação de Alinhamento](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

Para obter mais informações sobre permissões de projeto, consulte [Compartilhar um projeto em [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).


