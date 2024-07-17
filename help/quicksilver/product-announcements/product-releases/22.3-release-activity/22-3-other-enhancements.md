---
title: outras atualizações durante o período da versão 22.3
description: outras atualizações durante o período da versão 22.3
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 88d4c34e-9a3a-489d-ac97-2d81903104d8
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# 22.3 Outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 22.3 no ambiente de Pré-visualização. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 11 de julho de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.3, consulte a [Visão geral da versão 22.3](../../../product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Planilha de horas atualizada

Continuamos a melhorar e atualizar sua experiência ao trabalhar com folhas de horas. Veja a seguir alguns dos recursos incluídos nesta atualização:

* Uma nova aparência para corresponder à nova experiência do Workfront.

* Funcionalidade de salvamento automático para salvar automaticamente as horas reportadas e os comentários de hora no segundo em que forem adicionados.

* Um layout de página mais intuitivo para corresponder a outras páginas de objeto. Por exemplo, adicionamos um painel esquerdo à folha de horas. As atualizações da folha de horas agora são exibidas na seção Atualizações no painel esquerdo. Você também pode excluir uma folha de horas da página Folha de horas, bem como adicioná-la à lista Favoritos.

* Uma experiência melhor ao pesquisar e adicionar projetos, tarefas ou problemas à folha de horas. Isso corresponde à experiência em todas as outras listas no Workfront.

* O painel Resumo está disponível para tarefas e problemas para adicionar comentários ou atualizar informações diretamente da folha de horas.


Com a atualização atual, também substituímos os seguintes recursos:

* A criação de uma tarefa a partir de uma atualização foi removida. Esse recurso foi removido desde a versão 2018.2 das áreas Atualizações de todos os outros objetos, mas ainda estava disponível no fluxo de atualização da folha de horas.

* O &quot;Adicionar despesas de uma folha de horas. &quot;A preferência foi removida da área Preferências de Horas e Planilha de Horas da Configuração e você não pode mais registrar despesas da planilha de horas. Você ainda pode registrar despesas das páginas de tarefa e projeto.


Para obter mais informações, consulte os seguintes artigos:

* [Entender o layout de Planilha de Horas](/help/quicksilver/timesheets/timesheets/timesheet-layout.md)

* [Configurar preferências de horas e planilha de horas](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)


## Melhorias no painel de navegação esquerdo

Fizemos várias melhorias no painel de navegação esquerdo do Adobe Workfront.

* A aparência do painel de navegação esquerdo foi atualizada para os padrões de design de Adobe, incluindo cores e fontes.

* O link &quot;Adicionar seção personalizada&quot; na parte inferior do painel foi renomeado para &quot;Adicionar painel&quot; para explicar melhor sua função.

## Ativar a rotação automática do token de atualização nos aplicativos OAuth2 personalizados

Para permitir que você tenha mais controle sobre a segurança dos aplicativos OAuth2 personalizados, adicionamos a opção para habilitar a rotação do token de atualização. Quando essa opção é ativada, sempre que um token de atualização é usado, seu aplicativo cria e envia automaticamente um novo token de atualização e desativa o antigo.

Seu aplicativo deve armazenar o novo token de atualização após cada atualização. A Workfront não armazena esse token de atualização.

Anteriormente, os tokens de atualização expiravam após um período definido definido nas configurações personalizadas do aplicativo OAuth2.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).

## Use o PKCE em suas integrações OAuth2 personalizadas para aplicativos web de página única

Agora você pode criar aplicativos web de página única em suas integrações personalizadas usando o PKCE. O PKCE é um fluxo de autorização seguro que funciona bem com a atualização dinâmica de aplicativos, como aplicativos móveis, mas é valioso em todos os clientes OAuth2. Em vez de um segredo de cliente estático, o PKCE usa uma string gerada dinamicamente, eliminando o risco de um segredo de cliente vazado.

Anteriormente, as opções disponíveis para aplicativos OAuth2 personalizados usavam o nome de usuário e a senha ou um segredo do cliente.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](/help/quicksilver/administration-and-setup/configure-integrations/create-oauth-application.md).
