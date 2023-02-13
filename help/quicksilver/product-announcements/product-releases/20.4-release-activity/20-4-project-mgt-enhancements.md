---
title: 20.4 Melhorias no gerenciamento de projetos
description: 20.4 Melhorias no gerenciamento de projetos
author: Luke
draft: Probably
feature: Product Announcements
exl-id: f21f33b3-5e49-4bb0-9eda-7cf4c016361c
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1542'
ht-degree: 0%

---

# 20.4 Melhorias no gerenciamento de projetos

Esta página descreve todas as melhorias no gerenciamento de projetos realizadas com a versão 20.4 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 9 de novembro de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.4, consulte [Visão geral da versão 20.4](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## Novo para administradores: Controlar como um campo personalizado é compartilhado

Para oferecer maior controle sobre quem pode editar, excluir e usar campos personalizados criados, adicionamos a capacidade de configurar exatamente como você deseja que eles sejam compartilhados.

Até agora, quando você criava um campo personalizado, ele era editável por todos no sistema. Esse ainda é o estado padrão de um campo personalizado, mas agora é possível limitar o compartilhamento de um campo personalizado a determinados usuários, funções, equipes, grupos e empresas. E é possível determinar se os recipients podem gerenciar ou exibir apenas o campo personalizado.

Além disso, para tornar essa experiência familiar para você, projetamos a interface do usuário para que esse recurso seja semelhante a outras áreas de objeto que compartilham no Workfront.

Para obter mais informações, consulte [Configurar compartilhamento para campos e widgets personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md).

## Novo para administradores: Compartilhamento de formulário personalizado padronizado

Compartilhamento padronizado para Forms personalizado para que você possa usar o mesmo processo de compartilhamento de objetos do Workfront que já conhece. E a nova experiência de compartilhamento oferece maior controle sobre quem pode editar, excluir e usar o Forms personalizado criado por você. É possível limitar o compartilhamento de um Formulário personalizado para determinados usuários, funções, equipes, grupos e empresas. E você pode determinar se esses destinatários podem exibir ou gerenciar o Formulário personalizado.

Para obter mais informações, consulte [Compartilhar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).

## Exportar formulários personalizados e informações de visão geral da seção Detalhes de um projeto, tarefa ou problema

Agora é possível exportar as informações do formulário personalizado para um arquivo .pdf . É possível exportar formulários personalizados de projetos, tarefas ou problemas ao acessar o formulário na seção Detalhes dos objetos.

Além de exportar os formulários personalizados de projetos, tarefas e problemas, agora também é possível incluir a área Visão geral no seu pdf exportado.

Para obter informações sobre como exportar formulários personalizados de um objeto, consulte [Exportar formulários personalizados e detalhes do objeto](../../../workfront-basics/work-with-custom-forms/export-custom-forms-details.md).

## Adicionar rapidamente uma iteração

>[!NOTE]
>
>Esse recurso foi removido temporariamente do ambiente de Produção. Esta página será atualizada quando o recurso for disponibilizado.

Para simplificar a experiência de criação de uma iteração, adicionamos um novo botão que permite adicionar uma iteração da guia iterações. Aqui, você pode criar uma iteração e adicionar tarefas e problemas posteriormente.

Você ainda pode criar uma iteração na tag de backlog como antes.

Para obter mais informações, consulte [Criar uma iteração](../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md).

## Nova seção Métricas disponível em projetos

Para economizar tempo e aumentar a compreensão da integridade geral de um projeto, agora há uma seção Métricas disponível em um projeto que inclui informações sobre o seguinte:

* Trabalho completo, incompleto, vencido e que está por vir
* Valores de tarefa e emissão agrupados por status ou prioridade
* Trabalho atribuído a cada usuário

Você pode fazer seleções nos gráficos para ver diferentes aspectos das tarefas e problemas em um projeto e clicar em determinados elementos para exibir informações da tarefa.

Esse recurso agora está incluído na variável [Fundamentos do Planejador, caminho de aprendizagem da Parte 3](https://one.workfront.com/s/learningpath3/planner-fundamentals-for-the-new-workfront-experience-part-3-manage-a-project-20Y0z000000bm7xEAA) no Workfront One.

## Novo para administradores: Atribuir um líder comercial a um grupo

Para ajudar você a organizar e definir seus grupos de maneira mais eficaz, adicionamos a capacidade de atribuir um usuário como Líder de Negócios para um grupo (ou subgrupo). Um Líder de negócios é um usuário do Workfront que toma decisões de negócios para um grupo.

O novo campo Líder da empresa pode ser usado em filtros de relatório, visualizações e agrupamentos. Por exemplo, você pode filtrar por um determinado Líder de negócios para listar apenas os grupos para os quais essa pessoa está atribuída nessa função.

Para obter mais informações, consulte [Visão geral do líder empresarial](../../../administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador, caminho de aprendizagem da parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Novo para administradores: Associar portfólios, programas e empresas a grupos

Quando os administradores do Workfront criam ou editam um portfólio, programa ou empresa, eles podem atribuí-lo a um grupo. Com grupos atribuídos a esses objetos, é fácil identificar as responsabilidades do seu grupo para eles.

Por exemplo, você pode listar todos os portfólios de sua organização em um relatório e examinar a coluna Grupo para ver em quais deles seu grupo está trabalhando.

Para obter mais informações, consulte a seção &quot;Sobre a associação de um grupo a um objeto&quot; no artigo [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador, caminho de aprendizagem da parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Novo para administradores: Os administradores de um grupo atribuído a uma empresa podem gerenciar a empresa

Facilitamos para um Administrador de grupo o gerenciamento de uma empresa associada ao grupo no Workfront. O acesso para gerenciar a empresa é automaticamente disponibilizado quando a associação é feita. Isso é especialmente importante quando o Administrador de grupo não tem acesso administrativo às empresas.

Para obter mais informações, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

Para obter informações sobre o acesso administrativo às empresas, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador, caminho de aprendizagem da parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Substitua o botão Trabalho nele por um botão Iniciar

Para ajudar a capturar a data e a hora em que o trabalho realmente começa em um item de trabalho, os usuários podem substituir o botão Trabalhar nele por um botão Iniciar que atualiza automaticamente o status e a Data inicial real do item de trabalho.

Atualizado em 24 de setembro: Depois de clicar em Iniciar tarefa ou Iniciar problema, agora você tem a opção de reverter sua escolha e indicar que talvez não esteja pronto para começar a trabalhar em um item de trabalho clicando em Desfazer. O item de trabalho retorna ao status Novo e a Data de confirmação e a Data de início real são excluídas. A opção Desfazer é exibida por um curto período de tempo e é apagada depois que você sai ou atualiza a página.

Para obter mais informações sobre como configurar essa opção, consulte [Substitua o botão Trabalho nele por um botão Iniciar](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

Esse recurso agora está incluído na variável [Caminho de aprendizado dos Fundamentos do Trabalhador](https://one.workfront.com/s/learningpath3/worker-fundamentals-for-the-new-workfront-experience-20Y0z000000blg8EAA) e [Fundamentos do administrador, caminho de aprendizagem da parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Permitir vários rascunhos para um tópico da fila

Para proporcionar mais liberdade ao trabalhar com solicitações, não há mais um limite para quantos rascunhos você pode salvar em um tópico da fila. Ao criar uma nova solicitação, você pode selecionar um rascunho existente em uma lista de rascunhos para o mesmo tópico da fila, sobrescrevê-lo e enviá-lo como uma nova solicitação ou criar uma nova solicitação do zero.

Antes desse aprimoramento, o Workfront salvou apenas um rascunho para cada tópico da fila na fila de solicitações.

Para obter informações sobre como enviar solicitações, consulte &quot; [Criar e enviar solicitações do Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

## Atribuir um grupo a uma equipe

Para facilitar o gerenciamento e o relatório das equipes associadas a um grupo, agora é possível atribuir qualquer grupo a uma equipe que você tem acesso para editar.

Quando você atribui uma equipe a um grupo, os Administradores do grupo podem gerenciar a equipe sem ser membro dela. Na página Detalhes da equipe, eles podem ver as equipes atribuídas aos grupos que gerenciam. E eles podem executar um relatório para listar todas as equipes associadas a um determinado grupo.

Para obter mais informações, consulte [Criar um grupo](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Esse recurso agora está incluído na variável [Fundamentos do administrador, caminho de aprendizagem da parte 1](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) no Workfront One.

## Novos campos permitem criar relatórios sobre dados para um grupo de nível superior e todos os seus subgrupos

Para ajudar você a identificar dados associados a um grupo de nível superior e seus subgrupos, adicionamos um novo campo ID principal que pode ser usado em Filtros, Exibições e Agrupamentos ao criar relatórios sobre objetos do Grupo.

Esse campo deve ser útil especialmente para administradores de grupo que gerenciam grupos que contêm vários subgrupos.

Por exemplo, imagine que você gerencia um grupo chamado Marketing que tem os subgrupos de Marketing de campo e Marketing digital. Você pode listar os projetos que pertencem a todos os três grupos criando um filtro de área Projetos que tenha a seguinte Regra de filtro:
<pre>Grupo: Nome principal superior &gt; Igual &gt; Marketing</pre>Também adicionamos um novo campo Nome principal principal superior que pode ser usado para identificar dados associados a grupos de nível superior em Exibições (não em Filtros ou Agrupamentos).

Para obter informações sobre o uso de campos em listas e relatórios, consulte [Glossário da terminologia do Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

## Nova opção para cancelar a ação ao descartar um rascunho de solicitação

Ao descartar um rascunho salvo, você pode clicar em Cancelar na mensagem de confirmação que informa que seu rascunho será excluído. Dessa forma, você não perde o rascunho caso mude de ideia sobre descartá-lo.

Esse recurso está disponível somente na nova experiência do Workfront. Para obter mais informações, consulte [Criar e enviar solicitações do Workfront](https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FManage_work%2FRequests%2FCreate_Requests%2Fcreate-submit-requests.html).

