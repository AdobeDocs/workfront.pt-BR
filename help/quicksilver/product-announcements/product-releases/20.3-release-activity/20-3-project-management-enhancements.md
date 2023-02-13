---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 Melhorias no gerenciamento de projetos
description: Esta página descreve todas as melhorias no gerenciamento de projetos feitas com a versão 20.3 para o ambiente Produção. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 10 de agosto de 2020.
author: Luke
feature: Product Announcements
exl-id: acde4cf2-a755-4e77-9469-f5152991dd34
source-git-commit: d337008d4fca8c41b98b10f9059ec1cc379811e1
workflow-type: tm+mt
source-wordcount: '942'
ht-degree: 0%

---

# 20.3 Melhorias no gerenciamento de projetos

Esta página descreve todas as melhorias no gerenciamento de projetos feitas com a versão 20.3 para o ambiente Produção. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 10 de agosto de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.3, consulte [Visão geral da versão 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Formatação de campo personalizado em listas

>[!NOTE]
>
>Esse recurso é compatível somente na nova experiência do Adobe Workfront. Ele está disponível para algumas listas no Adobe Workfront Classic, mas não é compatível com o Adobe Workfront Classic.

Agora, quando o administrador do sistema cria campos de formulários personalizados configurados para formatação, é possível formatar o texto nesses campos onde você mais os usa: em listas em todo o Workfront. Em vez de entrar na área Detalhes para formatar o texto no formulário personalizado, você pode clicar em um campo em uma lista e aplicar Negrito, Itálico e Sublinhado ao texto.

Observe que esta funcionalidade está disponível somente nas listas atualizadas. Para obter mais informações sobre listas atualizadas, consulte [Introdução a listas no Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

Para obter informações sobre como um administrador do Workfront cria campos de texto com formatação, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Aparência e comportamento atualizados de vários cabeçalhos globais

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

As áreas globais de Projetos, Portfolio, Programas e Modelos agora têm um cabeçalho atualizado que aproveita melhor o espaço na tela. Esta atualização oferece mais espaço para as informações com as quais você precisa se concentrar.

O link Modelos da área Projetos foi removido. Você ainda pode acessar a área Modelos no Menu principal.

## Caixa Novo projeto de edição

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Como parte da atualização da aparência da nova experiência do Workfront, reprojetamos a caixa Editar projeto . Você pode acessar a nova caixa Editar projeto de um projeto individual ou ao editar um único projeto de uma lista.

Além de uma aparência atualizada, as seguintes melhorias estão disponíveis na caixa Editar projeto :

* Personalize seu modelo de layout uma vez e reflita as personalizações na página Detalhes e na caixa Editar objeto .
* Nomes de formulários personalizados individuais agora estão disponíveis no painel esquerdo, dentro da caixa Editar projeto , e você pode acessar rapidamente cada formulário a partir daí.
* A funcionalidade de comentários é removida da tela Editar projeto para eliminar a redundância com a seção Atualizações .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the new Edit Box box, see "New Edit Object box" (NEW ARTICLE, LINK LATER!!).</p>
-->

Para obter informações sobre a nova caixa Editar projeto, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Novo painel Resumo e Melhorias nas Atualizações da lista de documentos

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

O novo painel Resumo à direita da lista de documentos agora está disponível com um design aprimorado na nova experiência do Workfront. Esse painel fornece as mesmas ações e informações disponíveis no painel à direita ao selecionar um documento no Workfront Classic, incluindo detalhes do documento, atualizações, Forms personalizado, aprovações e versões de documento.

Algumas ações estão indisponíveis no momento, mas serão adicionadas em uma versão futura. Essas ações incluem o fluxo de trabalho de prova.

Para obter mais informações, consulte [Resumo para visão geral dos documentos](../../../documents/managing-documents/summary-for-documents.md).

## Melhorias nos detalhes do documento

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Procure as seguintes melhorias na página Detalhes do documento :

* As novas opções de versão foram movidas para um menu suspenso próximo ao painel esquerdo, facilitando o acesso.
* Ícone Abrir prova alterado para um rótulo de prova Abrir, facilitando a visualização na página.
* Miniatura de visualização maior, permitindo identificar facilmente o documento
* Adicionado o ícone de Edição global , que permite editar vários campos ao mesmo tempo.

Para obter mais informações, consulte [Visão geral dos detalhes do documento](../../../documents/managing-documents/document-details-overview.md).

## Para administradores: defina as preferências do projeto no nível do grupo

>[!NOTE]
>
>Essa funcionalidade está temporariamente indisponível para a maioria dos clientes nos clusters 1, 2, 3 e 5. Esta página será atualizada quando a funcionalidade for reinstalada para todos os clientes.

Para dar aos administradores do grupo mais autonomia e permitir uma personalização mais ampla dos fluxos de trabalho em nível de grupo, agora é possível definir as preferências do projeto no nível de grupo, para grupos que você administra. Ao criar um projeto, as preferências do grupo entrarão em vigor antes das do sistema.

Todas as preferências do projeto são personalizáveis no nível do grupo, exceto para Cálculos de Linha do Tempo e Trimestres Personalizados.

Para obter mais informações sobre Preferências de projeto de grupo, consulte [Configurar preferências de projeto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md).

## Novo para administradores: Criar campos de formulário personalizado onde os usuários podem formatar o texto

Em um Formulário personalizado, agora é possível criar campos que incluem botões de formatação de texto. Quando os usuários digitam nesses campos, eles podem realçar e organizar o texto usando negrito, itálico e sublinhado. O limite de 15.000 caracteres alto permite bastante texto e formatação.

Para obter mais informações, consulte Criar um formulário personalizado na nova experiência do Workfront.

## Novo para administradores: Crie um nome interno e um rótulo voltado para o usuário para um campo Formulário personalizado

Para oferecer mais flexibilidade na rotulagem e rerotulagem de campos de Formulário personalizado, agora é possível criar um formulário interno *name* para um campo, além do *label* você tem usado. Isso dá a liberdade de alterar o rótulo de campo que seus usuários veem sem alterar o nome do campo que o sistema vê.

No passado, o rótulo era exibido acima do campo para os usuários e usado pelo sistema para identificar o campo. Assim, a alteração da etiqueta para os usuários fazia com que o campo não funcionasse corretamente onde fosse usado porque o sistema não podia mais identificá-lo.

Para obter mais informações, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

