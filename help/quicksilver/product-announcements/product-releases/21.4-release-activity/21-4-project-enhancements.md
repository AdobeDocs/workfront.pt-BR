---
title: 21.4 Aprimoramentos do projeto
description: 21.4 Aprimoramentos do projeto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6bcd332e-bd4e-4a74-bae9-9ba507299a51
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '950'
ht-degree: 0%

---

# 21.4 Aprimoramentos do projeto

Esta página descreve todas as melhorias feitas no Project com a versão 21.4 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 4 de outubro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.4, consulte [21.4 Visão geral da versão](../../../product-announcements/product-releases/21.4-release-activity/21-4-release-overview.md).

## Incluir imagens em atualizações

Na guia Atualizações de um objeto, agora é possível adicionar imagens clicando no ícone Imagem na barra de ferramentas. Você também pode arrastar e soltar uma imagem na área de atualização. Observe que o administrador do Workfront deve habilitar a adição de imagens antes que você possa ver o ícone Imagem.

Você pode adicionar imagens em atualizações e respostas. Uma miniatura de imagem na atualização indica que os destinatários podem visualizar a imagem no navegador ou baixá-la, e as notificações por email e no aplicativo mostram que as imagens estão anexadas à atualização.

Anteriormente, a única maneira de compartilhar uma imagem no Workfront era anexá-la a um objeto como um documento. As imagens adicionadas na guia Atualizações só estão disponíveis nessa guia e não na guia Documentos.

Para obter mais informações, consulte [Atualizar trabalho](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

Antes que os usuários do Workfront possam incluir imagens em atualizações, esse recurso deve ser primeiro ativado pelo administrador do Adobe Workfront, conforme descrito em [Configurar preferências para atualizações de usuário](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-preferences-user-updates.md).

## Algoritmo atualizado para atribuições inteligentes

Melhoramos o algoritmo usado ao fazer atribuições inteligentes. Com o novo aprimoramento, o Workfront observa as 30 atribuições mais recentes feitas pelo usuário conectado para fazer sugestões ao atribuir tarefas e problemas. A lista de sugestões pode conter até 50 usuários.

Antes desse aprimoramento, a Workfront estava considerando as atribuições nas tarefas principais e outros atributos de usuário relacionados a essas atribuições ao sugerir usuários.

Para obter informações sobre atribuições inteligentes, consulte [Visão geral das atribuições inteligentes](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## Nova experiência ao criar um projeto a partir de um modelo

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para criar um projeto a partir de um modelo. A funcionalidade para criar um projeto usando um modelo não foi alterada. No entanto, algumas das melhorias dessa interface recém-reprojetada incluem:

* Visualizar informações do modelo antes de anexá-lo
* Adicionar modelos a uma lista de favoritos durante o processo de criação do projeto

Atualizamos a interface para criar o projeto ao criá-lo a partir da área Projetos e da área Modelos.

Para obter informações, [Criar um projeto usando um modelo](../../../manage-work/projects/create-projects/create-project-from-template.md).

## Nova experiência ao anexar modelos a projetos

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront.

Para tornar seu uso do Workfront consistente com a nova experiência do Workfront, reprojetamos a interface para anexar um modelo a um projeto. A funcionalidade para anexar um modelo não foi alterada. No entanto, há algumas melhorias nessa interface recém-reprojetada que incluem o seguinte:

* Visualizar informações do modelo antes de anexá-lo
* Adicionar modelos a uma lista de favoritos durante o processo de anexação
* Exibir todas as opções para gerenciar configurações de modelo e projeto em uma página contínua

Para obter informações, consulte [Anexar um modelo a um projeto](../../../manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

## Duração unificada e valores unitários de duração para tarefas

Para obter uma experiência do usuário mais limpa e simplificada, mesclamos o valor do campo Duração com a unidade de tempo da duração. Antes dessa melhoria, a unidade de tempo exibida em um campo suspenso separado após o campo Duração.

Além dos campos Duração nas caixas Detalhes da tarefa, Editar tarefas e Nova tarefa, também atualizamos os seguintes campos para corresponder a essa experiência:

* Campo de duração ao fazer atribuições avançadas
* Campo de atraso de nivelamento ao criar ou editar uma tarefa
* Campo de frequência ao criar uma tarefa recorrente (disponível em breve)
* Campo de atraso ao adicionar um predecessor (disponível em breve)

Para obter informações, consulte [Editar tarefas](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

![](assets/duration-combined-field-350x139.png)

## Desativar a adição de problemas em linha nos projetos

Para garantir que os usuários forneçam informações precisas ao adicionar problemas a projetos preenchendo um formulário de problema, introduzimos uma nova configuração que permite gerenciar se eles podem adicionar problemas a um projeto ou a suas tarefas em linha. Essa configuração é ativada por padrão na nova área Configurações de problema da caixa Editar projeto. Desativá-la esmaece a opção Adicionar mais problemas na seção Problemas de um projeto para que os usuários não possam adicionar mais problemas na lista. Os usuários ainda podem adicionar problemas aos projetos usando a opção Novo problema na seção Problemas ou usando uma fila de solicitações, se uma estiver configurada para o projeto.

>[!NOTE]
>
>Essa configuração está disponível somente na nova experiência do Workfront. Os usuários que trabalham no Workfront classic ainda podem adicionar problemas em linha a um projeto ou suas tarefas, mesmo que essa configuração tenha sido desativada para o projeto por um usuário que trabalha na nova experiência do Workfront.

Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Aprimoramento da exibição de campo personalizado para caixas de seleção e botões de opção

Visualizar e selecionar as opções de caixa de seleção e botão de opção em formulários personalizados ficou mais fácil: um campo personalizado com muitas opções de caixa de seleção ou botão de opção agora é exibido em várias colunas na página. Anteriormente, eles eram exibidos em uma única coluna, o que exigia rolagem extra para os usuários que preenchessem o formulário.

Isso depende de como você posiciona os campos no formulário personalizado. Se você colocar outro campo na mesma linha com a caixa de seleção ou o campo de botão de opção, as opções poderão ter apenas espaço horizontal suficiente para exibição em uma única coluna.

Para obter informações sobre como preencher um formulário personalizado, consulte [Editar informações em campos de formulário personalizados](../../../workfront-basics/work-with-custom-forms/edit-custom-forms.md).

Para obter informações sobre como criar um campo de caixa de seleção ou botão de opção em um formulário personalizado, consulte as seções [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#create) e [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#configur) no artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

