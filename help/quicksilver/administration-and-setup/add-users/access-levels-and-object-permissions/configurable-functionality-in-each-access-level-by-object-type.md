---
title: Acesso configurável à funcionalidade para cada tipo de objeto
description: Este artigo explica o que você pode permitir como administrador do Adobe Workfront para cada tipo de objeto em cada nível de acesso. Também explica qual é a configuração padrão para cada tipo de nível de acesso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '3508'
ht-degree: 10%

---

# Acesso configurável à funcionalidade para cada tipo de objeto

>[!NOTE]
>
>As informações neste artigo se referem aos níveis de acesso herdados. Para obter informações sobre os níveis de acesso atuais, consulte [Visão geral sobre novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Ao configurar um nível de acesso para sua organização, você pode determinar quais ações específicas estão disponíveis para o nível de acesso.

Este artigo explica as opções que um administrador do Adobe Workfront pode selecionar para cada tipo de objeto, em cada nível de acesso. Também explica qual é a configuração padrão para cada tipo de nível de acesso.

Por exemplo, se um administrador do Workfront selecionar &quot;Exibir&quot; para projetos em um determinado nível de acesso, os usuários com esse nível de acesso poderão apenas exibir projetos, não editá-los.

Para obter informações sobre todas as funcionalidades disponíveis para um tipo de objeto em cada nível de acesso, consulte [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projetos

Em cada nível de acesso, você pode configurar as seguintes opções para projetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador (Tipo de licença do plano)</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar projetos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo aos projetos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Copiar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Exibir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar projetos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição limitado a projetos. Para ver como o acesso de Edição é limitado em um nível de acesso Trabalhador em comparação a um nível de acesso Planejador (que permite acesso de Edição completo a projetos), consulte a seção <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projetos</a> no artigo <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Funcionalidade disponível para cada tipo de objeto</a>.</p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar projetos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Editar e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> (seleção padrão) <p>O acesso de visualização é limitado porque você não pode ajustá-lo para ativar ou desativar o compartilhamento de projetos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso aos projetos não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tarefas

Em cada nível de acesso, é possível configurar as seguintes opções para tarefas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar tarefas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo às tarefas.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar tarefas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo às tarefas.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> (seleção padrão)<p>O acesso de visualização é limitado porque você não pode ajustá-lo para ativar ou desativar o compartilhamento de projetos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>Acesso a tarefas não disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problemas

Em cada nível de acesso, você pode configurar as seguintes opções para problemas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a problemas.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a problemas.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a problemas.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a problemas.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a problemas não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portfólios

Em cada nível de acesso, você pode configurar as seguintes opções para portfólios:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar portfólios. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a portfólios.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> <p>O acesso a portfólios não está disponível.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a portfólios não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programas

Em cada nível de acesso, você pode configurar as seguintes opções para programas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar programas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo aos programas.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> <p>O acesso aos programas não está disponível.</p> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso aos programas não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Relatórios, painéis e calendários

Em cada nível de acesso, você pode configurar as seguintes opções para relatórios, painéis e calendários:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b></p><p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das ações a seguir. Ambos são ativados por padrão:</p> 
      <ul> 
       <li> <p>Visualizar relatórios integrados</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a relatórios, painéis e calendários.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos estão habilitados por padrão, exceto <b>Exibir relatórios internos</b>, <b>Compartilhar relatórios publicamente</b> e <b>Compartilhar em todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Visualizar relatórios integrados</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar relatórios publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> (seleção padrão)<p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das ações a seguir. Ambos são ativados por padrão:</p> 
      <ul> 
       <li> <p>Visualizar relatórios integrados</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b> (seleção padrão)<p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das ações a seguir. Somente a opção Compartilhar está habilitada por padrão.</p> 
      <ul> 
       <li> <p>Visualizar relatórios integrados</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Visualização</b> (seleção padrão): permite acesso somente visualização a relatórios, painéis e calendários que foram compartilhados com eles.</p> <p>Para ajustar isso, você pode configurar a capacidade de visualizar relatórios incorporados. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite o <b>Exibir Interno</b> (desabilitado por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a relatórios, painéis e calendários não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filtros, visualizações e agrupamentos

Em cada nível de acesso, você pode configurar as seguintes opções para filtros, visualizações e agrupamentos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, visualizações e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a filtros, visualizações e agrupamentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, visualizações e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a filtros, visualizações e agrupamentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, visualizações e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a filtros, visualizações e agrupamentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b>:</p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, visualizações e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a filtros, visualizações e agrupamentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a filtros, visualizações e agrupamentos não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Documentos

Em cada nível de acesso, você pode configurar as seguintes opções para documentos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a documentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos estão habilitados por padrão, exceto <b>Compartilhar Documentos Publicamente</b> e <b>Compartilhar em todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar documentos publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a documentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos estão habilitados por padrão, exceto <b>Compartilhar Documentos Publicamente</b> e <b>Compartilhar em todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar documentos publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a documentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das ações a seguir. Todos estão habilitados por padrão, exceto os dois últimos, <b>Compartilhar Documentos Publicamente</b> e <b>Compartilhar em todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar documentos publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a documentos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a documentos não é configurável neste nível de acesso. Mas os usuários externos podem usar o Workfront para exibir, revisar e baixar documentos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Usuários

Em cada nível de acesso, você pode configurar as seguintes opções para os usuários:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite a opção <b>Exibir Informações de Contato</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo aos usuários.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das ações a seguir. Somente as duas primeiras opções, <b>Criar</b> e <b>Excluir</b>, são habilitadas por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li>Administrador de Usuários (Todos os usuários)</li> 
       <li> <p>Administrador de Usuários (Usuários de Grupo)</p> </li> 
      </ul> <p>Para obter informações sobre as duas opções de Administrador de Usuários, consulte a seção <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado</a> no artigo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li><p> <b>Exibir</b> (somente a opção disponível)</p><p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite a opção <b>Exibir Informações de Contato</b> (habilitada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li><p> <b>Exibir</b> (somente a opção disponível)</p> <p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e habilite ou desabilite a opção <b>Exibir Informações de Contato</b> (desabilitada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b> (somente a opção disponível)</p><p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e habilite ou desabilite a opção <b>Exibir Informações de Contato</b> (desabilitada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a usuários não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Equipes

Em cada nível de acesso, você pode configurar as seguintes opções para as equipes:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li><b>Exibir</b> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Ambos são desativados por padrão.</p> 
      <ul> 
       <li>Exibir todas as equipes</li> 
       <li> <p>Exibir equipes associadas aos meu grupos</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo às equipes.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Todos estão habilitados por padrão, exceto para <b>Editar equipes em que estou</b>.</p> 
      <ul> 
       <li>Criar</li> 
       <li>Excluir</li> 
       <li> <p>Editar equipes das quais faço parte</p> </li> 
       <li> <p>Editar equipes nos grupos que eu gerencio (somente administradores de grupo)</p> </li> 
       <li> <p>Exibir todas as equipes</p> </li> 
       <li> <p>Exibir equipes associadas aos meu grupos</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Exibir</b>
      <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Ambos são ativados por padrão.</p> 
      <ul> 
       <li>Exibir todas as equipes</li> 
       <li> <p>Exibir equipes associadas aos meu grupos</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo às equipes.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Somente a primeira opção, <b>Editar equipes em que estou</b>, está desabilitada por padrão.</p> 
      <ul> 
       <li> <p>Editar equipes das quais faço parte</p> </li> 
       <li> <p>Exibir todas as equipes</p> </li> 
       <li> <p>Exibir equipes associadas aos meu grupos</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b> (somente a opção disponível)</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Ambos são ativados por padrão.</p> 
      <ul> 
       <li> <p>Exibir todas as equipes</p> </li> 
       <li>Exibir equipes associadas aos meu grupos</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b> (somente a opção disponível)</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Ambos são ativados por padrão.</p> 
      <ul> 
       <li> <p>Exibir todas as equipes</p> </li> 
       <li>Exibir equipes associadas aos meu grupos</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a equipes não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Modelos

Em cada nível de acesso, você pode configurar as seguintes opções para modelos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar modelos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e desative ou ative a opção <b>Compartilhar</b> (habilitada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo a modelos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Todos eles são ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar em todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (apenas a opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (apenas a opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (apenas a opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a modelos não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dados financeiros

Em cada nível de acesso, você pode configurar as seguintes opções para dados financeiros:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b>:</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Ambos são ativados por padrão.</p> 
      <ul> 
       <li>Ver taxas de custo e cobrança de função</li> 
       <li> <p>Ver taxas de custo e cobrança de usuário</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo aos dados financeiros.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Exibir</b> e desabilite ou habilite qualquer uma das seguintes opções*. Somente as duas últimas opções, <b>Exibir taxas de custo e cobrança de função</b> e <b>Exibir taxas de custo e cobrança de usuário</b>, estão habilitadas por padrão.</p> 
      <ul> 
       <li>Editar taxas de custo e cobrança de função</li> 
       <li> <p>Editar taxas de custo e cobrança de usuário</p> </li> 
       <li>Ver taxas de custo e cobrança de função</li> 
       <li> <p>Ver taxas de custo e cobrança de usuário</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (seleção padrão)</p> </li> 
     <li> <b>Exibir</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (seleção padrão)</p> </li> 
     <li><b>Exibir</b> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (apenas a opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a dados financeiros não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Para obter informações sobre essas opções, consulte [Visão Geral de Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Gerenciamento de recursos

Em cada nível de acesso, você pode configurar as seguintes opções para o Gerenciamento de recursos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Nível de acesso</th> 
   <th>Opções</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> </li> 
     <li> <p><b>Editar</b> (seleção padrão): permite acesso de edição completo ao Gerenciamento de Recursos.</p> <p>Para ajustar, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão <b>Editar</b> e desabilite ou habilite qualquer uma das opções a seguir. Somente a primeira opção, <b>Editar prioridades e horas de orçamento no Planejador</b>, é habilitada por padrão.</p> 
      <ul> 
       <li> <p> Editar prioridades e horas de orçamento no Planejador</p> </li> 
       <li> <p>Gerenciar Conjuntos de Recursos</p> <p><b>OBSERVAÇÃO</b>: para gerenciar conjuntos de recursos, um usuário precisa de acesso adicional a dados financeiros e permissões para as finanças do projeto. Se você conceder acesso ao Gerenciamento de recursos a um usuário do Planejador que não tem acesso a dados financeiros, o usuário ainda poderá ver as alocações por hora no Planejador de recursos, mas não poderá alternar para a visualização de custos ou visualizar o Business Case. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso a dados financeiros</a> e <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartilhar permissões financeiras em um objeto</a>.</p> </li> 
       <li> <p>Atualizar horas planejadas no Balanceador de carga de trabalho</p> <p><b>OBSERVAÇÃO</b>: para atualizar horas planejadas no Balanceador de carga de trabalho, um usuário precisa de permissão para contribuir com o objeto, com a opção Fazer atribuições habilitada em Configurações avançadas. Para obter informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral das permissões de compartilhamento em objetos</a>.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li><b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Revisor</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <b>Exibir</b> (seleção padrão)</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> (apenas a opção disponível) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>Acesso indisponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e visualizar calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Área do Planejador de Cenários

A configuração padrão para todos os níveis de acesso é Sem acesso. Um administrador do Workfront pode alterar isso para Exibir ou Editar acesso para qualquer nível de acesso de Planejador, Trabalhador e Revisor.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Os usuários poderão exibir um plano que outro usuário criou somente se um link para o plano for compartilhado com eles.

## Área Metas do Workfront

Todos os seis níveis de acesso padrão (e todos os quatro tipos de licença) podem editar e visualizar as Metas do Workfront.

Editar é a opção padrão.
