---
title: Aprimoramentos no gerenciamento de documentos e provas do terceiro trimestre de 2025
description: Aprimoramentos no gerenciamento de documentos e provas do terceiro trimestre de 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4829d487-7041-447f-9a68-fb1acf467734
source-git-commit: 9948927b4f61e0bafd815951bfaede0da064ef91
workflow-type: tm+mt
source-wordcount: '652'
ht-degree: 0%

---

# Aprimoramentos no gerenciamento de documentos e provas do terceiro trimestre de 2025

Esta página descreve todas as melhorias de gerenciamento de documentos feitas com a versão do terceiro trimestre de 2025 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2025, consulte [Visão geral da versão do terceiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

<!--## Adobe Express and Workfront Proof integration

We are excited to announce a new integration between Adobe Express and Workfront Proof.

With this integration, you can 

* Streamline collaboration between creative, legal, and compliance teams to reduce time-to-publish while maintaining oversight  

* Conduct for deep reviews using drawing markups, annotations, and commenting with the Workfront proofing viewer 

* Meet enterprise compliance standards with electronic signatures and full audit logs 

* Require approval on any remixed files from an Express branded template  

* Map an Express template to a multi-stage review and approval workflow using advanced proof templates

Note: The integration must be enabled for your accounts by the Adobe Product Team.

For more information, see [Get started with the Adobe Express and Workfront Proof integration](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-express.md).
-->

## Implantação em fases das aprovações unificadas

>[!NOTE]
>
>Versão de produção para clientes: implantação em fases a partir de 17 de julho de 2025


Estamos habilitando Aprovações unificadas, anteriormente conhecidas como Novas aprovações de documentos, em uma implantação em fases. Essa funcionalidade será ativada automaticamente na instância do Workfront nos próximos seis meses.

As Aprovações unificadas substituem as aprovações de documentos herdados e fornecem a seguinte funcionalidade diretamente em um documento:

* Designar uma equipe inteira do Workfront como revisores ou aprovadores
* Definir um prazo para a revisão ou aprovação
* Criar e reutilizar modelos de aprovação
* Utilizar novas versões
* Exibir vários indicadores-chave de desempenho para suas aprovações nos widgets da Página inicial do Workfront
* Usar Painéis do Canvas para exibir detalhes de relatórios sobre Aprovações unificadas

Para obter mais informações, consulte [Visão geral das aprovações unificadas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md).

## Atualização do visualizador de provas da área de trabalho

>[!NOTE]
>
>* Versão de produção para todos os clientes: 16 de junho de 2025

O Desktop Proofing Viewer foi atualizado para a versão 2.1.50.

Essa atualização inclui atualizações internas de ferramentas e não afeta a funcionalidade do usuário final.

Essa atualização é para Mac e Windows.

## Nova integração do Proofing e do GenStudio for Performance Marketing

>[!NOTE]
>
>* Versão de produção para todos os clientes: 12 de junho de 2025

Estamos animados em apresentar uma nova integração entre o Proofing e o GenStudio for Performance Marketing. Com essa integração, você pode

* Usar modelos de aprovação do Workfront para definir workflows de aprovação

* Revisar conteúdo de rascunho no visualizador de provas do Workfront

* Consulte decisões de revisão para aprovação final e publicação no GenStudio for Performance Marketing

### Requisitos de integração

O Workfront e o GenStudio for Performance Marketing devem ser implantados na mesma Organização IMS.

Para obter mais informações, consulte [Introdução à integração do GenStudio for Performance Marketing e do Workfront Proof](/help/quicksilver/workfront-integrations-and-apps/review-and-approval-integrations/wf-proof-and-genstudio.md).

## Atualização do visualizador de provas da área de trabalho

O Desktop Proofing Viewer foi atualizado para a versão 2.1.48.

Esta atualização é uma correção de problema para manter a compatibilidade do Desktop Viewer com os sistemas operacionais Mac. O elétron foi rebaixado para 34.4.0 e o cromo foi rebaixado para 132.

Essa atualização é para Mac e Windows.


## O Assets em uma pasta vinculada do Google deve ser adicionado individualmente para aparecer no Workfront

>[!NOTE]
>
>* Versão de pré-visualização: 2 de junho de 2025; Versão de produção para todos os clientes: 2 de junho de 2025

O Google está [aprimorando os controles de segurança](https://workspace.google.com/blog/product-announcements/enhancing-security-controls-for-google-drive-third-party-apps) para aplicativos de terceiros que acessam o Google Drive, exigindo que os aplicativos adotem um modelo de consentimento por usuário. Como resultado, os ativos individuais devem ser vinculados, um de cada vez, para ficarem visíveis no Workfront. Consulte [Configurar integrações de documentos](/help/quicksilver/administration-and-setup/configure-integrations/configure-document-integrations.md) para obter mais informações.

Principais recursos que permanecem inalterados:

* Pesquisar e filtrar ativos e pastas no modal do Google Drive
* Vincular ativos a objetos do Workfront a partir do Google Drive
* Faça upload de ativos no Google Drive por meio da lista suspensa &quot;Enviar para&quot; na página de documentos
* Exibir e acessar a estrutura de pastas na área Meu Drive de um usuário
* Vincular uma nova versão de um ativo do Google Drive a um documento existente no Workfront
* Vincular pastas a objetos do Workfront a partir do Google Drive
* Fazer upload de ativos no Google Drive arrastando e soltando documentos em uma pasta vinculada
* Criar um novo documento do Google Drive no Workfront


## Novos botões de decisão de aprovação de documento disponíveis no visualizador de provas

>[!IMPORTANT]
>
>Esse recurso faz parte de uma versão em fases e só está disponível para clientes específicos.

>[!NOTE]
>
>* Versão de pré-visualização: 10 de abril de 2025; Versão de produção para todos os clientes: 17 de abril de 2025

Os novos botões de decisão de aprovação de documento agora aparecem no visualizador de provas. Agora, ao criar uma prova simples e adicionar aprovadores e revisores a partir do Resumo do documento, eles podem tomar a decisão diretamente no visualizador de provas.

Anteriormente, era necessário sair do revisor de provas para tomar uma decisão.

As aprovações criadas antes desta versão não exibirão os botões no visualizador de provas.

Para obter mais informações, consulte [Usar novas aprovações e revisões de documentos juntas](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/doc-approvals-and-proofing.md).
