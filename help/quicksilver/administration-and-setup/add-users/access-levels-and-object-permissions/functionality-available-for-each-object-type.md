---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,modelo,funil,diagrama,níveis,permissões
navigation-topic: access-levels
title: Funcionalidade Disponível para Cada Tipo de Objeto para Vários Níveis de Acesso
description: As tabelas a seguir listam a funcionalidade disponível para cada tipo de objeto nos vários níveis de acesso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '1956'
ht-degree: 10%

---

# Funcionalidade disponível para cada tipo de objeto para vários níveis de acesso

{{highlighted-preview}}

As tabelas a seguir listam a funcionalidade disponível para cada tipo de objeto nos vários níveis de acesso.

Também indica quais ações os administradores do Workfront podem desativar ou ativar usando um nível de acesso.

>[!NOTE]
>
>Este artigo descreve a funcionalidade disponível para níveis de acesso no modelo de plano atual do Workfront. Para ver a funcionalidade disponível no novo modelo de plano, consulte [Funcionalidade disponível para cada tipo de objeto para novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

## Projetos

Somente os usuários com uma licença de Plano podem receber acesso total aos projetos.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; |   |   |   |   |
| Copiar | ✓ ➡&#42; |   |   |   |   |
| Excluir | ✓ ➡&#42; |   |   |   |   |
| Compartilhar | ✓ ➡&#42; | ✓ ➡&#42; |   |   |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; |   |   |   |   |
| Exibir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |   |
| Adicionar um formulário personalizado | ✓ µ |   |   |   |   |
| Atualizar campos personalizados | ✓ µ | ✓ µ |   |   |   |
| Adicionar um processo de aprovação | ✓ µ |   |   |   |   |
| Aprovar um projeto | ✓ µ | ✓ µ | ✓ µ |   |   |
| Adicionar documento | ✓ µ | ✓ µ | ✓ µ |   |   |
| Adicionar problema | ✓ µ | ✓ µ |   |   |   |
| Adicionar tarefas | ✓ µ | ✓ µ |   |   |   |
| Fornecer atualizações/comentários | ✓ µ | ✓ µ | ✓ µ |   |   |
| Alterar status | ✓ µ |   |   |   |   |
| Registrar horas | ✓ µ | ✓ µ |   |   |   |
| Editar atribuições | ✓ µ | ✓ µ |   |   |   |
| Gerenciar uma linha de base | ✓ µ |   |   |   |   |
| Gerenciar riscos | ✓ µ |   |   |   |   |
| Gerenciar finanças | ✓ µ |   |   |   |   |
| Adicionar/editar despesas | ✓ µ | ✓ µ |   |   |   |
| Anexar modelos | ✓ µ |   |   |   |   |
| Salvar como modelo | ✓ µ |   |   |   |   |
| Adicionar/editar um business case | ✓ µ |   |   |   |   |
| Editar detalhes do projeto | ✓ µ |   |   |   |   |
| Editar pessoal | ✓ µ |   |   |   |   |
| Exportar para o MS Project | ✓ µ | ✓ µ | ✓ µ |   |   |
| Recalcular finanças/linha do tempo | ✓ µ |   |   |   |   |
| Definir propriedades da fila | ✓ µ |   |   |   |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Tarefas

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; | ✓ ➡&#42; |   |   |   |
| Excluir | ✓ ➡&#42; | ✓ ➡&#42; |   |   |   |
| Compartilhar | ✓ ➡&#42; | ✓ ➡&#42; |   |   |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; |   |   |   |   |
| Exibir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Adicionar predecessores | ✓ µ | ✓ µ |   |   |   |
| Adicionar problemas | ✓ µ | ✓ µ |   |   |   |
| Editar uma tarefa (excluindo o status) | ✓ µ | ✓ µ |   |   |   |
| Alterar status da tarefa | ✓ µ | ✓ µ |   |   |   |
| Adicionar documentos | ✓ µ | ✓ µ | ✓ µ |   |   |
| Copiar uma tarefa | ✓ µ | ✓ µ |   |   |   |
| Mover uma tarefa | ✓ µ | ✓ µ |   |   |   |
| Registrar horas | ✓ µ | ✓ µ |   |   |   |
| Aceitar uma atribuição | ✓ µ | ✓ µ |   |   |   |
| Fazer uma atribuição | ✓ µ | ✓ µ | Somente em edição em linha | Somente em edição em linha |   |
| Anexar um formulário personalizado | ✓ µ | ✓ µ |   |   |   |
| Editar campos personalizados | ✓ µ | ✓ µ |   |   |   |
| Criar um processo de aprovação | ✓ µ | ✓ µ |   |   |   |
| Aprovar uma tarefa | ✓ µ | ✓ µ | ✓ µ |   |   |
| Editar finanças | ✓ µ |   |   |   |   |
| Adicionar/editar despesas | ✓ µ | ✓ µ |   |   |   |
| Exibir finanças | ✓ µ | ✓ µ | ✓ µ |   |   |
| Atualizações/comentários | ✓ µ | ✓ µ | ✓ µ |   |   |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problemas

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Editar | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Excluir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Compartilhar | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; |   |   |   |   |
| Exibir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Anexar formulários personalizados | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Editar campos personalizados | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Aprovar problemas | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Adicionar um processo de aprovação | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Adicionar documentos | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Copiar problemas | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Mover problemas | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Registrar horas | ✓ µ | ✓ µ |   |   |   |
| Converter um problema em um projeto | ✓ µ | ✓ µ |   |   |   |
| Converter um problema em tarefa | ✓ µ |   |   |   |   |
| Aceitar atribuições | ✓ µ | ✓ µ |   |   |   |
| Fazer atribuições | ✓ µ | ✓ µ |   |   |   |
| Adicionar atualizações e comentários | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portfólios

Somente os usuários com uma licença de Plano podem ter acesso total aos portfólios.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; |   |   |   |   |
| Excluir | ✓ ➡&#42; |   |   |   |   |
| Compartilhar | ✓ ➡&#42; |   |   |   |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; |   |   |   |   |
| Exibir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |   |
| Editar detalhes | ✓ µ |   |   |   |   |
| Anexar formulários personalizados | ✓ µ |   |   |   |   |
| Editar campos personalizados | ✓ µ |   |   |   |   |
| Adicionar e remover projetos | ✓ µ |   |   |   |   |
| Aprovar projetos | ✓ µ |   |   |   |   |
| otimização de Portfolio | ✓ µ |   |   |   |   |
| Adicionar documentos | ✓ µ | ✓ µ | ✓ µ |   |   |
| Adicionar atualizações e comentários | ✓ µ | ✓ µ | ✓ µ |   |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programas

Somente os usuários com uma licença de Plano podem ter acesso total aos programas.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; |   |   |   |   |
| Excluir | ✓ ➡&#42; |   |   |   |   |
| Compartilhar | ✓ ➡&#42; |   |   |   |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; |   |   |   |   |
| Exibir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |   |
| Editar detalhes | ✓ µ |   |   |   |   |
| Anexar formulários personalizados | ✓ µ |   |   |   |   |
| Editar campos personalizados | ✓ µ |   |   |   |   |
| Adicionar e remover projetos | ✓ µ |   |   |   |   |
| Aprovar projetos | ✓ µ |   |   |   |   |
| Otimização do Portfólio | ✓ µ |   |   |   |   |
| Adicionar documentos | ✓ µ | ✓ µ | ✓ µ |   |   |
| Adicionar Adicionar atualizações e comentários | ✓ µ | ✓ µ | ✓ µ |   |   |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Relatórios, painéis e calendários

Os usuários com uma licença de Plano podem ter acesso total aos relatórios. Todos os outros Níveis de Acesso têm acesso de Visualização aos relatórios.

| Ação | Planejador | Trabalhador | Revisor | Solicitar | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; |   |   |   |   |
| Excluir | ✓ ➡&#42; |   |   |   |   |
| Exibir relatórios internos | ✓ ➡&#42; |   |   |   |   |
| Compartilhar | ✓ ➡&#42; | ✓ µ | ✓ µ |   |   |
| Compartilhar calendários e relatórios publicamente | ✓ ➡&#42; |   |   |   |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; |   |   |   |   |
| Exibir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |
| Editar | ✓ µ |   |   |   |   |
| Copiar | ✓ µ |   |   |   |   |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

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
   <th> <p>Revisor</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th>Usuário externo<br></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Criar</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhar</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhar em todo o sistema</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documentos

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Excluir (documentos e pastas) | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Compartilhar | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |
| Compartilhar publicamente (externamente) | ✓ ➡&#42; |   |   |   |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; | ✓ ➡&#42; |   |   |   |
| Exibir | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |
| Editar detalhes | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Baixar | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |
| Check-out | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Adicionar aprovadores | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Aprovar documentos | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |
| Anexar formulários personalizados | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Editar campos personalizados | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Mover para (objeto) | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Enviar para (integração) | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Adicionar atualizações e comentários | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Carregar nova versão | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Excluir uma versão | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Visualização | ✓ µ | ✓ µ | ✓ µ | ✓ µ | ✓ µ |
| Prova | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Gerar prova | ✓ µ | ✓ µ |   |   |   |
| Remover prova | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Adicionar/Remover&#42;&#42; | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Renomear&#42;&#42; | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Link (com integração) | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |
| Desvincular (com integração) | ✓ µ | ✓ µ | ✓ µ | ✓ µ |   |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Disponível somente para pastas de documentos, não documentos

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
   <th> <p>Revisor</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th> <p>Usuário externo**</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Criar</td> 
   <td>✓ µ*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓ µ*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, excluir, desativar, fazer logon como ou redefinir a senha para qualquer usuário</td> 
   <td>✓ µ*<p><b>OBSERVAÇÃO</b>: você não pode fazer logon como qualquer usuário administrador do sistema.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, excluir, desativar, fazer logon como ou redefinir a senha de qualquer usuário em um grupo que ele administra</td> 
   <td>✓ µ*<p><b>OBSERVAÇÃO</b>: você não pode fazer logon como qualquer usuário administrador do sistema.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir usuários</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir informações de contato</td> 
   <td>✓ µ</td> 
   <td> ✓ µ</td> 
   <td>✓ µ </td> 
   <td> ✓ µ</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Usuários externos só podem procurar outros usuários

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
   <th> <p>Revisor</p> </th> 
   <th> <p>Solicitante</p> </th> 
   <th> <p>Usuário externo*</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Criar</td> 
   <td>✓ µ*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓ µ*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar equipes em que estão</td> 
   <td>✓ µ*</td> 
   <td>✓ µ*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar equipes nos grupos que elas gerenciam</td> 
   <td>✓ µ*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir todas as equipes</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir equipes associadas a seus grupos</td> 
   <td>✓ µ</td> 
   <td> ✓ µ</td> 
   <td>✓ µ </td> 
   <td> ✓ µ</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Modelos

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓ ➡&#42; |   |   |   |   |
| Excluir | ✓ ➡&#42; |   |   |   |   |
| Compartilhar | ✓ ➡&#42; |   |   |   |   |
| Compartilhar em todo o sistema | ✓ ➡&#42; |   |   |   |   |
| Exibir | ✓ ➡&#42; |   |   |   |   |
| Copiar | ✓ µ |   |   |   |   |
| Editar detalhes do modelo | ✓ µ |   |   |   |   |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Dados financeiros

Somente os usuários com uma licença de Plano podem ter acesso total aos dados financeiros.

Os tipos de licença de Solicitação e Usuário Externo não estão incluídos aqui porque eles não têm acesso a esses objetos e áreas.

| Ação | Planejador | Trabalhador | Revisor |
|---|---|---|---|
| Editar taxas de custo e cobrança de função | ✓ ➡&#42; |   |   |
| Editar taxas de custo e cobrança de usuário | ✓ ➡&#42; |   |   |
| Exibir taxas de custo e cobrança de função | ✓ ➡&#42; |   |   |
| Exibir taxas de custo e cobrança de usuário | ✓ ➡&#42; |   |   |
| Gerenciar registros de faturamento | ✓ µ |   |   |
| Gerenciar despesas | ✓ µ | ✓ µ |   |
| Exibir dados financeiros | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |
| <span class="preview">Gerenciar cartões de tarifa</span> | ✓ µ |   |   |
| Exibir informações por Custo nas ferramentas de Planejamento de Recursos | ✓ µ |   |   |
| Recursos de Orçamento nas ferramentas de Planejamento de Recursos&#42;&#42; | ✓ µ |   |   |
| Exibir alocação de recursos nas ferramentas de Planejamento de Recursos&#42; | ✓ µ | ✓ µ | ✓ µ |
| Criar riscos em projetos | ✓ µ |   |   |
| Exibir riscos em projetos | ✓ µ | ✓ µ | ✓ µ |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requer acesso adicional ao Gerenciamento de Recursos.

## Gerenciamento de recursos

Somente usuários com uma licença de Plano podem ter acesso total a [selecionar objeto ou área]. Outros tipos de licença podem ter acesso limitado ou inexistente ao Gerenciamento de recursos no Workfront.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Editar prioridades e horas de orçamento no Planejador | ✓ ➡&#42; |   |   |   |   |
| Criar, editar, excluir Conjuntos de Recursos&#42;&#42; | ✓ ➡&#42; |   |   |   |   |
| Atualizar Horas Planejadas no Balanceador de Carga de Trabalho&#42;&#42;&#42; | ✓ µ* |   |   |   |   |
| Exibir prioridades de projeto no Planejador de Recursos | ✓ ➡&#42; |   |   |   |   |
| Exibir alocação de recursos nas ferramentas de Planejamento de Recursos | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |   |
| Exibir Conjuntos de Recursos | ✓ ➡&#42; | ✓ ➡&#42; | ✓ ➡&#42; |   |   |
| Recursos de orçamento nas ferramentas de Planejamento de Recursos&#42;&#42; | ✓ µ |   |   |   |   |
| Anexar Conjuntos de Recursos a projetos, modelos e usuários | ✓ µ |   |   |   |   |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requer acesso adicional a Dados Financeiros e permissões para finanças do projeto. Se você conceder acesso ao Gerenciamento de recursos a um usuário do Planejador que não tem acesso aos Dados financeiros, o usuário ainda poderá ver as alocações por hora no Planejador de recursos, mas não poderá alternar para a visualização de custos ou visualizar o Business Case. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar permissões financeiras em um objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Requer permissão para o Contribute para o objeto, com a opção Fazer Atribuições habilitada em Configurações Avançadas. Para obter informações, consulte a seção [Entender as permissões herdadas e a hierarquia de objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) no artigo [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Área do Planejador de Cenários

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar/editar planos e iniciativas existentes | ✓ µ | ✓ µ | ✓ µ |   |   |
| Adicionar ou editar informações de função de trabalho em planos e iniciativas&#42; | ✓ µ | ✓ µ | ✓ µ |   |   |
| Adicionar ou editar informações de custo em planos e iniciativas&#42; | ✓ µ | ✓ µ | ✓ µ |   |   |
| Excluir planos e iniciativas | ✓ µ | ✓ µ | ✓ µ |   |   |
| Exibir Cenários no Menu Principal ![Ícone do planejador de cenários](assets/esp-icon-in-main-menu.png) | ✓ µ | ✓ µ | ✓ µ | |   |
| Exibir planos e iniciativas criados pelo usuário&#42; | ✓ µ | ✓ µ | ✓ µ |   |   |

{style="table-layout:auto"}

>[!NOTE]
>
>Os usuários poderão exibir um plano que outro usuário criou somente se um link para o plano for compartilhado com eles.

&#42; Para que os usuários visualizem dados financeiros em um plano ou iniciativa, eles precisam de acesso aos Dados Financeiros. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Área Metas do Workfront

| Ações | Exibir | Editar |
|---|---|---|
| Criar |   | ✓ µ |
| Editar/excluir todas as metas |   | ✓ µ |
| Exibir Metas no menu Principal | ✓ µ | ✓ µ |
| Exibir a área Metas de um link compartilhado | ✓ µ | ✓ µ |
| Exibir todas as metas no sistema | ✓ µ | ✓ µ |
| Ativar/ desativar/ fechar todas as metas |   | ✓ µ |
| Criar/ editar/ excluir atividades |   | ✓ µ |
| Criar/ editar/ excluir resultados |   | ✓ µ |
| Adicionar uma meta alinhada |   | ✓ µ |
| Atualizar progresso em um resultado ou atividade |   | ✓ µ |
| Ter uma meta, resultado ou atividade | ✓ µ | ✓ µ |
| Comentar em uma meta | ✓ µ | ✓ µ |
| Copiar metas |   | ✓ µ |
| Exibir a seção Lista de metas no painel esquerdo | ✓ µ | ✓ µ |
| Exibir a seção Gráficos no painel esquerdo | ✓ µ | ✓ µ |
| Exibir a seção Alinhamento de metas no painel esquerdo | ✓ µ | ✓ µ |


