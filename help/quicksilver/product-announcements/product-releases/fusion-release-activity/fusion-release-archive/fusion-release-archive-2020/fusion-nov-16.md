---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: "Atividade da versão do Workfront Fusion: Semana de 16 de novembro de 2020"
description: Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 16 de novembro de 2020.
author: Luke
feature: Product Announcements, Workfront Fusion
exl-id: 9221a69e-2482-478b-95a9-f62dd28538d6
hidefromtoc: true
source-git-commit: e18b23e7d58aced4c95c5df51769a6e959fa3d57
workflow-type: tm+mt
source-wordcount: '475'
ht-degree: 0%

---

# Atividade de lançamento do Workfront Fusion: semana de 16 de novembro de 2020

Esta página descreve todas as melhorias feitas no Adobe Workfront Fusion na semana de 16 de novembro de 2020.

Para obter uma lista de todas as alterações recentes, consulte [Atividade de versão do Adobe Workfront Fusion](../../../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Para obter uma lista de correções de erros recentes no Workfront Fusion, consulte o [Atualizações de manutenção do Workfront](https://one.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350) e verifique se há atualizações rotuladas como Atualização de manutenção do Workfront Fusion.

## Atualizações no conector da Jira Cloud

Para expandir as maneiras de usar o conector da Jira Cloud, adicionamos três novos módulos:

* Adicionar problema à impressão
* Listar Registros
* Procurar Registros

Também atualizamos módulos existentes para suportar o tipo de objeto &quot;Sprint&quot;. Anteriormente, o objeto &quot;Sprint&quot; só podia ser acessado por meio do módulo Chamada de API personalizada.

Para obter mais informações, consulte [Módulos de software Jira](../../../../../workfront-fusion/apps-and-their-modules/jira-software-modules.md).

## A ID de execução agora está disponível para mapeamento em cenários

A ID de execução de um cenário agora está disponível no painel de mapeamento. Essa ID representa uma execução específica do cenário e pode ser usada como metadados. Por exemplo, a ID de execução pode ser salva com um registro criado pelo Fusion, para que você possa determinar posteriormente qual execução do Fusion criou o registro. Você pode encontrar a ID de execução no painel de mapeamento, em Funções gerais.

Para obter mais informações sobre execuções de cenário, consulte [Execução, ciclos e fases do cenário no Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

## Atalhos de teclado para cenários do Workfront Fusion 2.0

Para tornar a criação de cenários mais conveniente, adicionamos alguns atalhos do teclado:

* Ctrl/Cmd+Shift+Enter: Executar um cenário uma vez
* Ctrl/Cmd + Shift + S: Salvar um cenário

Para obter mais informações sobre a criação de cenários do Workfront Fusion 2.0, consulte [Criar um cenário no Adobe Workfront Fusion](../../../../../workfront-fusion/scenarios/create-a-scenario.md).

## Atualizações para o conector do Office 365 Excel

Para expandir as maneiras de usar o conector do Office 365 Excel, adicionamos alguns novos módulos. Agora é possível:

* Acionar um módulo das alterações para pastas de trabalho
* Pesquisar ou baixar pastas de trabalho
* Listar planilhas, linhas de planilha, tabelas ou linhas de tabela
* Atualizar uma tabela ou linha de planilha
* Excluir uma tabela ou linha de planilha
* Recuperar metadados para uma tabela
* Efetuar uma chamada de API personalizada

Os módulos disponíveis anteriormente ainda estão presentes no aplicativo.

Para obter mais informações, consulte [Módulos Excel do Microsoft Office 365](../../../../../workfront-fusion/apps-and-their-modules/microsoft-365-excel-modules.md).

## Usar o OAuth 2.0 nas conexões do aplicativo Workfront

Atualizamos o conector do Workfront para usar o OAuth 2.0. Essa atualização significa que é mais fácil fazer alterações nas conexões do aplicativo Workfront. Por exemplo, se algo sobre sua conexão mudar (como uma senha), você não precisará mais atualizar cada conexão individual em seus cenários. Além disso, o OAuth2 oferece outros benefícios, como a melhoria da segurança e a capacidade de usar o Logon único (SSO).

As conexões existentes não exigem alterações no momento. No entanto, você pode reautorizar conexões existentes se quiser aproveitar os benefícios do OAuth 2.0.

Para obter mais informações, consulte [Módulos Adobe Workfront](../../../../../workfront-fusion/apps-and-their-modules/workfront-modules.md).
