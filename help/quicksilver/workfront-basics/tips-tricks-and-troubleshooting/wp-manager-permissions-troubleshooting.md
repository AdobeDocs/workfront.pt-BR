---
content-type: tips-tricks-troubleshooting
product-previous: workfront;workfront-proof
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Solução de problemas de permissões do Workfront Proof Manager
description: A seguir estão os perfis de permissão disponíveis em [!DNL Adobe] Workfront para usuários de prova - EDITE-ME.
feature: Get Started with Workfront
exl-id: 913241d0-f5b0-4674-b078-9a1ad3682aff
source-git-commit: ecb6928c946203b03a93cf5687fd53abf8e6a8f3
workflow-type: tm+mt
source-wordcount: '255'
ht-degree: 1%

---

# [!UICONTROL [!DNL Workfront] Gerenciador de prova] solução de problemas de permissões

A seguir estão os perfis de permissão disponíveis em [!DNL Adobe Workfront] para usuários de prova:

* [!UICONTROL Administrador]
* [!UICONTROL Supervisor]
* [!UICONTROL Gerente]

<!--For detailed information about these options and how to configure them, see .-->

Ao conceder um usuário [!UICONTROL Gerenciador] As seguintes informações de solução de problemas estão disponíveis:

* **PROBLEMA:** Usuários com [!UICONTROL Gerenciador] As permissões do não podem exibir provas criadas por outros usuários. Em vez disso, eles veem a variável [!UICONTROL Acesso negado] tela.

   ![](assets/access-denied-350x161.png)

   **SOLUÇÃO:** Usuários com [!UICONTROL Gerenciador] permissões devem ser explicitamente adicionadas às provas. As provas devem ser sempre criadas por meio da variável [!UICONTROL Opções avançadas de prova] e os usuários devem sempre ser adicionados por meio dessa opção.

* **PROBLEMA:** Usuários com [!UICONTROL Gerenciador] as permissões do não podem adicionar versões de prova às provas criadas por outros usuários (elas podem enviar uma prova no conjunto de documentos, mas as versões NÃO seriam conectadas ao conjunto original criado por outro usuário).\
   **SOLUÇÃO:** Usuários com [!UICONTROL Gerenciador] permissões podem enviar as versões para a prova de outro usuário somente se o usuário com [!UICONTROL Gerenciador] permissões quando:

   * Adição explícita às provas
   * Definir como [!UICONTROL Autores] (função de prova) nas provas

* **PROBLEMA:** Usuários com [!UICONTROL Gerenciador] As permissões do não podem editar comentários de outros usuários em uma prova que eles não possuem ou que não criaram.\
   **SOLUÇÃO:** Se usuários com [!UICONTROL Gerenciador] permissões não são proprietárias das provas, mas devem poder editar comentários, adicioná-los como [!UICONTROL Autores] ou [!UICONTROL Moderadores]).\
   Esses três tipos de permissões estão disponíveis em [!DNL Workfront] para [!UICONTROL Planejador], [!UICONTROL Trabalhador], [!UICONTROL Requerente], [!UICONTROL Revisor] licenças do tipo . Administrador do sistema ou Administrador do usuário em [!DNL Workfront] pode editar os perfis dos usuários e ajustar [!DNL Workfront Proof] permissões de lá.
