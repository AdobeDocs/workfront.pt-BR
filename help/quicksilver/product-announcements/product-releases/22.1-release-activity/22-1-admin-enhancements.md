---
title: 22.1 Aprimoramentos do administrador
description: 22.1 Aprimoramentos do administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
recommendations: noDisplay, noCatalog
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '1505'
ht-degree: 0%

---

# 22.1 Aprimoramentos do administrador

Esta página descreve todas as melhorias de Administrador feitas com a versão 22.1 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 17 de janeiro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.1, consulte a [Visão geral da versão 22.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Downloads de documentos registrados na área Atualizações

Para ajudar os usuários a rastrear downloads de documentos armazenados no Workfront, o sistema agora registra uma entrada na área Atualizações de um documento quando alguém faz o download.

>[!NOTE]
>
>Recomendamos testar esse recurso na Pré-visualização em um documento recém-carregado.

Para obter informações sobre como a Workfront registra atualizações automáticas em objetos, consulte [Atualizações rastreadas pelo sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Conceder acesso às equipes que usam níveis de acesso

Uma nova seção na área Níveis de acesso oferece controles mais granulares para gerenciar o acesso dos usuários às equipes. Agora você pode determinar quem pode criar, editar e visualizar equipes.

Isso não altera o acesso existente de seus usuários às equipes.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## Mapeamento de grupo agora disponível em blueprints

Alguns blueprints agora incluem grupos, que podem ser personalizados antes de instalar o blueprint. Você pode mapear um grupo no blueprint para um grupo existente na instância do Workfront ou criar um novo grupo, se necessário.

Para obter mais informações, consulte [Configurar um blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Atualizações de estilo na área Forms personalizado

A área Forms personalizado tem uma nova aparência que a atualiza com muitas outras áreas na nova experiência do Workfront.

Para obter informações sobre como criar um formulário personalizado, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Muitas melhorias na criação de campos personalizados calculados

A criação de campos personalizados calculados agora é muito mais fácil com essas adições no novo Editor de cálculo:

* Você pode passar o mouse sobre qualquer expressão no cálculo para exibir informações sobre ela, incluindo uma descrição, um exemplo de como ela pode ser usada e um link para obter mais informações em um artigo de ajuda.
* Cada expressão adicionada é codificada por cores, dependendo do tipo. Isso facilita a detecção de expressões e o reconhecimento imediato do tipo.
* Os números de linha ajudam a identificar e fazer referência a funções em um cálculo longo.
* Quando você começa a digitar uma expressão ou nome de campo, uma lista de itens disponíveis é exibida para que você possa escolher aquele que deseja. Quando você digita um parêntese de abertura, o parêntese de fechamento é adicionado automaticamente.
* Você pode visualizar o resultado do cálculo usando um objeto existente sem sair do editor de cálculo.

Além disso, no texto personalizável ao passar o mouse em &quot;Instruções&quot; para um campo personalizado calculado, é possível exibir ou ocultar a fórmula do campo. Isso é útil se você achar que os usuários que preencherão o formulário personalizado não precisarão dessas informações.

Para obter mais informações sobre como criar um campo personalizado calculado, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Exibir informações de log de auditoria sobre status e empresas

Agora é possível solucionar mais facilmente os incidentes envolvendo status e empresas exibindo informações sobre eles na área Logs de auditoria em Configuração.

Por exemplo:

* Você pode descobrir quem renomeou, bloqueou ou ocultou um status e quando o fizeram.
* Você pode descobrir quem removeu alguns membros ou funções de trabalho de uma empresa e quando eles o fizeram.

Para obter informações sobre como exibir informações de log de auditoria, consulte [Exibir e exportar logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Blueprints, mapeamento da empresa e outros aprimoramentos

Os seguintes aprimoramentos de blueprints estão disponíveis:

* Alguns blueprints agora incluem empresas, que você pode personalizar antes de instalar o blueprint. Você pode mapear uma empresa no blueprint para uma empresa existente na instância do Workfront ou criar uma nova empresa, se necessário.
* Um novo tipo de blueprint, Estrutura organizacional, agora está disponível. Alguns blueprints incluem elementos de vários tipos (por exemplo, Modelo de projeto e Estrutura organizacional). Você pode filtrar por tipo de blueprint na página do catálogo.
* As seções &quot;Preferências de instalação&quot; e &quot;Propriedade de modelo&quot; na página de configuração foram combinadas em &quot;Preferências de modelo&quot; para simplificar.

Para obter mais informações, consulte [Configurar um blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Gerenciar associações de empresa com mais facilidade

Na área Empresas, uma barra de ferramentas atualizada facilita adicionar usuários existentes do Workfront a uma empresa e remover membros dela.

Anteriormente, essas ações estavam disponíveis somente na caixa Editar empresa.

A barra de ferramentas atualizada também contém todas as ações que estavam disponíveis na barra de ferramentas anterior, como editar as informações de perfil do usuário dos membros e desativá-las no sistema.

Para obter mais informações, consulte [Gerenciar associações de empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Selecionar expressões e campos na nova janela de campo calculado

Continuamos a facilitar a criação de um campo calculado em um formulário personalizado. Agora, ao clicar em Maximizar para abrir o novo Editor de Cálculo, você poderá localizar e selecionar as expressões e os campos necessários.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Os grupos podem configurar suas próprias preferências de horas e planilha de horas

>[!NOTE]
>
>Esse recurso estava disponível inicialmente como parte de uma implantação em fases somente para clientes no Cluster 4, como parte da versão 21.4. Esse recurso estará disponível para todos os clusters restantes na produção em 8 de novembro de 2021.

Em uma organização grande, alguns grupos podem precisar configurar preferências de horas e folha de horas de maneira independente para ajustar seus fluxos de trabalho exclusivos, em vez de herdar as preferências configuradas por um administrador no nível do sistema. Agora, os administradores do Workfront podem desbloquear uma folha de horas e uma preferência de horas para todos os grupos no sistema para que possam configurá-la sozinhos.

Essa capacidade também foi adicionada recentemente para preferências de projeto e para preferências de tarefas e problemas.

Para obter informações sobre como um administrador do Workfront desbloqueia uma folha de horas e uma preferência de horas, consulte a seção [Desbloquear preferências de folha de horas e horas para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) no artigo [Configurar preferências de folha de horas e horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obter informações sobre como um administrador de grupo configura preferências desbloqueadas de tarefas e problemas para um grupo, consulte [Configurar preferências de horas e folha de horas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Selecione várias notificações que você deseja desbloquear ou rebloquear para grupos

Agora ficou mais rápido e fácil desbloquear ou rebloquear notificações por email para grupos. Agora é possível selecionar várias notificações, verificar se as seleções estão corretas e clicar no novo botão Desbloquear ou Bloquear exibido na barra de ferramentas.

Anteriormente, era necessário desbloquear e rebloquear uma notificação por vez. No momento, o Workfront tem 95 notificações, portanto, isso demorou um pouco se você precisasse fazer isso para todas ou muitas delas.

Para obter mais informações, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Para administradores de grupo: É mais fácil selecionar um grupo de substituição ao excluir um grupo

Quando você está excluindo um grupo, duas melhorias na caixa Excluir grupo facilitam a seleção do grupo de substituição que você deseja preservar os usuários, itens de trabalho e subgrupos do grupo excluído:

* Você pode começar a digitar o nome do grupo para encontrá-lo rapidamente. Anteriormente, só havia uma lista suspensa que você não podia digitar. Isso era problemático para organizações com muitos grupos porque você tinha que percorrer a lista para encontrar o grupo desejado. Além disso, a lista suspensa tinha um limite de item, portanto, era possível que o grupo desejado não fosse exibido.
* Você pode usar o ícone de novas informações para se certificar de que está selecionando o grupo de substituição desejado. Passar o mouse sobre o ícone exibe uma dica de ferramenta listando informações sobre o grupo, como a hierarquia de grupos acima dele e os nomes dos administradores.

Para obter mais informações, consulte [Excluir um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Área maior para criar campos calculados

Agora é mais fácil criar campos calculados complexos em um formulário personalizado. Clique no novo botão Maximizar para abrir uma janela de edição grande para criar seu cálculo. Quando terminar, clique em Minimizar para continuar trabalhando no formulário personalizado.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Adicionar formulários personalizados aos grupos

Formulários personalizados agora são compatíveis com o objeto Grupo. Isso facilita a captura e o compartilhamento de informações por grupos em sua organização, de acordo com suas necessidades e fluxos de trabalho específicos. Os usuários podem fazer o seguinte para um grupo, da mesma forma que podem para outros objetos do Workfront:

* Criar um formulário personalizado
* Anexar um formulário personalizado
* Salvar dados do formulário personalizado
* Remover um formulário personalizado
* Edite dados personalizados em listas e, na nova experiência do Workfront, na página Grupo

Para obter informações sobre formulários personalizados, consulte [Formulários personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Criar aplicativos OAuth2 para integrar aplicativos ao Workfront

Agora é possível integrar o Workfront a outros aplicativos para os quais a Workfront não oferece uma integração integrada. Ao criar um aplicativo OAuth2 para o aplicativo que deseja integrar, é possível permitir que esse aplicativo acesse o Workfront, sabendo que seus dados estão protegidos pelo protocolo de autenticação OAuth2 seguro e padrão do setor.

Anteriormente, só era possível integrar o a outros aplicativos por meio de integrações integradas, do Workfront Fusion ou da API do Workfront.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Melhorias no texto da interface na área Empresas

Na área Empresas em Configuração, novas mensagens de confirmação e pequenas alterações de texto facilitam o gerenciamento de associações de empresas. Por exemplo, o nome de seção &quot;Pessoas&quot; no painel esquerdo agora é &quot;Membros da empresa&quot;.

Para obter informações sobre como gerenciar associações de empresa, consulte [Gerenciar associações de empresa](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
