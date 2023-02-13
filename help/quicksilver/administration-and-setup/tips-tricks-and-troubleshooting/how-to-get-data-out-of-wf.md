---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Exportar dados históricos do Adobe Workfront: Prós e contras'
description: Este artigo explica os prós e contras de 4 opções que podem ser usadas para exportar dados históricos do Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: f3af39e760b2b407cda5ab78497cdc775defdcf6
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Exportar dados históricos de [!DNL Adobe Workfron]t: Prós e contras

Este artigo explica os prós e contras de 4 opções que podem ser usadas para exportar dados históricos de [!DNL Workfront].

## Usar um de nossos parceiros

[!DNL AtAppStore], a [!DNL Workfront] parceiro certificado, tem um aplicativo fácil de usar que permite baixar os dados. Este aplicativo também inclui um visualizador que permite que você visualize seus dados facilmente.

* **Vantagens:** Todos os seus [!DNL Workfront] são exportados, incluindo os campos personalizados. A interface do Visualizador é fácil de usar e ler, e é facilmente importante em um [!DNL MS Access] Banco de dados.

* **Desvantagens:** Os documentos não são exportados. Você terá que baixá-los separadamente. Para obter mais informações, acesse [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

## Solicitar um [!DNL Postgres] arquivo de despejo de dados da equipe de banco de dados

Seu Executivo de Conta pode enviar uma solicitação para nossa equipe de Banco de Dados para exportar um arquivo de despejo de banco de dados (.dmp [!DNL Postgres] com seus dados. Uma solicitação adicional será enviada à equipe do AOS para recuperar todos os documentos armazenados.

* **Prós**: Você recebe todo o carregamento de dados, incluindo campos personalizados, bem como documentos armazenados no sistema.

* **Desvantagens**: O arquivo de banco de dados é difícil de ler: não há como ler esse arquivo a menos que você o carregue para um [!DNL Postgres] banco de dados e restabelecer as relações entre as tabelas. Os documentos são armazenados em um servidor de arquivos separado e devem ser extraídos separadamente usando um processo separado pela equipe do AOS. Ao fazer isso, não há organização nos documentos e todos eles são referenciados pelo GUID.
* **Custo**: Há um custo associado a esse download, dependendo de quanto tempo a equipe leva para criar o arquivo. Consulte o AEM/CAE para obter mais informações ou iniciar esse processo.

## Exportar via [!UICONTROL Primeiros Passos]

Se você tiver horário de consultoria remota ou não, poderá usar um de nossos consultores para exportar seus dados na forma de relatórios ou [!UICONTROL início]ou você mesmo pode executar esses relatórios:

* **Prós**: Os relatórios são fáceis de ler e podem ser importados numa variedade de aplicações; eles podem ser personalizados para incluir agrupamentos e exibições desejados.

* **Desvantagens**: Os documentos terão de ser descarregados separadamente.

* **Custo**: É gratuito se você puder executar os relatórios por conta própria (tudo o que você precisaria é um logon de administrador do sistema) ou se poderá usar as horas restantes de consultoria remota. Se você estiver interessado em adquirir consultoria remota para isso, entre em contato com o AEM/CAE.

   Para obter mais informações sobre como usar o Kick-Starts para exportar dados, consulte [Exportar dados de [!DNL Adobe Workfront] via [!UICONTROL Primeiros Passos]](../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

## Usar nossa API aberta

se você tiver os recursos certos em sua organização, eles poderão criar uma API personalizada para recuperar todos os seus dados do Workfront:

* **Prós**: Você está controlando quais exportações do sistema.

* **Desvantagens**: O tempo é gasto do seu lado e você terá que encontrar recursos para codificar a API e executar a exportação.

* **Custo**: Interno para sua organização.
