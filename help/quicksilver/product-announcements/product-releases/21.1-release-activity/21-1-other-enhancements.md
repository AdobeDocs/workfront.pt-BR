---
content-type: release-notes
keywords: notas,trimestral,atualizar
navigation-topic: product-releases
title: 21.1 Outras melhorias
description: Esta página descreve todas as outras melhorias feitas com a versão 21.1 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 15 de fevereiro de 2021.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 0%

---

# 21.1 Outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 21.1 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de Produção na semana de 15 de fevereiro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.1, consulte a [visão geral da versão 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Atualizações dos requisitos de falha de Assinatura de Evento

Estamos atualizando os requisitos de desabilitação flexível de falhas de Assinatura de Evento. Além dos requisitos existentes, as Inscrições em eventos agora estarão desativadas por software se não conseguirem obter um delivery bem-sucedido em 2000 tentativas. Trata-se de reforçar a atual regra de 70 % de incumprimento, que pode conduzir a montantes excessivos de incumprimento, em determinadas condições.

Além disso, adicionaremos requisitos de desativação rígida a partir de fevereiro de 2021.

Para obter informações adicionais sobre os novos requisitos de desabilitação por software e desabilitação por hardware, consulte [Perguntas frequentes - Assinaturas de Eventos](../../../wf-api/general/event-subs-faq.md).

## Campos de nova equipe disponíveis para o Resumo diário do

Adicionamos os campos de aprovação de equipe e atribuições ao email Ação necessária no resumo diário.

Para obter mais informações, consulte [Notificações: ação necessária](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Substituição da opção de email POP em Filas de solicitações

Estamos substituindo a opção de email POP para filas de solicitações por um novo sistema gerenciado pela Workfront. Você ainda poderá enviar solicitações por email, mas precisará configurar um novo endereço de email gerenciado pela Adobe Workfront na área Fila de solicitações.

Essas alterações estão disponíveis para teste na Pré-visualização.

O email é desativado automaticamente em todos os ambientes de Visualização. Para habilitar email para fins de teste, consulte [Habilitar entrega de emails do ambiente de Pré-visualização de Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Para obter mais informações, consulte [Habilitar usuários a enviar um problema por email para um projeto da Fila de Solicitações](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Para obter mais informações sobre por que estamos fazendo essa alteração, consulte [Novo sistema gerenciado pela Adobe Workfront para substituir o email POP por Filas de solicitações 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Este recurso agora está incluído no [Gerenciamento da fila no novo caminho de aprendizado da experiência de Workfront](https://experienceleague.adobe.com/en/docs/workfront-learn/tutorials-workfront/home) no Workfront One.

## Restringir a edição de horas em folhas de horas

Para fornecer mais controle sobre folhas de horas e edição de horas, adicionamos uma configuração que permite restringir a edição de horas aos proprietários da folha de horas e administradores do sistema.

Anteriormente, os usuários com a opção Folhas de horas e Horas habilitada em seu nível de acesso podiam editar horas em qualquer folha de horas.

Para obter mais informações, consulte [Configurar preferências de horas e folha de horas](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Filtros e visualizações aprimorados na área Folhas de horas

Adicionamos as seguintes melhorias quando você adiciona um projeto, tarefa ou problema a uma folha de horas:

* Filtros: adicionamos filtros para projetos e problemas. Clique em Mais opções para visualizar esses filtros. Anteriormente, somente Tarefas tinham filtragem disponível.
* Exibições: adicionamos opções de Exibição e Agrupamento à página Pesquisar.

Para obter mais informações, consulte [Log time](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ocultar a caixa de horas extras na Planilha de horas

Agora você pode ocultar a caixa de horas extras para aliviar a confusão do usuário se não rastrear as horas extras no Workfront. Você pode ocultar a caixa de horas extras para uma folha de horas de uso único ou no Perfil da folha de horas:

* Folha de horas de uso único: quando você opta por ocultar a caixa de horas extras em uma folha de horas individual, ela fica oculta somente para essa folha de horas. Para obter mais informações, consulte [Criar uma folha de horas de uso único](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Perfil da folha de horas: quando você opta por ocultar a caixa horas extras no Perfil da folha de horas, todas as folhas de horas futuras criadas para o(s) usuário(s) atribuído(s) a esse perfil não verão a caixa horas extras. Para obter mais informações, consulte [Criar, editar e atribuir perfis de folha de horas](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Anteriormente, não era possível ocultar a caixa de horas extras em folhas de horas.

## Expandir ou recolher itens na navegação estrutural

Para facilitar a visualização do caminho completo da navegação estrutural, adicionamos a funcionalidade Expandir e recolher.

Agora, todos os itens truncados são agrupados antes do projeto com o texto &quot;mais&quot;. Por exemplo, &quot;mais 3&quot; indica que há 3 objetos que não estão sendo exibidos.

Anteriormente, você tinha que clicar nas reticências para exibir quaisquer objetos truncados em um menu suspenso.

Para exibir todos os itens na navegação estrutural, clique em &quot;mais&quot; no início da navegação estrutural para expandir os itens. Depois de expandido, você pode clicar em &quot;Menos&quot; para recolher os itens novamente.

## Nova aparência para navegação estrutural

Para ajudar os usuários a identificar melhor onde estão no Workfront e navegar mais facilmente entre objetos, fizemos as seguintes melhorias na navegação estrutural:

* Cada item na navegação estrutural agora inclui um rótulo de objeto.
* A página atual agora está incluída na navegação estrutural e está em itálico.
* A navegação pelo teclado e a navegação pelo leitor de tela agora estão disponíveis para navegação estrutural.
* Alterações adicionais de estilo secundárias

