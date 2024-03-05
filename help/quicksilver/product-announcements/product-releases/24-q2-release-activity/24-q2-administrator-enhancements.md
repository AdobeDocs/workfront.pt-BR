---
title: Aprimoramentos do administrador no segundo trimestre de 2024
description: Aprimoramentos do administrador no segundo trimestre de 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
source-git-commit: 2551089a20d3301ff1cf7dd633114dbb5235e959
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 0%

---

# Aprimoramentos do administrador no segundo trimestre de 2024

Esta página descreve todas as melhorias de administrador feitas com a versão do segundo trimestre de 2024 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do segundo trimestre de 2024, consulte [Visão geral da versão do segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## A integração JumpSeat agora está disponível para novos tipos de pacote

>[!NOTE]
>
>Versão de pré-visualização: 26 de fevereiro de 2024; Produção para lançamento rápido: Com o lançamento da versão 24.3 (14 de março de 2024); Produção para todos os clientes: 24.4 (abril de 2024)

A integração do JumpSeat existente agora está disponível para contas que usam um dos novos tipos de pacote (ou seja, Select, Prime ou Ultimate). Você ainda deve ter uma assinatura ativa do JumpSeat para habilitar a integração.

Para obter mais informações sobre a integração do JumpSeat, consulte [Configurar a integração do JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Os campos nativos do Workfront estão disponíveis no designer de formulário beta

>[!NOTE]
>
>Versão de pré-visualização: 29 de fevereiro de 2024; Produção para lançamento rápido: Com o lançamento da versão 24.3 (14 de março de 2024); Produção para todos os clientes: 24.4 (abril de 2024)

Os campos nativos do Workfront agora estão disponíveis para você adicionar aos seus formulários personalizados. Esse novo tipo de campo permite organizar e apresentar dados aos usuários de forma lógica, sem precisar recriar dados existentes em campos personalizados.

Depois de selecionar Campo nativo na lista de campos de formulários personalizados para adicionar o campo ao designer do formulário, você pode selecionar qualquer campo nativo para os objetos do formulário. Por exemplo, se a lista Tipos de objeto na parte superior do designer do formulário mostrar Projeto, você poderá selecionar campos nativos para projetos, mas não campos específicos para tarefas.

Quando o formulário personalizado é anexado a um objeto, o campo é preenchido a partir dos dados do objeto. Por exemplo, o campo Descrição em um formulário personalizado anexado a um projeto extrairá a descrição do projeto. (O campo pode mostrar &quot;N/D&quot; se nenhum dado estiver disponível.)

Os campos nativos usados em formulários personalizados ficam disponíveis na biblioteca de campos no designer para reutilização. Eles também ficam visíveis na área Configurar > Forms personalizados > Campos para que você possa ver em quais formulários são usados.

Esse recurso está disponível somente no designer de formulário beta, não no construtor de formulário herdado.

Os artigos de Experience League para esse recurso serão atualizados até 7 de março.

## O mapeamento de atributos agora está disponível para organizações que migraram para o Adobe IMS

>[!NOTE]
>
>Versão de pré-visualização: 22 de fevereiro de 2024; Produção para todos os clientes: 22 de fevereiro de 2024

Os administradores de sistema do Workfront agora podem configurar o mapeamento de atributos do usuário para organizações que migraram para o Adobe IMS. Isso permite que as informações do usuário sejam passadas para o Workfront pelo provedor de SSO (Logon único) da organização, para que os dados do usuário não precisem ser inseridos no Workfront e no provedor de SSO.

Anteriormente, essa funcionalidade só estava disponível para organizações que ainda não tinham sido integradas ao Adobe IMS.

Para obter instruções sobre como configurar o mapeamento de atributos, consulte **Mapear atributos do usuário na experiência unificada do Adobe** no artigo [Mapear atributos do usuário e provisionar automaticamente novos usuários](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md).

## A lógica de salto e a lógica de exibição agora estão disponíveis no designer de formulário beta

>[!NOTE]
>
>Versão de pré-visualização: 8 de fevereiro de 2024; Produção para lançamento rápido: Com o lançamento 24.2 (15 de fevereiro de 2024); Produção para todos os clientes: a ser definido

Agora é possível editar a exibição existente, ignorar a lógica e adicionar uma nova lógica aos formulários personalizados no designer de formulário beta. Um construtor de lógica fácil de usar ajuda a definir quais campos exibir ou ignorar com base nas seleções no formulário.

Os ícones em um campo na tela do designer do formulário indicam que a lógica está configurada nesse campo ou que o campo é usado em regras de lógica configuradas em outros campos.

Para obter mais informações, consulte [Adicionar lógica de exibição e lógica de salto com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).