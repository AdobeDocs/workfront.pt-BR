---
title: 22.4 Aprimoramentos do administrador
description: 22.4 Aprimoramentos do administrador
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 1e62e7b3-14b6-4669-b3e1-ac6507343479
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# 22.4 Aprimoramentos do administrador

Esta página descreve todas as melhorias de Administrador feitas com a versão 22.4 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas na semana de 3 de outubro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.4, consulte [22.4 Visão geral da versão](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Usar status desbloqueados em um processo de aprovação

>[!NOTE]
>
>Esse recurso foi introduzido pela primeira vez no ambiente de Pré-visualização durante o período de lançamento da versão 22.3. Ele é lançado para produção em 15 de setembro de 2022.

Para oferecer mais controle sobre os processos de aprovação e os status no sistema, possibilitamos a criação de um processo de aprovação com base em um status de sistema desbloqueado. Além disso, agora é possível desbloquear qualquer status que já seja usado em um processo de aprovação. Anteriormente, um status de sistema usado em um processo de aprovação tinha que ser bloqueado. Isso o tornou disponível para todos os grupos — sem a possibilidade de removê-lo ou renomeá-lo — de modo que os administradores de grupos não pudessem simplificar a lista de status do grupo para atender às suas necessidades específicas.

## Ícone de blueprints no menu principal agora controlado por meio de modelos de layout

Os administradores do sistema agora podem adicionar ou remover o ícone de blueprints no menu principal por meio da configuração de modelo de layout. Isso proporciona maior controle sobre quem pode navegar no catálogo de blueprints.

O ícone Blueprints aparece no menu principal quando:

* O usuário não tem nenhum modelo de layout atribuído

* O modelo de layout do usuário tem a opção Blueprints na lista Itens Ativos

* O modelo de layout do usuário tem a opção Blueprints na lista Itens Disponíveis; o ícone não é exibido no Menu Principal.

Os modelos de layout existentes incluem automaticamente o ícone de blueprints, e os administradores podem remover o ícone dos modelos de layout para restringir a visibilidade do catálogo de blueprints. Os novos modelos de layout criados após a versão 22.4 incluirão o ícone Blueprints na lista Itens ativos.

Para obter mais informações, consulte [Configurar acesso aos blueprints](/help/quicksilver/administration-and-setup/blueprints/configure-access-to-blueprints.md).

[Exibir uma demonstração em vídeo desse recurso](https://video.tv.adobe.com/v/3412382/){target=_blank}

## Personalização do cabeçalho do problema

Como administrador de grupo ou Workfront, agora é possível personalizar os campos que são exibidos no cabeçalho de um problema ao usar um Modelo de layout.

Essa atualização inclui os seguintes aprimoramentos:

* Remova ou reorganize campos existentes do cabeçalho do problema.

* Adicione novos campos de Visão geral de problemas não editáveis. Não é possível adicionar campos personalizados ou campos que podem ser editados. Você também pode exibir campos editáveis que estão atualmente no cabeçalho da ocorrência (por exemplo, Status ou Percentual concluído).

* O cabeçalho do problema pode incluir até cinco campos.

* Agora você pode adicionar o campo &quot;Resolvido por&quot; ao cabeçalho do problema. Quando um objeto de resolução é associado ao problema, o campo &quot;Resolvido por&quot; muda para &quot;Resolvendo problema&quot;, &quot;Resolvendo tarefa&quot; ou &quot;Resolvendo projeto&quot;, dependendo do tipo de objeto que está associado ao problema.

Antes desta versão, somente os cabeçalhos de projetos e tarefas podiam ser personalizados.



Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Exibir uma demonstração em vídeo desse recurso](https://video.tv.adobe.com/v/3412383/){target=_blank}

## Personalização do cabeçalho da tarefa

Como administrador de grupo ou Workfront, agora é possível personalizar os campos que são exibidos no cabeçalho de uma tarefa ao usar um Modelo de layout.

Essa atualização inclui os seguintes aprimoramentos:

* Remova ou reorganize os campos existentes do cabeçalho da tarefa.

* Adicionar novos campos de Visão geral da tarefa não editáveis. Não é possível adicionar campos personalizados ou campos que podem ser editados. Você também pode exibir campos editáveis que estão atualmente no cabeçalho da tarefa (por exemplo, Status ou Percentual concluído).

* O cabeçalho da tarefa pode incluir até cinco campos.

Antes desta versão, somente os cabeçalhos do projeto podiam ser personalizados.

Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um Modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412384/){target=_blank}

## Aceitação antecipada de recursos para os recursos mais recentes nos quadros

Estamos animados em abrir novos recursos de placas para a adesão antecipada. Essa ferramenta opcional está disponível para todas as organizações.

Somente um administrador do Workfront pode aceitar os recursos anteriores. Quando o administrador opta pelos recursos iniciais, todos os usuários na organização são aceitos e os recursos adicionais são ativados no ambiente de produção do Workfront.

Para obter mais informações, consulte [Aceitação antecipada de recursos para painéis do Adobe Workfront](/help/quicksilver/agile/get-started-with-boards/boards-early-feature-opt-in.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412386/){target=_blank}

## O editor de cálculo de campo de formulário personalizado exibe informações de erro

>[!NOTE]
>
>Esse recurso foi introduzido pela primeira vez no ambiente de Pré-visualização durante o período de lançamento da versão 22.3. Ele é lançado para produção com a versão 22.4.

A edição de cálculos para campos personalizados agora é mais fácil com informações de erro úteis indicadas diretamente no cálculo. Ao criar um campo calculado em um formulário personalizado, os erros são destacados em rosa. Quando você passa o mouse sobre a parte destacada, uma dica de ferramenta é exibida para descrever qual é o problema.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412387/){target=_blank}

## Migração para a experiência unificada do Adobe

OBSERVAÇÃO: essa migração foi adiada para o primeiro e o segundo trimestres de 2023. Todos os clientes afetados serão notificados nesse momento.

Se sua organização tiver sido integrada à Adobe Admin Console, sua instância do Workfront será migrada para a Experiência unificada do Adobe com a versão 22.4.

A Experiência unificada do Adobe inclui:

* Um login único para todos os aplicativos Adobe por meio do Adobe Experience Cloud

* Um &quot;alternador de organização&quot; para alternar entre organizações e ambientes do Workfront

* Navegação com opções para páginas do Workfront, preferências do Adobe Experience Cloud e seu perfil do Workfront

Para obter mais informações, consulte [Experiência unificada do Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412388/){target=_blank}
