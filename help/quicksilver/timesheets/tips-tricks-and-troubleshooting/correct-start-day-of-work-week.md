---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Corrigir o dia de início da semana de trabalho para Planilhas de Horas
description: O dia de início da semana em minha folha de horas não corresponde ao dia de início da semana configurado em meu perfil de folha de horas.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: d5d517a0c9a1292c37e66db07f7ed17d0a9a59e1
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Corrigir o dia de início da semana de trabalho para Planilhas de Horas

## Problema

O dia de início da semana em minha folha de horas não corresponde ao dia de início da semana configurado em meu perfil de folha de horas (conforme descrito em [Criar, editar e atribuir perfis de folha de horas](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).)

## Solução

O dia de início da semana de uma folha de horas no Adobe Workfront usa as configurações de idioma e localidade no navegador para determinar o dia da semana. Por causa disso, você precisa atualizar as configurações de idioma e localidade do seu navegador.

Por exemplo, com o idioma do navegador definido como inglês e o local definido como Estados Unidos, a semana começa no domingo. Como alternativa, o idioma do navegador é definido como inglês e o local é definido como Reino Unido, o dia de início é segunda-feira.

Essa configuração também afeta o dia de início da semana nos calendários pop-up em todo o sistema.

A alteração do local não afeta o dia de início da semana na Grade de Recursos (ou na exibição da grade de recursos). A semana sempre começa no domingo.

A seguir estão as instruções para alterar as configurações de idioma e local para vários navegadores compatíveis com o Workfront.

* **Chrome:** Copie e cole o seguinte link no navegador do Chrome: `chrome://settings/languages` e vá para Idiomas.
* **Firefox:**&#x200B;copie e cole o seguinte link no navegador Firefox: `about:preferences#content` e vá para Idiomas.
* **IE 11:** Ferramentas -> Opções da Internet -> Geral -> Idiomas
* **Safari:** infelizmente, o Safari não permite a alteração de idiomas de navegação na Web sem também alterar todo o idioma do sistema operacional. Provavelmente, é mais fácil simplesmente instalar outro navegador, como o Chrome ou o Firefox.


