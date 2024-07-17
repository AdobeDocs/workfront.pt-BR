---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Exportar dados históricos do Adobe Workfront: prós e contras"
description: Este artigo explica os prós e contras de quatro opções que você pode usar para exportar dados históricos do Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: ed40984f-602a-46e9-a72b-141936de8fcb
source-git-commit: 5d7ff744ed0721ffa6d793a224226f28a76c57a0
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Exportar dados históricos do [!DNL Adobe Workfron]t: prós e contras

Este artigo explica os prós e contras de quatro opções que você pode usar para exportar dados históricos de [!DNL Workfront].

## Use um de nossos parceiros

O [!DNL AtAppStore], um parceiro certificado do [!DNL Workfront], tem um aplicativo fácil de usar que permite baixar os dados. Esse aplicativo também inclui um visualizador que permite visualizar facilmente seus dados.

* **Vantagens:** todos os objetos do [!DNL Workfront] são exportados, incluindo os campos personalizados. A interface do Visualizador é fácil de usar e ler, e é facilmente importável em um Banco de Dados do [!DNL MS Access].

* **Contras:** os documentos não são exportados. Você terá que baixá-los separadamente. Para obter mais informações, acesse [http://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx.](https://www.atappstore.com/App/snapshot-to-msaccess/Default.aspx)

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
