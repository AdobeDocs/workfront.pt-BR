---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exportar dados históricos do Adobe Workfront: vantagens e desvantagens"
description: Este artigo explica os prós e contras de quatro opções que você pode usar para exportar dados históricos do Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---

# Exportar dados históricos do [!DNL Adobe Workfron]t: prós e contras

Este artigo explica os prós e contras de quatro opções que você pode usar para exportar dados históricos de [!DNL Workfront].

## Use um de nossos parceiros

O [!DNL AtAppStore] ([www.atappstore.com](https://www.atappstore.com)) tem um aplicativo fácil de usar (sua solução [Instantâneo do Workfront](https://store.atappstore.com/product/workfront-snapshot/)) que permite que você baixe os dados sozinho. Um visualizador opcional (sua solução [Visualizador de Instantâneos do Workfront](https://store.atappstore.com/product/workfront-snapshot-viewer/)) permite que você exiba facilmente seus dados offline.

* **Vantagens:** todos os objetos [!DNL Workfront] principais são exportados, incluindo os campos e anotações personalizados, que são armazenados em um banco de dados do [!DNL MS Access] de fácil acesso. A interface do Visualizador é fácil de usar e ler. A extração de documentos também está disponível separadamente como um serviço, com a saída organizada em uma estrutura de pastas lógica que mapeia para cada documento (e, opcionalmente, suas versões anteriores).

* **Contras:** Há uma limitação técnica de 2 GB de dados, mas a AtAppStore permite que você compre apenas o que precisa.

* **Custos:** Para obter mais informações, vá para [https://store.atappstore.com/product/workfront-snapshot/](https://store.atappstore.com/product/workfront-snapshot/).

## Solicitar um arquivo de despejo de dados [!DNL Postgres] da nossa equipe do banco de dados

Seu Executivo de contas pode enviar uma solicitação para nossa equipe do banco de dados para exportar um arquivo de despejo de banco de dados (arquivo .dmp [!DNL Postgres]) com seus dados. Uma solicitação adicional será enviada para nossa equipe do AOS para recuperar todos os documentos armazenados.

* **Vantagens**: você obtém toda a sua carga de dados, incluindo campos personalizados, bem como documentos que são armazenados no sistema.

* **Contras**: O arquivo de banco de dados é difícil de ler: não há como ler este arquivo, a menos que você carregue-o para um banco de dados [!DNL Postgres] e restabeleça as relações entre as tabelas. Os documentos são armazenados em um servidor de arquivos separado e devem ser extraídos separadamente usando um processo separado pela equipe do AOS. Ao fazer isso, não há organização para os documentos e todos são referenciados por seu GUID.

* **Custo**: há um custo associado a este download, dependendo do tempo que a equipe leva para criar o arquivo. Consulte seu AE/CAE para obter mais informações ou para iniciar esse processo.

## Exportar via [!UICONTROL Kick-Starts]

Independentemente de você ter horas de consultoria remota ou não, você pode usar um de nossos consultores para exportar seus dados na forma de relatórios ou de [!UICONTROL inícios], ou pode executar esses relatórios você mesmo:

* **Vantagens**: os relatórios são fáceis de ler e podem ser importados em diversos aplicativos; eles podem ser personalizados para incluir quaisquer agrupamentos e modos de exibição que você desejar.

* **Contras**: os documentos terão que ser baixados separadamente.

* **Custo**: é gratuito se você puder executar os relatórios sozinho (basta um logon de administrador do sistema) ou se puder usar as horas restantes de consultoria remota. Se você estiver interessado em adquirir consultoria remota para isso, entre em contato com seu AE/CAE.

  Para obter mais informações sobre como usar o Kick-Starts para exportar dados, consulte [Exportar dados de [!DNL Adobe Workfront] via [!UICONTROL Kick-Starts]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Use nossa API aberta

se você tiver os recursos certos em sua organização, eles poderão criar uma API personalizada para recuperar todos os dados da Workfront:

* **Vantagens**: você controla quais exportações do sistema.

* **Contras**: o tempo é gasto do seu lado e você terá que encontrar recursos para codificar a API e executar a exportação.

* **Custo**: interno para sua organização.
