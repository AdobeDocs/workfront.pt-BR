---
title: 2.3 Aprimoramentos do administrador
description: 2.3 Aprimoramentos do administrador
author: Luke
draft: false
feature: Product Announcements
exl-id: 4607703a-d70e-432c-9fa2-bd43af5a870e
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '805'
ht-degree: 0%

---

# 2.3 Aprimoramentos do administrador

Esta página descreve todas as melhorias do Administrador feitas com a versão 2.3 para o ambiente de Visualização. Esses aprimoramentos foram disponibilizados na semana de 11 de julho de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.3, consulte [Visão geral da versão 2.3](/help/quicksilver/product-announcements/product-releases/22.3-release-activity/22-3-release-overview.md).

## Integrar o Adobe Workfront com o JumpSeat

Agora é possível integrar o JumpSet ao Workfront para criar orientação personalizada no produto para seus usuários. Você deve ter uma licença corporativa da Adobe Workfront e uma assinatura JumpSeat ativa para habilitar a integração.

Para obter mais informações, consulte [Configurar a integração do JumpSeat](/help/quicksilver/administration-and-setup/configure-integrations/configure-jumpseat.md).

## Configurações padrão de prova movidas para o Workfront

Agora você pode editar as seguintes configurações de prova na Área de configuração do Workfront:

* Configurações padrão de prova

* Configurações de decisão de prova

Para obter mais informações, consulte [Definir configurações de prova padrão](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).

## Usar status desbloqueado em processos de aprovação

**Observação:** Remoção da versão 22.3 Production (Produção). Esse recurso está planejado para ser lançado para produção em 15 de setembro de 2022.

Para dar a você mais controle sobre os processos e status de aprovação em seu sistema, tornamos possível criar um processo de aprovação com base em um status de sistema desbloqueado. Além disso, agora é possível desbloquear qualquer status que já esteja sendo usado em um processo de aprovação.

Anteriormente, o status do sistema usado em um processo de aprovação tinha que ser bloqueado. Isso o disponibilizou para todos os grupos, sem a possibilidade de removê-lo ou renomeá-lo, de modo que os administradores de grupo não poderiam simplificar a lista de status de seus grupos para atender às suas necessidades específicas.

Para obter mais informações, consulte os seguintes artigos:

* [Criar um processo de aprovação para itens de trabalho](/help/quicksilver/administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)

* [Criar ou editar um status](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md)

* [Status de nível de sistema bloqueados e desbloqueados](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md)


## Adicionar um arquivo PDF a um formulário personalizado

Continuamos a ajudá-lo a tornar os formulários personalizados mais visuais e informativos com novos widgets de ativos que você pode adicionar, como imagens e vídeos. Agora é possível adicionar um link a um arquivo PDF a um formulário personalizado. Quando o formulário é anexado a um objeto, os usuários que trabalham com ele podem visualizar e interagir com o PDF a partir do formulário.

Para obter mais informações, consulte [Adicionar ou editar uma imagem ou outro widget de ativo em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## O editor de cálculo de campo de formulário personalizado exibe informações de erro

>[!NOTE]
>
>Este recurso está temporariamente indisponível. Esta página será atualizada quando o recurso estiver disponível.

A edição de cálculos para campos personalizados agora é mais fácil com informações de erro úteis indicadas diretamente no cálculo. Ao criar um campo calculado em um formulário personalizado, os erros são destacados em rosa. Quando você passa o mouse sobre a parte realçada, uma dica de ferramenta é exibida para descrever o problema.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Personalização do cabeçalho do projeto

Como administrador de grupo ou Workfront, agora é possível personalizar os campos exibidos no cabeçalho de um projeto ao usar um Modelo de layout.

Esta atualização inclui os seguintes aprimoramentos:

* Remova os campos existentes do cabeçalho do projeto.

* Adicione novos campos de Visão geral do projeto não editáveis. Não é possível adicionar campos personalizados ou campos que podem ser editados. Os campos editáveis que estão atualmente no cabeçalho do projeto podem permanecer no cabeçalho.

* O cabeçalho do objeto pode incluir até cinco campos.


Antes dessa versão, os campos nos cabeçalhos de objetos não podiam ser personalizados.

Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

## Controle da criação de um projeto em branco

Como administrador de sistema ou de grupo, agora é possível controlar se os usuários podem criar projetos em branco, sem usar um modelo. Introduzimos uma nova configuração na área Preferências do projeto da Configuração que permite desativar a criação de projetos em branco nas seguintes áreas:

* Na opção Novo projeto em uma lista de projetos

* Ao converter um problema em um projeto a partir da página de edição


A nova configuração é &quot;Permitir que usuários criem projetos sem usar um modelo&quot; e é ativada por padrão.

**Observação:** Os usuários ainda podem converter uma tarefa em um projeto em branco.

Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Desativar um grupo da página Grupos

Recentemente, adicionamos a capacidade de desativar e reativar grupos. Para tornar essa ação mais rápida e fácil, a adicionamos à página de um grupo. Agora, depois de clicar no nome de um grupo para ir para a página, você pode selecionar o menu Mais ![](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/assets/main-menu-icon.png) ao lado do nome do grupo, selecione Desativar ou Reativar.

Anteriormente, você podia desativar ou reativar um grupo somente usando a caixa de seleção Is ative na página Detalhes .

Para obter mais informações, consulte [Desativar ou reativar um grupo](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Adicionar vídeos a formulários personalizados

Agora é possível fornecer um novo modo de informação, interesse visual e criatividade para um formulário personalizado ao adicionar um vídeo. Quando o formulário é anexado a um objeto, os usuários que trabalham com ele podem reproduzir o vídeo a qualquer momento.

Anteriormente, era possível adicionar somente campos e imagens com base em texto a um formulário personalizado.

Para obter mais informações, consulte [Adicionar ou editar uma imagem ou um widget de ativo de vídeo em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

