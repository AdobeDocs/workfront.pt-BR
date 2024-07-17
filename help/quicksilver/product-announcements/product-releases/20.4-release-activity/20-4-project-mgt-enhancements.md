---
title: 20.4 Aprimoramentos no gerenciamento de projetos
description: 20.4 Aprimoramentos no gerenciamento de projetos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1485'
ht-degree: 0%

---

# 20.4 Aprimoramentos no gerenciamento de projetos

Esta página descreve todas as melhorias de gerenciamento de projeto feitas com a versão 20.4 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 9 de novembro de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.4, consulte a [visão geral da versão 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novo para administradores: controlar como um campo personalizado é compartilhado

Para oferecer maior controle sobre quem pode editar, excluir e usar os campos personalizados criados por você, adicionamos a capacidade de configurar exatamente como deseja que eles sejam compartilhados.

Até agora, quando você criou um campo personalizado, ele podia ser editado por todos no sistema. Esse ainda é o estado padrão de um campo personalizado, mas agora é possível limitar o compartilhamento de um campo personalizado a determinados usuários, funções, equipes, grupos e empresas. E você pode determinar se seus recipients podem gerenciar ou visualizar somente o campo personalizado.

Além disso, para tornar essa experiência familiar para você, projetamos a interface do usuário para que esse recurso seja semelhante a outras áreas de objeto compartilhadas no Workfront.

Para obter mais informações, consulte [Configurar compartilhamento para campos e widgets personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md).

## Novo para administradores: compartilhamento de formulário personalizado padronizado

Nós padronizamos o compartilhamento do Forms personalizado para que você possa usar o mesmo processo de compartilhamento de objetos do Workfront que já conhece. E a nova experiência de compartilhamento oferece maior controle sobre quem pode editar, excluir e usar o Forms personalizado que você cria. É possível limitar o compartilhamento de um Formulário personalizado a determinados usuários, funções, equipes, grupos e empresas. E você pode determinar se esses destinatários podem visualizar ou gerenciar o Formulário personalizado.

Para obter mais informações, consulte [Compartilhar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exportar formulários personalizados e informações de visão geral da seção Detalhes de um projeto, tarefa ou problema

Agora é possível exportar as informações de formulário personalizado para um arquivo .pdf. É possível exportar formulários personalizados de projetos, tarefas ou problemas ao acessar o formulário na seção Detalhes dos objetos.

Além de exportar os formulários personalizados de projetos, tarefas e problemas, agora também é possível incluir a área Visão geral no pdf exportado.

Para obter informações sobre como exportar formulários personalizados de um objeto, consulte [Exportar formulários personalizados e detalhes do objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Adicionar uma iteração rapidamente

>[!NOTE]
>
>Esse recurso foi removido temporariamente do ambiente de Produção do. Esta página será atualizada quando o recurso se tornar disponível.

Para simplificar a experiência de criar uma iteração, adicionamos um novo botão que permite adicionar uma iteração da guia iterações. Aqui, você pode criar uma iteração e, em seguida, adicionar tarefas e problemas posteriormente.

Você ainda pode criar uma iteração na tag de backlog como antes.

Para obter mais informações, consulte [Criar uma iteração](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nova seção Métricas disponível em projetos

Para economizar tempo e aumentar a compreensão da integridade geral de um projeto, agora há uma seção Métricas disponível em um projeto que inclui informações sobre o seguinte:

* Trabalho concluído, incompleto, atrasado e no futuro próximo
* Valores de tarefas e problemas agrupados por status ou prioridade
* Esforço de trabalho atribuído a cada usuário

Você pode fazer seleções nos gráficos para ver diferentes aspectos das tarefas e problemas em um projeto e clicar em determinados elementos para exibir informações da tarefa.

Este recurso agora está incluído no [Fundamentos do planejador, Parte 3 do caminho de aprendizado](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) no Workfront One.

## Novo para administradores: atribuir um líder de negócios a um grupo

Para ajudá-lo a organizar e definir melhor seus grupos, adicionamos a capacidade de atribuir um usuário como Líder de negócios para um grupo (ou subgrupo). Um Líder de negócios é um usuário do Workfront que toma decisões de negócios para um grupo.

O novo campo Líder de negócios pode ser usado em filtros, visualizações e agrupamentos de relatórios. Por exemplo, você pode filtrar por um determinado Líder de negócios para listar apenas os grupos aos quais essa pessoa está atribuída nessa função.

Para obter mais informações, consulte [Visão geral do Líder de negócios](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

Este recurso agora está incluído no [Princípios básicos do administrador, Parte 1 do caminho de aprendizado](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Novo para administradores: associe portfólios, programas e empresas a grupos

Quando os administradores do Workfront criam ou editam um portfólio, programa ou empresa, eles podem atribuí-lo a um grupo. Com grupos atribuídos a esses objetos, é fácil identificar as responsabilidades de seu grupo por eles.

Por exemplo, você pode listar todos os portfólios de sua organização em um relatório e examinar a coluna Grupo para ver em quais deles seu grupo está trabalhando.

Para obter mais informações, consulte a seção &quot;Sobre a associação de um grupo a um objeto&quot; no artigo [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Este recurso agora está incluído no [Princípios básicos do administrador, Parte 1 do caminho de aprendizado](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Novo para administradores: os administradores de um grupo atribuído a uma empresa podem gerenciar a empresa

Tornamos fácil para um Administrador de grupo gerenciar uma empresa associada ao grupo no Workfront. O acesso para gerenciar a empresa é disponibilizado automaticamente quando a associação é feita. Isso é especialmente importante quando o Administrador do grupo não tem acesso administrativo às empresas.

Para obter mais informações, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Para obter informações sobre acesso administrativo a empresas, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Este recurso agora está incluído no [Princípios básicos do administrador, Parte 1 do caminho de aprendizado](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Substitua o botão Trabalhar na tarefa por um botão Iniciar

Para ajudar a capturar a data e a hora em que o trabalho começa em um item de trabalho, os usuários podem substituir o botão Trabalhar na tarefa por um botão Iniciar que atualiza automaticamente o status e a Data de início real do item de trabalho.

Atualizado em 24 de setembro: depois de clicar em Iniciar tarefa ou Iniciar problema, você agora tem a opção de reverter sua escolha e indicar que pode não estar pronto para começar a trabalhar em um item de trabalho clicando em Desfazer. O item de trabalho retorna ao status Novo, e a Data de Confirmação e a Data de Início Efetivo são excluídas. A opção Desfazer é exibida por um período muito curto e é desmarcada depois de sair ou atualizar a página.

Para obter mais informações sobre como configurar esta opção, consulte [Substituir o botão Trabalhar na tarefa por um botão Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Este recurso agora está incluído no [Caminho de Aprendizado de Fundamentos do Trabalhador](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) e na [Parte Fundamentos do Administrador, Parte 1 do caminho de aprendizado](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Permitir vários rascunhos para um tópico da fila

Para lhe dar mais liberdade ao trabalhar com solicitações, não há mais um limite para quantos rascunhos você pode salvar para um tópico da fila. Ao criar uma nova solicitação, você pode selecionar um rascunho existente em uma lista de rascunhos para o mesmo tópico da fila, sobregravá-lo e submetê-lo como uma nova solicitação ou criar uma nova solicitação do zero.

Antes desse aprimoramento, o Workfront salvava apenas um rascunho para cada tópico da fila de solicitações.

Para obter informações sobre o envio de solicitações, consulte &quot; [Criar e enviar solicitações do Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Atribuir um grupo a uma equipe

Para facilitar o gerenciamento e a criação de relatórios sobre as equipes associadas a um grupo, agora é possível atribuir qualquer grupo a uma equipe que você tenha acesso para editar.

Quando você atribui uma equipe a um grupo, os Administradores de grupo podem gerenciá-la sem ser um membro dela. Na página Detalhes da equipe, é possível ver as equipes atribuídas aos grupos que gerenciam. E eles podem executar um relatório para listar todas as equipes associadas a um determinado grupo.

Para obter mais informações, consulte [Criar uma equipe](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Este recurso agora está incluído no [Princípios básicos do administrador, Parte 1 do caminho de aprendizado](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Novos campos permitem relatar dados de um grupo de nível superior e de todos os seus subgrupos

Para ajudar a identificar dados associados a um grupo de nível superior e a seus subgrupos, adicionamos um novo campo ID principal que pode ser usado em Filtros, Exibições e Agrupamentos quando você cria relatórios sobre objetos de Grupo.

Este campo deve ser especialmente útil para Administradores de grupo que gerenciam grupos que contêm vários subgrupos.

Por exemplo, imagine que você gerencia um grupo chamado Marketing que tem os subgrupos Marketing de campo e Marketing digital. Você pode listar os projetos que pertencem a todos os três grupos criando um filtro da área Projetos que tenha a seguinte regra de filtro:
<pre>Grupo: Nome do Pai Superior &gt; Igual &gt; Marketing</pre>Também adicionamos um novo campo Nome do pai superior que você pode usar para identificar dados associados a grupos de nível superior em Exibições (não em Filtros ou Agrupamentos).

Para obter informações sobre o uso de campos em listas e relatórios, consulte [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nova opção para cancelar sua ação ao descartar um rascunho de solicitação

Ao descartar um rascunho salvo, agora você pode clicar em Cancelar na mensagem de confirmação que informa que o rascunho será excluído. Dessa forma, você não perde o rascunho caso mude de ideia sobre descartá-lo.

Esse recurso está disponível somente na nova experiência do Workfront. Para obter informações, consulte [Criar e enviar solicitações do Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

