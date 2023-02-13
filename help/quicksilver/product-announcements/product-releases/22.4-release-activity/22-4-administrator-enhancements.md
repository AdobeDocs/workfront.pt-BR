---
title: 2.4 Melhorias do administrador
description: 2.4 Melhorias do administrador
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 80fa784e15c3b4a927ee8ba2d18a80a2d84f4a91
workflow-type: tm+mt
source-wordcount: '869'
ht-degree: 0%

---

# 2.4 Melhorias do administrador

Esta página descreve todas as melhorias do Administrador feitas com a versão 22.4 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados na semana de 3 de outubro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.4, consulte [Visão geral da versão 2.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Usar status desbloqueado em processos de aprovação

>[!NOTE]
>
>Esse recurso foi introduzido pela primeira vez no ambiente de Visualização durante o período de lançamento da versão 2.3. Ele é lançado para produção em 15 de setembro de 2022.

Para dar a você mais controle sobre os processos e status de aprovação em seu sistema, tornamos possível criar um processo de aprovação com base em um status de sistema desbloqueado. Além disso, agora é possível desbloquear qualquer status que já esteja sendo usado em um processo de aprovação. Anteriormente, o status do sistema usado em um processo de aprovação tinha que ser bloqueado. Isso o disponibilizou para todos os grupos, sem a possibilidade de removê-lo ou renomeá-lo, de modo que os administradores de grupo não poderiam simplificar a lista de status de seus grupos para atender às suas necessidades específicas.

## Ícone Blueprints no Menu principal agora é controlado pelos modelos de layout

Os administradores de sistema agora podem adicionar ou remover o ícone Blueprints no Menu principal por meio da configuração do modelo de layout. Isso fornece maior controle sobre quem pode navegar no catálogo de Blueprints.

O ícone Blueprints aparece no Menu principal quando:

* O usuário não tem nenhum modelo de layout atribuído

* O modelo de layout do usuário tem a opção Blueprints na lista Itens ativos

* O modelo de layout do usuário tem a opção Blueprints na lista Itens disponíveis. O ícone não é exibido no Menu principal.

Os modelos de layout existentes incluem automaticamente o ícone Blueprints , e os administradores podem remover o ícone dos modelos de layout para restringir a visibilidade do catálogo de Blueprints. Os novos modelos de layout criados após a versão 2.4 incluirão o ícone Blueprints na lista Itens ativos.

Para obter mais informações, consulte [Configurar o acesso ao Blueprints](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personalização do cabeçalho da ocorrência

Como administrador de grupo ou Workfront, agora é possível personalizar os campos exibidos no cabeçalho de um problema ao usar um Modelo de layout.

Esta atualização inclui os seguintes aprimoramentos:

* Remova ou reorganize os campos existentes do cabeçalho da ocorrência.

* Adicione novos campos de Visão geral de problema não editáveis. Não é possível adicionar campos personalizados ou campos que podem ser editados. Também é possível exibir campos editáveis que estão atualmente no cabeçalho do problema (por exemplo, Status ou Porcentagem concluída).

* O cabeçalho da edição pode incluir até cinco campos.

* Agora é possível adicionar o campo &quot;Resolvido por&quot; ao cabeçalho do problema. Quando um objeto de resolução é associado ao problema, o campo &quot;Resolvido por&quot; muda para &quot;Resolvendo problema&quot;, &quot;Resolvendo tarefa&quot; ou &quot;Resolvendo projeto&quot;, dependendo do tipo de objeto associado ao problema.

Antes desta versão, somente os cabeçalhos de projeto e tarefa podiam ser personalizados.



Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Ver uma demonstração em vídeo deste recurso](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personalização do cabeçalho da tarefa

Como administrador de grupo ou Workfront, agora é possível personalizar os campos exibidos no cabeçalho de uma tarefa ao usar um Modelo de layout.

Esta atualização inclui os seguintes aprimoramentos:

* Remova ou reorganize campos existentes do cabeçalho da tarefa.

* Adicione novos campos de Visão geral de tarefa não editáveis. Não é possível adicionar campos personalizados ou campos que podem ser editados. Também é possível exibir campos editáveis que estão atualmente no cabeçalho da tarefa (por exemplo, Status ou Porcentagem concluída).

* O cabeçalho da tarefa pode incluir até cinco campos.

Antes desta versão, somente os cabeçalhos do projeto podiam ser personalizados.

Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Aceitação de recursos antecipada para os recursos mais recentes nos quadros

Estamos animados em abrir novos recursos de quadros para aceitar os recursos antecipadamente. Essa ferramenta opcional está disponível para todas as organizações.

Somente um administrador do Workfront pode aceitar os recursos iniciais. Quando o administrador opta pelos recursos iniciais, todos os usuários da organização são aceitos e os recursos adicionais são ativados no ambiente de produção do Workfront.

Para obter mais informações, consulte [Opt-in de recurso antecipado para placas Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## O editor de cálculo de campo de formulário personalizado exibe informações de erro

>[!NOTE]
>
>Esse recurso foi introduzido pela primeira vez no ambiente de Visualização durante o período de lançamento da versão 2.3. Ele é lançado para produção com a versão 22.4.

A edição de cálculos para campos personalizados agora é mais fácil com informações de erro úteis indicadas diretamente no cálculo. Ao criar um campo calculado em um formulário personalizado, os erros são destacados em rosa. Quando você passa o mouse sobre a parte realçada, uma dica de ferramenta é exibida para descrever o problema.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migração para experiência unificada do Adobe

OBSERVAÇÃO: Essa migração foi adiada para o segundo trimestre de 2023. Os clientes afetados serão notificados no momento.

Se sua organização tiver sido integrada à Adobe Admin Console, sua instância do Workfront será migrada para o Adobe Unified Experience com a versão 22.4.

A experiência unificada do Adobe inclui:

* Um único logon para todos os aplicativos Adobe por meio do Adobe Experience Cloud

* Um &quot;alternador de organização&quot; para migrar entre organizações e ambientes da Workfront

* Navegação com opções para páginas do Workfront, preferências do Adobe Experience Cloud e seu perfil do Workfront

Para obter mais informações, consulte [Experiência unificada do Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412388/){target=_blank}
