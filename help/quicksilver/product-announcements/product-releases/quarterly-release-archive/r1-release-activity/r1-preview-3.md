---
content-type: release-notes
navigation-topic: product-releases-archive
title: Visualização 3 do R1
description: Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão R1.3. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 1 de fevereiro de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '1347'
ht-degree: 2%

---

# Visualização 3 do R1

Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão R1.3. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 1 de fevereiro de 2017.

Para obter uma lista de todas as alterações feitas no R1, consulte [Visão geral da atividade de versão R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Método aprimorado para vinculação de arquivos externos

A opção para vincular documentos de uma fonte externa (como Google Drive, Box, Dropbox e assim por diante) agora está em um local mais proeminente na área Documentos. 

Além disso, a ação de autorizar um provedor de documentos antes de vincular arquivos desse provedor pela primeira vez agora é mais intuitiva (é simplesmente uma etapa extra ao vincular arquivos de um provedor externo).

Antes dessas alterações, a opção para vincular arquivos de uma origem externa estava localizada na caixa de diálogo Adicionar documentos na área Documentos. Antes de vincular um documento de uma fonte externa pela primeira vez, o usuário que vincula o documento tinha que autorizar esse provedor de documentos na área Configuração.

Para obter mais informações, consulte  [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Calendário de trabalho da equipe atualizado

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

O calendário de Trabalho em disponível para equipes agora contém funcionalidades adicionais e uma aparência atualizada. O calendário da equipe de Trabalho em agora funciona de forma semelhante à ferramenta de agendamento de recursos para projetos.

O calendário de Trabalho em equipe atualizado inclui as seguintes melhorias:

* Exibir usuários em ordem alfabética ou agrupados por função.
* Filtre a linha do tempo de agendamento por prioridades de projeto, status e projetos individuais. Também é possível filtrar a linha do tempo de agendamento por funções e usuários. (A área Filtro inclui menos opções do que ao agendar recursos para projetos.)
* Incluir problemas na linha do tempo do agendamento.
* Exibir alocações de usuários e modificar o número de horas que os usuários são alocados para determinadas tarefas e problemas para cada dia.
* Visualize indicadores que mostram quando os usuários estão superalocados em um determinado dia.
* Configure se o trabalho concluído será exibido na linha do tempo do agendamento.

Diferenças da ferramenta de agendamento de recursos ao agendar recursos para projetos:

* Todos os membros da equipe são exibidos no calendário de Trabalho em equipe.\
  Ao agendar recursos para projetos, somente os usuários que têm uma função associada a eles que corresponde a uma função de uma ou mais tarefas na área Não atribuído são exibidos.
* A ferramenta de troca não está disponível e não está incluída no calendário de Trabalho em equipe.
* Qualquer membro da equipe pode fazer alterações no calendário de Trabalho em equipe.\
  Ao agendar recursos para projetos, somente os Gerentes de recursos podem tomar decisões de recursos para o projeto.
* Os problemas são exibidos por padrão no calendário de Trabalho em equipe.\
  Ao agendar recursos para projetos, os problemas não são exibidos por padrão.

Para obter mais informações sobre como usar o calendário de Trabalho em equipe atualizado, consulte &quot;Agendamento de recursos&quot;.

## Aprimoramentos de agendamento de recursos

A linha do tempo de agendamento inclui os seguintes aprimoramentos:

* &quot;Use o filtro para controlar quais usuários são exibidos na linha de tempo de agendamento&quot;
* &quot;Os usuários permanecem na linha do tempo depois de receberem uma tarefa&quot;

### Use o filtro para controlar quais usuários são exibidos na linha de tempo do agendamento {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

O filtro agora pode ser usado para controlar quais usuários são exibidos na linha do tempo do agendamento, além de quais tarefas e problemas são exibidos na área Não atribuído. Quando os usuários são selecionados no filtro, somente os usuários selecionados são exibidos, independentemente de terem ou não uma atribuição de função que corresponda à atribuição de função de tarefas na área Não atribuído. Todas as tarefas atualmente atribuídas a esse usuário também são exibidas.

Antes dessa alteração, o filtro controlava apenas quais tarefas e problemas eram exibidos na área Não atribuído. Os usuários eram exibidos na linha do tempo do agendamento somente se o usuário correspondesse à atribuição de função de uma tarefa na área Não atribuído.

Para obter mais informações sobre como usar o filtro para controlar o que é exibido na linha do tempo do agendamento, consulte &quot;Filtrar informações na área Agendamento&quot; e &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

### Os usuários permanecem na linha do tempo depois de receberem uma tarefa {#users-remain-on-the-timeline-after-being-assigned-a-task}

Os usuários permanecem na linha do tempo de agendamento depois de receberem uma tarefa ou problema, mesmo se não houver tarefas ou problemas restantes com uma atribuição de função correspondente. Isso permite fazer as alterações necessárias depois que os usuários são atribuídos.

Antes dessa alteração, os usuários desapareceriam da linha do tempo do agendamento imediatamente após receberem uma tarefa ou problema se não houvesse tarefas ou problemas restantes na área Não atribuído com uma atribuição de função correspondente.

Para obter mais informações, consulte &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

## Personalizar a terminologia do Workfront alterando os nomes de objetos

Agora é possível personalizar a terminologia do Workfront alterando os nomes de determinados objetos.\
Usando um Modelo de layout, agora é possível alterar os nomes dos seguintes objetos de trabalho para atender às necessidades na organização:

* Portfólio
* Programa
* Projeto
* Tarefa
* Problema

Por exemplo, se em sua organização você trabalha com campanhas em vez de projetos, é possível substituir o nome do objeto &quot;Projeto&quot; por &quot;Campanha&quot;.

Quando você faz essa substituição, as seguintes áreas do aplicativo mostram o nome atualizado dos objetos:

* Barra de navegação global
* Todas as guias
* Todos os menus 
* Elementos do Report Builder e de relatórios (exibições, filtros e agrupamentos)
* Botões Salvar
* Arquivos exportados
* Emails

As áreas a seguir não mostram o nome atualizado dos objetos:

* Estimativas de Recursos
* Gerenciador de Estimativa de Recursos
* Planejador de Capacidade
* Grade de Recursos
* Construtor de Equipe
* Otimizador de Portfolio 
* Aplicativos móveis
* Suplemento do Outlook

Para obter mais informações sobre como personalizar a terminologia do Workfront usando um Modelo de Layout, consulte a seção &quot;Personalizando Terminologia&quot; em &quot;Criando e Gerenciando Modelos de Layout&quot; e a seção &quot;Entendendo as Implicações da Personalização de Nomes de Objeto&quot; em [Entender objetos no Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Incluir datas de início e término da aprovação em relatórios

Agora você pode incluir os seguintes campos ao criar ou modificar relatórios:

* Data de início do caminho de aprovação
* Data de conclusão do caminho de aprovação

Esses campos permitem ter informações sobre quando o caminho de aprovação atual ou mais recente foi iniciado e quando foi marcado como Concluído.

Para obter mais informações sobre esses campos, consulte [Glossário da terminologia do Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Para obter mais informações sobre caminhos de aprovação, como eles são criados e acionados e a função que desempenham nos processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Os seguintes campos foram removidos do Workfront e não podem mais ser incluídos nos relatórios (esses campos forneceram informações sobre o projeto em vez de informações sobre as próprias aprovações e foram frequentemente usados incorretamente):

* Data de início planejada das aprovações
* Data de início projetada para aprovação
* Data estimada de início da aprovação

## Novas opções de resumo de email para &quot;Solicitações que fiz&quot;

A opção de entrega de Resumo diário foi adicionada à área &quot;Solicitações que fiz&quot; das configurações de Notificações.

Para obter mais informações, consulte [Modificar suas próprias notificações por email](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Lembre-se de atualizar o endereço de email associado à sua conta para testar essa funcionalidade. Isso é necessário porque a Sandbox de visualização apaga os endereços de email de todos os usuários.

## Notificações por email sobre a aparência e a aprovação de documentos atualizadas

A aparência da notificação para &quot;Aprovação de documento&quot; foi atualizada com uma nova interface:

Para obter mais informações sobre notificações por email, consulte [Notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Lembre-se de atualizar o endereço de email associado à sua conta para testar essa funcionalidade. Isso é necessário porque a Sandbox de visualização apaga os endereços de email de todos os usuários.

## Melhorias na visualização de Marco

A visualização de Marco disponível ao visualizar uma lista de projeto ou relatório de projeto agora contém as seguintes melhorias:

* As datas planejadas são editáveis
* O Percentual concluído para projetos e tarefas é exibido

Antes dessa alteração, para editar as datas ou exibir o percentual concluído, você tinha que ir para a tarefa individual.

Para obter mais informações, consulte [Usar a visualização de Etapas](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
