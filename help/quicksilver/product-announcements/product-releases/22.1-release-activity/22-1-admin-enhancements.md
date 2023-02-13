---
title: 2.1 Aprimoramentos do administrador
description: 2.1 Aprimoramentos do administrador
author: Luke
draft: Probably
feature: Product Announcements, System Setup and Administration
exl-id: 63ff1334-aebe-4df4-a855-10011707808b
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 0%

---

# 2.1 Aprimoramentos do administrador

Esta página descreve todas as melhorias do Administrador feitas com a versão 2.1 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente Produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 17 de janeiro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.1, consulte [Visão geral da versão 2.1](../../../product-announcements/product-releases/22.1-release-activity/22-1-release-overview.md).

## Downloads de documentos conectados na área Atualizações

Para ajudar seus usuários a rastrear downloads de documentos que eles armazenam no Workfront, o sistema agora registra uma entrada na área Atualizações de um documento quando alguém a baixa.

>[!NOTE]
>
>Recomendamos testar esse recurso em Visualizar em um documento recém-carregado.

Para obter informações sobre como o Workfront registra atualizações automáticas em objetos, consulte [Atualizações controladas pelo sistema](../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md).

## Conceder acesso a equipes usando níveis de acesso

Uma nova seção na área Níveis de acesso oferece controles mais granulares para gerenciar o acesso dos usuários às equipes. Agora você pode determinar quem pode criar, editar e exibir equipes.

Isso não altera o acesso existente dos usuários às equipes.

<!--
For more information, see [Grant access to teams](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md).
-->

## O mapeamento de grupo agora está disponível em blueprints

Alguns blueprints agora incluem grupos, que você pode personalizar antes de instalar o blueprint. Você pode mapear um grupo no blueprint para um grupo existente na sua instância do Workfront ou criar um novo grupo, se necessário.

Para obter mais informações, consulte [Configurar um blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Atualizações de estilo na área Forms personalizado

A área Forms personalizada tem uma nova aparência que a atualiza com muitas outras áreas da nova experiência do Workfront.

Para obter informações sobre como criar um formulário personalizado, consulte [Criar ou editar um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Várias melhorias para criar campos personalizados calculados

A criação de campos personalizados calculados agora é muito mais fácil com essas adições no novo Editor de Cálculo:

* Você pode passar o mouse sobre qualquer expressão no cálculo para exibir informações sobre ela, incluindo uma descrição, um exemplo de como ela pode ser usada e um link para mais informações em um artigo de ajuda.
* Cada expressão adicionada é codificada por cores, dependendo do tipo. Isso facilita detectar suas expressões e reconhecer imediatamente seu tipo.
* Os números de linha ajudam a identificar e referenciar funções em um cálculo longo.
* Quando você começa a digitar uma expressão ou um nome de campo, uma lista de itens disponíveis é exibida para que você possa escolher o que deseja. E, ao digitar um parênteses aberto, o parênteses de fechamento é adicionado automaticamente.
* Você pode visualizar o resultado do cálculo usando um objeto existente sem sair do editor de cálculo.

Além disso, no texto personalizável do mouse &quot;Instruções&quot; para um campo personalizado calculado, é possível exibir ou ocultar a fórmula do campo. Isso é útil se você achar que os usuários que preencherão o formulário personalizado não precisarão dessas informações.

Para obter mais informações sobre como criar um campo personalizado calculado, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Exibir informações de log de auditoria sobre status e empresas

Agora é possível solucionar problemas de incidentes envolvendo status e empresas mais facilmente, visualizando informações sobre eles na área Logs de auditoria em Configurar.

Por exemplo:

* Você pode descobrir quem renomeou, bloqueou ou ocultou um status e quando o fizeram.
* Você pode descobrir quem removeu alguns membros ou funções de trabalho de uma empresa e quando eles o fizeram.

Para obter informações sobre a exibição de informações de log de auditoria, consulte [Exibir e exportar logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Mapeamento de empresas do Blueprints e outras melhorias

Os seguintes aprimoramentos de Blueprints já estão disponíveis:

* Alguns blueprints agora incluem empresas, que você pode personalizar antes de instalar o blueprint. Você pode mapear uma empresa no blueprint para uma empresa existente na sua instância do Workfront ou criar uma nova empresa, se necessário.
* Um novo tipo de blueprint, Estrutura Organizacional, está disponível. Alguns blueprints incluem elementos de vários tipos (por exemplo, Modelo de projeto e Estrutura organizacional). Você pode filtrar por tipo de blueprint na página do catálogo.
* As seções &quot;Preferências de instalação&quot; e &quot;Propriedade de modelo&quot; na página de configuração foram combinadas em &quot;Preferências de modelo&quot; para simplificar.

Para obter mais informações, consulte [Configurar um blueprint](../../../administration-and-setup/blueprints/configure-template-package.md).

## Gerenciar associações de empresas com mais facilidade

Na área Empresas , uma barra de ferramentas atualizada facilita a adição de usuários existentes do Workfront a uma empresa e a remoção de membros da empresa.

Anteriormente, essas ações estavam disponíveis somente na caixa Editar empresa .

A barra de ferramentas atualizada também contém todas as ações que estavam disponíveis na barra de ferramentas anterior, como editar as informações de perfil do usuário dos membros e desativá-las no sistema.

Para obter mais informações, consulte [Gerenciar associações de empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).

## Selecione expressões e campos na nova janela de campo calculado

Continuamos a facilitar a criação de um campo calculado em um formulário personalizado. Agora, ao clicar em Maximizar para abrir o novo Editor de cálculos, é possível encontrar e selecionar as expressões e os campos necessários.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Os grupos podem configurar suas próprias preferências de hora e de folha de ponto

>[!NOTE]
>
>Inicialmente, esse recurso estava disponível como parte de uma implantação em fases somente para clientes no Cluster 4 como parte da versão 21.4. Esse recurso estará disponível para todos os clusters restantes em Produção em 8 de novembro de 2021.

Em uma organização grande, alguns grupos podem precisar configurar as preferências de hora e folha de ponto de modo independente para se adequar aos fluxos de trabalho exclusivos, em vez de herdar as preferências configuradas por um administrador no nível do sistema. Agora, os administradores do Workfront podem desbloquear uma folha de ponto e uma preferência de hora para todos os grupos no sistema, para que possam configurá-la sozinhos.

Essa capacidade também foi adicionada recentemente para preferências de projeto e para preferências de tarefa e emissão.

Para obter informações sobre como um administrador do Workfront desbloqueia uma folha de ponto e uma preferência de hora, consulte a seção [Desbloquear folha de horas e preferências de hora para grupos](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md#lock) no artigo [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

Para obter informações sobre como um administrador de grupo configura a tarefa desbloqueada e emite preferências para um grupo, consulte [Configurar as preferências de hora e folha de ponto para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

## Selecione várias notificações que deseja desbloquear ou rebloquear para grupos

Agora é mais rápido e fácil desbloquear ou rebloquear notificações por email para grupos. Agora é possível selecionar várias notificações, verificar as seleções para certificar-se de que elas estão corretas e clicar no novo botão Desbloquear ou Bloquear , exibido na barra de ferramentas.

Anteriormente, era necessário desbloquear e rebloquear notificações uma de cada vez. No momento, a Workfront tem 95 notificações, então isso levou algum tempo se você tivesse que fazer isso para todas ou muitas delas.

Para obter mais informações, consulte [Desbloquear ou bloquear a configuração de notificações de eventos para todos os grupos](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

## Para administradores de grupo: É mais fácil selecionar um grupo de substituição ao excluir um grupo

Ao excluir um grupo, duas melhorias na caixa Excluir grupo facilitam a seleção do grupo de substituição que você deseja preservar os usuários, itens de trabalho e subgrupos do grupo excluído:

* Você pode começar a digitar o nome do grupo para encontrá-lo rapidamente. Anteriormente, havia apenas uma lista suspensa na qual não era possível digitar. Isso foi problemático para organizações com muitos grupos porque você tinha que rolar pela lista para encontrar o grupo que queria. Além disso, a lista suspensa tinha um limite de item, então era possível que o grupo desejado não fosse exibido.
* Você pode usar o novo ícone de informações para verificar se está selecionando o grupo de substituição desejado. Passar o mouse sobre o ícone exibe uma dica de ferramenta que lista informações sobre o grupo, como a hierarquia de grupos acima dele e os nomes de seus administradores.

Para obter mais informações, consulte [Excluir um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).

## Maior área para criar campos calculados

Agora é mais fácil criar campos calculados complexos em um formulário personalizado. Clique no novo botão Maximizar para abrir uma grande janela de edição para criar o cálculo. Quando terminar, clique em Minimizar para continuar trabalhando no formulário personalizado.

Para obter mais informações, consulte [Adicionar dados calculados a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

## Adicionar formulários personalizados a grupos

Os formulários personalizados agora são compatíveis com o objeto Grupo. Isso facilita que os grupos da organização capturem e compartilhem informações que atendam às necessidades e fluxos de trabalho específicos. Os usuários podem fazer o seguinte para um grupo, assim como para outros objetos Workfront:

* Criar um formulário personalizado
* Anexar um formulário personalizado
* Salvar dados de formulário personalizado
* Remover um formulário personalizado
* Editar dados personalizados em listas e, na nova experiência do Workfront, na página Grupo

Para obter informações sobre formulários personalizados, consulte [Formulários personalizados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-and-manage-custom-forms.md).

## Criar aplicativos OAuth2 para integrar aplicativos com o Workfront

Agora é possível integrar o Workfront com outros aplicativos para os quais a Workfront não oferece uma integração incorporada. Ao criar um aplicativo OAuth2 para o aplicativo com o qual você deseja integrar, você pode permitir que esse aplicativo acesse o Workfront, sabendo que seus dados estão protegidos pelo protocolo de autenticação OAuth2 seguro e padrão do setor.

Anteriormente, você só podia integrar com outros aplicativos por meio de integrações integradas, Workfront Fusion ou a API do Workfront.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../../../administration-and-setup/configure-integrations/create-oauth-application.md).

## Melhorias no texto da interface na área Empresas

Na área Empresas em Configurar, novas mensagens de confirmação e pequenas alterações de texto facilitam o gerenciamento de associações a empresas. Por exemplo, o nome da seção &quot;Pessoas&quot; no painel esquerdo agora é &quot;Membros da empresa&quot;.

Para obter informações sobre como gerenciar associações de empresas, consulte [Gerenciar associações de empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md).
