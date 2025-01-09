---
title: Aprimoramentos do administrador no primeiro trimestre de 2025
description: Aprimoramentos do administrador no primeiro trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: fa24040d-0403-4799-b690-c3d172797115
source-git-commit: d2e3379e9390f2b419bb2d78b1999c8c2dd7d0d3
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

# Aprimoramentos do administrador no primeiro trimestre de 2025

Esta página descreve todas as melhorias de administrador feitas com a versão do Primeiro trimestre de 2025 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do Primeiro trimestre de 2025, consulte [Visão geral da versão do Primeiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md).

## Comparar objetos entre ambientes para promoção do ambiente

>[!NOTE]
>
>Versão de pré-visualização: 6 de janeiro de 2024; Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)

Para facilitar a determinação do objeto que deve ser incluído em um pacote de promoção de ambiente, adicionamos a capacidade de comparar objetos entre ambientes. Agora, você pode selecionar tipos de objetos e ambientes. O Workfront gera uma lista de objetos desse tipo, se eles estão presentes no ambiente de destino e se esse objeto tem diferenças entre o ambiente de origem e o ambiente de destino. Você pode então adicionar objetos a um pacote diretamente dessa lista.

Anteriormente, se um usuário quisesse comparar objetos entre ambientes, ele deveria verificar esses objetos manualmente.

Para obter mais informações, consulte [Comparar objetos entre ambientes](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-compare.md).

## Mais objetos disponíveis para promoção de ambiente

>[!NOTE]
>
>Versão de pré-visualização: 6 de janeiro de 2024; Versão de produção para todos os clientes: com a versão 25.1 (janeiro de 2025)

Para expandir os recursos da funcionalidade de promoção do ambiente, adicionamos mais objetos. Agora, é possível adicionar os seguintes objetos a um pacote de promoção de ambiente:

* Locais
* Cartões de tarifas
* Atribuições

Anteriormente, esses objetos não estavam disponíveis para promoção do ambiente.

Para obter mais informações sobre objetos disponíveis para promoção de ambiente, consulte [Objetos compatíveis para promoção de ambiente](/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/environment-promotion-in-wf.md#supported-objects-for-environment-promotion) no artigo Visão geral da promoção de ambiente.

## Impedir a movimentação de tarefas quando há Horas registradas

>[!NOTE]
>
>Versão de pré-visualização: 19 de dezembro de 2024; Versão de produção para todos os clientes: com a versão 25.1 (16 de janeiro de 2025)

Como a movimentação de tarefas ou problemas que registraram horas pode, às vezes, causar problemas de conformidade ou auditoria, adicionamos uma preferência na área Preferências de tarefas e problemas da Configuração que permite impedir que os usuários movam tarefas e problemas se houver horas registradas. Antes dessa melhoria, os usuários podiam mover tarefas e problemas para outros projetos, mesmo se houvesse horas registradas neles.

Para obter informações, consulte [Configurar preferências de tarefas e problemas do sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Preferência para usar projeto ou agendamento de usuário para tarefas de atribuição única

>[!NOTE]
>
>Versão de pré-visualização: 21 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (16 de janeiro de 2025)

Como administrador de sistema ou de grupo, agora você tem uma nova preferência para indicar se o Workfront deve usar o cronograma do projeto ou do usuário para calcular a linha do tempo do projeto ao atribuir um usuário a uma tarefa e se o projeto e o usuário estão associados a um cronograma. Antes desse aprimoramento, essa configuração existia para atribuições de vários usuários. A configuração agora está disponível para atribuições de usuário único a tarefas.

Para obter mais informações, consulte [Configurar preferências de projeto do sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Agora as regras de negócios oferecem suporte a hiperlinks

>[!NOTE]
>
>Versão de pré-visualização: 21 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (16 de janeiro de 2025)

Agora é possível incluir hiperlinks na mensagem de erro personalizada de uma regra de negócios para orientar o usuário sobre como modificar sua ação dentro da restrição da regra. O URL estático pode vincular à documentação ou outras páginas que seriam úteis para o usuário.

Para obter informações, consulte [Criar e editar regras de negócios](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

## A filtragem em campos de digitação antecipada nativos agora está disponível

>[!NOTE]
>
>Versão de pré-visualização: 21 de novembro de 2024; Produção para lançamento rápido: Com o lançamento 24.12 (12 de dezembro de 2024); Produção para lançamento trimestral: Com o lançamento 25.1 (16 de janeiro de 2025)

Quando você adiciona uma referência de campo nativo a um formulário personalizado e ela faz referência a um campo de digitação antecipada (como Portfolio, Empresa ou Proprietário), uma opção de filtro está disponível. O filtro permite limitar os objetos que os usuários podem escolher quando estão usando o campo. Esse filtro personalizado funciona da mesma forma que um filtro em um campo de digitação antecipada personalizado, usando o Modo de texto para definir o filtro.

Para obter informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Ícone &quot;Mover para&quot; adicionado a campos personalizados

>[!NOTE]
>
>Versão de pré-visualização: 29 de outubro de 2024; Produção para lançamento rápido: Com o lançamento do 24.11 (14 de novembro de 2024); Produção para lançamento trimestral: Com o lançamento do 25.1 (16 de janeiro de 2025)

Quando um formulário personalizado contém várias seções com muitos campos, pode ser difícil mover um campo de uma seção para outra arrastando e soltando. Um ícone &quot;mover para&quot; foi adicionado a cada campo, permitindo selecionar a seção em que o campo é colocado.

Para obter mais informações, consulte [Organizar e visualizar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md).
