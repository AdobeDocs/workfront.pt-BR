---
title: 22.3 Aprimoramentos do administrador
description: 22.3 Aprimoramentos do administrador
author: Luke
draft: false
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# 22.3 Aprimoramentos do administrador

Esta página descreve todas as melhorias de Administrador feitas com a versão 22.3 no ambiente de Pré-visualização. Essas melhorias foram disponibilizadas na semana de 11 de julho de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.3, consulte [Visão geral da versão 22.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrar o Adobe Workfront com o JumpSeat

Agora é possível integrar o JumpSeat ao Workfront para criar orientação personalizada no produto para seus usuários. Você deve ter uma licença corporativa da Adobe Workfront e uma assinatura ativa do JumpSeat para habilitar a integração.

Para obter mais informações, consulte [Configurar a integração do JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Configurações padrão de prova movidas para o Workfront

Agora você pode editar as seguintes configurações de prova na Área de configuração do Workfront:

* Configurações padrão de prova

* Configurações de decisão da prova

Para obter mais informações, consulte [Definir configurações padrão de prova](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Usar status desbloqueados em um processo de aprovação

**Nota:** Removido da versão de Produção 22.3. O lançamento desse recurso está planejado para a produção em 15 de setembro de 2022.

Para oferecer mais controle sobre os processos de aprovação e os status no sistema, possibilitamos a criação de um processo de aprovação com base em um status de sistema desbloqueado. Além disso, agora é possível desbloquear qualquer status que já seja usado em um processo de aprovação.

Anteriormente, um status de sistema usado em um processo de aprovação tinha que ser bloqueado. Isso o tornou disponível para todos os grupos — sem a possibilidade de removê-lo ou renomeá-lo — de modo que os administradores de grupos não pudessem simplificar a lista de status do grupo para atender às suas necessidades específicas.

Para obter mais informações, consulte os seguintes artigos:

* [Criar um processo de aprovação para itens de trabalho](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Criar ou editar um status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Status bloqueados e desbloqueados no nível do sistema](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Adicionar um arquivo PDF a um formulário personalizado

Continuamos a ajudá-lo a tornar os formulários personalizados mais visuais e informativos com os novos widgets de ativos que você pode adicionar, como imagens e vídeos. Agora é possível adicionar um link para um arquivo PDF a um formulário personalizado. Quando o formulário é anexado a um objeto, os usuários que trabalham com o objeto podem visualizar e interagir com o PDF de dentro do formulário.

Para obter mais informações, consulte [Adicionar ou editar uma imagem ou outro widget de ativo em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## O editor de cálculo de campo de formulário personalizado exibe informações de erro

>[!NOTE]
>
>Este recurso está temporariamente indisponível. Esta página será atualizada quando o recurso estiver disponível.

A edição de cálculos para campos personalizados agora é mais fácil com informações de erro úteis indicadas diretamente no cálculo. Ao criar um campo calculado em um formulário personalizado, os erros são destacados em rosa. Quando você passa o mouse sobre a parte destacada, uma dica de ferramenta é exibida para descrever qual é o problema.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Personalização do cabeçalho do projeto

Como administrador de grupo ou Workfront, agora é possível personalizar os campos que são exibidos no cabeçalho de um projeto ao usar um Modelo de layout.

Essa atualização inclui os seguintes aprimoramentos:

* Remover campos existentes do cabeçalho do projeto.

* Adicionar novos campos de Visão geral do projeto não editáveis. Não é possível adicionar campos personalizados ou campos que podem ser editados. Campos editáveis que estão atualmente no cabeçalho do projeto podem permanecer no cabeçalho.

* O cabeçalho do objeto pode incluir até cinco campos.


Antes desta versão, os campos nos cabeçalhos do objeto não podiam ser personalizados.

Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Controle criando um projeto em branco

Como administrador de sistema ou de grupo, agora é possível controlar se os usuários podem criar projetos em branco, sem usar um modelo. Introduzimos uma nova configuração na área Preferências do projeto da Configuração que permite desativar a criação de projetos em branco nas seguintes áreas:

* Na opção Novo projeto em uma lista de projetos

* Ao converter um problema em um projeto a partir da página de problemas


A nova configuração é &quot;Permitir que usuários criem projetos sem usar um modelo&quot; e está habilitada por padrão.

**Nota:** Os usuários ainda podem converter uma tarefa em um projeto em branco.

Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Desativar um grupo na página Grupos

Recentemente, adicionamos a capacidade de desativar e reativar grupos. Para tornar essa ação mais rápida e fácil, a adicionamos à página de um grupo. Agora, depois de clicar no nome de um grupo para ir para a página dele, você pode selecionar o menu Mais ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) ao lado do nome do grupo, selecione Desativar ou Reativar.

Anteriormente, só era possível desativar ou reativar um grupo usando a caixa de seleção Está ativo na página Detalhes.

Para obter mais informações, consulte [Desativar ou reativar um grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Adicionar vídeos a formulários personalizados

Agora você pode fornecer um novo modo de informação, interesse visual e criatividade para um formulário personalizado ao adicionar um vídeo. Quando o formulário é anexado a um objeto, os usuários que trabalham com o objeto podem reproduzir o vídeo a qualquer momento.

Anteriormente, só era possível adicionar campos e imagens baseados em texto a um formulário personalizado.

Para obter mais informações, consulte [Adicionar ou editar um widget de ativo de imagem ou vídeo em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

