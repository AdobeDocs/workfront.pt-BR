---
content-type: release-notes
navigation-topic: 2020-3-release-activity
title: 20.3 outras melhorias
description: Esta página descreve todos os outros aprimoramentos feitos com a versão 20.3 para o ambiente Produção. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 10 de agosto de 2020.
author: Luke
feature: Product Announcements
exl-id: 6fef7261-114f-4c26-861e-61a4acb22d40
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 0%

---

# 20.3 outras melhorias

Esta página descreve todos os outros aprimoramentos feitos com a versão 20.3 para o ambiente Produção. Esses aprimoramentos foram disponibilizados no ambiente de Produção na semana de 10 de agosto de 2020.

Para obter uma lista de todas as alterações disponíveis com a versão 20.3, consulte [Visão geral da versão 20.3](../../../product-announcements/product-releases/20.3-release-activity/20.3-release-overview.md).

## Compartilhar um calendário com um link privado

Para aliviar a carga do compartilhamento de calendários no Workfront, você pode compartilhar um link privado que leva os usuários diretamente para o calendário. O calendário deve ser compartilhado com o usuário e ele deve fazer logon para exibi-lo.

Anteriormente, você podia compartilhar um URL público que não precisava de um logon para visualizar.

Para obter mais informações, consulte [Compartilhar um relatório de calendário](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

## Nova área Rascunhos ao criar solicitações

Para proporcionar mais flexibilidade ao trabalhar com solicitações, o Workfront agora salva automaticamente todas as solicitações que você criar como rascunho na nova área Rascunhos . Se você não tiver todas as informações necessárias para concluir a nova solicitação, poderá deixá-la como rascunho, retornar a ela e finalizá-la posteriormente. O Workfront salva uma solicitação por tópico da fila na nova área Rascunhos . As solicitações de rascunho podem ser salvas enquanto você precisar delas até que esteja pronto para concluí-las e enviá-las. Também é possível remover ou reposicionar a área Rascunhos no painel esquerdo usando um Modelo de layout.

Para obter mais informações sobre como criar solicitações, consulte [Criar e enviar solicitações do Workfront](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

>[!NOTE]
>
>Na versão de Visualização, se você tiver um Modelo de layout personalizado atribuído a você, será necessário adicionar a área Rascunhos das suas Solicitações modificando seu Modelo de layout.

## Expandir ou recolher itens na folha de horas

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Para ajudá-lo a gerenciar facilmente as folhas de horas com vários itens, agora é possível expandir ou recolher todos os itens com o clique de um botão.

Anteriormente, você tinha que clicar em cada item individualmente.

Para obter mais informações, consulte [Tempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ignorar datas reais em calendários do Workfront

>[!NOTE]
>
>Esse recurso foi lançado no ambiente de visualização em 5 de junho de 2020. Ele estará disponível no ambiente de Produção em 19 de junho de 2020.

Para obter mais controle sobre como os objetos são exibidos nos Relatórios de calendário, é possível optar por ignorar as datas reais mesmo quando elas estiverem disponíveis.

Anteriormente, o calendário usava automaticamente as Datas reais assim que estivessem disponíveis.

Para obter mais informações, consulte [Visão geral dos relatórios de calendário](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

## Usar campos de data personalizados em relatórios de calendário

>[!NOTE]
>
>Esse recurso foi lançado no ambiente de visualização em 29 de maio de 2020. Ele estará disponível no ambiente de Produção em 12 de junho de 2020.

Para ajudá-lo a visualizar e gerenciar melhor seu trabalho diário com calendários, campos de data personalizados agora estão disponíveis como uma opção de data.

Anteriormente, você podia gerenciar seu calendário somente com datas projetadas, planejadas quando as datas reais não estavam disponíveis.

Para obter mais informações, consulte [Usar campos de data personalizados em um relatório de calendário](../../../reports-and-dashboards/reports/calendars/use-custom-dates.md) (ou se estiver usando o Workfront Classic, consulte [Usar campos de data personalizados em um relatório de calendário](https://one.workfront.com/s/article/Use-custom-date-fields-in-a-calendar-report-432597950?language=en_US)).

## Alterações de email

**Alterações no email de saída:** Todos os emails do Workfront virão de notifications@my.workfront.com. Isso inclui alertas automatizados e comunicação usuário-usuário.

Anteriormente, os administradores do sistema podiam adicionar um endereço de email personalizado na área Configuração de email .

**Alterações na resposta POP do email de entrada:** Os administradores do sistema não terão mais a capacidade de configurar um servidor de email POP personalizado para respostas de email recebidas a notificações.

Para obter mais informações, consulte [Falsificação de email e alterações de email de resposta POP](https://one.workfront.com/s/article/Email-spoofing-and-POP-reply-email-changes?language=en_US).

## DomainKeys Identified Mail (DKIM) agora incluído nos emails de saída do Workfront

Uma técnica de autenticação de email (DKIM) será incluída em todos os emails de saída. Essa assinatura DKIM não é visível para o usuário final, mas permite a validação em nível de servidor e reforça nossa estrutura de autenticação existente.

## Atualizações para inscrição na nova experiência do Workfront

Para tornar a inscrição de usuários na nova experiência do Workfront mais gerenciável, os administradores de grupo agora têm acesso para inscrever e cancelar a inscrição de usuários que pertencem aos grupos que gerenciam.

Agora também há um link Detalhes do usuário que exibe as seguintes informações do usuário:

* Nome
* Função
* Endereço de email
* Imagem do perfil

## Novo para administradores: Workfront de marca para grupos, equipes, funções e usuários específicos

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

Agora você pode usar um Modelo de layout para alterar os logotipos na área de navegação superior e no Menu principal para grupos específicos, equipes, funções de trabalho e usuários que possuem sua própria marca.

Para obter mais informações, consulte [Marca sua instância do Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

## Os administradores de grupo podem criar e gerenciar processos de aprovação

Para permitir mais autonomia e controle dos fluxos de trabalho de seus grupos, um Administrador de grupo agora pode acessar a área Processo de aprovação em Configurar e criar e editar processos de aprovação para um grupo que ele gerencia. Esses processos de aprovação são baseados nos status desse grupo.

Para garantir que os administradores de grupo não editem inadvertidamente os processos de aprovação que são usados em todo o sistema ou que são criados por outros grupos, eles podem acessar apenas os processos de aprovação associados aos grupos que gerenciam.

Para obter mais informações, consulte [Criar um processo de aprovação para itens de trabalho](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## Para administradores: A página Novos grupos facilita a criação e o gerenciamento de grupos

Os administradores de grupo podem gerenciar grupos mais facilmente, agora que tudo o que eles precisam está na nova página Grupos . Não é mais necessário navegar entre várias caixas de sobreposição e páginas de Configuração para criar e modificar grupos.

Estes são os principais destaques:

* Detalhes do grupo: Exiba e edite informações básicas sobre o grupo, como o nome do grupo, a descrição, os nomes dos administradores do grupo e se o grupo é público ou privado.
* Lista de membros do grupo: Visualize todos os membros do grupo e use a nova barra de ferramentas para adicionar, remover, exportar, ativar e desativar rapidamente as associações. Também é possível editar os perfis dos membros e enviar comentários de atualização a eles.
* Campo Administrador de grupo no cabeçalho: Ao visualizar um grupo que você gerencia, atribua ou cancele a atribuição rápida de um membro do grupo como administrador do grupo. Também é possível fazer isso na lista de membros do grupo usando a nova coluna Função do grupo .
* Lista de subgrupos: Exiba, edite, copie, exporte e exclua os subgrupos em um grupo que você gerencia.
* Lista de status: Visualize e gerencie os status do seu grupo.

Para obter mais informações, consulte [Criar um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

## Novo para administradores: Criar até 14 níveis de subgrupos

Para facilitar a organização dos grupos da Workfront para corresponder à hierarquia da organização, aumentamos os níveis de subgrupos que podem ser criados em um grupo de 3 para 14.

Para obter mais informações, consulte [Visão geral dos grupos](../../../administration-and-setup/manage-groups/groups-overview/groups.md).

## Novo para administradores: Nova barra lateral de configuração

>[!NOTE]
>
>Esse recurso está disponível somente na nova experiência do Adobe Workfront

A barra lateral esquerda em Configurar agora é mais rápida e fácil de usar e aproveita o layout básico e a funcionalidade que você já conhece. Juntamente com uma aparência mais moderna, aqui está o que mais é novo:

* Um novo fundo off-branco na barra lateral facilita a diferenciação do restante da área de configuração.
* Os ícones na barra lateral são um pouco maiores e alguns são reprojetados para sugerir mais claramente o que a opção faz.
* Mais espaço vertical entre itens da barra lateral facilita a leitura.
* Você pode recolher a barra lateral quando precisar de espaço na área principal para ver e fazer mais, como visualizar colunas adicionais. E você pode expandir a barra lateral novamente quando precisar ver os nomes dos recursos.
* Enquanto a barra lateral é recolhida, você vê apenas os ícones para cada recurso. Para ver os subitens em um item principal da barra lateral, passe o mouse sobre seu ícone para exibi-los em um menu flutuante. Por exemplo, passe o mouse sobre o ícone Processos para exibir um menu contendo Aprovações e Caminhos de marcos.
* Você pode acessar as duas opções de Início rápido (Importar dados e Exportar dados) com um clique mais rápido. Eles saíram de System para exibir o nível principal da barra lateral.

Para obter informações sobre como usar a área Configuração, consulte [Administração e configuração](../../../administration-and-setup/administration-and-setup.md).

## Incluir o número do cluster na área Informações do cliente

Como administrador do Workfront, agora é possível encontrar facilmente o número do cluster dentro do Workfront, sem precisar gastar mais tempo e esforço para obtê-lo da nossa equipe de suporte. Adicionamos um campo Configuração de cluster na área Informações do cliente da Configuração.

Para obter informações sobre a área Informações do cliente , consulte [Configurar informações básicas para seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

## Codificação Base64 para assinaturas de evento

O campo base64Encoding é um campo opcional usado para habilitar a codificação Base64 de cargas de assinatura de evento. Se uma solicitação for feita usando o campo base64Encoding definido como true, os objetos newState e oldState na carga útil serão entregues como strings de codificação Base64. Esse recurso pode ser útil se sua rede estiver configurada de modo que não permita caracteres especiais em Assinaturas de eventos.

Para obter mais informações, consulte [API de assinatura de evento](../../../wf-api/general/event-subs-api.md).

## Remoção da capacidade de criar Assinaturas de Evento duplicadas

Para evitar o delivery de mensagens duplicadas, não é mais possível criar assinaturas duplicadas. Além disso, as assinaturas duplicadas criadas anteriormente foram removidas.

Para obter mais informações, consulte [Perguntas frequentes - Assinaturas de eventos](../../../wf-api/general/event-subs-faq.md).
