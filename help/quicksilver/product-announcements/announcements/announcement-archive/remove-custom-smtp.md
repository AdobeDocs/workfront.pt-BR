---
content-type: reference
navigation-topic: announcements
title: Remover SMTP personalizado como uma opção de email de saída
description: Com a versão 20.3 (prevista para agosto de 2020), o Adobe Workfront está migrando para um novo sistema de email que melhorará muito a confiabilidade da sua entrega de email para atualizações e notificações do Workfront. Como resultado, os clientes não poderão mais usar seu próprio servidor de email SMTP para retransmitir seu email da plataforma Workfront para o recipient pretendido. Todos os e-mails serão enviados diretamente do servidor de e-mail da Workfront.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '281'
ht-degree: 0%

---

# Remover SMTP personalizado como uma opção de email de saída

Com a versão 20.3 (prevista para agosto de 2020), o Adobe Workfront está migrando para um novo sistema de email que melhorará muito a confiabilidade da sua entrega de email para atualizações e notificações do Workfront. Como resultado, os clientes não poderão mais usar seu próprio servidor de email SMTP para retransmitir seu email da plataforma Workfront para o recipient pretendido. Todos os e-mails serão enviados diretamente do servidor de e-mail da Workfront.

Esse recurso é acessado fazendo logon como Administrador do sistema e navegando até Configuração > Email > Configuração. Esta é uma captura de tela destacando o recurso:

![Configurações do servidor de email](assets/email-server-settings-350x226.png)

A configuração destacada nesta captura de tela fará a transição automática para usar a opção Workfront Mail Server com a versão 20.3.

Se você configurou um servidor de email SMTP personalizado, **recomendamos que você entre em contato com a equipe de TI** para garantir que os emails de notifications@my.workfront.com não sejam bloqueados para emails de entrada em seu sistema. Você também pode consultar Configuração do firewall para obter detalhes sobre os endereços IP de onde vêm nosso tráfego e email.

Se tiver outras dúvidas ou dúvidas, entre em contato com a [Equipe de suporte da Workfront](https://experienceleague.adobe.com/?support-tab=home#support).
