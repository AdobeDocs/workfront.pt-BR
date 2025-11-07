---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Solução de problemas de permissões do Workfront Proof Manager
description: Os perfis de permissão disponíveis no  [!DNL Adobe] Workfront para usuários de comprovação são Administrador, Supervisor e Gerente.
feature: Get Started with Workfront
auhor: Courtney
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# [!UICONTROL [!DNL Workfront] Gerenciador de provas ] permissões solução de problemas

A seguir estão os perfis de permissão disponíveis em [!DNL Adobe Workfront] para usuários de revisão:

* [!UICONTROL Admin]
* [!UICONTROL Supervisor]
* [!UICONTROL Gerente]

<!--For detailed information about these options and how to configure them, see .-->

Ao conceder permissões de [!UICONTROL Gerente] a um usuário, as seguintes informações de solução de problemas estão disponíveis:

* **PROBLEMA:** usuários com permissões de [!UICONTROL Gerente] não podem exibir provas criadas por outros usuários. Em vez disso, eles veem a tela [!UICONTROL Acesso Negado].

  ![](assets/access-denied-350x161.png)

  **SOLUÇÃO:** usuários com permissões de [!UICONTROL Gerente] devem ser adicionados explicitamente às provas. As provas devem ser sempre criadas por meio da janela [!UICONTROL Opções de prova avançada] e os usuários devem ser sempre adicionados por meio dessa opção.

* **PROBLEMA:** usuários com permissões de [!UICONTROL Gerente] não podem adicionar versões de prova às provas criadas por outros usuários (possivelmente eles poderiam enviar uma prova no conjunto de documentos, mas as versões NÃO estariam conectadas ao conjunto original criado por outro usuário).\
   **SOLUÇÃO:** usuários com permissões de [!UICONTROL Gerente] podem enviar as versões para prova de outro usuário somente se o usuário com permissões de [!UICONTROL Gerente] tiver ambas as seguintes permissões:

   * Adicionado explicitamente às provas
   * Definir como [!UICONTROL Autores] (função de prova) nas provas

* **PROBLEMA:** usuários com permissões de [!UICONTROL Gerente] não podem editar comentários de outros usuários em uma prova que não sejam seus ou que não tenham sido criados.\
   **SOLUÇÃO:** Se os usuários com permissões de [!UICONTROL Gerente] não forem proprietários das provas, mas não puderem editar comentários, adicione-os como [!UICONTROL Autores] (ou [!UICONTROL Moderadores]).\
   Estes três tipos de permissões estão disponíveis no [!DNL Workfront] para licenças do tipo [!UICONTROL Planejador], [!UICONTROL Trabalhador], [!UICONTROL Solicitante], [!UICONTROL Revisor]. O Administrador do Sistema ou o Administrador de Usuários no [!DNL Workfront] pode editar os perfis dos usuários e ajustar as permissões do [!DNL Workfront Proof] a partir daí.
