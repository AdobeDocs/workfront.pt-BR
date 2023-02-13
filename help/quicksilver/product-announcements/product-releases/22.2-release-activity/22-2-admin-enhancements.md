---
title: 2.2 Aprimoramentos do administrador
description: 2.2 Aprimoramentos do administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '1009'
ht-degree: 0%

---

# 2.2 Aprimoramentos do administrador

Esta página descreve todas as melhorias do Administrador feitas com a versão 2.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente Produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 4 de abril de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.2, consulte [Visão geral da versão 2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configurar um formulário personalizado para funcionar com vários tipos de objeto

Agora é possível configurar um formulário personalizado novo ou existente para funcionar com vários tipos de objeto, tornando o formulário muito mais útil. Os usuários poderão anexar e preencher o formulário em objetos de todos os tipos para os quais você o configura.

Anteriormente, era possível configurar um formulário personalizado para funcionar com apenas um tipo de objeto.

Essa funcionalidade funciona com todos os formulários personalizados criados anteriormente no sistema Workfront. Por exemplo, se você já tiver um formulário personalizado criado para o tipo de objeto Tarefa, será possível configurar o formulário para funcionar com outros tipos de objeto, como Projeto e Problema.

Para obter mais informações, consulte a seção [Comece a criar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md#start) no artigo [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

>[!NOTE]
>
>* No momento da versão inicial de Visualização dessa funcionalidade, desativamos temporariamente a capacidade de copiar um formulário personalizado de vários objetos. Essa capacidade foi ativada em 24 de março. Para obter informações sobre como copiar um formulário personalizado, consulte [Copiar um formulário personalizado para criar um novo](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).
>* Em um campo personalizado calculado, alguns campos que você faz referência podem não ser compatíveis com os tipos de objeto configurados para o formulário. Nossa solução é um curinga que permitirá que o cálculo produza valores diferentes, dependendo do objeto ao qual o formulário está anexado. Adicionamos o curinga em 24 de março. Para obter informações sobre como usá-lo, consulte a seção [Campos personalizados calculados em formulários personalizados com vários objetos](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat) no artigo [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
>* Para quebras de seção em formulários personalizados, criamos um conjunto de permissões comuns de visualização e edição que funcionam para todos os tipos de objetos que podem ser configurados para um formulário. Em um cenário, descobrimos que uma dessas permissões, Edição limitada, pode causar erros em um formulário. Isso foi corrigido em 24 de março. Para obter mais informações sobre quebras de seção, consulte [Adicionar uma quebra de seção a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).
>


## O catálogo de blueprints está disponível para todos os usuários, e os administradores podem permitir solicitações

Todos os usuários do Adobe Workfront agora podem navegar pelo catálogo de blueprints disponíveis. Para obter mais informações, consulte [Navegue pelo catálogo de blueprints e solicite a instalação de blueprints](../../../administration-and-setup/blueprints/browse-catalog.md).

Além disso, o administrador do sistema pode habilitar o acesso de usuários para solicitar a instalação de blueprints. Atribuir uma fila de solicitações para armazenar as solicitações permite que os usuários façam solicitações do catálogo de blueprints. Para obter mais informações, consulte [Configurar o acesso a blueprints](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Adicionar uma imagem a um formulário personalizado

Em um formulário personalizado que você cria ou edita, agora é possível adicionar uma imagem e incluir uma dica de ferramenta informativa ou instrutiva que os usuários podem ler ao passar o mouse sobre ela.

Isso pode ser útil, por exemplo, para mostrar a marca de um novo produto ou para fornecer informações visuais que as pessoas precisam ao preencherem o formulário.

Anteriormente, os formulários personalizados eram completamente baseados em texto.

>[!NOTE]
>
>Nas novas áreas de experiência do Adobe Workfront que ainda não foram modernizadas, como a caixa exibida ao editar itens em massa, imagens de formulário personalizadas não são exibidas. Elas serão exibidas à medida que atualizamos essas áreas.

Para obter mais informações, consulte [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Novas configurações padrão de nível de acesso

Para atender melhor às necessidades da maioria dos administradores que criam novos níveis de acesso, alteramos a configuração padrão das opções de &quot;Ajustar as configurações&quot; listadas abaixo. Elas são exibidas ao clicar no ícone de engrenagem ![](assets/gear-icon-in-access-levels.png) em um botão Editar.

Todas essas alterações desativam uma opção que foi ativada anteriormente por padrão. Se isso não atender às necessidades de sua organização, você poderá ativá-las ao configurar um novo nível de acesso ou a qualquer momento posteriormente.

>[!IMPORTANT]
>
>Essa alteração na configuração padrão afeta apenas os níveis de acesso criados a partir de agora, não os criados anteriormente.

* Em um novo nível de acesso com um tipo de licença Plano:

   * O Compartilhamento em todo o sistema agora está desativado para projetos, tarefas, problemas, portfólios, programas, relatórios, filtros, documentos e modelos.
   * Exibir relatórios internos e compartilhar relatórios publicamente também estão desativados para os relatórios.
   * Compartilhar documentos publicamente também está desativado para documentos.

* Em um novo nível de acesso com um tipo de licença Trabalho:

   * O Compartilhamento em todo o sistema agora está desativado para filtros e documentos.
   * Compartilhar documentos publicamente também está desativado para documentos.

* Em um novo nível de acesso com um tipo de licença Solicitação ou Revisão :

   * O Compartilhamento em todo o sistema agora está desativado para filtros.

## Desativar um grupo

À medida que suas organizações internas mudam, pode ser necessário parar de usar determinados grupos no Workfront e criar novos grupos. Para ajudar nisso, adicionamos a capacidade de desativar um grupo sem perder seus dados históricos. Para usuários regulares que não precisam visualizá-los, os grupos inativos são apagados dos campos tipo-forward do grupo.

Ainda é possível encontrar e configurar opções, preferências e associações de objetos para grupos inativos que você gerencia. E desativar um grupo não altera nada sobre os objetos aos quais ele está anexado.

Anteriormente, não era possível desativar um grupo.

Para obter mais informações, consulte [Desativar ou reativar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Aprimoramentos no histórico de instalação do Blueprints

Ao instalar um blueprint, uma mensagem agora exibe os objetos específicos (como funções, equipes ou grupos) que foram instalados com êxito com o blueprint e quaisquer objetos que não foram instalados. Você também pode exibir a lista de objetos instalados na página Detalhes do Blueprint clicando em Exibir detalhes ao lado de uma instalação específica na tabela Histórico de instalação.

Para obter mais informações, consulte [Instalar um blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).

![](assets/blueprints-installation-history-350x95.png)

## Um aviso agora é exibido ao instalar um blueprint somente visualização em Produção

Determinados blueprints só estão disponíveis para instalação no ambiente Preview para fins de teste.

Se você acessar o conteúdo Somente visualização no ambiente de Produção, Sandbox 1 ou Sandbox 2, o botão de instalação não estará ativo e poderá ver uma mensagem de aviso.

Para obter mais informações, consulte [Instalar um blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).
