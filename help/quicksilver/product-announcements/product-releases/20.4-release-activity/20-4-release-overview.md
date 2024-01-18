---
content-type: release-notes
navigation-topic: product-releases
title: Visão geral da versão 20.4
description: A versão 20.4 foi disponibilizada no ambiente de Produção na semana de 9 de novembro de 2020. Para obter datas e horas de lançamento específicas para cada cluster, consulte o Site de Status do Workfront.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 7cf7f6ed-fe85-4c86-bb4b-dd93197338cf
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '3694'
ht-degree: 0%

---

# Visão geral da versão 20.4

A versão 20.4 foi disponibilizada no ambiente de Produção na semana de 9 de novembro de 2020.

Esta página fornece informações sobre a funcionalidade do Adobe Workfront Classic e da nova experiência do Adobe Workfront incluída na versão 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
[Marketing one-liner for the release]
</MadCap:conditionalText>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">As the 20.4 release nears its planned Production release, this page will be updated with all functionality included with 20.4.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">These enhancements are currently available in the Preview environment and will be made available in the Production environment the week of November 9, 2020. For specific release dates and times for each cluster, see the <a href="https://status.workfront.com/" target="_blank">Workfront Status Site</a>. </p>
-->

## Aprimoramentos do Workfront

* [Melhorias do administrador](#administrator-enhancements)
* [Melhorias no gerenciamento de recursos](#resource-management-enhancements)
* [Aprimoramentos no gerenciamento de projetos](#project-management-enhancements)
* [Analítica aprimorada](#enhanced-analytics)
* [Aprimoramentos de provas](#proofing-enhancements)
* [Aprimoramentos de mobilidade e integração](#mobile-and-integration-enhancements)
* [Outras melhorias](#other-enhancements)

### Melhorias do administrador {#administrator-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Novo para administradores: controlar como um campo personalizado é compartilhado</a> </p> <p>Para oferecer maior controle sobre quem pode editar, excluir e usar os campos personalizados criados por você, adicionamos a capacidade de configurar exatamente como deseja que eles sejam compartilhados.</p> <p>Até agora, quando você criou um campo personalizado, ele podia ser editado por todos no sistema. Esse ainda é o estado padrão de um campo personalizado, mas agora é possível limitar o compartilhamento de um campo personalizado a determinados usuários, funções, equipes, grupos e empresas. E você pode determinar se seus recipients podem gerenciar ou visualizar somente o campo personalizado.</p> <p>Além disso, para tornar essa experiência familiar para você, projetamos a interface do usuário para que esse recurso seja semelhante a outras áreas de objeto compartilhadas no Workfront.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 15 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new7" class="MCXref xref" xrefformat="{para}">Novo para administradores: compartilhamento de formulário personalizado padronizado</a> </p> <p>Nós padronizamos o compartilhamento do Forms personalizado para que você possa usar o mesmo processo de compartilhamento de objetos do Workfront que já conhece. E a nova experiência de compartilhamento oferece maior controle sobre quem pode editar, excluir e usar o Forms personalizado que você cria. É possível limitar o compartilhamento de um Formulário personalizado a determinados usuários, funções, equipes, grupos e empresas. E você pode determinar se esses destinatários podem visualizar ou gerenciar o Formulário personalizado.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 15 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Novo para administradores: opção de alternar ambiente do Workfront disponível</a> </p> <p>Para obter uma experiência mais eficiente e conveniente, os administradores de grupo e os administradores do Workfront agora podem alternar rapidamente entre diferentes ambientes do Workfront de qualquer página no Workfront sem precisar fazer logoff.</p> <p>Na nova experiência do Workfront, a opção Alternar para o clássico aparece no Menu principal.</p> <p>No Workfront Classic, a opção Alternar para a nova experiência é exibida no menu exibido ao clicar na imagem do perfil no canto superior direito da Barra de navegação global.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new8" class="MCXref xref" xrefformat="{para}">Novo para administradores: os administradores de um grupo atribuído a uma empresa podem gerenciar a empresa</a> </p> <p>Tornamos fácil para um Administrador de grupo gerenciar uma empresa associada ao grupo no Workfront. O acesso para gerenciar a empresa é disponibilizado automaticamente quando a associação é feita. Isso é especialmente importante quando o Administrador do grupo não tem acesso administrativo às empresas.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new5" class="MCXref xref" xrefformat="{para}">Novo para administradores: melhorias na notificação por email</a> </p> <p>Agora, com um único clique, você pode ativar ou desativar uma notificação por email de evento em Configurar. Basta clicar na opção Ligar/Desligar ao lado do nome da notificação.</p> <p>Além disso, observe que nosso estilo moderno agora melhora a experiência de configuração de notificações de eventos na área Notificações por email.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Novo para administradores: associe portfólios, programas e empresas a grupos</a> </p> <p>Quando os administradores do Workfront criam ou editam um portfólio, programa ou empresa, eles podem atribuí-lo a um grupo. Com grupos atribuídos a esses objetos, é fácil identificar as responsabilidades de seu grupo por eles. </p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 25 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#assign" class="MCXref xref" xrefformat="{para}">Atribuir um grupo a uma equipe</a> </p> <p>Para facilitar o gerenciamento e a criação de relatórios sobre as equipes associadas a um grupo, agora é possível atribuir qualquer grupo a uma equipe que você tenha acesso para editar.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 29 de agosto de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Novo para administradores: atribuir um líder de negócios a um grupo</a> </p> <p>Para ajudá-lo a organizar e definir melhor seus grupos, adicionamos a capacidade de atribuir um usuário como Líder de negócios para um grupo (ou subgrupo). Um Líder de negócios é um usuário do Workfront que toma decisões de negócios para um grupo.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 21 de agosto de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#introduc" class="MCXref xref" xrefformat="{para}">Apresentação do Workfront para MobileIron</a> </p> <p>A Workfront fez parceria com a MobileIron, uma plataforma MDM (Mobile Device Management, gerenciamento de dispositivos móveis), para fornecer às organizações uma experiência móvel mais segura e controlada.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta Preview: N/D</p> <p>Versão de produção: 21 de agosto de 2020</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Melhorias no gerenciamento de recursos {#resource-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#plan" class="MCXref xref" xrefformat="{para}">Planeje o trabalho usando o esforço do trabalho em vez das horas planejadas</a> </p> <p>Para oferecer flexibilidade ao planejar um trabalho em seus projetos, introduzimos o novo conceito de Esforço de trabalho para tarefas. Você pode estimar se o Esforço de trabalho de uma tarefa é pequeno, médio ou grande sem estimar manualmente as Horas planejadas da tarefa. Cada nível de esforço é calculado com base em uma porcentagem de tempo das horas típicas por dia, conforme configurado em sua instância.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#project" class="MCXref xref" xrefformat="{para}">Cores baseadas no status do projeto para itens de trabalho no Balanceador de carga de trabalho</a> </p> <p>Para melhor visibilidade e maior personalização de sua experiência no Balanceador de carga de trabalho, agora é possível alterar as cores dos projetos e seus itens de trabalho para corresponder ao status dos projetos. As cores correspondem aos status de projeto de nível de grupo ou de sistema. As cores exibidas podem corresponder aos status do sistema e do projeto personalizado.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#adjust" class="MCXref xref" xrefformat="{para}">Ajustar a alocação de usuários usando valores percentuais no Balanceador de carga de trabalho</a> </p> <p>Agora é possível gerenciar as alocações dos usuários no Balanceador de carga de trabalho usando porcentagens em vez de horas.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Novo ícone para alternar entre horas e valores percentuais ou tempo alocado e restante no Balanceador de carga de trabalho</a> <p>Adicionamos uma nova configuração que permite alternar entre Horas e Porcentagens alocadas à medida que você visualiza o Balanceador de carga de trabalho. Com esse novo ícone, também eliminamos a seção Carga de trabalho do usuário no painel Configurações. O Balanceador de carga de trabalho mostra o tempo alocado por padrão e movemos a configuração Horas restantes para o novo ícone Porcentagem ou Horas.</p></td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 25 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#a" class="MCXref xref" xrefformat="{para}">Um novo filtro integrado para o Balanceador de carga de trabalho: Usuários em projetos</a> </p> <p>Para tornar sua experiência de filtragem no Balanceador de carga de trabalho mais eficiente, adicionamos um novo filtro incorporado na área Trabalho atribuído. Agora é possível aplicar o filtro Usuários em projetos, que exibe os usuários atribuídos a tarefas e problemas nos projetos especificados.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 25 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#visualiz" class="MCXref xref" xrefformat="{para}">Visualizar trabalho concluído no Balanceador de carga de trabalho</a> </p> <p>Para permitir que você identifique facilmente o trabalho que já foi concluído e gerencie as atribuições de usuário corretamente, ativamos um indicador visual no Balanceador de carga de trabalho que mostra quando os itens de um período selecionado foram concluídos. Agora você pode ver uma marca de seleção verde para tarefas, problemas quando são concluídas. O projeto também exibe a marca de seleção verde quando há itens de trabalho concluídos durante o período exibido na tela.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 11 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Novo filtro padrão para a área Trabalho atribuído no Balanceador de carga de trabalho</a> </p> <p>O filtro Padrão da área Trabalho atribuído no Balanceador de carga de trabalho agora exibe somente os usuários que são membros de todas as equipes às quais você, como usuário conectado, está associado. O novo filtro agora exibe as informações mais relevantes para você, por padrão.</p> <p>Antes dessa melhoria, todos os usuários que você tinha acesso para visualizar eram exibidos nessa área. </p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 11 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#user" class="MCXref xref" xrefformat="{para}">Gráfico de alocação de usuários no Balanceador de carga de trabalho</a> </p> <p>Para permitir que você tenha uma representação visual de alto nível da alocação de usuários em um determinado período, uma nova configuração agora permite uma visualização de gráfico de como as alocações são exibidas no Balanceador de carga de trabalho. Ativar essa configuração exibe a alocação dos usuários em um gráfico de linhas que indica as superalocações em blocos vermelhos e as subalocações em azul. </p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 29 de agosto de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#show" class="MCXref xref" xrefformat="{para}">Mostrar ou ocultar o trabalho concluído no Balanceador de carga de trabalho</a> </p> <p>Uma nova configuração agora permite mostrar ou ocultar itens de trabalho concluídos no Balanceador de carga de trabalho. A configuração é ativada por padrão e itens de trabalho concluídos que correspondem aos critérios de filtragem e ao período selecionado são exibidos no Balanceador de carga de trabalho. </p> <p>Antes dessa melhoria, os itens de trabalho concluídos sempre eram exibidos no Balanceador de carga de trabalho.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 21 de agosto de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-resource-mgt-enhancements.md#usabilit" class="MCXref xref" xrefformat="{para}">Melhorias de usabilidade no Balanceador de carga de trabalho</a> </p> <p>Para garantir uma experiência simplificada e amigável ao gerenciar os recursos no Balanceador de carga de trabalho, várias melhorias de usabilidade estão disponíveis.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 21 de agosto de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Aprimoramentos no gerenciamento de projetos {#project-management-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#export" class="MCXref xref" xrefformat="{para}">Exportar formulários personalizados e informações de visão geral da seção Detalhes de um projeto, tarefa ou problema</a> </p> <p>Agora é possível exportar as informações de formulário personalizado para um arquivo .pdf. É possível exportar formulários personalizados de projetos, tarefas ou problemas ao acessar o formulário na seção Detalhes dos objetos. </p> <p>Além de exportar os formulários personalizados de projetos, tarefas e problemas, agora também é possível incluir a área Visão geral no pdf exportado.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de visualização beta: 15 de outubro de 2020 (a exportação da área Visão geral foi adicionada em 3 de novembro de 2020)</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#quickly" class="MCXref xref" xrefformat="{para}">Adicionar uma iteração rapidamente</a> </p> <p>Para simplificar a experiência de criar uma iteração, adicionamos um novo botão que permite adicionar uma iteração da guia iterações. Aqui, você pode criar uma iteração e, em seguida, adicionar tarefas e problemas posteriormente.</p> <p>Você ainda pode criar uma iteração na tag de backlog como antes.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 15 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4 <span style="color: #dc143c; font-weight: bold;">Temporariamente indisponível</span></p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new6" class="MCXref xref" xrefformat="{para}">Nova seção Métricas disponível em projetos</a> </p> <p>Para economizar tempo e aumentar a compreensão da integridade geral de um projeto, agora há uma seção Métricas disponível em um projeto que inclui informações sobre o seguinte:</p> 
    <ul> 
     <li>Trabalho concluído, incompleto, atrasado e no futuro próximo</li> 
     <li>Valores de tarefas e problemas agrupados por status ou prioridade</li> 
     <li>Esforço de trabalho atribuído a cada usuário</li> 
    </ul> <p>Você pode fazer seleções nos gráficos para ver diferentes aspectos das tarefas e problemas em um projeto e clicar em determinados elementos para exibir informações da tarefa.</p> <p>Para saber mais, consulte <a href="../../../manage-work/projects/manage-projects/project-metrics.md" class="MCXref xref" xrefformat="{para}" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Visão geral das métricas do projeto</a>.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 23 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Nova opção para cancelar sua ação ao descartar um rascunho de solicitação</a> <p>Ao descartar um rascunho salvo, agora você pode clicar em Cancelar na mensagem de confirmação que informa que o rascunho será excluído. Dessa forma, você não perde o rascunho caso mude de ideia sobre descartá-lo.</p></td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 25 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#replace" class="MCXref xref" xrefformat="{para}">Substitua o botão Trabalhar na tarefa por um botão Iniciar</a> </p> <p>Para ajudar a capturar a data e a hora em que o trabalho começa em um item de trabalho, os usuários podem substituir o botão Trabalhar na tarefa por um botão Iniciar que atualiza automaticamente o status e a Data de início real do item de trabalho.</p> </td> 
   <td> <p><strong>Disponível nas seguintes datas:</strong> </p> <p>Versão de pré-visualização beta: 20 de agosto de 2020</p> <p>Versão de produção: 8 de outubro de 2020</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#new4" class="MCXref xref" xrefformat="{para}">Novos campos permitem relatar dados de um grupo de nível superior e de todos os seus subgrupos</a> </p> <p>Para ajudar a identificar dados associados a um grupo de nível superior e a seus subgrupos, adicionamos um novo campo ID principal que pode ser usado em Filtros, Exibições e Agrupamentos quando você cria relatórios sobre objetos de Grupo.</p> <p>Este campo deve ser especialmente útil para Administradores de grupo que gerenciam grupos que contêm vários subgrupos.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 29 de agosto de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-project-mgt-enhancements.md#allow" class="MCXref xref" xrefformat="{para}">Permitir vários rascunhos para um tópico da fila</a> </p> <p>Para lhe dar mais liberdade ao trabalhar com solicitações, não há mais um limite para quantos rascunhos você pode salvar para um tópico da fila. Ao criar uma nova solicitação, você pode selecionar um rascunho existente em uma lista de rascunhos para o mesmo tópico da fila, sobregravá-lo e submetê-lo como uma nova solicitação ou criar uma nova solicitação do zero. </p> <p>Antes desse aprimoramento, o Workfront salvava apenas um rascunho para cada tópico da fila de solicitações. </p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 21 de agosto de 2020</p> <p>Versão de produção: 17 de setembro de 2020</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Analítica aprimorada  {#enhanced-analytics}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-analytics-enhancements.md#paginati" class="MCXref xref" xrefformat="{para}">Paginação e classificação adicionadas à Análise aprimorada</a> </p> <p>Para permitir que você visualize as informações que deseja ver sem precisar aplicar filtros restritivos, adicionamos opções de paginação e classificação a cada gráfico na área Analítica aprimorada.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Aprimoramentos de provas {#proofing-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#carry" class="MCXref xref" xrefformat="{para}">Continuar o fluxo de trabalho de prova existente ao gerar uma nova versão</a> </p> <p>Agora, o fluxo de trabalho de prova existente é transferido para qualquer nova versão criada, independentemente do método em que é gerada.</p> <p>Anteriormente, havia uma pequena diferença em como o fluxo de trabalho de prova era transportado, dependendo de onde você os gerava no Workfront.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 8 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4 <span class="uitext" style="color: #dc143c;">(Adiado para março de 2021)</span></p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#auto-gen" class="MCXref xref" xrefformat="{para}">Gerar uma prova automaticamente ao carregar uma configuração de documento desativada por padrão</a> </p> <p>A opção no perfil do usuário de gerar provas automaticamente ao fazer upload de documentos agora está desativada por padrão para novos usuários de prova. Essa alteração não afeta os usuários atuais. Se essa configuração estiver ativada, ela permanecerá assim.</p> <p>Anteriormente, essa configuração era ativada para novos usuários por padrão.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 18 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-proof-enhancements.md#document" class="MCXref xref" xrefformat="{para}">Botões de aprovação de documento disponíveis no Visualizador de provas</a> </p> <p>Para alinhar-se à experiência de prova no Classic, os botões de aprovação de documentos agora estão disponíveis no Visualizador de provas na nova experiência do Adobe Workfront.</p> <p>Anteriormente, só era possível aprovar um documento na área Detalhes do documento.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de pré-visualização beta: 9 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> </td> 
  </tr> 
 </tbody> 
</table>

### Aprimoramentos de mobilidade e integração {#mobile-and-integration-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#added" class="MCXref xref" xrefformat="{para}">Adição da funcionalidade em notificações do Microsoft Teams </a> </p> <p>Para facilitar o uso do Workfront por meio do Microsoft Teams, adicionamos uma nova funcionalidade às notificações de Microsoft Teams enviadas pelo Workfront.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão de visualização Beta: a ser definida</p> <p>Versão de produção: com a versão 20.4 <strong>(Adiado para dezembro de 2020 ou início de 2021)</strong></p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#get" class="MCXref xref" xrefformat="{para}">Obter ajuda com os comandos do assistente virtual do Workfront Mobile</a> </p> <p>No aplicativo móvel, você pode pedir ao assistente virtual para ajudá-lo com comandos dizendo O que posso fazer?" e "Ajude-me com os comandos".</p> <p>Esses comandos exibem uma lista das coisas diferentes sobre as quais você pode perguntar ao assistente.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta Preview: N/D</p> <p>Versão de produção: com a versão 20.4 </p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-mobile-enhancements.md#create" class="MCXref xref" xrefformat="{para}">Criar uma tarefa rapidamente no aplicativo móvel do Workfront</a> </p> <p>Use a nova opção de tarefa rápida no aplicativo móvel Workfront para criar tarefas rapidamente. Basta digitar o nome da tarefa e anexar todos os documentos que você possa ter. Você ainda pode preencher campos adicionais como descrições e atribuições, se necessário. Basta clicar na seta à direita do nome da tarefa.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 18 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

### Outras melhorias {#other-enhancements}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Recurso</strong> </p> </td> 
   <td> <p><strong>Datas e ambientes de lançamento</strong> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#improved" class="MCXref xref" xrefformat="{para}">Criptografia aprimorada para Workfront Proof</a> </p> <p>Estamos fazendo algumas alterações para melhorar a força da criptografia de dados em movimento do Workfront Proofing Application. As cifras TLS fracas serão descontinuadas em 11 de novembro de 2020.</p> <p>Verifique se você está usando um navegador compatível ao acessar o Workfront. </p> <p> </p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 20 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new2" class="MCXref xref" xrefformat="{para}">Nova aparência para 3 modelos de email</a> </p> <p>Para melhorar a legibilidade e a experiência geral, os seguintes modelos de email têm uma nova aparência</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 15 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new3" class="MCXref xref" xrefformat="{para}">Novas notificações por email para equipes</a> </p> <p>Adicionamos duas novas notificações por email para equipes: quando um único predecessor de uma tarefa atribuída à sua equipe é concluído e quando todos os predecessores de uma tarefa atribuída à sua equipe são concluídos.</p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 15 de outubro de 2020</p> <p>Versão de produção: com a versão 20.4</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><a href="../../../product-announcements/product-releases/20.4-release-activity/20-4-other-enhancements.md#new" class="MCXref xref" xrefformat="{para}">Novos objetos de API que acionam atualizações de assinatura de evento</a> </p> <p>Dois novos objetos de API, documentVersion e proofApproval, foram criados e estão configurados para acionar atualizações de assinatura de evento quando um documento é versionado ou aprovado. </p> </td> 
   <td><strong>Disponível nas seguintes datas:</strong> <p>Versão Beta de pré-visualização: 11 de setembro de 2020</p> <p>Versão de produção: com a versão 20.4 para produção</p> <p><strong>Disponível nestes ambientes:</strong> </p> <p>A nova experiência do Adobe Workfront </p> <p>Adobe Workfront Classic </p> </td> 
  </tr> 
 </tbody> 
</table>

## Aprimoramentos no Planejador de cenários do Workfront

A maioria dos novos recursos chegando à versão do Planejador de cenários do Workfront com a versão 20.4. Para obter informações sobre esses novos recursos agora disponíveis na Pré-visualização, consulte [Planejador de cenários do Workfront com a versão 20.4 - 14 de outubro de 2020](../../../product-announcements/product-releases/scenario-planner-release-activity/sp-release-20.4.md).

## Aprimoramentos das metas do Workfront

A maioria dos novos recursos chegando ao Workfront Goals versão 20.4. Para obter informações sobre esses novos recursos agora disponíveis na Pré-visualização, consulte [Workfront Goals com a versão 20.4](../../../product-announcements/product-releases/goals-release-activity/goals-release-20-4.md).

## Aprimoramentos do Workfront Fusion

Os novos recursos do Workfront Fusion estão disponíveis na Produção em uma cadência fora da programação de lançamento 20.4. Para obter mais informações sobre os recursos mais recentes, consulte [Atividade de lançamento do Adobe Workfront Fusion](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md)

## Aprimoramentos na API

A API versão 12 já está disponível com a versão 20.4.

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
This section will be updated with more information prior to the 20.4 release being available in Production.
</MadCap:conditionalText>
-->

Para obter informações sobre novidades e atualizações, consulte [Novidades da API versão 12](https://one.workfront.com/s/document-item?bundleId=workfront-classic&amp;topicId=Content%2FWF_API%2FAPI%2Fnew-api-version-12.htm).

Para obter mais informações sobre versões de API, consulte [Controle de versão da API e programação de suporte](../../../wf-api/api/api-version-support-schedule.md)

<!--
<a href="https://experience.workfront.com/s/article/API-Version-Release-and-Support-Schedule-272875487?language=en_US&r=13&ui-comm-runtime-components-aura-components-siteforce-qb.Quarterback.validateRoute=1&ui-communities-components-aura-components-forceCommunity-breadcrumbs.Breadcrumbs.getAncestors=1&ui-communities-components-aura-components-forceCommunity-seoAssistant.SeoAssistant.getSeoData=1&ui-force-components-controllers-recordGlobalValueProvider.RecordGvp.getRecord=1&ui-self-service-components-controller.ArticleTopicList.getTopics=1&ui-self-service-components-controller.ArticleView.getArticleHeaderDetail=1" target="_blank" data-mc-conditions="OnlineOrPDF.PrintOnly,QuicksilverOrClassic.Draft mode">API Version Release and Support Schedule</a>
-->

.

## Atualizações de manutenção do Workfront 

Para obter informações sobre as atualizações de manutenção feitas durante a versão 20.3, consulte [Atualizações de manutenção do Workfront](https://experience.workfront.com/s/article/Workfront-Maintenance-Updates-1882317350).

## Anúncios

* [Descontinuação do Flash](#flash-deprecation)
* [Webinário da versão 20.4](#20-4-release-webinar)
* [Alteração na cadência de lançamento da Visualização](#change-in-preview-release-cadence)
* [➡ Inclui na lista de permissões de domínios adicionais necessários para acessar o Workfront](#allowlist-of-additional-domains-required-for-accessing-workfront)
* [Workfront One](#workfront-one)

### Descontinuação do Flash {#flash-deprecation}

No final de 2020, o Adobe e todos os principais navegadores finalizarão a tecnologia de Flash Adobe em desativação, o que significa que essas ferramentas deixarão de funcionar.

A Workfront tem como objetivo ajudá-lo a migrar para a tecnologia mais recente, fornecendo um conjunto de novas soluções que não dependem do Flash. Saiba mais sobre as soluções de substituição para cada ferramenta baseada em Flash específica no seguinte artigo: [Substituição de ferramentas baseadas em Flashes no Adobe Workfront](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md).

Todas as ferramentas baseadas em Flashes serão removidas de todos os produtos em 19 de novembro de 2020. Recomendamos começar a usar as novas ferramentas e desativar as ferramentas do Flash antes disso, para aumentar a segurança da sua instância. Se desejar que desativemos as ferramentas do Flash antes de 19 de novembro, entre em contato com o Suporte ao cliente.

### Webinário da versão 20.4 {#20-4-release-webinar}

O webinário da versão do Workfront 20.4 será apresentado na quarta-feira, 28 de outubro de 2020, às 11h, horário do Pacífico. Inscreva-se no webinário [aqui](https://webinars.on24.com/workfront/204release?partnerref=CXnewsletter).

### Alteração na cadência de lançamento da Visualização {#change-in-preview-release-cadence}

A partir de 20 de maio de 2020, o Workfront começou a disponibilizar a funcionalidade no ambiente de Pré-visualização semanalmente. Antes dessa alteração, a funcionalidade normalmente era lançada no ambiente de Pré-visualização a cada duas semanas.

Para obter mais informações, consulte [Perguntas frequentes sobre alteração na cadência de versão de visualização do Workfront](https://one.workfront.com/s/article/Change-in-Workfront-Preview-release-cadence)

### ➡ Inclui na lista de permissões de domínios adicionais necessários para acessar o Workfront {#allowlist-of-additional-domains-required-for-accessing-workfront}

Se sua organização usar um firewall, você deverá adicionar os seguintes domínios adicionais ao incluo na lista de permissões para garantir acesso ininterrupto ao Workfront:

* event.split.io
* sdk.split.io

Para obter mais informações, consulte [Incluir na lista de permissões Configurar o arquivo de pesquisa do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

### Workfront One {#workfront-one}

Com o Workfront One, você descobrirá o conteúdo, os recursos e as notícias mais importantes da Workfront — tudo em um único local, com um único logon. Unificamos os sites de Experiência, Comunidade e Treinamento, facilitando encontrar o que você está procurando.

[Saiba mais sobre o Workfront One](https://www.workfront.com/campaigns/workfront-one).
