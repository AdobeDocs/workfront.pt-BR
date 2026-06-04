---
content-type: reference
navigation-topic: announcements
title: Falsificação de email e remoção de resposta POP
description: Estamos fazendo duas alterações no modo como o Adobe Workfront envia e recebe emails com a versão 20.3 (prevista para agosto de 2020).
author: Luke
feature: Product Announcements
exl-id: 9110f04d-b7a9-428b-928c-c4eb746fec3f
TQID: https://experienceleague.adobe.com/eOFRSbJicMbYHqq74-O9VW0c73RDQmAC-OIkLX-FKFw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 319
ht-degree: 3%

---

# Falsificação de email e resposta POP

Estamos fazendo duas alterações no modo como o Adobe Workfront envia e recebe emails com a versão 20.3 (prevista para agosto de 2020).

## Email de saída do Workfront

Em um esforço para aumentar o sucesso da entrega de emails, eliminaremos a falsificação de emails, que geralmente são marcados como spam (consulte Falsificação de email). Todos os emails do Workfront serão enviados de `notifications@my.workfront.com`, incluindo alertas automatizados e comunicação entre usuários. Um email de exemplo de Joan Harris terá esta aparência na área de do seu email:

![Exemplo de email](assets/noreply.png)

*É altamente recomendável entrar em contato com a equipe de TI* para garantir que os emails de `notifications@my.workfront.com` não sejam bloqueados para emails de entrada no sistema. Você também pode consultar [Configurar o incluo na lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) para obter detalhes sobre os endereços IP de onde vêm nosso tráfego e email.

## Respostas de email de entrada para notificações (resposta POP)

Certas notificações por email permitem que os usuários respondam por email e que a resposta seja copiada para o Workfront como uma resposta de comentário no sistema Workfront. Tradicionalmente, os administradores de sistema no Workfront podem escolher entre fornecer seu próprio servidor de email POP para receber essas respostas ou usar o sistema de resposta integrado do Workfront. A opção de servidor de email POP personalizado está sendo removida com a versão 20.3. Todas as contas configuradas para usar um servidor personalizado passarão automaticamente para usar o sistema de resposta de email nativo do Workfront. Nenhuma ação é necessária para administradores do sistema ou outros usuários do Workfront.

Não haverá alterações nos emails provenientes diretamente do sistema do Workfront Proof. Você continuará a receber esses emails como recebeu no passado.

Se tiver outras dúvidas ou dúvidas, entre em contato com a [Equipe de suporte da Workfront](https://experienceleague.adobe.com/pt-br?support-tab=home&lang=pt-BR#support).
