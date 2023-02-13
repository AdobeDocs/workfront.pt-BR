---
content-type: reference
navigation-topic: announcements
title: Remoção de falsificação de email e de resposta POP
description: Estamos fazendo duas alterações na maneira como o Adobe Workfront envia e recebe emails com a versão 20.3 (direcionada para agosto de 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Spoofing de email e resposta de POP

Estamos fazendo duas alterações na maneira como o Adobe Workfront envia e recebe emails com a versão 20.3 (direcionada para agosto de 2020).

## Email de saída do Workfront

Em um esforço para aumentar o delivery bem-sucedido de emails, estaremos eliminando a falsificação de emails, que geralmente é marcada como spam (consulte falsificação de email). Todos os emails do Workfront serão enviados de notifications@my.workfront.com, incluindo alertas automatizados e comunicação de usuário para usuário. Um exemplo de email de Joan Harris será semelhante a este na área de formulário do seu email:

![](assets/noreply.png)

*Recomendamos que você entre em contato com a equipe de TI* para garantir que o email de notifications@my.workfront.com não será bloqueado para o email de entrada em seu sistema. Também é possível fazer referência a [Configurar a  lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) para obter detalhes sobre quais endereços IP são originados pelo tráfego e-mail.

## Respostas de email de entrada para notificações (Resposta POP)

Certas notificações por email permitem que os usuários respondam por email e que a resposta seja copiada para o Workfront como uma resposta de comentário no sistema Workfront. Tradicionalmente, os administradores de sistema no Workfront têm conseguido escolher entre fornecer seu próprio servidor de email POP para receber essas respostas ou usar o sistema de resposta Workfront integrado. A opção de servidor de email POP personalizado está sendo removida com a versão 20.3. Todas as contas configuradas para usar um servidor personalizado serão automaticamente transferidas para usar o sistema de resposta de email nativo do Workfront. Não é necessária nenhuma ação para administradores do sistema ou outros usuários do Workfront.

Não haverá alterações nos emails provenientes diretamente do sistema Workfront Proof. Você continuará recebendo esses emails como recebeu anteriormente.

Se tiver outras dúvidas ou preocupações, entre em contato com o [Equipe de suporte da Workfront](https://one.workfront.com/s/support?language=en_US).
