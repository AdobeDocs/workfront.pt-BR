---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Visualização 5
description: Esta página descreve todas as alterações disponíveis no ambiente de Visualização com a versão R1 Preview 5 . A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 16 de março de 2017.
author: Luke
feature: Product Announcements
exl-id: 4fba14b5-6c5a-4b03-99a7-f0e6f75807c3
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1283'
ht-degree: 13%

---

# R1 Visualização 5

Esta página descreve todas as alterações disponíveis no ambiente de Visualização com a versão R1 Preview 5 . A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 16 de março de 2017.

Para obter uma lista de todas as alterações feitas em R1, consulte [Visão geral da atividade de versão do R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/r1-release-activity-overview.md).

## Rastrear o progresso do projeto com um relatório de utilização

Agora, um usuário com acesso Gerenciar a um projeto pode acompanhar o progresso do projeto com um relatório de utilização.

O relatório de utilização permite manter o projeto dentro do orçamento, permitindo que você veja rapidamente como as horas reais estão sendo rastreadas em relação às horas orçadas ou às horas planejadas de uma determinada semana ou mês, ou para o projeto geral. Além disso, você pode exibir informações detalhadas sobre o número de horas em cada categoria (orçada, planejada e real), categorizadas por função de cargo ou usuário individual.

Para obter mais informações sobre o rastreamento da utilização em um projeto, consulte [Visão Geral do Relatório de Utilização de Recursos](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

Como administrador do sistema, você pode configurar se a guia Utilização está disponível para os usuários. Por padrão, a guia Utilização está localizada no menu suspenso Mais em um projeto. Você pode mover a guia Utilização para outro local, ou pode ocultá-la completamente. Se você tiver definido modelos de layout personalizados para usuários em sua organização, precisará adicionar manualmente a guia Utilização aos modelos de layout personalizados.

Para obter mais informações sobre como configurar o local da guia Utilização, consulte &quot;Personalizar guias&quot; em &quot;Criação e gerenciamento de modelos de layout&quot;.

## Modificar um Processo de Aprovação Global Existente para um Objeto Individual

Agora você pode modificar um processo de aprovação global existente ao associar esse processo de aprovação global a um objeto. As modificações feitas se aplicam somente ao processo de aprovação no objeto ao qual você o está associando.

Para obter mais informações, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md) em [Associar um processo de aprovação novo ou existente ao trabalho](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)

## Configurar relatórios para mostrar o novo gráfico de Gantt por padrão

Você pode configurar os relatórios de projeto e tarefa criados para mostrar o novo gráfico de Gantt por padrão com a nova opção, &quot;Mostrar este relatório em uma exibição de Gantt por padrão&quot;.

Para obter mais informações sobre como configurar relatórios para mostrar o novo gráfico de Gantt, consulte [Editar configurações de relatório](../../../../reports-and-dashboards/reports/creating-and-managing-reports/edit-report-settings.md).

Para obter mais informações sobre como visualizar o gráfico de Gantt em relatórios de projeto e relatórios de tarefa, consulte [Exibir informações no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)&quot; in [Exibir informações no Gráfico de Gantt](../../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md).

## Melhoria da Lixeira: Tarefas e subtarefas são restauradas à ordem anterior

Agora, quando você restaurar uma tarefa ou subtarefa após sua exclusão, a tarefa ou subtarefa será restaurada para seu local anterior (na lista de tarefas ou abaixo da tarefa pai), na mesma ordem em que foi exibida antes de ser excluída.

Antes dessa alteração, as tarefas e subtarefas que eram restauradas eram sempre restauradas como a última tarefa (na lista de tarefas ou abaixo da tarefa pai), independentemente da ordem em que apareciam antes de serem excluídas.

Para obter mais informações sobre como restaurar objetos no Workfront, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Melhorias na exibição de marco

As seguintes melhorias agora estão disponíveis ao visualizar uma lista de projetos ou relatório de projetos na exibição de Marco:

* **Configure se Progress Status e Porcentagem de Conclusão são exibidos na visualização:** Há uma nova opção que permite configurar se os ícones de Status do Progresso são exibidos na visualização de Marco. Além disso, você também pode configurar se as informações da porcentagem concluída são exibidas relacionadas a projetos e tarefas.\
   Para obter mais informações, consulte [Usar a exibição de Marco](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) em [Usar a exibição de Marco](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md).

* **Edite a porcentagem concluída diretamente da exibição de Marco:** Agora é possível editar a porcentagem de conclusão de projetos e tarefas diretamente da visualização de marcos.\
   Para obter mais informações, consulte [Usar a exibição de Marco](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md) em [Usar a exibição de Marco](../../../../reports-and-dashboards/reports/reporting-elements/use-milestone-view.md). 

## Aparência atualizada de várias páginas de configuração do sistema

A aparência das seguintes páginas no menu Sistema da área Configuração foi atualizada (a funcionalidade permanece a mesma):

* Diagnósticos
* Logon único (SSO) que inclui:

   * Active Directory
   * LDAP
   * SAML 1.1
   * SAML 2.0

* Atualizar usuários para SSO

## Agrupamentos de notificação de evento atualizados na área Configuração de email

Os cabeçalhos organizacionais das Notificações de eventos na área Configuração de email agora correspondem aos cabeçalhos de seção usados na área de configurações do perfil do usuário.

Para obter mais informações sobre notificações de eventos, consulte  [Configurar notificações de evento para todos no sistema](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

## Recusar notificações instantâneas: Configuração de resumo no contexto

As opções a seguir agora estão disponíveis nas notificações instantâneas por email. Essas opções estão disponíveis somente para notificações instantâneas que também têm uma contrapartida diária de compilação:

* “Adicionar isto ao resumo diário”
* &quot;Parar Emails deste Tipo&quot;

Agora, ao receber uma notificação por email instantânea, você pode adicionar essa notificação a uma notificação de resumo diária ou cancelar a assinatura completamente dessa notificação.

Essas opções estão disponíveis na notificação por email. Para obter mais informações sobre o recebimento de notificações por email, consulte [Notificações do Adobe Workfront](../../../../workfront-basics/using-notifications/wf-notifications.md)

## Várias notificações por email movidas da seção &quot;Ação necessária&quot; para outras seções relacionadas ao projeto

Várias notificações foram movidas da seção &quot;Ação necessária&quot; da página de perfil do usuário para outras seções, da seguinte maneira:

Para obter mais informações sobre como configurar notificações por email, consulte [Ativar ou desativar suas próprias notificações de evento](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Notificação</strong> </th> 
   <th><strong>Seção Antiga</strong> </th> 
   <th><strong>Nova seção</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Quando um problema for adicionada enviar email para o proprietário do projeto.</td> 
   <td> <p> Ação necessária </p> </td> 
   <td>   <p>Informações sobre Projetos dos quais sou proprietário</p></td> 
  </tr> 
  <tr> 
   <td>Quando um problema for adicionada enviar email para a equipe.</td> 
   <td>   <p>Ação necessária</p><p> </p></td> 
   <td> <p> Informações sobre Projetos dos quais sou proprietário </p>   </td> 
  </tr> 
  <tr> 
   <td>Quando um problema atribuída for adicionada enviar email para o proprietário do projeto.</td> 
   <td>   <p>Ação necessária</p></td> 
   <td>   <p>Informações sobre Projetos dos quais sou proprietário</p></td> 
  </tr> 
  <tr> 
   <td> <p> Quando um problema não atribuída for adicionada enviar email para a equipe. </p> </td> 
   <td> <p> Ação necessária </p>   </td> 
   <td> <p> Informações sobre Projetos dos quais sou proprietário </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> A data de compromisso de uma tarefa em um dos meus projetos mudou </p> </td> 
   <td>   <p>Ação necessária</p></td> 
   <td>   <p>Informações sobre Projetos dos quais sou proprietário</p></td> 
  </tr> 
  <tr> 
   <td> <p> Mudança da data de compromisso de um problema em um dos meus projetos </p>   </td> 
   <td>   <p>Ação necessária</p></td> 
   <td> <p> Informações sobre Projetos dos quais sou proprietário </p>   </td> 
  </tr> 
  <tr> 
   <td> <p> A data de conclusão de uma tarefa atribuída a mim mudou </p> </td> 
   <td>   <p>Ação necessária</p></td> 
   <td>   <p>Informações sobre Trabalho atribuído a mim</p></td> 
  </tr> 
  <tr> 
   <td> <p> A data de conclusão de um problema atribuído a mim mudou </p> </td> 
   <td> <p> Ação necessária </p>   </td> 
   <td>   <p>Informações sobre Trabalho atribuído a mim</p></td> 
  </tr> 
  <tr> 
   <td> <p> O status é alterado em uma tarefa para a qual fui atribuído </p>   </td> 
   <td> <p> Ação necessária </p>   </td> 
   <td> <p> Informações sobre Trabalho atribuído a mim </p>   </td> 
  </tr> 
 </tbody> 
</table>

## Nova Funcionalidade de Planejamento de Recursos (Não Disponível em Produção em R1)

>[!NOTE]
>
>Essa funcionalidade está disponível no ambiente de Visualização. Ele será removido do ambiente de Pré-visualização aproximadamente um mês antes do lançamento do R1 para produção. Em seguida, ele será reintroduzido no ambiente de Visualização no R2 Preview 1.

 

As seguintes alterações foram adicionadas para suportar a futura funcionalidade de Planejamento de Recursos:

* A guia atual &quot;Planejamento de recursos&quot; foi renomeada para &quot;Planejamento de recursos herdados&quot; na área Pessoas. 
* Uma nova guia &quot;Planejamento de recursos&quot; foi introduzida na área Pessoas, onde a nova funcionalidade será desenvolvida.\
   Para obter mais informações sobre a nova guia Planejamento de Recursos, consulte [Introdução ao planejamento de recursos](../../../../resource-mgmt/resource-planning/get-started-resource-planning.md) 

* O objeto atual &quot;Pool de Recursos&quot; foi renomeado para &quot;Pool de Recursos Herdados&quot;.\
   Para obter mais informações sobre como criar os novos Pools de Recursos Baseados no Usuário, consulte [Visão geral dos pools de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

* Um novo objeto &quot;Pool de Recursos&quot; foi criado para oferecer suporte aos novos Pools de Recursos (baseados no usuário).

   >[!NOTE]
   * Se, atualmente, você estiver executando relatórios sobre os Pools de Recursos Legados existentes, os relatórios existentes não serão alterados.
   * Para criar um novo relatório para os Pools de Recursos Legados existentes (baseados em funções de trabalho), será necessário selecionar &quot;Pools de Recursos Legados&quot; como o objeto do relatório.
   * Se quiser criar um novo relatório para os novos Pools de Recursos (baseados no usuário), será necessário selecionar &quot;Pools de Recursos&quot; como o objeto do relatório.

  >   
