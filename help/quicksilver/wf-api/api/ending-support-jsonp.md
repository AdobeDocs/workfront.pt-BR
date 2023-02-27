---
content-type: api
navigation-topic: api-navigation-topic
title: Encerramento do suporte para JSONP
description: Encerramento do suporte para JSONP
author: Becky
feature: Workfront API
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# Encerramento do suporte para JSONP

Como JSONP (Javascript com preenchimento) é um padrão antigo com vulnerabilidades de segurança conhecidas, a Adobe Workfront não será mais compatível com JSONP a partir de novembro de 2018. Esta decisão apoia a nossa maior iniciativa de modernização da plataforma Workfront.

JSONP é um padrão pelo qual as solicitações entre origens ou entre sites podem ser executadas. Muitos clientes e parceiros da Workfront usam JSONP para acessar o Workfront de um sistema em seu próprio domínio como parte de uma integração. O JSONP permite que solicitações de domínios que não sejam da Workfront sejam processadas pelo aplicativo Workfront.

Se você estiver usando JSONP como parte de qualquer integração do Workfront, deverá atualizar sua integração para usar o padrão CORS (Cross-Origin Resource Sharing). Esta atualização requer que você faça o seguinte:

1. Envie uma solicitação com a equipe de suporte da Workfront para que todos os domínios que estão sendo usados para fazer solicitações entre origens sejam .

   Para que seus domínios sejam adicionados à  de lista de permissões do CORS, entre em contato com o Suporte ao cliente da Workfront pelo número 844-306-HELP(4357) ou enviando um tíquete de suporte online.

   >[!NOTE]
   >
   >A adição de domínios à lista de permissões do CORS é compatível somente para clientes que usavam JSONP antes de 1º de agosto de 2018.


1. Faça alterações no código de integração para usar o CORS.
