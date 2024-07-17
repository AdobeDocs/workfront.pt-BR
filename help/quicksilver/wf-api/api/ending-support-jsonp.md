---
content-type: api
navigation-topic: api-navigation-topic
title: Encerramento do suporte para JSONP
description: Encerramento do suporte para JSONP
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '206'
ht-degree: 0%

---

# Encerramento do suporte para JSONP

Como o JSONP (Javascript com preenchimento) é um padrão antigo com vulnerabilidades de segurança conhecidas, a Adobe Workfront não oferecerá mais suporte ao JSONP a partir de novembro de 2018. Essa decisão apoia nossa iniciativa maior de modernizar a plataforma Workfront.

JSONP é um padrão pelo qual solicitações entre origens ou sites podem ser executadas. Muitos clientes e parceiros da Workfront usam o JSONP para acessar o Workfront de um sistema em seu próprio domínio como parte de uma integração. O JSONP permite que solicitações de domínios que não são da Workfront sejam processadas pelo aplicativo do Workfront.

Se estiver usando o JSONP como parte de qualquer integração do Workfront, você deve atualizar sua integração para usar o padrão CORS (Cross-Origin Resource Sharing). Esta atualização requer que você faça o seguinte:

1. Envie uma solicitação com a equipe de suporte da Workfront para ter quaisquer domínios que estejam sendo usados para fazer solicitações entre origens para nossa inclui na lista de permissões.

   Incluir na lista de permissões Para adicionar seus domínios à pesquisa do CORS, entre em contato com o Suporte ao cliente da Workfront pelo telefone 844-306-HELP(4357) ou enviando um tíquete de suporte online.

   >[!NOTE]
   >
   >A adição de domínios ao incluo na lista de permissões para CORS só é compatível com clientes que estavam usando JSONP antes de 1º de agosto de 2018.


1. Faça alterações no código de integração para usar o CORS.
