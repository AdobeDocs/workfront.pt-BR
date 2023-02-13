---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: Corrija o dia de início da semana de trabalho para Folhas de Horas
description: O dia de início da semana na minha folha de ponto não corresponde ao dia de início da semana configurado no meu perfil de folha de ponto.
author: Alina
feature: Timesheets
exl-id: 5c6c100f-2a04-4a6b-9f95-acc8de3a90f1
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 0%

---

# Corrija o dia de início da semana de trabalho para Folhas de Horas

## Problema

O dia de início da semana na minha folha de horas não corresponde ao dia de início da semana configurado no meu perfil da folha de horas (como descrito em [Criar, editar e atribuir perfis de folha de ponto](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).).

## Solução

O dia de início da semana de uma folha de ponto no Adobe Workfront usa as configurações de idioma e local no navegador para determinar o dia da semana. Por causa disso, é necessário atualizar o idioma e as configurações de local do navegador. 

Por exemplo, com o idioma do navegador definido como inglês e a localidade definida como Estados Unidos, a semana começa no domingo. Como alternativa, o idioma do navegador definido como inglês e a localidade definida como Reino Unido, o dia de início é segunda-feira.

Essa configuração também afeta o dia de início da semana nos calendários pop-up do sistema.

A alteração de local não afeta o dia de início da semana na Grade de Recurso (ou exibição de grade de recursos). A semana sempre começa no domingo.

A seguir estão as instruções para alterar as configurações de idioma e local para vários navegadores compatíveis com o Workfront.

* **Chrome:** Copie e cole o seguinte link no navegador Chrome: `chrome://settings/languages` em seguida, vá para Languages.
* **Firefox:**Copie e cole o seguinte link no navegador Firefox: `about:preferences#content` em seguida, vá para Languages.
* **IE 11:** Ferramentas -> Opções da Internet -> Geral -> Idiomas
* **Safari:** Infelizmente, o Safari não permite a alteração de idiomas de navegação na Web sem também alterar todo o idioma do sistema operacional. Provavelmente, é mais fácil simplesmente instalar outro navegador como o Chrome ou o Firefox.

 
