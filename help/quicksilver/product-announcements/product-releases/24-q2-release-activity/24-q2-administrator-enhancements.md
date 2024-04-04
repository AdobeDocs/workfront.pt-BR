---
title: Aprimoramentos do administrador no segundo trimestre de 2024
description: Aprimoramentos do administrador no segundo trimestre de 2024
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a297ee8d-d949-45ab-a219-437316fa8fa3
source-git-commit: c2513beb50867fe1e1d065037a068a846f96d50b
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Aprimoramentos do administrador no segundo trimestre de 2024

Esta página descreve todas as melhorias de administrador feitas com a versão do segundo trimestre de 2024 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do segundo trimestre de 2024, consulte [Visão geral da versão do segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).

## A lógica de exibição e a lógica de salto agora estão disponíveis no modo de visualização do designer de formulário

>[!NOTE]
>
>Versão de pré-visualização: 28 de março de 2024; Produção para todos os clientes: 24.4 (11 de abril de 2024)

O designer de formulário personalizado beta agora permite testar a lógica de exibição e ignorar a lógica no modo de visualização. Anteriormente, todos os campos eram exibidos na visualização mesmo quando a lógica era aplicada.

Para obter mais informações sobre a visualização de um formulário personalizado no designer do formulário, consulte [Organizar e visualizar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).

## Agora, empresas e usuários oferecem suporte a campos de formulário personalizados avançados

>[!NOTE]
>
>Versão de pré-visualização: 14 de março de 2024; Produção para todos os clientes: 24.4 (11 de abril de 2024)

Recursos avançados de formulário personalizado, como campos de Pesquisa externa e campos nativos do Workfront, agora estão disponíveis quando você anexa um formulário personalizado a uma empresa ou usuário. Os recursos avançados estão disponíveis nas páginas Detalhes da empresa e Detalhes do usuário, não nas caixas de diálogo Editar empresa e Editar usuário. O formulário personalizado deve ser criado no novo designer de formulário para aproveitar esses tipos de campo.

Para obter mais informações sobre campos de formulário personalizados, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## A integração JumpSeat agora está disponível para novos tipos de pacote

>[!NOTE]
>
>Versão de pré-visualização: 26 de fevereiro de 2024; Produção para lançamento rápido: Com o lançamento do 24.3 (14 de março de 2024); Produção para todos os clientes: 24.4 (11 de abril de 2024)

A integração do JumpSeat existente agora está disponível para contas que usam um dos novos tipos de pacote (ou seja, Select, Prime ou Ultimate). Você ainda deve ter uma assinatura ativa do JumpSeat para habilitar a integração.

Para obter mais informações sobre a integração do JumpSeat, consulte [Configurar a integração do JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Os campos nativos do Workfront estão disponíveis no designer de formulário beta

>[!NOTE]
>
>Versão de pré-visualização: 29 de fevereiro de 2024; Produção para lançamento rápido: Com o lançamento do 24.3 (14 de março de 2024); Produção para todos os clientes: 24.4 (11 de abril de 2024)

Os campos nativos do Workfront agora estão disponíveis para você adicionar aos seus formulários personalizados. Esse novo tipo de campo permite organizar e apresentar dados aos usuários de forma lógica, sem precisar recriar dados existentes em campos personalizados.

Depois de selecionar Campo nativo na lista de campos de formulários personalizados para adicionar o campo ao designer do formulário, você pode selecionar qualquer campo nativo para os objetos do formulário. Por exemplo, se a lista Tipos de objeto na parte superior do designer do formulário mostrar Projeto, você poderá selecionar campos nativos para projetos, mas não campos específicos para tarefas.

Quando o formulário personalizado é anexado a um objeto, o campo é preenchido a partir dos dados do objeto. Por exemplo, o campo Descrição em um formulário personalizado anexado a um projeto extrairá a descrição do projeto. (O campo pode mostrar &quot;N/D&quot; se nenhum dado estiver disponível.)

Os campos nativos usados em formulários personalizados ficam disponíveis na biblioteca de campos no designer para reutilização. Eles também ficam visíveis na área Configurar > Forms personalizados > Campos para que você possa ver em quais formulários são usados.

Esse recurso está disponível somente no designer de formulário beta, não no construtor de formulário herdado.

Para obter mais informações, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3427702/){target=_blank}

## O mapeamento de atributos agora está disponível para organizações que migraram para o Adobe IMS

>[!NOTE]
>
>Versão de pré-visualização: 22 de fevereiro de 2024; Produção para todos os clientes: 22 de fevereiro de 2024

Os administradores de sistema do Workfront agora podem configurar o mapeamento de atributos do usuário para organizações que migraram para o Adobe IMS. Isso permite que as informações do usuário sejam passadas para o Workfront pelo provedor de SSO (Logon único) da organização, para que os dados do usuário não precisem ser inseridos no Workfront e no provedor de SSO.

Anteriormente, essa funcionalidade só estava disponível para organizações que ainda não tinham sido integradas ao Adobe IMS.

Para obter instruções sobre como configurar o mapeamento de atributos, consulte [Mapear atributos do usuário na experiência unificada do Adobe](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) no artigo **Mapear atributos do usuário e provisionar automaticamente novos usuários**.

## A lógica de salto e a lógica de exibição agora estão disponíveis no designer de formulário beta

>[!NOTE]
>
>Versão de pré-visualização: 8 de fevereiro de 2024; Produção para lançamento rápido: Com o lançamento 24.2 (15 de fevereiro de 2024); Produção para todos os clientes: a ser definido

Agora é possível editar a exibição existente, ignorar a lógica e adicionar uma nova lógica aos formulários personalizados no designer de formulário beta. Um construtor de lógica fácil de usar ajuda a definir quais campos exibir ou ignorar com base nas seleções no formulário.

Os ícones em um campo na tela do designer do formulário indicam que a lógica está configurada nesse campo ou que o campo é usado em regras de lógica configuradas em outros campos.

Para obter mais informações, consulte [Adicionar lógica de exibição e lógica de salto com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md).
