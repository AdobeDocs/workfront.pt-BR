---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: Nome de usuário já em uso
description: Leia estas dicas quando receber um erro informando que o nome de usuário já está sendo usado.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

# Nome de usuário já em uso

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença</strong></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Administrador do sistema]</p> </td> 
  </tr> 
 </tbody> 
</table>

## Questão

Ao criar um novo usuário, uma [!UICONTROL Boias] será exibido informando que o nome de usuário já está sendo usado. Não há outras ocorrências desse email no sistema. Por que isso está sendo exibido?

## Solução

Isso pode ocorrer porque o nome de usuário ou endereço de email não é exclusivo no [!DNL Adobe Workfront] instância. Os usuários podem ter o mesmo nome de usuário ou endereço de email em instâncias separadas. Por exemplo, o Usuário A pode ter os seguintes endereços de email associados a um [!DNL Workfront] conta: usera@company1.com e usera@company2.com.

>[!NOTE]
>
>O principal [!DNL Workfront] o administrador não pode ter o mesmo nome de usuário ou endereço de email se estiver em instâncias separadas do Workfront no mesmo cluster.
>
>Se as instâncias estiverem em clusters diferentes, o administrador principal poderá ter o mesmo nome de usuário ou endereço de email. Você pode exibir o cluster no qual sua instância está [!UICONTROL Configuração] > [!UICONTROL Sistema] > [!UICONTROL Informações do cliente].

### Verifique se o seu nome de usuário é exclusivo em sua instância

Certifique-se de que o nome de usuário e o endereço de email sejam exclusivos no [!DNL Workfront] instância:

1. Como [!DNL Workfront] administrador, clique no botão **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe Workfront], depois clique em **[!UICONTROL Usuários]**.
1. Na lista de pessoas, verifique o **[!UICONTROL Email]** para garantir que não haja emails duplicados.
1. Adicione uma coluna para nome de usuário à exibição.

   1. No **[!UICONTROL Exibir]** , clique em **[!UICONTROL Personalizar exibição]**.
   1. Clique em **[!UICONTROL Adicionar coluna]**.
   1. No campo de pesquisa, digite *[!UICONTROL username]*.
   1. Selecionar **[!UICONTROL Usuário]** > **[!UICONTROL Nome do usuário]**.
   1. Salve a visualização.\
      Isso resulta em uma exibição para exibir os nomes de usuário, onde é possível procurar a duplicata.

1. Na lista de pessoas, verifique o **[!UICONTROL Nome do usuário]** para garantir que não haja nomes de usuário duplicados.
