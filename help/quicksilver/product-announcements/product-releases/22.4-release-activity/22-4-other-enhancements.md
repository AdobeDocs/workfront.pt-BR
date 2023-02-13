---
title: 2.4 Outras melhorias
description: 2.4 Outras melhorias
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 4e41eed3-1a3b-4247-8c0c-630efc9c1b69
source-git-commit: 0fea13b0a1d8f14c2d601e0ed0a8d15684a3c4d7
workflow-type: tm+mt
source-wordcount: '588'
ht-degree: 0%

---

# 2.4 Outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 2.4 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados na semana de 3 de outubro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.4, consulte [Visão geral da versão 2.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Adobe Workfront para InDesign

Este plug-in agora está disponível para instalação no InDesign. Ele permite acessar detalhes de itens de trabalho, colaborar com colegas na área Atualizações e enviar provas para revisão sem deixar XD. Vá para o Adobe Creative Cloud Marketplace para baixar o plug-in hoje mesmo.

Para obter mais informações sobre o plug-in, consulte [[!DNL Adobe Workfront] plugin for [!DNL Creative Cloud] Aplicativos](/help/quicksilver/workfront-integrations-and-apps/adobe-workfront-for-creative-cloud/wf-adobe-cc.md).

[Baixe o Adobe Workfront para InDesign no marketplace hoje](https://exchange.adobe.com/apps/cc/108938/adobe-workfront-for-indesign).

Os administradores também podem [criar um pacote com os plug-ins](https://helpx.adobe.com/in/enterprise/using/manage-extensions.html) do Admin Console e implantar em usuários de maneira gerenciada ou autogerenciada.

## Sincronizar metadados do objeto com a integração nativa do Experience Manager Assets

Agora, os campos de portfólio, programa, projeto, tarefa, problema e documento do Workfront são atualizados automaticamente quando o campo é alterado no Workfront.

Para permitir a sincronização automática dos metadados do objeto, é necessário ativar a alternância de metadados do objeto de sincronização para suas integrações em Configurar > Integrações do Experience Manager.

Anteriormente, somente os campos do projeto eram atualizados automaticamente.

Para obter mais informações, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

## Os metadados enviam objetos pai de programa e portfólio

Agora, quando um ativo é enviado pela primeira vez para o Experience Manager Assets ou Assets Essentials, qualquer metadado configurado para mapear objetos pai de programa e portfólio também é enviado.

Anteriormente, somente os dados do projeto pai eram enviados.

Para obter mais informações, consulte [Enviar um documento para o Experience Manager Assets ou Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/send-to-aem.md).

## Descrição da equipe expandida

Na área Equipes, agora é possível exibir a descrição completa da equipe clicando na descrição para exibi-la em um pop-up. Todos os URLs na descrição são clicáveis no pop-up e você pode clicar no texto da descrição para editá-los (se tiver acesso para editar as configurações do grupo).

Anteriormente, a rolagem pela descrição em uma área estreita era a única maneira de visualizar todo o conteúdo.

Esse aprimoramento na descrição se aplica a equipes ágeis e não ágeis.

Para obter mais informações, consulte [Criar um grupo](/help/quicksilver/people-teams-and-groups/create-and-manage-teams/create-a-team.md).

## Campanhas do Workfront (Beta) - uma nova maneira de gerenciar seu trabalho

>[!NOTE]
>
>Esse recurso foi originalmente introduzido na Visualização durante o ciclo de versão 2.3.

>[!NOTE]
>
>Essa funcionalidade está disponível somente como um beta e está em construção no momento. Continuaremos a adicionar recursos para o fluxo de trabalho do Campaign com versões futuras. A participação no programa beta para Campanhas Workfront é voluntária.

Estamos introduzindo um novo objeto no Adobe Workfront que tem o potencial de mudar a maneira como você gerencia o trabalho.

As Campanhas do Workfront permitem organizar projetos de diferentes portfólios e programas em um novo contêiner de trabalho. Esse novo contêiner evoluirá em versões futuras para eventualmente incluir todos os objetos de trabalho que estão gerenciados no momento em silos separados.

Os seguintes recursos estão incluídos nesta versão:

* Um novo objeto do Workfront chamado Campaign

* Uma nova área Campanhas (Beta) no Menu principal

* Uma lista de campanhas na área Campanhas

* Uma página Detalhes da campanha que exibe informações adicionais sobre uma campanha

* Capacidade de adicionar projetos a uma campanha

* Capacidade de editar informações sobre uma campanha

* Capacidade de renomear o objeto da campanha a partir do modelo de layout

   Os administradores de sistema e de grupo do Workfront podem adicionar a área Campanhas (Beta) no Menu principal de um modelo de layout. Isso o disponibiliza para todos os usuários atribuídos ao modelo. Depois que estiver disponível, qualquer pessoa no Workfront poderá criar uma campanha.


