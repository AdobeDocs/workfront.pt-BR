---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acessar,modelo,funil,diagrama,níveis,permissões
navigation-topic: access-levels
title: Funcionalidade disponível para cada tipo de objeto
description: As tabelas a seguir listam a funcionalidade disponível para cada tipo de objeto nos vários níveis de acesso.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 12%

---

# Funcionalidade disponível para cada tipo de objeto

As tabelas a seguir listam a funcionalidade disponível para cada tipo de objeto nos vários níveis de acesso.

Também indica quais ações os administradores do Workfront podem desativar ou ativar usando um nível de acesso.

## Projetos

Somente os usuários com uma licença do Plano podem ter acesso total aos projetos.

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |   |   |   |   |
| Copiar | ✓&#42; |   |   |   |   |
| Excluir | ✓&#42; |   |   |   |   |
| Compartilhar | ✓&#42; | ✓&#42; |   |   |   |
| Compartilhar todo o sistema | ✓&#42; |   |   |   |   |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Adicionar um formulário personalizado | ✓ |   |   |   |   |
| Atualizar campos personalizados | ✓ | ✓ |   |   |   |
| Adicionar um processo de aprovação | ✓ |   |   |   |   |
| Aprovar um projeto | ✓ | ✓ | ✓ |   |   |
| Adicionar documento | ✓ | ✓ | ✓ |   |   |
| Adicionar problema | ✓ | ✓ |   |   |   |
| Adicionar  tarefas | ✓ | ✓ |   |   |   |
| Fornecer atualizações/comentários | ✓ | ✓ | ✓ |   |   |
| Alterar status | ✓ |   |   |   |   |
| Horas de registro | ✓ | ✓ |   |   |   |
| Editar atribuições | ✓ | ✓ |   |   |   |
| Gerenciar uma linha de base | ✓ |   |   |   |   |
| Gerenciar riscos | ✓ |   |   |   |   |
| Gerenciar finanças | ✓ |   |   |   |   |
| Adicionar/editar despesas | ✓ | ✓ |   |   |   |
| Anexar modelos | ✓ |   |   |   |   |
| Salvar como modelo | ✓ |   |   |   |   |
| Adicionar/editar um caso comercial | ✓ |   |   |   |   |
| Editar detalhes do projeto | ✓ |   |   |   |   |
| Editar equipe | ✓ |   |   |   |   |
| Exportar para o MS Project | ✓ | ✓ | ✓ |   |   |
| Recalcular linha do tempo/financiamento | ✓ |   |   |   |   |
| Definir propriedades da fila | ✓ |   |   |   |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Tarefas

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; | ✓&#42; |   |   |   |
| Excluir | ✓&#42; | ✓&#42; |   |   |   |
| Compartilhar | ✓&#42; | ✓&#42; |   |   |   |
| Compartilhar todo o sistema | ✓&#42; |   |   |   |   |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Adicionar predecessores | ✓ | ✓ |   |   |   |
| Adicionar  problemas | ✓ | ✓ |   |   |   |
| Editar uma tarefa (excluindo status) | ✓ | ✓ |   |   |   |
| Alterar status da tarefa | ✓ | ✓ |   |   |   |
| Adicionar documentos | ✓ | ✓ | ✓ |   |   |
| Copiar uma tarefa | ✓ | ✓ |   |   |   |
| Mover uma tarefa | ✓ | ✓ |   |   |   |
| Horas de registro | ✓ | ✓ |   |   |   |
| Aceitar uma atribuição | ✓ | ✓ |   |   |   |
| Fazer uma atribuição | ✓ | ✓ | Somente edição em linha | Somente edição em linha |   |
| Anexar um formulário personalizado | ✓ | ✓ |   |   |   |
| Editar campos personalizados | ✓ | ✓ |   |   |   |
| Criar um processo de aprovação | ✓ | ✓ |   |   |   |
| Aprovar uma tarefa | ✓ | ✓ | ✓ |   |   |
| Editar finanças | ✓ |   |   |   |   |
| Adicionar/editar despesas | ✓ | ✓ |   |   |   |
| Exibir financiamento | ✓ | ✓ | ✓ |   |   |
| Atualizações/comentários | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problemas

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Editar | ✓ | ✓ | ✓ | ✓ |   |
| Excluir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartilhar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartilhar todo o sistema | ✓&#42; |   |   |   |   |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Anexar formulários personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Aprovar problemas | ✓ | ✓ | ✓ | ✓ |   |
| Adicionar um processo de aprovação | ✓ | ✓ | ✓ | ✓ |   |
| Adicionar documentos | ✓ | ✓ | ✓ | ✓ |   |
| Copiar problemas | ✓ | ✓ | ✓ | ✓ |   |
| Mover problemas | ✓ | ✓ | ✓ | ✓ |   |
| Horas de registro | ✓ | ✓ |   |   |   |
| Converter um problema em um projeto | ✓ | ✓ |   |   |   |
| Converter um problema em uma tarefa para | ✓ |   |   |   |   |
| Aceitar atribuições | ✓ | ✓ |   |   |   |
| Fazer atribuições | ✓ | ✓ |   |   |   |
| Adicionar atualizações e comentários | ✓ | ✓ | ✓ | ✓ |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portfólios

Somente os usuários com uma licença de Plano podem ter acesso total a portfólios.

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |   |   |   |   |
| Excluir | ✓&#42; |   |   |   |   |
| Compartilhar | ✓&#42; |   |   |   |   |
| Compartilhar todo o sistema | ✓&#42; |   |   |   |   |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Editar detalhes | ✓ |   |   |   |   |
| Anexar formulários personalizados | ✓ |   |   |   |   |
| Editar campos personalizados | ✓ |   |   |   |   |
| Adicionar e remover projetos | ✓ |   |   |   |   |
| Aprovar projetos | ✓ |   |   |   |   |
| Otimização de Portfolio | ✓ |   |   |   |   |
| Adicionar documentos | ✓ | ✓ | ✓ |   |   |
| Adicionar atualizações e comentários | ✓ | ✓ | ✓ |   |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programas

Somente os usuários com uma licença do Plano podem ter acesso total a programas.

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |   |   |   |   |
| Excluir | ✓&#42; |   |   |   |   |
| Compartilhar | ✓&#42; |   |   |   |   |
| Compartilhar todo o sistema | ✓&#42; |   |   |   |   |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Editar detalhes | ✓ |   |   |   |   |
| Anexar formulários personalizados | ✓ |   |   |   |   |
| Editar campos personalizados | ✓ |   |   |   |   |
| Adicionar e remover projetos | ✓ |   |   |   |   |
| Aprovar projetos | ✓ |   |   |   |   |
| Otimização do Portfólio | ✓ |   |   |   |   |
| Adicionar documentos | ✓ | ✓ | ✓ |   |   |
| Adicionar Adicionar atualizações e comentários | ✓ | ✓ | ✓ |   |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Relatórios, painéis e calendários

Os usuários com uma licença do Plan podem ter acesso total aos relatórios. Todos os outros Níveis de Acesso têm Acesso de Exibição aos relatórios.

| Ação | Planejador | Trabalhador | Oliveira | Solicitar | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |   |   |   |   |
| Excluir | ✓&#42; |   |   |   |   |
| Exibir relatórios internos | ✓&#42; |   |   |   |   |
| Compartilhar | ✓&#42; | ✓ | ✓ |   |   |
| Compartilhar calendários e relatórios publicamente | ✓&#42; |   |   |   |   |
| Compartilhar todo o sistema | ✓&#42; |   |   |   |   |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar | ✓ |   |   |   |   |
| Copiar | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

>[!NOTE]
>
>Os solicitantes podem exibir somente relatórios que foram compartilhados com eles

## Filtros, visualizações e agrupamentos

<table> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Ação</p> </th> 
   <th> <p>Planejador</p> </th> 
   <th> <p>Trabalhador</p> </th> 
   <th> <p>Oliveira</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th>Usuário externo<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Criar</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhar</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhar todo o sistema</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documentos

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Excluir (documentos e pastas) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartilhar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |   |
| Compartilhar publicamente (externamente) | ✓&#42; |   |   |   |   |
| Compartilhar todo o sistema | ✓&#42; | ✓&#42; |   |   |   |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar detalhes | ✓ | ✓ | ✓ | ✓ |   |
| Baixar | ✓ | ✓ | ✓ | ✓ | ✓ |
| Check-out | ✓ | ✓ | ✓ | ✓ |   |
| Adicionar aprovadores | ✓ | ✓ | ✓ | ✓ |   |
| Aprovar documentos | ✓ | ✓ | ✓ | ✓ | ✓ |
| Anexar formulários personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |   |
| Mover para (objeto) | ✓ | ✓ | ✓ | ✓ |   |
| Enviar para (integração) | ✓ | ✓ | ✓ | ✓ |   |
| Adicionar atualizações e comentários | ✓ | ✓ | ✓ | ✓ |   |
| Fazer upload de nova versão | ✓ | ✓ | ✓ | ✓ |   |
| Excluir uma versão | ✓ | ✓ | ✓ | ✓ |   |
| Pré-visualização | ✓ | ✓ | ✓ | ✓ | ✓ |
|  Prova | ✓ | ✓ | ✓ | ✓ |   |
| Gerar prova | ✓ | ✓ |   |   |   |
| Remover prova | ✓ | ✓ | ✓ | ✓ |   |
| Adicionar/remover&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Renomear&#42;&#42; | ✓ | ✓ | ✓ | ✓ |   |
| Link (com integração) | ✓ | ✓ | ✓ | ✓ |   |
| Desvincular (com integração) | ✓ | ✓ | ✓ | ✓ |   |

{style=&quot;table-layout:auto&quot;}

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Disponível apenas para pastas de documentos, não documentos

## Usuários

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th> <p>Ação</p> </th> 
   <th> <p>Planejador</p> </th> 
   <th>Trabalhador</th> 
   <th> <p>Oliveira</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th> <p>Usuário externo**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Criar</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, excluir, desativar, fazer logon como ou redefinir a senha de qualquer usuário</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, excluir, desativar, fazer logon como ou redefinir a senha de qualquer usuário de um grupo que eles administram</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir usuários</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir informações de contato</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Usuários externos só podem pesquisar por outros usuários

## Equipes

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Ação</p> </th> 
   <th> <p>Planejador</p> </th> 
   <th>Trabalhador</th> 
   <th> <p>Oliveira</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th> <p>Usuário externo*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Criar</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar equipes nas quais eles estão</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar equipes em grupos que eles gerenciam</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir todas as equipes</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir equipes associadas a seus grupos</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Modelos

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |   |   |   |   |
| Excluir | ✓&#42; |   |   |   |   |
| Compartilhar | ✓&#42; |   |   |   |   |
| Compartilhar todo o sistema | ✓&#42; |   |   |   |   |
| Exibir | ✓&#42; |   |   |   |   |
| Copiar | ✓ |   |   |   |   |
| Editar detalhes do modelo | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Dados financeiros

Somente os usuários com uma licença do Plano podem ter acesso total a dados financeiros.

Os tipos de licença Solicitação e Usuário Externo não estão incluídos aqui porque eles não têm acesso a [selecionar objeto ou área].

| Ação | Planejador | Trabalhador | Oliveira |
|---|---|---|---|
| Editar taxas de custo e faturamento de função | ✓&#42; |   |   |
| Editar faturamento do usuário e taxas de custo | ✓&#42; |   |   |
| Exibir taxas de faturamento e custo de função | ✓&#42; |   |   |
| Exibir faturamento do usuário e taxas de custo | ✓&#42; |   |   |
| Gerenciar registros de faturamento | ✓ |   |   |
| Gerenciar despesas | ✓ | ✓ |   |
| Exibir dados financeiros | ✓&#42; | ✓&#42; | ✓&#42; |
| Exibir informações por Custo nas ferramentas de Planejamento de Recursos | ✓ |   |   |
| Recursos de Orçamento nas ferramentas de Planejamento de Recursos&#42;&#42; | ✓ |   |   |
| Exibir alocação de recursos nas ferramentas de Planejamento de Recursos&#42; | ✓ | ✓ | ✓ |
| Criar riscos em projetos | ✓ |   |   |
| Exibir riscos em projetos | ✓ | ✓ | ✓ |

{style=&quot;table-layout:auto&quot;}

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requer acesso adicional ao Gerenciamento de Recursos.

## Gerenciamento de recursos

Somente os usuários com uma licença do Plano podem ter acesso total a [selecionar objeto ou área]. Outros tipos de licença podem ter acesso limitado ou inexistente ao Gerenciamento de recursos no Workfront.

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Editar prioridades e horas de orçamento no Planejador | ✓&#42; |   |   |   |   |
| Criar, editar, excluir Conjuntos de Recursos&#42;&#42; | ✓&#42; |   |   |   |   |
| `Update Planned Hours in the Workload Balancer`&#42;&#42;&#42; | `✓*` |   |   |   |   |
| Exibir as prioridades do projeto no Planejador de Recursos | ✓&#42; |   |   |   |   |
| Exibir alocação de recursos nas ferramentas de Planejamento de Recursos | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Exibir Pools de Recursos | ✓&#42; | ✓&#42; | ✓&#42; |   |   |
| Recursos de orçamento nas ferramentas de Planejamento de Recursos&#42;&#42; | ✓ |   |   |   |   |
| Anexar pools de recursos a projetos, modelos e usuários | ✓ |   |   |   |   |

{style=&quot;table-layout:auto&quot;}

&#42; Usando um nível de acesso, os administradores do Workfront podem desativar ou ativar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requer acesso adicional aos Dados financeiros e permissões para as finanças do projeto. Se você conceder acesso ao Gerenciamento de Recursos a um usuário do Planejador que não tem acesso a Dados Financeiros, o usuário ainda poderá ver as alocações por hora no Planejador de Recursos, mas não poderá alternar para a Visualização de Custo ou exibir o Caso de Negócios. Para obter mais informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar permissões financeiras em um objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Requer permissão para Contribuir para o objeto, com Tornar atribuições ativadas em Configurações avançadas. Para obter mais informações, consulte a seção [Entender as permissões herdadas e a hierarquia de objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) no artigo [Visão geral do compartilhamento de permissões em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Área do Planejador de Cenário

| Ação | Planejador | Trabalhador | Oliveira | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar/editar planos e iniciativas existentes | ✓ | ✓ | ✓ |   |   |
| Adicionar ou editar informações de função de trabalho em planos e iniciativas&#42; | ✓ | ✓ | ✓ |   |   |
| Adicionar ou editar informações de custo sobre planos e iniciativas&#42; | ✓ | ✓ | ✓ |   |   |
| Excluir planos e iniciativas | ✓ | ✓ | ✓ |   |   |
| Visualizar cenários no menu principal ![](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ |  |   |
| Visualizar planos e iniciativas que o usuário criou&#42; | ✓ | ✓ | ✓ |   |   |

{style=&quot;table-layout:auto&quot;}

>[!NOTE]
>
>Os usuários podem exibir um plano criado por outro usuário somente se um link para o plano for compartilhado com eles.

&#42; Para que os usuários visualizem dados financeiros em um plano ou iniciativa, eles precisam ter acesso aos dados financeiros. Para obter mais informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Área de metas do Workfront

| Ações | Exibir | Editar |
|---|---|---|
| Criar |   | ✓ |
| Editar/excluir todas as metas |   | ✓ |
| Exibir metas no menu principal | ✓ | ✓ |
| Exibir a área de Metas a partir de um link compartilhado | ✓ | ✓ |
| Ver todas as metas no sistema | ✓ | ✓ |
| Ativar/desativar/fechar todas as metas |   | ✓ |
| Criar/editar/excluir atividades |   | ✓ |
| Criar/editar/excluir resultados |   | ✓ |
| Adicionar uma meta alinhada |   | ✓ |
| Atualizar o progresso em um resultado ou atividade |   | ✓ |
| Ter uma meta, resultado ou atividade | ✓ | ✓ |
| Comentário sobre uma meta | ✓ | ✓ |
| Copiar metas |   | ✓ |
| Exibir a seção Lista de metas no painel esquerdo | ✓ | ✓ |
| Exibir a seção Gráficos no painel esquerdo | ✓ | ✓ |
| Exibir a seção Alinhamento da meta no painel esquerdo | ✓ | ✓ |

