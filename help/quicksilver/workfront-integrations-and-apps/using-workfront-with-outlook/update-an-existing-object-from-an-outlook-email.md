---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-outlook
title: Atualizar um objeto existente a partir de um email do Outlook
description: Você pode atualizar um projeto, tarefa ou problema existente com informações de um email do Outlook.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 297eb1c4-ee9f-4bb3-a412-18f23c74b0eb
source-git-commit: b4b45bbc8bb68dbac35488c1777fca85fa0cc7e3
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Atualizar um objeto existente a partir de um email [!DNL Outlook]

>[!IMPORTANT]
>
>[O Microsoft está desabilitando o suporte para tokens herdados do Exchange online](https://learn.microsoft.com/en-us/office/dev/add-ins/outlook/faq-nested-app-auth-outlook-legacy-tokens), que são usados atualmente pelo suplemento do Workfront Outlook para autenticação. Essa alteração pela Microsoft já começou a afetar os clientes e continuará a ser implementada em fases até outubro de 2025.
>
>* **Depois que o Microsoft desabilitar totalmente esses tokens, a integração do Workfront para Microsoft Outlook não funcionará mais.**
>
>Como parte dessa alteração, a Microsoft tomou a decisão de alterar a maneira como os tokens são reativados. Após **30 de junho de 2025**, os administradores não poderão mais reabilitar tokens, somente o Suporte da Microsoft poderá conceder exceções. **Em 1º de outubro de 2025, os tokens herdados serão desativados para todos os locatários. Exceções não serão concedidas.**

Você pode atualizar um projeto, tarefa ou problema existente com informações de um email [!DNL Outlook].


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

## Atualizar um objeto existente a partir de um email [!DNL Outlook]

1. Em [!DNL Outlook], selecione o email que contém as informações que você deseja incluir em um [!DNL Adobe Workfront update].
1. Clique no ícone **[!DNL Workfront]** no canto superior direito da mensagem de email para exibir o suplemento do Workfront.\
   Talvez seja necessário clicar na seta para baixo na parte superior direita do email para acessar o ícone [!DNL Workfront].

1. Clique no ícone **[!UICONTROL Menu]** ![o365_addin_menu_icon.png](assets/o365-addin-menu2-icon.png) para exibir a lista de opções [!DNL Workfront] disponíveis.\


1. Clique em **[!UICONTROL Atualizar] no Workfront**.\
   Você pode atualizar as seguintes informações do email antes de salvá-lo como uma tarefa:

   * **[!UICONTROL Tipo]**: selecione o tipo de objeto que você está atualizando. Você pode selecionar **[!UICONTROL Projeto]**, **[!UICONTROL Tarefa]** ou **[!UICONTROL Problema]**. O objeto selecionado determina os resultados exibidos no campo **[!UICONTROL Nome]** abaixo. Se não tiver certeza do tipo de objeto, selecione **[!UICONTROL Todos]** para procurar projetos, tarefas e problemas simultaneamente.

   * **[!UICONTROL Nome]**: comece a digitar o nome do projeto, tarefa ou problema que deseja atualizar. Clique no nome quando ele aparecer na lista suspensa.
   * **[!UICONTROL Atualização]**: por padrão, a atualização é a mesma que o corpo do email. Você pode modificar a atualização conforme desejado.\

     Esta [!UICONTROL atualização] é exibida como o status de atualização no Workfront.

   * **[!UICONTROL Anexos]**: todos os anexos de email são salvos na área [!UICONTROL Documentos] da tarefa. Você pode deletar quaisquer anexos antes de submeter a atualização.

1. (Opcional) Clique em **[!UICONTROL Incluir outros]**, comece digitando o nome dos usuários que deseja incluir na atualização e, em seguida, clique no nome quando ele aparecer na lista suspensa.\
   Repita esse processo para incluir usuários adicionais e clique em **[!UICONTROL Concluído]**.\
   Por padrão, o usuário ao qual você está respondendo recebe uma notificação, independentemente de você incluí-lo ou não.\

1. (Opcional) Clique no ícone **[!UICONTROL Bloquear]** para restringir esta atualização aos usuários em sua empresa. Quando a atualização é bloqueada, os usuários fora da empresa não podem vê-la.

   * **[!UICONTROL Desbloqueado]:** Qualquer usuário com acesso ao projeto, tarefa ou problema em que está a atualização pode exibi-la.\

     Por padrão, a atualização é desbloqueada.\
      ![o365_addin_unlock.png](assets/o365-addin-unlock.png)

   * **[!UICONTROL Bloqueado]:** Somente usuários em sua empresa podem exibir a atualização.\

     ![o365_addin_lock.png](assets/o365-addin-lock.png)

1. Clique em **[!UICONTROL Atualizar]**.
1. (Opcional) Clique em **[!UICONTROL Exibir no Workfront]** para exibir o item atualizado com a integração do [!DNL Workfront] no [!UICONTROL Outlook].
