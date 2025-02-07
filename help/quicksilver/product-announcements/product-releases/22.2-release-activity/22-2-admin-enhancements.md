---
title: 22.2 Aprimoramentos do administrador
description: 22.2 Aprimoramentos do administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 55fb0b85-937d-4903-8a64-6f627dd4291f
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# 22.2 Aprimoramentos do administrador

Esta página descreve todas as melhorias de Administrador feitas com a versão 22.2 no ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 4 de abril de 2022. Para obter uma lista de todas as alterações disponíveis com a versão 22.2, consulte a [Visão geral da versão 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Configurar um formulário personalizado para trabalhar com vários tipos de objeto

Agora é possível configurar um formulário personalizado novo ou existente para funcionar com vários tipos de objeto, tornando o formulário muito mais útil. Os usuários poderão anexar e preencher o formulário em objetos de todos os tipos para os quais você o configura.

Anteriormente, você podia configurar um formulário personalizado para funcionar com apenas um tipo de objeto.

Essa funcionalidade funciona com todos os formulários personalizados criados anteriormente em seu sistema Workfront. Por exemplo, se você já tiver um formulário personalizado que foi criado para o tipo de objeto Tarefa, poderá configurar o formulário para funcionar com outros tipos de objeto, como Projeto e Problema.

>[!NOTE]
>
>* No momento de nosso lançamento inicial de Pré-visualização dessa funcionalidade, desativamos temporariamente a capacidade de copiar um formulário personalizado de vários objetos. Essa habilidade foi ativada em 24 de março.
>* Em um campo personalizado calculado, alguns campos referenciados podem não ser compatíveis com os tipos de objeto configurados para o formulário. Nossa solução é um curinga que permitirá que o cálculo produza valores diferentes, dependendo do objeto ao qual o formulário está anexado. Adicionamos o curinga em 24 de março.
>* Para quebras de seção em formulários personalizados, criamos um conjunto de permissões comuns de visualização e edição que funcionam para todos os tipos de objeto que você pode configurar para um formulário. Em um cenário, descobrimos que uma dessas permissões, Edição limitada, pode causar erros em um formulário. Isso foi corrigido em 24 de março.
>

## O catálogo de blueprints está disponível para todos os usuários e os administradores podem permitir solicitações

Todos os usuários do Adobe Workfront agora podem navegar pelo catálogo de blueprints disponíveis. Para obter mais informações, consulte [Procurar o catálogo de blueprints e solicitar a instalação de blueprints](../../../administration-and-setup/blueprints/browse-catalog.md).

Além disso, o administrador do sistema pode habilitar o acesso para que os usuários solicitem a instalação de blueprints. Atribuir uma fila de solicitações para armazenar as solicitações permite que os usuários façam solicitações no catálogo de blueprints. Para obter mais informações, consulte [Configurar acesso a blueprints](../../../administration-and-setup/blueprints/configure-access-to-blueprints.md).

## Adicionar uma imagem a um formulário personalizado

Em um formulário personalizado que você cria ou edita, agora é possível adicionar uma imagem e incluir uma dica de ferramenta informativa ou instrutiva que os usuários podem ler ao passar o mouse sobre ela.

Isso pode ser útil, por exemplo, para mostrar a identidade visual de um novo produto ou para fornecer informações visuais que as pessoas precisam ao preencher o formulário.

Anteriormente, os formulários personalizados eram completamente baseados em texto.

>[!NOTE]
>
>Nas novas áreas de experiência do Adobe Workfront que ainda não foram modernizadas, como a caixa que é exibida ao editar itens em massa, as imagens de formulário personalizado não são exibidas. Elas serão exibidas à medida que continuarmos a atualizar essas áreas.


## Novas configurações de nível de acesso padrão

Para atender melhor às necessidades da maioria dos administradores que criam novos níveis de acesso, alteramos a configuração padrão das opções &quot;Ajuste as configurações&quot; listadas abaixo. Elas são exibidas quando você clica no ícone de engrenagem ![Ícone de engrenagem dos níveis de acesso](assets/gear-icon-in-access-levels.png) em um botão Editar.

Todas essas alterações desativam uma opção que estava ativada anteriormente por padrão. Se isso não atender às necessidades de sua organização, você poderá habilitá-los ao configurar um novo nível de acesso, ou posteriormente.

>[!IMPORTANT]
>
>Essa alteração de configuração padrão afeta apenas os níveis de acesso criados a partir de agora, não os criados anteriormente.

* Em um novo nível de acesso com um tipo de licença de Plano:

   * Compartilhar em todo o sistema agora está desativado para projetos, tarefas, problemas, portfólios, programas, relatórios, filtros, documentos e modelos.
   * Exibir relatórios internos e compartilhar relatórios publicamente também estão desativados para relatórios.
   * Compartilhar documentos publicamente também está desativado para documentos.

* Em um novo nível de acesso com um tipo de licença de Trabalho:

   * O compartilhamento em todo o sistema agora está desativado para filtros e documentos.
   * Compartilhar documentos publicamente também está desativado para documentos.

* Em um novo nível de acesso com um tipo de licença de Solicitação ou Revisão:

   * O compartilhamento em todo o sistema agora está desativado para filtros.

## Desativar um grupo

À medida que suas organizações internas mudam, talvez seja necessário parar de usar determinados grupos no Workfront e criar novos. Para ajudar nisso, adicionamos a capacidade de desativar um grupo sem perder seus dados históricos. Para usuários regulares que não precisam vê-los, os grupos inativos são apagados dos campos de digitação antecipada de grupo.

Você ainda pode encontrar e configurar opções, preferências e associações de objetos para grupos inativos que gerencia. E desativar um grupo não altera nada sobre os objetos aos quais o grupo está anexado.

Anteriormente, não era possível desativar um grupo.

Para obter mais informações, consulte [Desativar ou reativar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).

## Aprimoramentos no histórico de instalação de blueprints

Ao instalar um blueprint, uma mensagem agora exibe os objetos específicos (como funções, equipes ou grupos) que foram instalados com êxito com o blueprint e quaisquer objetos que falharam na instalação. Você também pode exibir a lista de objetos instalados na página Detalhes do blueprint clicando em Exibir detalhes ao lado de uma instalação específica na tabela de histórico de instalação.

Para obter mais informações, consulte [Instalar um blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).

![Histórico de instalação de blueprints](assets/blueprints-installation-history-350x95.png)

## Um aviso agora é exibido ao instalar um blueprint somente para visualização na produção

Determinados blueprints só estão disponíveis para instalação no ambiente de Pré-visualização para fins de teste.

Se você acessar somente o conteúdo de Visualização no seu ambiente de Produção, Sandbox 1 ou Sandbox 2, o botão Instalar não estará ativo e você poderá ver uma mensagem de aviso.

Para obter mais informações, consulte [Instalar um blueprint](../../../administration-and-setup/blueprints/blueprints-install.md).
