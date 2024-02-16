---
content-type: release-notes
navigation-topic: product-releases-archive
title: Atividade da versão Beta 1 2017.2
description: Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão Beta 1 2017.2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 10 de maio de 2017.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 0%

---

# Atividade da versão Beta 1 2017.2

Esta página descreve todas as alterações disponíveis no ambiente de Pré-visualização com a versão Beta 1 2017.2. A funcionalidade nesta página foi disponibilizada no ambiente de Pré-visualização em 10 de maio de 2017.

>[!IMPORTANT]
>
>A funcionalidade descrita nesta página está sujeita a alterações antes da disponibilidade no ambiente de produção.

A versão Beta 1 2017.2 contém melhorias para administradores do Workfront e outros usuários:

**Para administradores:**

* [Restaurar Documentos](#restore-documents)
* [Novo banner de visualização com informações de lançamento](#new-preview-banner-with-release-information) 
* [Disponibilidade da API 7](#api-7-availability)

**Para Todos Os Usuários:**

* [Inscrever-se em tarefas e problemas](#subscribe-to-tasks-and-issues)
* [Melhorias no Agendamento de Recursos](#resource-scheduling-improvements)
* [Comparar provas](#compare-proofs)
* [Novo campo para conjuntos de recursos para usuários e projetos](#new-field-for-resource-pools-for-users-and-projects)
* [Aparência atualizada na lista de painéis](#updated-look-and-feel-in-the-dashboard-list)
* [Remoção da funcionalidade de endossos no Workfront](#removing-the-endorsements-functionality-in-workfront)
* [Reordenar colunas em qualquer lista com o recurso de arrastar e soltar (a funcionalidade está sendo removida)](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## Restaurar Documentos {#restore-documents}

Os administradores do Workfront agora podem restaurar documentos individuais que foram excluídos nos últimos 30 dias. 

Antes dessa alteração, os administradores do Workfront podiam restaurar somente projetos, tarefas e problemas (incluindo documentos que foram excluídos juntamente com o projeto, tarefa ou problema excluído).

Para obter mais informações, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

## Novo banner de visualização com informações de lançamento {#new-preview-banner-with-release-information}

O banner azul na parte superior do ambiente Visualizar sandbox agora exibe o nome da versão e o número da versão do ambiente Visualizar. Clicar no nome da versão levará você a um artigo do Site de ajuda, no qual você pode encontrar mais informações sobre a versão de Pré-visualização atual. Para obter mais informações sobre o Ambiente de pré-visualização da sandbox, consulte [O ambiente de sandbox de visualização do Adobe Workfront](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md) 

## Disponibilidade da API 7 {#api-7-availability}

A API 7 agora está disponível e inclui objetos novos e atualizados.

Para obter mais informações, consulte [Novidades da API versão 7](../../../../wf-api/api/new-api-version-7.md).

## Inscrever-se em tarefas e problemas {#subscribe-to-tasks-and-issues}

O Workfront envia notificações sobre os itens aos quais você está atribuído ou que você possui.

A partir da versão atual, se você quiser seguir itens que não estão atribuídos a você, mas que podem afetar seu trabalho, poderá assiná-los.

Você pode assinar problemas e tarefas para os quais tem permissão ao menos Exibir. Quando um novo comentário for adicionado à questão ou tarefa que você assina, você será notificado por email sobre esse comentário.

Para obter mais informações sobre a assinatura de problemas e tarefas, consulte [Assinar itens no Adobe Workfront](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)

## Melhorias no Agendamento de Recursos {#resource-scheduling-improvements}

>[!NOTE]
>
>As ferramentas de Agendamento de recursos foram substituídas e removidas do Workfront com a versão 23.1. Para obter informações sobre como programar recursos usando o Balanceador de carga de trabalho, consulte [Visão geral do Balanceador de carga de trabalho](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

As seguintes melhorias estão disponíveis ao agendar recursos:

* [Exibir mais itens no cronograma de agendamento de recursos em uma única visualização](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [Configurar o nome do projeto para exibir em tarefas e problemas na linha de tempo do cronograma](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [Configurar se as tarefas pai são exibidas na linha de tempo de agendamento](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [Expanda ou reduza mais facilmente todas as tarefas e problemas na linha de tempo de agendamento](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [As informações de função e usuário permanecem no topo da linha de tempo de agendamento ao rolar a tela](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### Exibir mais itens no cronograma de agendamento de recursos em uma única visualização {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

Ao agendar recursos para uma equipe ou para qualquer projeto para o qual você seja o Gerenciador de recursos, as tarefas e problemas agora consomem menos espaço vertical no cronograma do agendamento. Isso permite que você veja mais tarefas e problemas em uma única visualização.

Se você decidir mostrar nomes de projeto em cada tarefa e problema na linha do tempo de agendamento, o espaço vertical de cada tarefa e problema será expandido, resultando em menos tarefas e problemas sendo exibidos em um único modo de exibição.

Para obter mais informações sobre a programação de recursos, consulte &quot;Introdução ao Agendamento de recursos&quot;.

### Configurar o nome do projeto para exibir em tarefas e problemas na linha de tempo do cronograma {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

Ao agendar recursos para uma equipe ou para qualquer projeto para o qual você seja o Gerente de recursos, agora é possível configurar o nome do projeto a ser exibido em cada tarefa e problema na linha do tempo do agendamento. Isso permite que os usuários que visualizam a linha do tempo do agendamento vejam rapidamente o nome do projeto no qual a tarefa ou problema reside.

Para obter mais informações, consulte &quot;Introdução ao agendamento de recursos&quot;.

### Configurar se as tarefas pai são exibidas na linha de tempo de agendamento {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

Ao agendar recursos para projetos para os quais você é o Gerenciador de recursos, agora é possível configurar se as tarefas pai serão exibidas na linha do tempo do agendamento quando a opção Modo de conclusão em resumo no projeto estiver definida como Manual.

Antes dessa alteração, as tarefas pai sempre eram exibidas na linha do tempo do agendamento quando o Modo de conclusão em resumo no projeto era definido como Manual. 

Quando o Modo de conclusão em resumo no projeto está definido como Automático, as tarefas pai não podem ser exibidas na linha do tempo do agendamento. Essa experiência não mudou.

Para obter mais informações, consulte &quot;Introdução ao agendamento de recursos&quot;.

### Expanda ou reduza mais facilmente todas as tarefas e problemas na linha de tempo de agendamento {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

Um novo link está disponível e permite que você reduza mais facilmente todas as tarefas e problemas na linha do tempo de agendamento.

Para obter mais informações, consulte &quot;Introdução ao agendamento de recursos&quot;.

### As informações de função e usuário permanecem no topo da linha de tempo de agendamento ao rolar a tela {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

Agora, ao rolar para baixo na linha do tempo de agendamento para exibir informações adicionais, o nome da função e o nome do usuário permanecem na parte superior da área Usuários e funções na linha do tempo de agendamento, facilitando a visualização de a qual usuário e função as tarefas e problemas estão associados.

Antes dessa alteração, o nome da função e o nome do usuário saíam da exibição atual.

Para obter mais informações sobre a programação de recursos, consulte &quot;Introdução ao Agendamento de recursos&quot;.

## Comparar provas {#compare-proofs}

Agora é possível comparar duas provas de documento em qualquer lista de documentos única, como na guia Documentos em um projeto, tarefa, problema, portfólio ou na área Documentos principal da Barra de navegação global. 

As duas provas são exibidas na ferramenta Revisão e Aprovação, e você pode revisar cada documento enquanto as compara em uma exibição lado a lado.

Para obter mais informações, consulte [Comparar provas](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md).

## Novo campo para conjuntos de recursos para usuários e projetos {#new-field-for-resource-pools-for-users-and-projects}

A versão R1.5 apresentou uma nova funcionalidade em torno do Planejamento de recursos para o ambiente de Pré-visualização. Essa funcionalidade permite criar novos Conjuntos de recursos, que são coleções de usuários.

Agora é possível associar esses Conjuntos de recursos a projetos e usuários. Agora você verá um novo campo chamado &quot;Conjuntos de recursos&quot; no projeto, bem como no objeto do usuário.

Para obter mais informações sobre os novos Conjuntos de recursos e como eles podem ser associados a projetos e usuários, consulte [Visão geral dos conjuntos de recursos](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)

## Aparência atualizada na lista de painéis {#updated-look-and-feel-in-the-dashboard-list}

Agora, ao visualizar uma lista de painéis, a aparência é mais moderna e escalável.

Essa funcionalidade estava disponível anteriormente somente para usuários inscritos no Acesso antecipado. Agora isso está disponível para todos os usuários no ambiente de Pré-visualização. Ele será disponibilizado para todos os usuários no ambiente de Produção com a versão 2017.2. 

Para obter mais informações sobre painéis, consulte [Criar um painel](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Remoção da funcionalidade de endossos no Workfront {#removing-the-endorsements-functionality-in-workfront}

Ao avaliar a funcionalidade contida no fluxo de atualização, identificamos os Endossos como sendo de baixa adoção e um recurso de baixa utilização. Em 2017.2, a seguinte funcionalidade em torno de Endossos será removida do Workfront a partir da versão 2017.2 (essa funcionalidade não está mais disponível na Pré-visualização):

* A guia Endossos na área de perfil do usuário;
* O objeto Endossos será removido do explorador de API; se você estiver enviando relatórios de API para os objetos &quot;Endosso&quot; ou &quot;Compartilhamento de Endosso&quot;, as chamadas serão inválidas após a remoção desse objeto.

A seguinte funcionalidade continuará a permanecer no aplicativo web:

* O endosso de um usuário por outro usuário feito antes da remoção desse recurso permanecerá no fluxo de atualização do endossador. 

Endossos não foram um objeto reportável, portanto, não há alterações nos relatórios para esse objeto.

## Reordenar colunas em qualquer lista com o recurso de arrastar e soltar (a funcionalidade está sendo removida) {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

A funcionalidade para alterar a ordem das colunas em qualquer lista arrastando uma coluna de um local e soltando-a em outro está sendo removida de Acesso antecipado no ambiente de produção com a versão 2017.2 e não estará mais disponível para nenhum usuário. 

Para obter mais detalhes sobre essa funcionalidade, consulte [Modificar a largura e a ordem da coluna](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md).
