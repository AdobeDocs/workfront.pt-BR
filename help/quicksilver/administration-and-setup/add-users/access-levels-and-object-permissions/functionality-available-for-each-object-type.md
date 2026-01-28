---
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,modelo,funnel,diagrama,níveis,permissões
navigation-topic: access-levels
title: Funcionalidade disponível para cada tipo de objeto para vários níveis de acesso (herdado)
description: As tabelas a seguir listam a funcionalidade disponível para cada tipo de objeto nos vários níveis de acesso.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 91b1b448-5a0b-4e64-a59e-458c8387ecbc
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '1588'
ht-degree: 14%

---

# Funcionalidade disponível para cada tipo de objeto para vários níveis de acesso (Herdado)

{{highlighted-preview}}

>[!NOTE]
>
>As informações neste artigo se referem aos níveis de acesso herdados. Para obter informações sobre os níveis de acesso atuais, consulte [Visão geral sobre novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

As tabelas a seguir listam a funcionalidade disponível para cada tipo de objeto nos vários níveis de acesso.

Também indica quais ações os administradores do Workfront podem desativar ou ativar usando um nível de acesso.

>[!NOTE]
>
>Este artigo descreve a funcionalidade disponível para níveis de acesso no modelo de pacote atual do Workfront. Para ver a funcionalidade disponível no novo modelo de pacote, consulte [Funcionalidade disponível para cada tipo de objeto para novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/functionality-available-for-objects.md).

## Projetos

Somente os usuários com uma licença de Plano podem receber acesso total aos projetos.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |  |  |  |  |
| Copiar | ✓&#42; |  |  |  |  |
| Excluir | ✓&#42; |  |  |  |  |
| Compartilhar | ✓&#42; | ✓&#42; |  |  |  |
| Compartilhar em todo o sistema | ✓&#42; |  |  |  |  |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Adicionar um formulário personalizado | ✓ |  |  |  |  |
| Atualizar campos personalizados | ✓ | ✓ |  |  |  |
| Adicionar um processo de aprovação | ✓ |  |  |  |  |
| Aprovar um projeto | ✓ | ✓ | ✓ |  |  |
| Adicionar documento | ✓ | ✓ | ✓ |  |  |
| Adicionar problema | ✓ | ✓ |  |  |  |
| Adicionar tarefas | ✓ | ✓ |  |  |  |
| Fornecer atualizações/comentários | ✓ | ✓ | ✓ |  |  |
| Alterar status | ✓ |  |  |  |  |
| Registrar horas | ✓ | ✓ |  |  |  |
| Editar atribuições | ✓ | ✓ |  |  |  |
| Gerenciar uma linha de base | ✓ |  |  |  |  |
| Gerenciar riscos | ✓ |  |  |  |  |
| Gerenciar finanças | ✓ |  |  |  |  |
| Adicionar/editar despesas | ✓ | ✓ |  |  |  |
| Anexar modelos | ✓ |  |  |  |  |
| Salvar como modelo | ✓ |  |  |  |  |
| Adicionar/editar um business case | ✓ |  |  |  |  |
| Editar detalhes do projeto | ✓ |  |  |  |  |
| Editar pessoal | ✓ |  |  |  |  |
| Exportar para o MS Project | ✓ | ✓ | ✓ |  |  |
| Recalcular finanças/linha do tempo | ✓ |  |  |  |  |
| Definir propriedades da fila | ✓ |  |  |  |  |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Tarefas

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; | ✓&#42; |  |  |  |
| Excluir | ✓&#42; | ✓&#42; |  |  |  |
| Compartilhar | ✓&#42; | ✓&#42; |  |  |  |
| Compartilhar em todo o sistema | ✓&#42; |  |  |  |  |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Adicionar predecessores | ✓ | ✓ |  |  |  |
| Adicionar problemas | ✓ | ✓ |  |  |  |
| Editar uma tarefa (excluindo o status) | ✓ | ✓ |  |  |  |
| Alterar status da tarefa | ✓ | ✓ |  |  |  |
| Adicionar documentos | ✓ | ✓ | ✓ |  |  |
| Copiar uma tarefa | ✓ | ✓ |  |  |  |
| Mover uma tarefa | ✓ | ✓ |  |  |  |
| Registrar horas | ✓ | ✓ |  |  |  |
| Aceitar uma atribuição | ✓ | ✓ |  |  |  |
| Fazer uma atribuição | ✓ | ✓ | Somente em edição em linha | Somente em edição em linha |  |
| Anexar um formulário personalizado | ✓ | ✓ |  |  |  |
| Editar campos personalizados | ✓ | ✓ |  |  |  |
| Criar um processo de aprovação | ✓ | ✓ |  |  |  |
| Aprovar uma tarefa | ✓ | ✓ | ✓ |  |  |
| Editar finanças | ✓ |  |  |  |  |
| Adicionar/editar despesas | ✓ | ✓ |  |  |  |
| Exibir finanças | ✓ | ✓ | ✓ |  |  |
| Atualizações/comentários | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Problemas

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Editar | ✓ | ✓ | ✓ | ✓ |  |
| Excluir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Compartilhar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Compartilhar em todo o sistema | ✓&#42; |  |  |  |  |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Anexar formulários personalizados | ✓ | ✓ | ✓ | ✓ |  |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |  |
| Aprovar problemas | ✓ | ✓ | ✓ | ✓ |  |
| Adicionar um processo de aprovação | ✓ | ✓ | ✓ | ✓ |  |
| Adicionar documentos | ✓ | ✓ | ✓ | ✓ |  |
| Copiar problemas | ✓ | ✓ | ✓ | ✓ |  |
| Mover problemas | ✓ | ✓ | ✓ | ✓ |  |
| Registrar horas | ✓ | ✓ |  |  |  |
| Converter um problema em um projeto | ✓ | ✓ |  |  |  |
| Converter um problema em tarefa | ✓ |  |  |  |  |
| Aceitar atribuições | ✓ | ✓ |  |  |  |
| Fazer atribuições | ✓ | ✓ |  |  |  |
| Adicionar atualizações e comentários | ✓ | ✓ | ✓ | ✓ |  |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Portfólios

Somente os usuários com uma licença de Plano podem ter acesso total aos portfólios.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |  |  |  |  |
| Excluir | ✓&#42; |  |  |  |  |
| Compartilhar | ✓&#42; |  |  |  |  |
| Compartilhar em todo o sistema | ✓&#42; |  |  |  |  |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Editar detalhes | ✓ |  |  |  |  |
| Anexar formulários personalizados | ✓ |  |  |  |  |
| Editar campos personalizados | ✓ |  |  |  |  |
| Adicionar e remover projetos | ✓ |  |  |  |  |
| Aprovar projetos | ✓ |  |  |  |  |
| Otimização do Portfolio | ✓ |  |  |  |  |
| Adicionar documentos | ✓ | ✓ | ✓ |  |  |
| Adicionar atualizações e comentários | ✓ | ✓ | ✓ |  |  |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Programas

Somente os usuários com uma licença de Plano podem ter acesso total aos programas.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |  |  |  |  |
| Excluir | ✓&#42; |  |  |  |  |
| Compartilhar | ✓&#42; |  |  |  |  |
| Compartilhar em todo o sistema | ✓&#42; |  |  |  |  |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Editar detalhes | ✓ |  |  |  |  |
| Anexar formulários personalizados | ✓ |  |  |  |  |
| Editar campos personalizados | ✓ |  |  |  |  |
| Adicionar e remover projetos | ✓ |  |  |  |  |
| Aprovar projetos | ✓ |  |  |  |  |
| Otimização do Portfólio | ✓ |  |  |  |  |
| Adicionar documentos | ✓ | ✓ | ✓ |  |  |
| Adicionar Adicionar atualizações e comentários | ✓ | ✓ | ✓ |  |  |



&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Relatórios, painéis e calendários

Os usuários com uma licença de Plano podem ter acesso total aos relatórios. Todos os outros Níveis de Acesso têm acesso de Visualização aos relatórios.

| Ação | Planejador | Trabalhador | Revisor | Solicitação | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |  |  |  |  |
| Excluir | ✓&#42; |  |  |  |  |
| Exibir relatórios internos | ✓&#42; |  |  |  |  |
| Compartilhar | ✓&#42; | ✓ | ✓ |  |  |
| Compartilhar calendários e relatórios publicamente | ✓&#42; |  |  |  |  |
| Compartilhar em todo o sistema | ✓&#42; |  |  |  |  |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar | ✓ |  |  |  |  |
| Copiar | ✓ |  |  |  |  |

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
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhar</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhar em todo o sistema</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Documentos

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Excluir (documentos e pastas) | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Compartilhar | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |  |
| Compartilhar publicamente (externamente) | ✓&#42; |  |  |  |  |
| Compartilhar em todo o sistema | ✓&#42; | ✓&#42; |  |  |  |
| Exibir | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; | ✓&#42; |
| Editar detalhes | ✓ | ✓ | ✓ | ✓ |  |
| Baixar | ✓ | ✓ | ✓ | ✓ | ✓ |
| Check-out | ✓ | ✓ | ✓ | ✓ |  |
| Adicionar aprovadores | ✓ | ✓ | ✓ | ✓ |  |
| Aprovar documentos | ✓ | ✓ | ✓ | ✓ | ✓ |
| Anexar formulários personalizados | ✓ | ✓ | ✓ | ✓ |  |
| Editar campos personalizados | ✓ | ✓ | ✓ | ✓ |  |
| Mover para (objeto) | ✓ | ✓ | ✓ | ✓ |  |
| Enviar para (integração) | ✓ | ✓ | ✓ | ✓ |  |
| Adicionar atualizações e comentários | ✓ | ✓ | ✓ | ✓ |  |
| Carregar nova versão | ✓ | ✓ | ✓ | ✓ |  |
| Excluir uma versão | ✓ | ✓ | ✓ | ✓ |  |
| Visualização | ✓ | ✓ | ✓ | ✓ | ✓ |
| Prova | ✓ | ✓ | ✓ | ✓ |  |
| Gerar prova | ✓ | ✓ |  |  |  |
| Remover prova | ✓ | ✓ | ✓ | ✓ |  |
| Adicionar/Remover&#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| Renomear&#42;&#42; | ✓ | ✓ | ✓ | ✓ |  |
| Link (com integração) | ✓ | ✓ | ✓ | ✓ |  |
| Desvincular (com integração) | ✓ | ✓ | ✓ | ✓ |  |

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
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, excluir, desativar, fazer logon como ou redefinir a senha para qualquer usuário</td> 
   <td>✓*<p><b>OBSERVAÇÃO</b>: você não pode fazer logon como qualquer usuário administrador do sistema.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar, excluir, desativar, fazer logon como ou redefinir a senha de qualquer usuário em um grupo que ele administra</td> 
   <td>✓*<p><b>OBSERVAÇÃO</b>: você não pode fazer logon como qualquer usuário administrador do sistema.</p></td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir usuários</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir informações de contato</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
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
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Excluir</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar equipes em que estão</td> 
   <td>✓*</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Editar equipes nos grupos que elas gerenciam</td> 
   <td>✓*</td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir todas as equipes</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir equipes associadas a seus grupos</td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td>✓ </td> 
   <td> ✓</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Modelos

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar | ✓&#42; |  |  |  |  |
| Excluir | ✓&#42; |  |  |  |  |
| Compartilhar | ✓&#42; |  |  |  |  |
| Compartilhar em todo o sistema | ✓&#42; |  |  |  |  |
| Exibir | ✓&#42; |  |  |  |  |
| Copiar | ✓ |  |  |  |  |
| Editar detalhes do modelo | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

## Dados financeiros

Somente os usuários com uma licença de Plano podem ter acesso total aos dados financeiros.

Os tipos de licença de Solicitação e Usuário Externo não estão incluídos aqui porque eles não têm acesso a esses objetos e áreas.

| Ação | Planejador | Trabalhador | Revisor |
|---|---|---|---|
| Editar taxas de custo e cobrança de função | ✓&#42; |  |  |
| Editar taxas de custo e cobrança de usuário | ✓&#42; |  |  |
| Exibir taxas de custo e cobrança de função | ✓&#42; |  |  |
| Exibir taxas de custo e cobrança de usuário | ✓&#42; |  |  |
| Gerenciar registros de cobrança | ✓ |  |  |
| Gerenciar despesas | ✓ | ✓ |  |
| Exibir dados financeiros | ✓&#42; | ✓&#42; | ✓&#42; |
| <span class="preview">Gerenciar cartões de tarifa</span> | ✓ |  |  |
| Exibir informações por Custo nas ferramentas de Planejamento de Recursos | ✓ |  |  |
| Recursos de Orçamento nas ferramentas de Planejamento de Recursos&#42;&#42; | ✓ |  |  |
| Exibir alocação de recursos nas ferramentas de Planejamento de Recursos&#42; | ✓ | ✓ | ✓ |
| Criar riscos em projetos | ✓ |  |  |
| Exibir riscos em projetos | ✓ | ✓ | ✓ |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requer acesso adicional ao Gerenciamento de Recursos.

## Gerenciamento de recursos

Somente usuários com uma licença de Plano podem ter acesso total a [selecionar objeto ou área]. Outros tipos de licença podem ter acesso limitado ou inexistente ao Gerenciamento de recursos no Workfront.

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Editar prioridades e horas de orçamento no Planejador | ✓&#42; |  |  |  |  |
| Criar, editar, excluir Conjuntos de Recursos&#42;&#42; | ✓&#42; |  |  |  |  |
| Atualizar Horas Planejadas no Balanceador de Carga de Trabalho&#42;&#42;&#42; | ✓* |  |  |  |  |
| Exibir prioridades de projeto no Planejador de Recursos | ✓&#42; |  |  |  |  |
| Exibir alocação de recursos nas ferramentas de Planejamento de Recursos | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Exibir Conjuntos de Recursos | ✓&#42; | ✓&#42; | ✓&#42; |  |  |
| Recursos de orçamento nas ferramentas de Planejamento de Recursos&#42;&#42; | ✓ |  |  |  |  |
| Anexar Conjuntos de Recursos a projetos, modelos e usuários | ✓ |  |  |  |  |

{style="table-layout:auto"}

&#42; Usando um nível de acesso, os administradores do Workfront podem desabilitar ou habilitar essa funcionalidade. Para obter mais informações, consulte [Acesso configurável à funcionalidade para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

&#42;&#42;Requer acesso adicional a Dados Financeiros e permissões para finanças do projeto. Se você conceder acesso ao Gerenciamento de recursos a um usuário do Planejador que não tem acesso aos Dados financeiros, o usuário ainda poderá ver as alocações por hora no Planejador de recursos, mas não poderá alternar para a visualização de custos ou visualizar o Business Case. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar permissões financeiras em um objeto](../../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md).

&#42;&#42;&#42;Requer permissão para contribuir com o objeto, com a opção Fazer atribuições habilitada em Configurações avançadas. Para obter informações, consulte a seção [Entender as permissões herdadas e a hierarquia de objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md#sharing-an-object) no artigo [Visão geral das permissões de compartilhamento em objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Área do Planejador de Cenários

| Ação | Planejador | Trabalhador | Revisor | Solicitante | Usuário externo |
|---|---|---|---|---|---|
| Criar/editar planos e iniciativas existentes | ✓ | ✓ | ✓ |  |  |
| Adicionar ou editar informações de função de trabalho em planos e iniciativas&#42; | ✓ | ✓ | ✓ |  |  |
| Adicionar ou editar informações de custo em planos e iniciativas&#42; | ✓ | ✓ | ✓ |  |  |
| Excluir planos e iniciativas | ✓ | ✓ | ✓ |  |  |
| Exibir Cenários no Menu Principal ![Ícone do planejador de cenários](assets/esp-icon-in-main-menu.png) | ✓ | ✓ | ✓ | |  |
| Exibir planos e iniciativas criados pelo usuário&#42; | ✓ | ✓ | ✓ |  |  |

{style="table-layout:auto"}

>[!NOTE]
>
>Os usuários poderão exibir um plano que outro usuário criou somente se um link para o plano for compartilhado com eles.

&#42; Para que os usuários visualizem dados financeiros em um plano ou iniciativa, eles precisam de acesso aos Dados Financeiros. Para obter mais informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

## Área Metas do Workfront

| Ações | Exibir | Editar |
|---|---|---|
| Criar |  | ✓ |
| Editar/excluir todas as metas |  | ✓ |
| Exibir Metas no menu Principal | ✓ | ✓ |
| Exibir a área Metas de um link compartilhado | ✓ | ✓ |
| Exibir todas as metas no sistema | ✓ | ✓ |
| Ativar/ desativar/ fechar todas as metas |  | ✓ |
| Criar/ editar/ excluir atividades |  | ✓ |
| Criar/ editar/ excluir resultados |  | ✓ |
| Adicionar uma meta alinhada |  | ✓ |
| Atualizar progresso em um resultado ou atividade |  | ✓ |
| Ter uma meta, resultado ou atividade | ✓ | ✓ |
| Comentar em uma meta | ✓ | ✓ |
| Copiar metas |  | ✓ |
| Exibir a seção Lista de metas no painel esquerdo | ✓ | ✓ |
| Exibir a seção Gráficos no painel esquerdo | ✓ | ✓ |
| Exibir a seção Alinhamento de metas no painel esquerdo | ✓ | ✓ |


