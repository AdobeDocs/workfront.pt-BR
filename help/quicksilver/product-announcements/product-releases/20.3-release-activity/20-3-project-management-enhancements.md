---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Aprimoramentos no gerenciamento de projetos
description: Esta página descreve todas as melhorias de gerenciamento de projeto feitas com a versão 20.3 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 10 de agosto de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '953'
ht-degree: 0%

---

# 20.3 Aprimoramentos no gerenciamento de projetos

Esta página descreve todas as melhorias de gerenciamento de projeto feitas com a versão 20.3 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 10 de agosto de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.3, consulte [Visão geral da versão 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Formatação de campo personalizado em listas

>[!NOTE]
>
>Esse recurso é compatível somente com a nova experiência do Adobe Workfront. Ele está disponível para algumas listas no Adobe Workfront Classic, mas não é compatível com o Adobe Workfront Classic.

Agora, quando o administrador do sistema cria campos de formulários personalizados configurados para formatação, é possível formatar o texto nos campos em que você mais os usa: em listas em todo o Workfront. Em vez de entrar na área Detalhes para formatar o texto no formulário personalizado, você pode clicar em um campo em uma lista e aplicar Negrito, Itálico e Sublinhado ao texto lá.

Observe que essa funcionalidade está disponível somente nas listas atualizadas. Para obter mais informações sobre listas atualizadas, consulte [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Para obter informações sobre como um administrador do Workfront cria campos de texto com formatação, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Atualização da aparência de vários cabeçalhos globais

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

As áreas globais de Projetos, Portfolio, Programas e Modelos agora têm um cabeçalho atualizado que faz melhor uso do espaço na tela. Essa atualização oferece mais espaço para as informações com as quais você precisa se concentrar.

O link Modelos da área Projetos foi removido. Você ainda pode acessar a área Modelos no Menu principal.

## Nova caixa Editar projeto

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Como parte da atualização da aparência da nova experiência do Workfront, reprojetamos a caixa Editar projeto. Você pode acessar a nova caixa Editar projeto a partir de um projeto individual ou ao editar um único projeto de uma lista.

Além de uma aparência atualizada, as seguintes melhorias estão disponíveis na caixa Editar projeto:

* Personalizar o modelo de layout uma vez e refletir essas personalizações na página Detalhes e na caixa Editar objeto.
* Nomes de formulários personalizados individuais agora estão disponíveis no painel esquerdo dentro da caixa Editar projeto e você pode acessar rapidamente cada formulário a partir daí.
* A funcionalidade de comentários é removida da tela editar projeto para eliminar redundância com a seção Atualizações.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

Para obter informações sobre a nova caixa Editar projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Novo painel Resumo e melhorias de Atualizações para a lista de documentos

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

O novo painel Resumo à direita da lista de documentos agora está disponível com um design aprimorado na nova experiência do Workfront. Esse painel fornece as mesmas ações e informações disponíveis no painel à direita ao selecionar um documento no Workfront Classic, incluindo detalhes do documento, atualizações, Forms personalizado, aprovações e versões do documento.

Algumas ações estão indisponíveis no momento, mas serão adicionadas em uma versão futura. Essas ações incluem o fluxo de trabalho de prova.

Para obter mais informações, consulte [Resumo para visão geral de documentos](../../../documents/managing-documents/summary-for-documents.md).

## Melhorias nos detalhes do documento

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Procure as seguintes melhorias na página Detalhes do documento:

* As novas opções de versão são movidas para um menu suspenso próximo ao painel esquerdo, facilitando o acesso.
* O ícone de prova aberta foi alterado para um rótulo de Prova aberta, facilitando a visualização na página.
* Miniatura de visualização maior, permitindo identificar facilmente o documento
* Ícone Edição global adicionado, que oferece a capacidade de editar vários campos de uma só vez.

Para obter mais informações, consulte [Visão geral dos detalhes do documento](../../../documents/managing-documents/document-details-overview.md).

## Para administradores: definir preferências de projeto no nível do grupo

>[!NOTE]
>
>Essa funcionalidade está temporariamente indisponível para a maioria dos clientes nos clusters 1, 2, 3 e 5. Esta página será atualizada quando a funcionalidade for restabelecida para todos os clientes.

Para dar mais autonomia aos administradores de grupo e permitir maior personalização dos fluxos de trabalho no nível do grupo, agora é possível definir as preferências do projeto no nível do grupo, para os grupos que você administra. Ao criar um projeto, as preferências do grupo entrarão em vigor antes das preferências do sistema.

Todas as preferências do projeto podem ser personalizadas no nível do grupo, exceto Cálculos de linha do tempo e Trimestres personalizados.

Para obter mais informações sobre Preferências de Projeto de Grupo, consulte [Configurar as preferências do projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## Novo para administradores: criar campos de formulário personalizados em que os usuários podem formatar texto

Em um Formulário personalizado, agora é possível criar campos que incluem botões de formatação de texto. Quando os usuários digitam nesses campos, eles podem realçar e organizar o texto usando negrito, itálico e sublinhado. O limite superior de 15.000 caracteres permite bastante texto e formatação.

Para obter mais informações, consulte Criar um formulário personalizado na nova experiência do Workfront.

## Novo para administradores: crie um nome interno e um rótulo voltado para o usuário para um campo de Formulário personalizado

Para oferecer mais flexibilidade na rotulagem e no renomeamento de campos de Formulário personalizado, agora é possível criar uma *name* para um campo, além do campo voltado para o usuário *rótulo* você tem usado. Isso dá a você a liberdade de alterar o rótulo de campo que os usuários veem sem alterar o nome do campo que o sistema vê.

Anteriormente, o rótulo era exibido acima do campo para usuários e usado pelo sistema para identificar o campo. Assim, alterar o rótulo para os usuários fazia com que o campo funcionasse mal onde quer que fosse usado, porque o sistema não podia mais identificá-lo.

Para obter mais informações, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

