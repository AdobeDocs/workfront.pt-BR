---
title: Logs de auditoria
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Adobe Workfront, você pode rastrear as alterações de usuário acionadas no sistema nos últimos 90 dias usando logs de auditoria.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 6adb4146-42fd-4eda-b46f-c61d7ff71df6
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '1527'
ht-degree: 3%

---

# Logs de auditoria

<!--Audited: 01/2024-->

Como administrador do Adobe Workfront, você pode rastrear as alterações de usuário acionadas no sistema nos últimos 90 dias usando os logs de auditoria descritos abaixo.

Para obter instruções sobre como visualizar e filtrar o que deseja ver nesses logs de auditoria, consulte [Exibir e exportar logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Informações que você pode encontrar em um log de auditoria

Os seguintes campos são registrados em cada entrada do log de auditoria:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Data e Hora</td> 
   <td>Quando a ação ocorreu.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Tipo de log</td> 
   <td>Tipo do log de auditoria, como Nível de acesso ou Formulário personalizado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nome do usuário</td> 
   <td> <p>Nome do usuário que executou a ação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ação</td> 
   <td> Ações executadas pelo usuário, como Alterar, Criar e Excluir. </td> 
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
   <td> <p>Endereço IP do usuário que executou a ação no momento da ação.</p> <p>Endereço IP não disponível para algumas ações do sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de log de auditoria e as ações que os acionam

* [Nível de Acesso](#access-level)
* [Regras de negócios](#business-rules)
* [Empresa](#company)
* [Condição](#condition)
* [Campo personalizado](#custom-field)
* [Formulário personalizado](#custom-forms)
* [Seção personalizada](#custom-section)
* [Taxa de Câmbio](#exchange-rate)
* [Grupo](#group)
* [Funções de trabalho](#job-roles)
* [Tentativa de login](#login-attempt)
* [Prioridade](#priority)
* [Preferência do projeto](#project-preference)
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
   * Altera permissões de projetos, tarefas, problemas, Portfolio, programas, relatórios, documentos, usuários ou modelos

     >[!NOTE]
     >
     >O sistema não registra nenhuma alteração de permissão nos Dados financeiros ou nos seguintes tipos de acesso: Exibir e Editar.
     >
     >Por exemplo, se um usuário alterar o tipo de acesso Planejador de Exibir para Editar, o sistema não exibirá as informações contidas no menu suspenso Ajustar as configurações.

### Regras de negócios

O Business Rules só está disponível para clientes que compraram um Plano Ultimate Workfront. Para obter mais informações, consulte [Criar e editar regras de negócios](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/business-rules.md).

O sistema gera uma entrada de log de auditoria da Regra de Negócios quando um usuário realiza uma das seguintes ações:

* Cria uma regra de negócios
* Edita uma regra de negócios:

   * Renomeia
   * Adiciona ou remove expressões
   * Altera um acionador

* Exclui uma regra de negócios

### Empresa {#company}

O sistema gera uma entrada de log de auditoria da empresa quando um usuário executa um dos seguintes procedimentos:

* Cria uma empresa
* Muda uma empresa:

   * Renomeia
   * Adiciona ou remove membros
   * Adiciona, edita ou exclui o valor no campo Grupo
   * Adiciona ou edita uma taxa de cobrança da empresa para uma função de trabalho
   * Remove uma taxa de cobrança da empresa para uma função de trabalho
   * Define a empresa como a empresa principal da organização
   * Anexa ou remove um formulário personalizado

* Exclui uma empresa

Para obter mais informações sobre status, consulte [Visão geral dos status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Condição {#condition}

O sistema gera uma entrada de log de auditoria de Condição quando um usuário executa uma das seguintes ações:

* Cria uma condição
* Altera uma condição:

   * Altera o nome
   * Altera a cor
   * Define como padrão
   * Altera ou remove a descrição da condição
   * Oculta ou mostra a condição

* Exclui uma condição

Para obter mais informações sobre como configurar funções de trabalho, consulte [Criar ou editar uma condição personalizada](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

### Campo personalizado {#custom-field}

O sistema gera uma entrada de log de auditoria Campo personalizado quando um usuário executa uma das seguintes ações:

* Cria um campo personalizado
* Altera um campo personalizado:

   * Altera o nome, rótulo, instruções ou formato
   * Altera o tipo de exibição

     Isso só estará disponível se o campo for de um dos seguintes tipos: linha única, parágrafo, lista suspensa, caixa de seleção, botão de opção

   * Altera o tamanho do campo

     Isso só estará disponível se o campo for de um dos seguintes tipos: linha única, parágrafo, texto com formatação

   * Adiciona, remove ou oculta uma escolha de campo
   * Edita um rótulo ou valor de escolha de campo
   * Configura a opção de campo a ser selecionada ou não por padrão
   * Configura um campo suspenso para permitir várias seleções ou uma única seleção
   * Configura um campo de data para exibir ou não a hora do dia
   * Edita o hiperlink ou altera o valor em um campo de texto descritivo

* Exclui um campo personalizado
* Compartilha um campo personalizado

### Formulário personalizado {#custom-form}

O sistema gera uma entrada de log de auditoria Forms personalizada quando um usuário executa uma das seguintes ações:

* Cria um formulário personalizado
* Altera um formulário personalizado:

   * Altera o nome ou a descrição
   * Ativa ou desativa está ativo
   * Adiciona ou remove um campo ou seção
   * Para uma seção personalizada, altera uma configuração em Configurações adicionais
   * Altera um campo para obrigatório ou não obrigatório
   * Altera um cálculo em um campo personalizado
   * Oculta ou exibe a fórmula associada a um campo calculado no texto ao passar o mouse das Instruções
   * Habilita ou desabilita Atualizar cálculos anteriores
   * Adiciona ou altera a lógica de salto ou de exibição

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>Adds or changes a filter for a typeahead field</p></li>   
     -->

* Exclui um formulário personalizado
* Compartilha um formulário personalizado

### Seção personalizada {#custom-section}

O sistema gera uma entrada de log de auditoria Seção personalizada quando um usuário executa uma das seguintes ações em um formulário personalizado:

* Cria uma seção personalizada
* Altera o nome ou a descrição de uma seção personalizada
* Exclui uma seção personalizada

Para obter informações sobre seções personalizadas em formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Taxa de câmbio {#exchange-rate}

O sistema gera uma entrada de log de auditoria de Taxa de Câmbio quando um usuário executa uma das seguintes ações:

* Cria uma taxa de câmbio
* Altera uma taxa de câmbio:

   * Adiciona uma moeda
   * Altera a taxa da moeda
   * Define a moeda como a moeda base (padrão) para todos os projetos e relatórios no sistema

* Exclui uma taxa de câmbio

Para obter mais informações sobre como configurar taxas de câmbio, consulte [Configurar taxas de câmbio](../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

### Grupo {#group}

O sistema gera uma entrada de log de auditoria de Grupo quando um usuário executa uma das seguintes ações:

* Cria um grupo
* Exclui um grupo
* Altera um grupo:

   * Adiciona ou remove usuários
   * Adiciona ou remove subgrupos

### Função no trabalho {#job-roles}

O sistema gera uma entrada de log de auditoria Funções de trabalho quando um usuário executa uma das seguintes ações:

* Cria uma função de trabalho
* Altera uma função de trabalho:

   * Altera o nome
   * Adiciona, altera ou remove a descrição
   * Adiciona, altera ou remove o custo por hora (Custo/Hr.)
   * Adiciona, altera ou remove a taxa de cobrança (Fatura/Hr.)

* Exclui uma função de trabalho

Para obter mais informações sobre como configurar funções de trabalho, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

### Tentativa de login {#login-attempt}

O sistema gera uma entrada de log de auditoria de Tentativa de login quando um usuário executa uma das seguintes ações:

* Faz logon, logout ou falha em uma tentativa de logon no Workfront (em um navegador e no aplicativo móvel)
* Faz logon, logout ou falha em uma tentativa de logon em qualquer integração do Workfront (como Workfront para Slack e Workfront para Salesforce)
* Faz logon ou logout da API do Workfront

Os logs de tentativa de logon não registram quando um administrador do Workfront usa o recurso &quot;Login como&quot;.

>[!NOTE]
>
>Isso não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte o administrador de rede ou de TI se precisar de mais informações.

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

### Preferências do projeto {#project-preference}

O sistema gera uma entrada de log de auditoria de Preferências do projeto quando um usuário executa uma das seguintes ações:

* Cria um trimestre personalizado
* Altera uma preferência de projeto:

   * Bloqueia ou desbloqueia
   * Altera uma de suas configurações
   * Ativa, desativa ou edita o script
   * Edita um cálculo de linha do tempo

* Exclui um trimestre personalizado

Para obter mais informações sobre preferências de projeto, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

### Severidade {#severity}

O sistema gera uma entrada de log de auditoria de severidade quando um usuário executa uma das seguintes ações:

* Cria uma severidade de problema
* Altera a gravidade de um problema:

   * Altera o nome
   * Altera a cor
   * Define como padrão
   * Altera ou remove a descrição da severidade
   * Oculta ou mostra a severidade

* Exclui a gravidade de um problema

Para obter mais informações sobre como configurar funções de trabalho, consulte [Criar ou personalizar severidades de problemas](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-issue-severities.md).

### Status {#status}

O sistema gera uma entrada de log de auditoria de status quando um usuário executa uma das seguintes ações:

* Cria um status no nível do sistema ou do grupo
* Altera um status no nível do sistema ou do grupo:

   * Renomeia
   * Transforma em um status padrão
   * Bloqueia ou desbloqueia
   * Oculta ou reexibe
   * Altera a cor ou a descrição

* Exclui um status no nível do sistema ou do grupo

Para obter mais informações sobre status, consulte [Visão geral dos status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

### Preferências de tarefas e problemas {#tasks-issues-preferences}

O sistema gera uma entrada de log de auditoria de Preferências de tarefas e problemas quando um usuário altera a preferência de Tarefas e problemas de uma das seguintes maneiras:

* Bloqueia ou desbloqueia uma preferência
* Altera a configuração de uma preferência
* Altera uma configuração de Acesso para tarefas, problemas ou solicitações

Para obter mais informações sobre preferências de tarefas e problemas, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

### Usuário {#user}

O sistema gera uma entrada de log de auditoria do usuário quando um usuário executa uma das seguintes ações:

* Cria um usuário

  <!--
  DRAFTED IN FLARE:
  Gevorg checking with Jonah on whether this note should be here:
  
  -->

  >[!NOTE]
  >
  >Isso não estará disponível se sua organização tiver sido integrada à Adobe Admin Console. Consulte o administrador de rede ou de TI se precisar de mais informações.

* Exclui um usuário
* Altera o nível de acesso, a empresa, a equipe ou o grupo de um usuário
* Ativa um usuário
* Desativa um usuário
