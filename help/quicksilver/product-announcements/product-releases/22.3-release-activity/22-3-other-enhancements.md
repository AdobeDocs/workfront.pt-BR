---
title: outras atualizações durante o período de lançamento da versão 2.3
description: outras atualizações durante o período de lançamento da versão 2.3
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# 2.3 Outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 2.3 para o ambiente de visualização. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 11 de julho de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.3, consulte [Visão geral da versão 2.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Folhas de horas atualizadas

Continuamos a melhorar e atualizar sua experiência ao trabalhar com folhas de horas. Estes são alguns dos recursos incluídos nesta atualização:

* Uma nova aparência corresponde à nova experiência do Workfront.

* A funcionalidade de salvamento automático salva as horas e os comentários da hora registrados automaticamente no segundo em que você os adiciona.

* Um layout de página mais intuitivo para corresponder a outras páginas de objeto. Por exemplo, adicionamos um painel esquerdo à folha de ponto. As atualizações da folha de ponto agora são exibidas na seção Atualizações no painel esquerdo. Também é possível excluir uma folha de ponto da página da folha de ponto, bem como adicionar a folha de ponto à lista Favoritos.

* Uma experiência melhor ao procurar e adicionar projetos, tarefas ou problemas à folha de ponto. Isso corresponde à experiência em todas as outras listas no Workfront.

* O painel Resumo está disponível para tarefas e problemas para adicionar comentários ou atualizar informações diretamente da folha de ponto.


Com a atualização atual, também substituímos os seguintes recursos:

* A criação de uma tarefa a partir de uma atualização foi removida. Esse recurso foi removido desde a versão 2018.2 das áreas de Atualizações de todos os outros objetos, mas ainda estava disponível no fluxo de atualização da folha de ponto.

* A opção &quot;Adicionar despesas de uma folha de ponto. &quot;A preferência foi removida da área Folha de Horas e Preferências de Horas da Configuração e você não pode mais registrar despesas da folha de horas. Ainda é possível registrar despesas nas páginas de tarefa e projeto.


Para obter mais informações, consulte os seguintes artigos:

* [Noções básicas sobre o layout da folha de horas](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configurar preferências de hora e folha de ponto](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Melhorias no painel de navegação esquerdo

Fizemos vários aprimoramentos no painel de navegação esquerdo no Adobe Workfront.

* A aparência do painel de navegação esquerdo foi atualizada para os padrões de design do Adobe, incluindo cores e fontes.

* O link &quot;Adicionar seção personalizada&quot; na parte inferior do painel foi renomeado para &quot;Adicionar painel&quot; para explicar melhor sua função.

## Habilitar a rotação de token de atualização automática em seus aplicativos OAuth2 personalizados

Para permitir mais controle sobre a segurança de seus aplicativos OAuth2 personalizados, adicionamos à opção para ativar a atualização da rotação do token. Quando essa opção está ativada, sempre que um token de atualização é usado, o aplicativo cria e envia automaticamente um novo token de atualização e desativa o antigo.

Seu aplicativo deve armazenar o novo token de atualização após cada atualização. O Workfront não armazena esse token de atualização.

Anteriormente, os tokens de atualização expiravam após um período definido nas configurações personalizadas do aplicativo OAuth2.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Use PKCE em suas integrações OAuth2 personalizadas para aplicativos Web de página única

Agora é possível criar aplicativos Web de página única em suas integrações personalizadas usando o PKCE. O PKCE é um fluxo de autorização seguro que funciona bem com a atualização dinâmica de aplicativos, como aplicativos móveis, mas é valioso em todos os clientes OAuth2. Em vez de um segredo de cliente estático, o PKCE usa uma sequência de caracteres gerada dinamicamente, eliminando o risco de um segredo de cliente vazado.

Anteriormente, as opções disponíveis para aplicativos OAuth2 personalizados usavam nome de usuário e senha ou um segredo de cliente.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
