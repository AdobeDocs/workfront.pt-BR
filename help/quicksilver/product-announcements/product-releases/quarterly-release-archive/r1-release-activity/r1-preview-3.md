---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Pré-visualização 3
description: Esta página descreve todas as alterações disponíveis no ambiente de Visualização com a versão R1.3. A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 1 de fevereiro de 2017.
author: Luke
feature: Product Announcements
exl-id: d1502a17-b131-4d29-9b0c-03ad44be4ba6
source-git-commit: f4cc5ae89c8746ec4c40ece88bfdb21dc1996575
workflow-type: tm+mt
source-wordcount: '1345'
ht-degree: 2%

---

# R1 Pré-visualização 3

Esta página descreve todas as alterações disponíveis no ambiente de Visualização com a versão R1.3. A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 1 de fevereiro de 2017.

Para obter uma lista de todas as alterações feitas em R1, consulte [Visão geral da atividade de versão do R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md). 

## Método aprimorado para vinculação de arquivos externos

A opção para vincular documentos de uma fonte externa (como Google Drive, Box, Dropbox e assim por diante) agora está em um local mais proeminente na área Documentos. 

Além disso, a ação de autorizar um provedor de documentos antes de vincular arquivos desse provedor pela primeira vez agora é mais intuitiva (é apenas uma etapa extra ao vincular arquivos de um provedor externo).

Antes dessas alterações, a opção de vincular arquivos de uma fonte externa estava localizada na caixa de diálogo Adicionar documentos na área Documentos . Antes de vincular um documento de uma fonte externa pela primeira vez, o usuário que vincula o documento tinha que autorizar esse provedor de documentos na área Configuração.

Para obter mais informações, consulte  [Vincular documentos de aplicativos externos](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

## Equipe Atualizada Trabalhando No Calendário

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram descontinuadas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de Carga de Trabalho, consulte [Visão Geral do Balanceador de Carga de Trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

O calendário Trabalhar no , disponível para equipes, agora contém funcionalidades adicionais e uma aparência atualizada. O calendário Trabalho em equipe agora funciona de forma semelhante à ferramenta de agendamento de recursos para projetos.

A equipe atualizada Trabalhando no calendário inclui as seguintes melhorias:

* Exibir usuários em ordem alfabética ou agrupados por função.
* Filtre a linha do tempo de programação por prioridades do projeto, status e projetos individuais. Também é possível filtrar a linha do tempo de agendamento por funções e usuários. (A área Filtro inclui menos opções do que ao agendar recursos para projetos.)
* Inclua problemas na linha do tempo do agendamento.
* Exiba alocações de usuários e modifique o número de horas que os usuários são alocados para determinadas tarefas e problemas para cada dia.
* Exibir indicadores que mostram quando os usuários estão alocados em excesso em um determinado dia.
* Configure se o trabalho concluído é exibido na linha do tempo de agendamento.

Diferenças da ferramenta de agendamento de recursos ao agendar recursos para projetos:

* Todos os membros da equipe são exibidos no calendário Trabalhando da equipe.\
   Ao agendar recursos para projetos, somente os usuários que têm uma função associada a eles que corresponda a uma função de uma ou mais tarefas na área Não atribuído são exibidos.
* A ferramenta Trocar não está disponível não está incluída no calendário Trabalhar em equipe.
* Qualquer membro da equipe pode fazer alterações no calendário Trabalhando na equipe.\
   Ao programar recursos para projetos, somente os Gerentes de Recursos podem tomar decisões de recursos para o projeto.
* Os problemas são exibidos por padrão no calendário Trabalhando da equipe.\
   Ao programar recursos para projetos, os problemas não são exibidos por padrão.

Para obter mais informações sobre como usar a equipe atualizada no calendário, consulte &quot;Agendamento de recursos&quot;.

## Aprimoramentos no agendamento de recursos

A linha do tempo de programação inclui as seguintes melhorias:

* &quot;Use o filtro para controlar quais usuários são exibidos na linha do tempo do agendamento&quot;
* &quot;Os usuários permanecem na linha do tempo depois de receber uma tarefa&quot;

### Usar o filtro para controlar quais usuários são exibidos na linha do tempo de agendamento {#use-the-filter-to-control-which-users-are-displayed-on-the-scheduling-timeline}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram descontinuadas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de Carga de Trabalho, consulte [Visão Geral do Balanceador de Carga de Trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

O filtro agora pode ser usado para controlar quais usuários são exibidos na linha do tempo do agendamento, além de quais tarefas e problemas são exibidos na área Não atribuído. Quando os usuários são selecionados no filtro, somente os usuários selecionados são exibidos, independentemente de terem uma atribuição de função que corresponda à atribuição de função de tarefas na área Não atribuído. Todas as tarefas atribuídas a esse usuário também são exibidas.

Antes dessa alteração, o filtro controlava somente quais tarefas e problemas eram exibidos na área Não atribuído. Os usuários eram exibidos na linha do tempo de agendamento somente se o usuário correspondesse à atribuição de função de uma tarefa na área Não atribuído.

Para obter mais informações sobre como usar o filtro para controlar o que é exibido na linha do tempo de agendamento, consulte &quot;Filtrar informações na área Agendamento&quot; e &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de Agendamento&quot;.

### Os usuários permanecem na linha do tempo depois de receberem uma tarefa {#users-remain-on-the-timeline-after-being-assigned-a-task}

Os usuários permanecem na linha do tempo de agendamento depois de receberem uma tarefa ou um problema, mesmo que não haja tarefas ou problemas restantes que tenham uma atribuição de função correspondente. Isso permite fazer as alterações necessárias após a atribuição dos usuários.

Antes dessa alteração, os usuários desapareciam da linha do tempo de agendamento imediatamente depois de receberem uma tarefa ou problema se não houvesse tarefas ou problema restantes na área Não atribuído com uma atribuição de função correspondente.

Para obter mais informações, consulte &quot;Atribuir manualmente tarefas e problemas não atribuídos nas áreas de agendamento&quot;.

## Personalizar a terminologia do Workfront ao alterar os nomes dos objetos

Agora é possível personalizar a terminologia do Workfront alterando os nomes de determinados objetos.\
Usando um modelo de layout, agora é possível alterar os nomes dos seguintes objetos de trabalho para atender às necessidades em sua organização:

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
* Construtor de relatórios e elementos de relatório (exibições, filtros e agrupamentos)
* Botões Salvar
* Arquivos exportados
* Emails

As seguintes áreas não mostram o nome atualizado dos objetos:

* Estimativas de Recursos
* Gerenciador de Estimativa de Recursos
* Planejador de Capacidade
* Grade de Recursos
* Construtor de Equipe
* Portfolio Otimizer 
* Aplicativos móveis
* Suplemento do Outlook

Para obter mais informações sobre como personalizar a terminologia do Workfront usando um modelo de layout, consulte a seção &quot;Personalizando terminologia&quot; em &quot;Criação e gerenciamento de modelos de layout&quot; e a seção &quot;Noções básicas sobre como personalizar nomes de objetos&quot; em [Entender objetos no Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

## Incluir datas de início e término da aprovação em relatórios

Agora é possível incluir os seguintes campos ao criar ou modificar relatórios:

* Data de início do caminho de aprovação
* Data de conclusão do caminho de aprovação

Esses campos permitem ter informações sobre quando o caminho de aprovação atual ou mais recente foi iniciado e quando foi marcado como Concluído.

Para obter mais informações sobre esses campos, consulte [Glossário da terminologia do Adobe Workfront](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).

Para obter mais informações sobre caminhos de aprovação, como eles são criados e acionados e a função que eles servem nos processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Os seguintes campos foram removidos do Workfront e não podem mais ser incluídos nos relatórios (esses campos forneciam informações sobre o projeto em vez de informações sobre as próprias aprovações e eram frequentemente mal utilizados):

* Aprovações Data de Início Planejada
* Data de início projetada para aprovação
* Data estimada de início da aprovação

## Novas opções de resumo de email para &quot;Solicitações que fiz&quot;

A opção Daily Digest delivery foi adicionada à área &quot;Requests I Have&quot; das configurações de Notificações.

Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de evento](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Lembre-se de atualizar o endereço de email associado à sua conta para poder testar essa funcionalidade. Isso é necessário porque a sandbox de visualização limpa os endereços de email de todos os usuários.

## Atualização da aparência e do sentimento de notificações por email de aprovação de documentos

A aparência da notificação para &quot;Aprovação de documento&quot; foi atualizada com uma nova interface do usuário:

Para obter mais informações sobre notificações por email, consulte [Notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md).

Lembre-se de atualizar o endereço de email associado à sua conta para poder testar essa funcionalidade. Isso é necessário porque a sandbox de visualização limpa os endereços de email de todos os usuários.

## Melhorias na exibição de marco

A exibição de Marco, disponível ao visualizar uma lista de projetos ou um relatório de projeto, agora contém os seguintes aprimoramentos:

* As datas planejadas são editáveis
* Porcentagem concluída para projetos e tarefas é exibida

Antes dessa alteração, para editar as datas ou visualizar o percentual de conclusão, era necessário ir para a tarefa individual.

Para obter mais informações, consulte [Usar a exibição de Marco](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).
