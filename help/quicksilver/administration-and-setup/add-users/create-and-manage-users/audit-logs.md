---
title: Logs de auditoria
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, você pode rastrear as alterações do usuário acionadas no sistema durante os últimos 90 dias usando logs de auditoria.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '1462'
ht-degree: 4%

---

# Logs de auditoria

Como administrador do Adobe Workfront, você pode rastrear as alterações do usuário acionadas no sistema durante os últimos 90 dias usando os logs de auditoria descritos abaixo.

Para obter instruções sobre como visualizar e filtrar o que deseja ver nesses logs de auditoria, consulte [Exibir e exportar logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informações que você pode encontrar em um log de auditoria

Os seguintes campos são registrados em cada entrada de log de auditoria:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Data e hora</td> 
   <td>Quando a ação ocorreu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de log</td> 
   <td>Tipo de log de auditoria, como Nível de acesso ou Formulário personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do usuário</td> 
   <td> <p>Nome do usuário que executou a ação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ação</td> 
   <td> Ação executada pelo usuário, como Alterar, Criar e Excluir. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objeto</td> 
   <td> Nome do objeto afetado como resultado da ação. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Detalhes</td> 
   <td>Detalhes adicionais sobre a ação. Passe o mouse sobre o texto para ler a mensagem completa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Endereço IP</td> 
   <td> <p>Endereço IP do usuário que executou a ação no momento da ação.</p> <p>O endereço IP não está disponível para algumas ações do sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de log de auditoria e ações que os acionam

* [Nível de acesso](#access-level)
* [Empresa](#company)
* [Condição](#condition)
* Campo personalizado [ ](#custom-field)
* [Formulários personalizados](#custom-forms)
* [Seção personalizada](#custom-section)
* [Taxa de câmbio](#exchange-rate)
* [Grupo](#group)
* [Função no trabalho](#job-roles)
* [Tentativa de login](#login-attempt)
* [Prioridade](#priority)
* [Preferências do projeto](#project-preferences)
* [Severidade](#severity)
* [Status](#status)
* [Preferências de tarefas e problemas](#tasks-issues-preferences)
* [Usuário](#user)

### Nível de acesso {#access-level}

O sistema gera uma entrada de log de Nível de acesso quando um usuário executa uma das seguintes ações:

* Cria um nível de acesso
* Exclui um nível de acesso
* Altera um nível de acesso:

   * Modifica o tipo de licença
   * Altera as permissões para Projetos, Tarefas, Problemas, Portfolio, Programas, Relatórios, Documentos, Usuários ou Modelos

      >[!NOTE]
      >
      >O sistema não registra nenhuma alteração de permissão para Dados Financeiros ou nos seguintes tipos de acesso: Exibir e editar.
      >
      >Por exemplo, se um usuário alterar o tipo de acesso do Planejador de Exibir para Editar, o sistema não exibirá as informações contidas no menu suspenso Ajustar configurações.

### Empresa {#company}

O sistema gera uma entrada de log de auditoria da empresa quando um usuário executa um dos seguintes procedimentos:

* Cria uma empresa
* Altera uma empresa:

   * Renomeia
   * Adiciona ou remove membros
   * Adiciona, edita ou exclui o valor em seu campo Grupo
   * Adiciona ou edita uma taxa de faturamento da empresa para uma função de cargo
   * Remove uma taxa de faturamento da empresa para uma função de trabalho
   * Define como a principal empresa da organização
   * Anexa ou remove um formulário personalizado

* Exclui uma empresa

Para obter mais informações sobre status, consulte [Visão geral dos status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condição {#condition}

O sistema gera uma entrada de log de auditoria de condição quando um usuário executa uma das seguintes ações:

* Cria uma condição
* Altera uma condição:

   * Altera o nome
   * Altera a cor
   * Define como padrão
   * Altera ou remove a descrição da condição
   * Oculta ou mostra a condição

* Exclui uma condição

Para obter mais informações sobre como configurar funções de job, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Campo personalizado {#custom-field}

O sistema gera uma entrada de log de auditoria de Campo personalizado quando um usuário executa uma das seguintes ações:

* Cria um campo personalizado
* Altera um campo personalizado:

   * Altera o nome, rótulo, instruções ou formato
   * Altera o tipo de exibição

      Isso só estará disponível se o campo for um dos seguintes tipos: linha única, parágrafo, lista suspensa, caixa de seleção, botão de opção

   * Altera o tamanho do campo

      Isso só estará disponível se o campo for um dos seguintes tipos: linha única, parágrafo, texto com formatação

   * Adiciona, remove ou oculta uma opção de campo
   * Edita um rótulo ou valor de escolha de campo
   * Configura a opção de campo a ser selecionada ou não selecionada por padrão
   * Configura um campo suspenso para permitir várias seleções ou uma única seleção
   * Configura um campo de data para exibir ou não a hora do dia
   * Edita o hiperlink ou altera o valor em um campo de texto descritivo

* Exclui um campo personalizado
* Compartilha um campo personalizado

### Formulários personalizados {#custom-forms}

O sistema gera uma entrada de log de auditoria Forms personalizada quando um usuário executa uma das seguintes ações:

* Cria um formulário personalizado
* Altera um formulário personalizado:

   * Altera o nome ou a descrição
   * Ativa ou desativa Está Ativa
   * Adiciona ou remove um campo ou seção
   * Para uma seção personalizada, altera uma configuração em Configurações adicionais
   * Altera um campo para obrigatório ou não
   * Altera um cálculo em um campo personalizado
   * Oculta ou exibe a fórmula associada a um campo calculado no texto de flutuação de Instruções
   * Ativa ou desativa Atualizar cálculos anteriores
   * Adiciona ou altera a lógica de ignorar ou a lógica de exibição

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Exclui um formulário personalizado
* Compartilha um formulário personalizado

### Seção personalizada {#custom-section}

O sistema gera uma entrada de log de auditoria da Seção personalizada quando um usuário executa uma das seguintes ações em um formulário personalizado:

* Cria uma seção personalizada
* Altera o nome ou a descrição de uma seção personalizada
* Exclui uma seção personalizada

Para obter informações sobre seções personalizadas em formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

### Taxa de câmbio {#exchange-rate}

O sistema gera uma entrada de log de auditoria da Taxa de Câmbio quando um usuário executa uma das seguintes ações:

* Cria uma taxa de câmbio
* Altera uma taxa de câmbio:

   * Adiciona uma moeda
   * Altera a taxa da moeda
   * Define a moeda como moeda base (padrão) para todos os projetos e relatórios em todo o sistema

* Exclui uma taxa de câmbio

Para obter mais informações sobre como configurar as taxas de câmbio, consulte [Configurar taxas de câmbio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Grupo {#group}

O sistema gera uma entrada de log de auditoria do grupo quando um usuário executa uma das seguintes ações:

* Cria um grupo
* Exclui um grupo
* Altera um grupo:

   * Adiciona ou remove usuários
   * Adiciona ou remove subgrupos

### Função no trabalho {#job-roles}

O sistema gera uma entrada de log de auditoria de Funções de Trabalho quando um usuário executa uma das seguintes ações:

* Cria uma função de trabalho
* Altera uma função de trabalho:

   * Altera o nome
   * Adiciona, altera ou remove a descrição
   * Adiciona, altera ou remove o custo por hora (Custo/Hora).
   * Adiciona, altera ou remove a taxa de faturamento (Faturamento/Hora)

* Exclui uma função de trabalho

Para obter mais informações sobre como configurar funções de job, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Tentativa de login {#login-attempt}

O sistema gera uma entrada de log de tentativa de logon quando um usuário executa uma das seguintes ações:

* Faz logon, faz logoff ou falha em uma tentativa de logon no Workfront (em um navegador e no aplicativo móvel)
* Faz logon, faz logoff ou falha em uma tentativa de logon em qualquer integração do Workfront (como Workfront for Slack e Workfront for Salesforce)
* Faz logon ou logout da API do Workfront

Os registros de tentativas de logon não são registrados quando um administrador do Workfront usa o recurso Fazer logon como .

>[!NOTE]
>
>Isso não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte seu administrador de rede ou de TI se precisar de mais informações.

### Prioridade {#priority}

O sistema gera uma entrada de log de auditoria de prioridade quando um usuário executa uma das seguintes ações:

* Cria uma prioridade
* Altera uma prioridade:

   * Altera o nome
   * Altera a cor
   * Define como padrão
   * Adiciona, altera ou remove a descrição da prioridade
   * Oculta ou mostra a prioridade

* Exclui uma prioridade

Para obter mais informações sobre como configurar prioridades, consulte [Criar e personalizar prioridades](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md).

### Preferências do projeto {#project-preferences}

O sistema gera uma entrada de log de auditoria de Preferências de projeto quando um usuário executa uma das seguintes ações:

* Cria um trimestre personalizado
* Altera uma preferência de projeto:

   * Bloqueia ou desbloqueia
   * Altera uma de suas configurações
   * Ativa, desativa ou edita
   * Edita um cálculo de linha do tempo

* Exclui um trimestre personalizado

Para obter mais informações sobre as preferências do projeto, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Severidade {#severity}

O sistema gera uma entrada de log de auditoria de Gravidade quando um usuário executa uma das seguintes ações:

* Cria uma severidade de problema
* Altera a gravidade de um problema:

   * Altera o nome
   * Altera a cor
   * Define como padrão
   * Altera ou remove a descrição da gravidade
   * Oculta ou mostra a gravidade

* Exclui uma gravidade de problema

Para obter mais informações sobre como configurar funções de job, consulte [Criar ou personalizar severidades de problemas](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Status {#status}

O sistema gera uma entrada de log de auditoria de status quando um usuário executa uma das seguintes ações:

* Cria um status no nível do sistema ou do grupo
* Altera um status no sistema ou no nível do grupo:

   * Renomeia
   * Torna-o um status padrão
   * Bloqueia ou desbloqueia
   * Oculta ou desoculta
   * Altera a cor ou a descrição

* Exclui um status no sistema ou no nível do grupo

Para obter mais informações sobre status, consulte [Visão geral dos status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Preferências de tarefas e problemas {#tasks-issues-preferences}

O sistema gera uma entrada de log de auditoria de Preferências de Tarefas e Problemas quando um usuário altera uma preferência Tarefas e Problemas de uma das seguintes maneiras:

* Bloqueia ou desbloqueia uma preferência
* Altera a configuração de uma preferência
* Altera uma configuração de Acesso para tarefas, problemas ou solicitações

Para obter mais informações sobre as preferências de tarefa e emissão, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Usuário {#user}

O sistema gera uma entrada de log de auditoria do usuário quando ele executa uma das seguintes ações:

* Cria um usuário

   <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

   >[!NOTE]
   >
   >Isso não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte seu administrador de rede ou de TI se precisar de mais informações.

* Exclui um usuário
* Altera o nível de acesso, a empresa, a equipe ou o grupo de um usuário
* Ativa um usuário
* Desativa um usuário
