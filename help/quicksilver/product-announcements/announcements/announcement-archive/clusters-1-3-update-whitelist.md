---
content-type: reference
navigation-topic: announcements
title: Os clientes dos Clusters 1, 2 e 3 devem atualizar todos os blocos IP de lista de permissões para evitar o bloqueio dos serviços da Adobe Workfront
description: Para aprimorar e melhorar nossa infraestrutura principal, migraremos em breve os clientes do Adobe Workfront nos Clusters 01, 02 e 03 para a nuvem pública do AWS.
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 4%

---

# Os clientes dos Clusters 1, 2 e 3 devem atualizar todos os blocos IP de lista de permissões para evitar o bloqueio dos serviços da Adobe Workfront

Para aprimorar e melhorar nossa infraestrutura principal, migraremos em breve os clientes do Adobe Workfront nos Clusters 01, 02 e 03 para a nuvem pública do AWS.

Como parte dessa alteração, você precisa adicionar os seguintes IPs ao seu bloco de IP de lista de permissões para evitar o bloqueio dos serviços da Workfront:

Para SSO e POP:

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

Para email:

* 54.240.60.174
* 54.240.60.175

Certifique-se de que seus blocos IP de lista de permissões sejam atualizados até 13 de maio de 2019. Para obter mais informações, consulte [Configurar a  lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Agradecemos seu contínuo apoio à Workfront enquanto trabalhamos para criar uma experiência mais confiável e robusta para nossos clientes.

Em caso de dúvidas adicionais, entre em contato com a equipe de suporte visitando experience.workfront.com ou ligando para 844.306.4357 (EUA) ou +44.1256.274200 (EMEA).

## Perguntas frequentes

### Por que a Workfront está fazendo essa alteração?

Em um esforço para fornecer consistentemente o melhor serviço possível aos clientes, a Workfront procura constantemente formas de melhorar a experiência do usuário. Essa mudança utiliza novas tecnologias que nos permitem fornecer a melhor experiência possível e melhorar o nosso já robusto modelo de segurança.

### Quais ações são necessárias para mim como administrador do Workfront?

Entre em contato com seu departamento interno de TI ou segurança para obter assistência na análise dos blocos IP de  de lista de permissões e na adição dos IPs listados acima.

### O que minha organização pode esperar se não fizermos essa alteração?

Você não poderá acessar os serviços da Workfront enquanto migramos os serviços para os novos IPs.
