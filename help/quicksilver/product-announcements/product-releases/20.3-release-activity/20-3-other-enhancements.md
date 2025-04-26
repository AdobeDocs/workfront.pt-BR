---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 outras melhorias
description: Esta página descreve todas as outras melhorias feitas com a versão 20.3 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 10 de agosto de 2020.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1503'
ht-degree: 0%

---

# 20.3 outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 20.3 para o ambiente de Produção. Essas melhorias foram disponibilizadas no ambiente de Produção na semana de 10 de agosto de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.3, consulte a [visão geral da versão 20.3](../../../product-announcements/product-releases/20.3-release-activity/20-3-release-overview.md).

## Compartilhar um calendário com um link privado

Para aliviar a carga do compartilhamento de calendários no Workfront, você pode compartilhar um link privado que leva os usuários diretamente para o calendário. O calendário deve ser compartilhado com o usuário, que precisa fazer logon para visualizá-lo.

Anteriormente, você podia compartilhar um URL público que não exigia um logon para exibição.

Para obter mais informações, consulte [Compartilhar um relatório de calendário](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Nova área Rascunhos ao criar solicitações

Para oferecer mais flexibilidade ao trabalhar com solicitações, o Workfront salva automaticamente cada solicitação criada como rascunho na nova área Rascunhos. Se você não tiver todas as informações necessárias para concluir a nova solicitação, poderá deixá-la como rascunho, voltar para ela e concluí-la posteriormente. O Workfront salva uma solicitação por tópico da fila na nova área Rascunhos. Os rascunhos de solicitações podem ser salvos pelo tempo necessário até que você esteja pronto para concluí-los e submetê-los. Também é possível remover ou reposicionar a área Rascunhos no painel esquerdo usando um Modelo de layout.

Para obter mais informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Para a versão de Pré-visualização, se você tiver um Modelo de layout personalizado atribuído, será necessário adicionar a área Rascunhos das solicitações modificando o Modelo de layout.

## Expandir ou recolher itens na folha de horas

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Para ajudá-lo a gerenciar facilmente folhas de horas com vários itens, agora você pode expandir ou recolher todos os itens com apenas um clique.

Anteriormente, você tinha que clicar em cada item individualmente.

Para obter mais informações, consulte [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignorar Datas Reais nos Calendários do Workfront

>[!NOTE]
>
>Esse recurso foi lançado no ambiente de Pré-visualização em 5 de junho de 2020. Ele estará disponível no ambiente de Produção em 19 de junho de 2020.

Para ter mais controle sobre como os objetos são exibidos nos Relatórios de calendário, você pode optar por ignorar as datas reais mesmo quando elas estiverem disponíveis.

Anteriormente, o calendário usaria automaticamente as Datas efetivas quando estivessem disponíveis.

Para obter mais informações, consulte [Visão geral dos relatórios do calendário](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Usar campos de data personalizados em relatórios de calendário

>[!NOTE]
>
>Esse recurso foi lançado no ambiente de Pré-visualização em 29 de maio de 2020. Ele estará disponível no ambiente de Produção em 12 de junho de 2020.

Para ajudá-lo a visualizar e gerenciar melhor seu trabalho diário com calendários, agora os campos de data personalizados estão disponíveis como uma opção de data.

Anteriormente, só era possível gerenciar o calendário com datas projetadas e planejadas quando não havia datas reais disponíveis.

Para obter mais informações, consulte [Usar campos de data personalizados em um relatório de calendário](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (ou se estiver usando o Workfront Classic, consulte [Usar campos de data personalizados em um relatório de calendário](https://experienceleague.adobe.com/en/docs/workfront/using/home)).

## Alterações no email

**Alterações nos emails de saída:** Todos os emails do Workfront serão provenientes de notifications@my.workfront.com. Isso inclui alertas automatizados e comunicação entre usuários.

Anteriormente, os administradores do sistema podiam adicionar um endereço de email personalizado na área Configuração de email.

**Alterações de resposta POP de email de entrada:** Os administradores do sistema não poderão mais configurar um servidor de email POP personalizado para respostas de email de entrada a notificações.

Para obter mais informações, consulte [Alterações de email de resposta POP e falsificação de email](https://experienceleague.adobe.com/en/docs/workfront/using/home).

## O DomainKeys Identified Mail (DKIM) agora é incluído nos emails de saída do Workfront

Uma técnica de autenticação de email (DKIM) será incluída em todos os emails de saída. Essa assinatura do DKIM não é visível para o usuário final, mas permite a validação no nível do servidor e reforça nossa estrutura de autenticação existente.

## Atualizações da inscrição na nova experiência do Workfront

Para tornar a inscrição do usuário na nova experiência do Workfront mais gerenciável, os Administradores de grupo agora têm acesso para inscrever e cancelar a inscrição de usuários que pertencem aos grupos que gerenciam.

Agora também há um link Detalhes do usuário que exibe as seguintes informações do usuário:

* Nome
* Função de trabalho
* Endereço de email
* Imagem do perfil

## Novo para administradores: Workfront da marca para grupos, equipes, funções de trabalho e usuários específicos

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Agora é possível usar um Modelo de layout para alterar os logotipos na área de navegação superior e no Menu principal para grupos, equipes, funções de trabalho e usuários específicos que têm sua própria marca.

Para obter mais informações, consulte [Marcar sua instância do Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Os administradores de grupo podem criar e gerenciar processos de aprovação

Para permitir mais autonomia e controle dos fluxos de trabalho de seus grupos, um Administrador de grupo agora pode acessar a área Processo de aprovação em Configurar, criar e editar processos de aprovação para um grupo gerenciado por ele. Esses processos de aprovação se baseiam nos status desse grupo.

Para garantir que os Administradores de grupo não editem inadvertidamente os processos de aprovação usados em todo o sistema ou criados por outros grupos, eles podem acessar apenas os processos de aprovação associados aos grupos gerenciados.

Para obter mais informações, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Para administradores: a nova página Grupos facilita a criação e o gerenciamento de grupos

Os administradores de grupo podem gerenciar grupos mais facilmente, agora que tudo o que precisam está na nova página Grupos. Não é mais necessário navegar entre várias caixas de sobreposição e páginas de Configuração para criar e modificar grupos.

Estes são os principais destaques:

* Detalhes do Grupo: Exiba e edite informações básicas sobre o grupo, como nome do grupo, descrição, nomes dos Administradores do Grupo e se o grupo é público ou privado.
* Lista de membros do grupo: visualize todos os membros do grupo e use a nova barra de ferramentas para adicionar, remover, exportar, ativar e desativar associações rapidamente. Também é possível editar os perfis dos membros e enviá-los para Atualizar comentários.
* Campo Administrador do Grupo no cabeçalho: Quando estiver exibindo um grupo gerenciado, atribua ou cancele rapidamente a atribuição de um membro do grupo como administrador do grupo. Também é possível fazer isso na lista de membros do grupo usando a nova coluna Função do grupo.
* Lista de subgrupos: exibir, editar, copiar, exportar e excluir os subgrupos de um grupo gerenciado por você.
* Lista de status: exibe e gerencia os status do seu grupo.

Para obter mais informações, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Novo para administradores: criar até 14 níveis de subgrupos

Para facilitar a organização dos grupos do Workfront para corresponder à hierarquia da organização, aumentamos os níveis de subgrupos que você pode criar em um grupo de 3 para 14.

Para obter mais informações, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Novo para administradores: nova barra lateral de instalação

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

A barra lateral esquerda em Configuração agora é mais rápida e fácil de usar e aproveita o layout básico e a funcionalidade que você já conhece. Junto com uma aparência mais moderna, veja o que há de novo:

* Um novo fundo fora de branco na barra lateral facilita a diferenciação do restante da área de Configuração.
* Os ícones na barra lateral são um pouco maiores e alguns são reprojetados para sugerir com mais clareza o que a opção faz.
* Mais espaço vertical entre os itens da barra lateral facilita a leitura.
* Você pode recolher a barra lateral quando precisar de espaço na área principal para ver e fazer mais, como visualizar colunas adicionais. E você pode expandir a barra lateral novamente quando precisar ver nomes de recursos.
* Enquanto a barra lateral estiver recolhida, você verá apenas os ícones de cada recurso. Para ver os subitens sob um item da barra lateral principal, passe o mouse sobre o ícone para exibi-los em um menu suspenso. Por exemplo, passe o mouse sobre o ícone Processos para exibir um menu contendo Aprovações e Caminhos de Etapas.
* Você pode acessar as duas opções de Kick-Starts (Importar dados e Exportar dados) com um clique mais rápido. Eles foram movidos do sistema para exibir no nível principal da barra lateral.

Para obter informações sobre como usar a área Instalação, consulte [Administração e configuração](../../../administration-and-setup/administration-and-setup.md).

## Incluir número de cluster na área Informações do Cliente

Como administrador do Workfront, agora é possível encontrar facilmente o número do cluster dentro do Workfront, sem precisar gastar tempo e esforço adicionais para obtê-lo da nossa equipe de suporte. Adicionamos um campo Configuração do cluster na área Informações do cliente da Configuração.

Para obter informações sobre a área Informações do cliente, consulte [Configurar informações básicas do sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Codificação Base64 para Assinaturas de Evento

O campo base64Encoding é um campo opcional usado para habilitar a codificação Base64 de cargas de assinatura de evento. Se uma solicitação for feita usando o campo base64Encoding definido como true, os objetos newState e oldState na carga serão entregues como strings de codificação Base64. Esse recurso pode ser útil se sua rede estiver configurada de forma a não permitir caracteres especiais em Assinaturas de eventos.

Para obter mais informações, consulte [API de Assinatura de Evento](../../../wf-api/general/event-subs-api.md).

## Remoção da capacidade de criar Assinaturas de Eventos duplicadas

Para impedir a entrega de mensagens duplicadas, não é mais possível criar assinaturas duplicadas. Além disso, as assinaturas duplicadas criadas anteriormente foram removidas.

Para obter mais informações, consulte [Perguntas frequentes - Assinaturas de Eventos](../../../wf-api/general/event-subs-faq.md).
