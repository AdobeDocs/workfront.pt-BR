---
product-area: workfront-basics
navigation-topic: workfront-mcp-server
title: Ferramentas de servidor Adobe Workfront MCP
description: Lista de referência das ferramentas disponíveis no servidor MCP do Adobe Workfront, agrupadas por área do Workfront.
author: Courtney
feature: Get Started with Workfront
hide: true
source-git-commit: 98d5b93bcb99c468de2ad107a2aca3a9a1995429
workflow-type: tm+mt
source-wordcount: '1392'
ht-degree: 3%

---


# Ferramentas de servidor Adobe Workfront MCP

Este artigo lista as ferramentas que o servidor MCP [!DNL Adobe Workfront] expõe a uma plataforma de agente de IA conectada. A plataforma chama essas ferramentas em seu nome quando você solicita que elas encontrem, criem, atualizem ou excluam itens do Workfront.

As ferramentas são agrupadas por área do Workfront: Aprovações, Planejamento e Fluxo de trabalho.

Para obter informações sobre como usar essas ferramentas por meio de uma plataforma de agente de IA, consulte [Usar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md). Para obter informações sobre como configurar a conexão, consulte [Configurar o servidor MCP do Adobe Workfront](/help/quicksilver/workfront-basics/workfront-mcp-server/configure-workfront-mcp-server.md).

>[!IMPORTANT]
>
>A plataforma do agente de IA atua no Workfront usando sua conta da Workfront, o nível de acesso e as permissões do objeto. Uma ferramenta só funciona se você tiver o acesso correspondente no Workfront. A Adobe não se responsabiliza pelas alterações que a plataforma de IA Agent faz nos dados do Workfront.

## Ferramentas de aprovação (23 no total)

### Documentos

<!-- 
VERIFY BEFORE PUBLISHING: The following three tools may not be customer-facing. If engineering confirms they're internal-only, delete these rows from the table below:
- approvals_get_document_by_version_id
- approvals_list_aem_linked_folders
- approvals_send_documents_to_aem_folder
-->

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Localizar versão do documento por nome | `approvals_find_document_version_by_name` | Pesquisa a ID de versão atual de um documento por nome de arquivo. Suporta correspondências parciais. |
| Obter documento por ID de versão | `approvals_get_document_by_version_id` | Busca detalhes do documento (nome, tamanho, data de upload, carregador) para uma ID de versão de documento conhecida. |
| Obter documentos por projeto | `approvals_get_documents_by_project` | Lista documentos dentro de um projeto Workfront, com cada ID de versão atual do documento. |
| Resolver escopo do documento | `approvals_resolve_document_scope` | Expande um projeto ou pasta para a lista de IDs de versão de documento que ela contém. Suporta escopos de projeto, pasta e pasta por nome. |
| Listar pastas vinculadas ao AEM | `approvals_list_aem_linked_folders` | Lista as pastas de documentos do Workfront vinculadas ao Adobe Experience Manager. |
| Enviar documentos para a pasta do AEM | `approvals_send_documents_to_aem_folder` | Move um ou mais documentos do Workfront para uma pasta vinculada ao AEM. |

### Fluxos de trabalho de aprovação

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter informações de fluxo de trabalho de aprovação | `approvals_get_approval_info` | Retorna o fluxo de trabalho de aprovação atual (estágios, participantes, status) para uma versão do documento. |
| Criar ou atualizar fluxo de trabalho de aprovação | `approvals_create_or_update_approval_workflow` | Cria ou atualiza os estágios do fluxo de trabalho de aprovação para uma versão do documento. Suporta dependências de estágio linear e paralelo (gráfico). |
| Criar aprovação a partir do modelo | `approvals_create_approval_from_template` | Cria um fluxo de trabalho de aprovação em um documento usando um modelo existente. |
| Solicitar aprovação de documento | `approvals_request_document_approval` | Abre um formulário guiado para solicitar aprovação em uma versão do documento (título, aprovadores/revisores, data de vencimento e mensagem opcionais). |
| Excluir estágio de aprovação | `approvals_delete_approval_stage` | Exclui um único estágio de um fluxo de trabalho de aprovação por nome ou posição. Somente estágios não iniciados podem ser excluídos. |

### Lembretes

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Enviar lembrete aos participantes | `approvals_send_reminder_to_participants` | Envia emails de lembrete para participantes específicos em um estágio de aprovação. Funciona somente para estágios iniciados, não concluídos e não bloqueados. |
| Enviar lembrete para participantes indecisos | `approvals_send_reminder_to_undecided` | Envia emails de lembrete para todos os participantes indecisos (notificados, abertos ou comentados) em um estágio de aprovação. |

### Modelos de aprovação

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Listar modelos de aprovação | `approvals_list_templates` | Lista os modelos de aprovação disponíveis nesta instância do Workfront. Suporta filtragem por criador, participante e classificação por uso. |
| Pesquisar modelo por nome | `approvals_search_template_by_name` | Localiza modelos de aprovação por nome (não diferencia maiúsculas de minúsculas). |
| Criar modelo de aprovação | `approvals_create_template` | Cria um novo modelo de aprovação com dependências de estágio lineares ou baseadas em gráfico. |
| Atualizar modelo de aprovação | `approvals_update_template` | Atualiza um modelo existente com modificações estruturadas (adicionar ou remover participantes, renomear estágios, definir prazos, etc.). |

### Pesquisas e usuários

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter usuário atual | `approvals_get_current_user` | Retorna a identidade do Workfront do usuário que faz a chamada, incluindo nome, ID de usuário, nome da equipe inicial e ID da equipe inicial. |
| Localizar usuário por nome | `approvals_find_user_by_name` | Pesquisa a ID de um usuário do Workfront por nome (correspondência difusa ou parcial). Retorna nome, ID, email, título e URL do avatar. |
| Localizar equipe por nome | `approvals_find_team_by_name` | Pesquisa a ID de uma equipe do Workfront por nome (correspondência difusa ou parcial). |
| Localizar projeto por nome | `approvals_find_project_by_name` | Procura projetos do Workfront por correspondência de nome parcial no sistema. |
| Obter projetos por proprietário | `approvals_get_projects_by_owner` | Lista os projetos do Workfront dos quais o usuário que faz a chamada é o proprietário. |
| Obter região do Adobe | `approvals_get_adobe_region` | Retorna o nome da Adobe de uma região do provedor de nuvem. |

## Ferramentas de planejamento (43 no total)

### Espaços de trabalho

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter espaço de trabalho | `planning_get_workspace` | Recupera detalhes completos de um espaço de trabalho por ID ou alias. |
| Obter lista do espaço de trabalho | `planning_get_workspace_list` | Lista todos os espaços de trabalho disponíveis com paginação baseada em cursor. |
| Criar espaço de trabalho | `planning_create_workspace` | Cria um novo espaço de trabalho vazio para organizar tipos de registro, campos e dados. |
| Criar espaço de trabalho a partir do modelo | `planning_create_workspace_from_template` | Cria um novo espaço de trabalho pré-preenchido usando um modelo existente. |
| Atualizar espaço de trabalho | `planning_update_workspace` | Atualiza parcialmente um espaço de trabalho — nome, descrição, ícone, seções ou proprietário. |
| Excluir espaço de trabalho | `planning_delete_workspace` | Exclui permanentemente um espaço de trabalho e todos os seus dados. |
| Converter espaço de trabalho em modelo | `planning_convert_workspace_to_template` | Salva um espaço de trabalho existente como um modelo reutilizável (requer admin). |
| Obter compartilhamento do espaço de trabalho | `planning_get_workspace_sharing` | Retorna a configuração atual de compartilhamento e permissões de um espaço de trabalho. |
| Modificar compartilhamento do espaço de trabalho | `planning_modify_workspace_sharing` | Atualiza quem tem acesso a um espaço de trabalho e em qual nível de permissão. |

### Tipos de registro

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter tipo de registro | `planning_get_record_type` | Obtém detalhes completos de um tipo de registro, incluindo seus campos e visualizações. |
| Criar tipos de registro | `planning_create_record_types` | Cria um ou mais tipos de registro em uma seção do espaço de trabalho. |
| Atualizar tipo de registro | `planning_update_record_type` | Atualiza parcialmente o nome, a descrição, o ícone ou a cor de um tipo de registro. |
| Excluir um tipo de registro | `planning_delete_record_type` | Exclui permanentemente um tipo de registro e todos os seus registros, campos e visualizações. |
| Listar tipos de registros globais | `planning_list_global_record_types` | Lista todos os tipos de registro (global) definidos centralmente visíveis para o usuário atual. |
| Listar tipos de registros globais que podem ser adicionados | `planning_list_addable_global_record_types` | Lista os tipos de registro global que podem ser adicionados a um espaço de trabalho específico. |
| Adicionar tipo de registro global ao espaço de trabalho | `planning_add_global_record_type_to_workspace` | Vincula um tipo de registro global a um espaço de trabalho especificado. |
| Remover tipo de registro global do espaço de trabalho | `planning_remove_global_record_type_from_workspace` | Desvincula um tipo de registro global de um espaço de trabalho; exclui todos os seus registros nesse espaço de trabalho. |
| Obter espaços de trabalho de registro externo | `planning_get_external_record_workspaces` | Localiza quais espaços de trabalho e tipos de registro estão conectados a um registro externo específico. |
| Obter compartilhamento de tipo de registro | `planning_get_record_type_sharing` | Retorna o compartilhamento e as permissões de um tipo de registro específico. |
| Modificar compartilhamento de tipo de registro | `planning_modify_record_type_sharing` | Atualiza quem pode acessar um tipo de registro e em qual nível de permissão. |

### Registros

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter registro | `planning_get_record` | Recupera detalhes completos de um único registro por ID. |
| Pesquisar registros | `planning_search_records` | Pesquisa e filtra registros dentro de um tipo de registro. |
| Ações de registro em massa | `planning_bulk_record_actions` | Cria, atualiza, exclui ou restaura vários registros em uma única solicitação. |
| Criar registro de conexão | `planning_create_connection_record` | Cria um novo registro em um sistema externo conectado (por exemplo, um projeto do Workfront). |
| Atualizar ordem de registros | `planning_update_records_order` | Altera a ordem de exibição dos registros dentro de um tipo de registro. |
| Obter log de alterações de registro | `planning_get_record_change_log` | Retorna o histórico de edição em nível de campo de um registro. |
| Obter compartilhamento de registros | `planning_get_record_sharing` | Retorna a configuração de compartilhamento de um registro específico. |
| Modificar compartilhamento de registros | `planning_modify_records_sharing` | Atualiza quem pode acessar um ou mais registros e em qual nível de permissão. |

### Campos

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter campo | `planning_get_field` | Recupera detalhes completos e o esquema de valor de um campo por ID. |
| Criar campos | `planning_create_fields` | Adiciona um ou mais campos (colunas) a um tipo de registro. |
| Atualizar campo | `planning_update_field` | Atualiza parcialmente o nome, a descrição, as opções ou a configuração de um campo. |
| Excluir campo | `planning_delete_field` | Remove permanentemente um campo e todos os seus dados de um tipo de registro. |

### Exibições

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter visualização | `planning_get_view` | Retorna detalhes completos de uma exibição por ID. |
| Criar visualização | `planning_create_view` | Cria uma nova tabela, linha do tempo ou exibição de calendário para um tipo de registro. |
| Atualizar exibição | `planning_update_view` | Atualiza parcialmente a configuração, os filtros ou a classificação de uma visualização existente. |
| Excluir visualização | `planning_delete_view` | Exclui permanentemente uma exibição (os registros não são afetados). |
| Obter compartilhamento de visualização | `planning_get_view_sharing` | Retorna a configuração de compartilhamento de uma exibição específica. |
| Modificar compartilhamento de visualização | `planning_modify_view_sharing` | Atualiza quem pode acessar uma visualização e em qual nível de permissão. |

### Modelos

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Obter lista de modelos | `planning_get_template_list` | Lista todos os modelos de espaço de trabalho disponíveis com informações de resumo. |
| Obter modelo | `planning_get_template` | Recupera detalhes completos de um modelo específico por ID. |

### Busca e utilitários

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Pesquisar recursos | `planning_search_resources` | Pesquisas em espaços de trabalho, tipos de registro e exibições por nome. |
| Pesquisar dados de compartilhamento | `planning_search_sharing_data` | Localiza usuários, grupos, equipes, funções e empresas por nome para compartilhamento e permissões. |
| Procurar usuários | `planning_search_users` | Pesquisa usuários com suporte à paginação. |

## Ferramentas de fluxo de trabalho (5 no total)

As ferramentas de fluxo de trabalho são ações de uso geral que a plataforma de IA usa para trabalhar com qualquer objeto do Workfront — projetos, tarefas, problemas, horas, atribuições, programas, portfólios e assim por diante.

| Título | Nome da ferramenta | O que faz |
|---|---|---|
| Pesquisar objetos | `workflow_search_any_object` | Pesquisa por objetos do Workfront com parâmetros de filtro, ordenação e paginação flexíveis. |
| Criar objeto | `workflow_create_any_object` | Cria um novo objeto do Workfront, como um projeto, tarefa, problema, hora, atribuição, programa ou portfólio. |
| Atualizar objeto | `workflow_update_any_object` | Atualiza campos em um objeto Workfront existente. |
| Excluir objeto | `workflow_delete_any_object` | Exclui um objeto do Workfront por ID. Requer confirmação explícita do usuário antes que a ação seja executada. |
| Resolver nomes de campo | `workflow_resolve_field_names_any_object` | Converte nomes de campo ou rótulos fornecidos pelo usuário em nomes de campo subjacentes da API do Workfront para que a plataforma do agente de IA possa criar solicitações precisas. |

## Como as ferramentas são atualizadas

Quando o Adobe lança uma nova versão do servidor MCP do Workfront, a plataforma de agente de IA usa o novo conjunto de ferramentas automaticamente. Você não precisa reconectar ou alterar nada em seu lado.
