---
content-type: reference
navigation-topic: announcements
title: Remover SMTP personalizado como uma opção de email de saída
description: Com a versão 20.3 (direcionada para agosto de 2020), a Adobe Workfront está migrando para um novo sistema de email que melhorará muito a confiabilidade de seu delivery de email para atualizações e notificações do Workfront. Como resultado, os clientes não poderão mais usar seu próprio servidor de email SMTP para retransmitir seus emails da plataforma Workfront para o recipient pretendido. Todos os emails serão enviados diretamente do Workfront Mail Server.
author: Luke
feature: Product Announcements
exl-id: 73abd185-81c6-43fc-b8b0-cad14d15b348
source-git-commit: 9bc394c718becbac2848c2d91ba3202483699b6f
workflow-type: tm+mt
source-wordcount: '279'
ht-degree: 0%

---

# Remover SMTP personalizado como uma opção de email de saída

Com a versão 20.3 (direcionada para agosto de 2020), a Adobe Workfront está migrando para um novo sistema de email que melhorará muito a confiabilidade de seu delivery de email para atualizações e notificações do Workfront. Como resultado, os clientes não poderão mais usar seu próprio servidor de email SMTP para retransmitir seus emails da plataforma Workfront para o recipient pretendido. Todos os emails serão enviados diretamente do Workfront Mail Server.

Este recurso é acessado fazendo logon como Administrador do sistema e navegando até Configuração > Email > Configuração. Esta é uma captura de tela destacando o recurso :

![](assets/email-server-settings-350x226.png)

A configuração realçada nesta captura de tela fará a transição automática para usar a opção Workfront Mail Server com a versão 20.3.

Se você configurou um servidor de email SMTP personalizado, **recomendamos que você entre em contato com a equipe de TI** para garantir que o email de notifications@my.workfront.com não será bloqueado para o email de entrada em seu sistema. Você também pode consultar Configuração do firewall para obter detalhes sobre quais endereços IP são originados pelo nosso tráfego e email.

Se tiver outras dúvidas ou preocupações, entre em contato com o [Equipe de suporte da Workfront](https://one.workfront.com/s/support?language=en_US).
