---
title: Acesso herdado configurável à funcionalidade para cada tipo de objeto
description: Este artigo explica o que você pode permitir como administrador do Adobe Workfront para cada tipo de objeto, em cada nível de acesso herdado. Ele também explica qual é a configuração padrão para cada tipo de nível de acesso herdado.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 94e0b205-140c-41c9-bb5a-f89b4c3aaea0
source-git-commit: e3211ac5801c1318978427bc0a48d9b3a3028984
workflow-type: tm+mt
source-wordcount: '3456'
ht-degree: 10%

---

# Acesso herdado configurável à funcionalidade para cada tipo de objeto

Este artigo explica o que você pode permitir como administrador do Adobe Workfront para cada tipo de objeto, em cada nível de acesso herdado. Ele também explica qual é a configuração padrão para cada tipo de nível de acesso herdado.

Para obter informações sobre toda a funcionalidade disponível para um tipo de objeto em cada nível de acesso, consulte [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Projetos

Em cada nível de acesso herdado, você pode configurar as seguintes opções para projetos:

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
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar projetos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de projetos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Copiar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Exibir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar projetos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso limitado à edição de projetos. Para ver como o acesso à Edição é limitado em um nível de acesso do Trabalhador em comparação com um nível de acesso do Planejador (que permite o acesso completo da Edição aos projetos), consulte a seção <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects" class="MCXref xref">Projetos</a> no artigo <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md" class="MCXref xref">Funcionalidade disponível para cada tipo de objeto</a>.</p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar projetos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Editar, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
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
     <li><p> <b>Exibir</b></p> (seleção padrão) <p>O acesso à visualização é limitado porque você não pode ajustá-lo para ativar ou desativar o compartilhamento de projeto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a projetos não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tarefas

Em cada nível de acesso herdado, você pode configurar as seguintes opções para tarefas:

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
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar tarefas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de tarefas.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar tarefas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de tarefas.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
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
     <li><p> <b>Exibir</b></p> (seleção padrão)<p>O acesso à visualização é limitado porque você não pode ajustá-lo para ativar ou desativar o compartilhamento de projeto.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a tarefas não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Problemas

Em cada nível de acesso herdado, você pode configurar as seguintes opções para problemas:

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
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso total à edição de problemas.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso total à edição de problemas.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso total à edição de problemas.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
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
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar problemas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso total à edição de problemas.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a problemas não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Portfólios

Em cada nível de acesso herdado, você pode configurar as seguintes opções para portfólios:

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
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar portfólios. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de portfólios.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
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
   <td>Oliveira</td> 
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
   <td> <p>O acesso a portfólios não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Programas

Em cada nível de acesso herdado, você pode configurar as seguintes opções para programas:

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
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar programas. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de programas.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
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
   <td>Oliveira</td> 
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
   <td> <p>O acesso aos programas não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Relatórios, painéis e calendários

Em cada nível de acesso herdado, você pode configurar as seguintes opções para relatórios, painéis e calendários:

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
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> ) e, em seguida, desative ou ative qualquer uma das ações a seguir. Ambos estão ativados por padrão:</p> 
      <ul> 
       <li> <p>Visualizar Relatórios Internos</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de relatórios, painéis e calendários.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão, exceto por <b>Exibir relatórios internos</b>, <b>Compartilhar relatórios publicamente</b>e <b>Compartilhar todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Visualizar Relatórios Internos</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar relatórios publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> (seleção padrão)<p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das ações a seguir. Ambos estão ativados por padrão:</p> 
      <ul> 
       <li> <p>Visualizar Relatórios Internos</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b> (seleção padrão)<p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das ações a seguir. Somente a opção Compartilhar é ativada por padrão.</p> 
      <ul> 
       <li> <p>Visualizar Relatórios Internos</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b> (seleção padrão): Permite acesso somente visualização a relatórios, painéis e calendários que foram compartilhados com eles.</p> <p>Para ajustar isso, você pode configurar a capacidade de exibir relatórios internos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative <b>Exibir incorporado</b>(desabilitado por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a relatórios, painéis e calendários não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Filtros, visualizações e agrupamentos

Em cada nível de acesso herdado, você pode configurar as seguintes opções para filtros, visualizações e agrupamentos:

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
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, exibições e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de filtros, visualizações e agrupamentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, exibições e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de filtros, visualizações e agrupamentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
   <td> 
    <ul> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, exibições e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de filtros, visualizações e agrupamentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b>:</p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar filtros, exibições e agrupamentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de filtros, visualizações e agrupamentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a filtros, visualizações e agrupamentos não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Documentos

Em cada nível de acesso herdado, você pode configurar as seguintes opções para documentos:

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
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de documentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão, exceto por <b>Compartilhar documentos publicamente</b> e <b>Compartilhar todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar documentos publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de documentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão, exceto por <b>Compartilhar documentos publicamente</b> e <b>Compartilhar todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar documentos publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de documentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das ações a seguir. Todos estão ativados por padrão, exceto os últimos dois, <b>Compartilhar documentos publicamente</b> e <b>Compartilhar todo o sistema</b>.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar documentos publicamente (externamente)</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <b>Sem acesso</b> </li> 
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de compartilhar documentos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de documentos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a documentos não pode ser configurado neste nível de acesso. Mas usuários externos podem usar o Workfront para exibir, revisar e baixar documentos.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Usuários

Em cada nível de acesso herdado, você pode configurar as seguintes opções para os usuários:

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
     <li> <p><b>Exibir</b></p><p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative o <b>Exibir Informações de Contato</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso total à edição para usuários.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das ações a seguir. Apenas as duas primeiras opções, <b>Criar</b> e <b>Excluir</b>, são ativadas por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li>Administrador de Usuários (Todos os usuários)</li> 
       <li> <p>Administrador de Usuários (Usuários de Grupo)</p> </li> 
      </ul> <p>Para obter informações sobre as duas opções de Administrador do usuário, consulte a seção <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md#access-to-edit" class="MCXref xref">Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado</a> no artigo <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li><p> <b>Exibir</b> (somente opção disponível)</p><p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative o <b>Exibir Informações de Contato</b> (ativada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
   <td> 
    <ul> 
     <li><p> <b>Exibir</b> (somente opção disponível)</p> <p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, ative ou desative o <b>Exibir Informações de Contato</b> (desabilitada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b> (somente opção disponível)</p><p>Para ajustar isso, você pode configurar a capacidade de exibir as informações de contato dos usuários. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, ative ou desative o <b>Exibir Informações de Contato</b> (desabilitada por padrão).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso aos usuários não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Equipes

Em cada nível de acesso herdado, você pode configurar as seguintes opções para as equipes:

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
     <li><b>Exibir</b> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Ambos estão desativados por padrão.</p> 
      <ul> 
       <li>Exibir todas as equipes</li> 
       <li> <p>Exibir equipes associadas aos meu grupos</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso total à edição de equipes.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Todos estão ativados por padrão, exceto para <b>Editar equipes nas quais estou</b>.</p> 
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
      <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Ambos estão ativados por padrão.</p> 
      <ul> 
       <li>Exibir todas as equipes</li> 
       <li> <p>Exibir equipes associadas aos meu grupos</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite acesso total à edição de equipes.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Somente a primeira opção, <b>Editar equipes nas quais estou</b>, é desativado por padrão.</p> 
      <ul> 
       <li> <p>Editar equipes das quais faço parte</p> </li> 
       <li> <p>Exibir todas as equipes</p> </li> 
       <li> <p>Exibir equipes associadas aos meu grupos</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
   <td> 
    <ul> 
     <li> <p><b>Exibir</b> (somente opção disponível)</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Ambos estão ativados por padrão.</p> 
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
     <li> <p><b>Exibir</b> (somente opção disponível)</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Ambos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Exibir todas as equipes</p> </li> 
       <li>Exibir equipes associadas aos meu grupos</li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso às equipes não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>


## Modelos

Em cada nível de acesso herdado, você pode configurar as seguintes opções para modelos:

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
     <li><p> <b>Exibir</b></p> <p>Para ajustar isso, você pode configurar a capacidade de compartilhar modelos. Clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no botão Exibir e, em seguida, desative ou ative o <b>Compartilhar</b> (ativada por padrão).</p> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de modelos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Todos estão ativados por padrão.</p> 
      <ul> 
       <li> <p>Criar</p> </li> 
       <li> <p>Excluir</p> </li> 
       <li> <p>Compartilhar</p> </li> 
       <li> <p>Compartilhar todo o sistema</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Trabalhador </td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (somente opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Oliveira</td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (somente opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Solicitante</td> 
   <td> 
    <ul> 
     <li> <p><b>Sem acesso</b> (somente opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso a modelos não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Dados financeiros

Em cada nível de acesso herdado, você pode configurar as seguintes opções para dados financeiros:

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
     <li> <p><b>Exibir</b>:</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Ambos estão ativados por padrão.</p> 
      <ul> 
       <li>Ver taxas de custo e cobrança de função</li> 
       <li> <p>Ver taxas de custo e cobrança de usuário</p> </li> 
      </ul> </li> 
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição de dados financeiros.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Exibir</b> , em seguida, desative ou ative qualquer uma das opções a seguir*. Apenas as duas últimas opções, <b>Exibir Faturamento de Função e Taxas de Custo</b> e <b>Exibir Faturamento do Usuário e Taxas de Custo</b>, são ativadas por padrão.</p> 
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
   <td>Oliveira</td> 
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
     <li> <p><b>Sem acesso</b> (somente opção disponível)</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso aos dados financeiros não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Para obter informações sobre essas opções, consulte [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

## Gerenciamento de recursos

Em cada nível de acesso herdado, você pode configurar as seguintes opções para o Gerenciamento de recursos:

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
     <li> <p><b>Editar</b> (seleção padrão): Permite o acesso total à edição do Gerenciamento de recursos.</p> <p>Para ajustar isso, clique no ícone de engrenagem <img src="assets/gear-icon-in-access-levels.png"> no <b>Editar</b> , em seguida, desative ou ative qualquer uma das opções a seguir. Somente a primeira opção, <b>Editar prioridades e horas do orçamento no Planejador</b>, está ativada por padrão.</p> 
      <ul> 
       <li> <p> Editar prioridades e horas de orçamento no Planejador</p> </li> 
       <li> <p>Gerenciar Conjuntos de Recursos</p> <p><b>OBSERVAÇÃO</b>: Para gerenciar pools de recursos, um usuário precisa de acesso adicional a dados financeiros e permissões para financiar projetos. Se você conceder acesso ao Gerenciamento de Recursos a um usuário do Planejador que não tem acesso a dados financeiros, o usuário ainda poderá ver as alocações por hora no Planejador de Recursos, mas não poderá alternar para a visualização de Custo ou exibir o Caso de Negócios. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso aos dados financeiros</a> e <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Compartilhar permissões financeiras em um objeto</a>.</p> </li> 
       <li> <p>Atualizar horas planejadas no Balanceador de carga de trabalho</p> <p><b>OBSERVAÇÃO</b>: Para atualizar as horas planejadas no Balanceador de Carga de Trabalho, um usuário precisa de permissão para contribuir com o objeto, com a opção Fazer Atribuições ativada em Configurações Avançadas. Para obter mais informações, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Visão geral do compartilhamento de permissões em objetos</a>.</p> </li> 
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
   <td>Oliveira</td> 
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
     <li> <b>Sem acesso</b> (somente opção disponível) </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Usuário externo</td> 
   <td> <p>O acesso não está disponível. Usuários externos podem usar o Workfront somente para revisar e baixar documentos e ver calendários compartilhados com eles.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Área do Planejador de Cenário

A configuração padrão para todos os níveis de acesso herdados é Sem acesso. Um administrador do Workfront pode alterar isso para Visualizar ou Editar o acesso para qualquer nível de acesso do Planejador, Trabalhador e Revisor.

<!--
DRAFTED IN FLARE:
Alina says: This will change overtime for some of the access levels, but right now once they get Edit access, they can do everything

-->

>[!NOTE]
>
>Os usuários podem exibir um plano criado por outro usuário somente se um link para o plano for compartilhado com eles.

## Área de metas do Workfront

Todos os seis níveis de acesso herdados padrão (e todos os quatro tipos de licença) podem editar e exibir as Metas do Workfront.

Editar é a opção padrão.
