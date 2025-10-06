---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Adicionar um email do Outlook a um projeto como uma tarefa ou um problema
description: Você pode converter emails em  [!DNL Adobe Workfront] tarefas ou problemas. Depois que um email é convertido, a tarefa ou o problema é exibido no projeto selecionado ao convertê-lo.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 00755c27-9fc9-4357-a39b-4f9772484252
source-git-commit: 793c8c940c8cb7ac53169edf21ddf28af2554120
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Adicionar um email do [!DNL Outlook] a um projeto como tarefa ou problema


>[!IMPORTANT]
>
>[O Microsoft desabilitou o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que foram usados pelo suplemento do Workfront Outlook para autenticação. Essa alteração pelo Microsoft foi implementada em fases e está concluída a partir de 1 de outubro de 2025.
>
>**Como o Microsoft desabilitou esses tokens, a integração do Workfront para Microsoft Outlook não funciona mais.**

Você pode converter emails em [!DNL Adobe Workfront] tarefas ou problemas. Depois que um email é convertido, a tarefa ou o problema é exibido no projeto selecionado ao convertê-lo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Trabalho], [!UICONTROL Plano]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

O administrador do [!DNL Workfront] deve habilitar [!DNL Outlook for Office] com [!DNL Workfront] antes que você possa usar essa integração.

## Adicionar um email do [!DNL Outlook] a um projeto como uma tarefa ou problema

1. Selecione o email em [!DNL Outlook] que você deseja converter em tarefa ou problema.
1. Clique no ícone **[!DNL Workfront]** no canto superior direito da mensagem de email para exibir o suplemento do Workfront.

   Talvez seja necessário clicar na seta para baixo na parte superior direita do email para acessar o ícone [!DNL Workfront].

1. Clique no ícone **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) para exibir a lista de opções [!DNL Workfront] disponíveis.



1. Clique em **[!UICONTROL Adicionar ao Trabalho]**.

1. Selecione o campo **[!UICONTROL Adicionar ao projeto]**.
1. Comece digitando o nome de um projeto no campo **[!UICONTROL Projeto]** e selecione-o quando ele aparecer na lista.
1. Selecione o botão de opção **[!UICONTROL Tarefa]** se desejar adicionar uma tarefa ao projeto selecionado.

   Ou

   Selecione o botão de opção **[!UICONTROL Problema]** se desejar adicionar um problema ao projeto selecionado.

1. (Opcional) Especifique a quem esta tarefa ou problema está atribuído no campo **[!UICONTROL Atribuir a tarefa a]**.

   >[!TIP]
   >
   >Você pode atribuir a tarefa ou o problema a uma equipe, se quiser que várias pessoas estejam cientes disso. Se as notificações por email dos membros da equipe estiverem habilitadas, eles receberão um email sobre a nova tarefa ou problema atribuído a eles.


1. (Opcional) Especifique a **[!UICONTROL Data de vencimento]**. Esta se torna a [!UICONTROL Data de conclusão planejada] da tarefa ou problema.
1. (Opcional) Atualize as seguintes informações do email antes de salvá-lo como uma tarefa ou problema (os campos obrigatórios são precedidos por um asterisco).

   <table style="table-layout:auto">
      <tr>
        <td>[!UICONTROL Nome da Tarefa ou Problema]</td>
        <td>Por padrão, o nome da tarefa é igual ao Assunto do email. Você pode modificar o nome da tarefa conforme desejado.</td>
        <td></td>
      </tr>
      <tr>
        <td>[!UICONTROL Descrição]</td>
        <td>Por padrão, a descrição é igual ao corpo do email. Você pode modificar a descrição conforme desejado.</td>
      </tr>
      <tr>
        <td>[!UICONTROL Anexos]</td>
        <td>Todos os anexos de email são salvos na área [!UICONTROL Documentos] da tarefa ou problema. Você pode excluir quaisquer anexos antes de salvar o email como uma tarefa ou problema.</td>
      </tr>
   </table>

1. Clique em **[!UICONTROL Adicionar]**.

   A tarefa ou problema é adicionado ao projeto especificado

1. (Opcional) Clique em **[!UICONTROL Exibir em[!DNL Workfront]]** para exibir a tarefa no aplicativo [!DNL Workfront] em uma nova guia.

1. (Opcional) Volte para [!DNL Outlook] e selecione o email convertido.

   Na parte superior do painel de suplementos do [!DNL Workfront], observe a confirmação com um link de que o email foi adicionado ao [!DNL Workfront] como uma tarefa ou um problema. O link inclui a data em que foi convertido.



