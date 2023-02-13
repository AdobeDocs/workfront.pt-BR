---
content-type: release-notes
keywords: notas,trimestral,atualizar
navigation-topic: product-releases
title: 21.1 Outras melhorias
description: Esta página descreve todas as outras melhorias feitas com a versão 21.1 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 15 de fevereiro de 2021.
author: Luke
feature: Product Announcements
exl-id: aa6cfba2-d1df-4d7c-975b-2ae0e63b6d85
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 0%

---

# 21.1 Outras melhorias

Esta página descreve todas as outras melhorias feitas com a versão 21.1 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção na semana de 15 de fevereiro de 2021.

Para obter uma lista de todas as alterações disponíveis com a versão 21.1, consulte [Visão geral da versão 21.1](../../../product-announcements/product-releases/21.1-release-activity/21-1-release-overview.md).

## Atualizações dos requisitos de falha da assinatura de evento

Estamos atualizando os requisitos de desativação temporária das falhas de assinatura de evento. Além dos requisitos existentes, as Assinaturas de eventos agora serão desabilitadas se não conseguirem obter um delivery bem-sucedido em 2000 tentativas. Trata-se de reforçar a atual regra de fracasso de 70%, que pode conduzir a montantes excessivos de falhas, sob algumas condições.

Além disso, adicionaremos requisitos de desativação permanente a partir de fevereiro de 2021.

Para obter mais informações sobre os novos requisitos de desativação flexível e desativação permanente, consulte [Perguntas frequentes - Assinaturas de eventos](../../../wf-api/general/event-subs-faq.md).

## Novos campos de Equipe disponíveis no Resumo diário

Adicionamos campos de Aprovação de equipe e atribuições ao email Ação necessária de resumo diário.

Para obter mais informações, consulte [Notificações: Ação necessária](../../../workfront-basics/using-notifications/notifications-action-needed.md).

## Substituição da opção de email POP em filas de solicitação

Estamos substituindo a opção de email POP para filas de solicitação por um novo sistema gerenciado pela Workfront. Você ainda poderá enviar solicitações por email, mas precisará configurar um novo endereço de email gerenciado pela Adobe Workfront na área Fila de solicitações .

Essas alterações estão disponíveis para teste em Visualização.

O email é desativado automaticamente em todos os ambientes de Visualização. Para ativar emails para fins de teste, consulte [Ativar a entrega de emails do ambiente Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

Para obter mais informações, consulte [Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações](/help/quicksilver/manage-work/requests/create-requests/enable-email-issues-into-projects.md).

Para obter mais informações sobre por que estamos fazendo essa alteração, consulte [Novo sistema gerenciado pela Adobe Workfront para substituir o email POP para filas de solicitações por 21.1](../../../product-announcements/announcements/announcement-archive/pop-removal-request-queue.md).

Esse recurso agora está incluído na variável [Gerenciamento de fila na nova experiência do Workfront](https://one.workfront.com/s/learningpath4/queue-management-MCYCJRWK36QZBP7PGMNDMSPRN3LE) caminho de aprendizagem no Workfront One.

## Restringir edição de hora em folhas de ponto

Para fornecer mais controle sobre folhas de horas e edição de hora, adicionamos uma configuração que permite restringir a edição de hora aos proprietários da folha de ponto e administradores do sistema.

Anteriormente, os usuários com a opção Folhas de horas e horas ativada em seu nível de acesso podiam editar horas em qualquer folha de ponto.

Para obter mais informações, consulte [Configurar preferências de hora e folha de ponto](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

## Filtros e visualizações aprimorados na área Folhas de horas

Adicionamos as seguintes melhorias quando você adiciona um Projeto, Tarefa ou Problema a uma Folha de Horas:

* Filtros: Adicionamos filtros para Projetos e Problemas. Clique em Mais opções para exibir esses filtros. Anteriormente, somente as Tarefas tinham filtragem disponível.
* Exibições: Adicionamos opções de Exibição e Agrupamento à página Pesquisar .

Para obter mais informações, consulte [Tempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Ocultar a caixa de horas extras nas Folhas de Horas

Agora é possível ocultar a caixa de horas extras para facilitar a confusão do usuário caso você não acompanhe horas extras no Workfront. Você pode ocultar a caixa de horas extras para uma folha de horas de uso único ou no Perfil da folha de horas:

* Folha de Horas de Uso Único: Quando você opta por ocultar a caixa de horas extras em uma folha de horas individual, ela fica oculta somente para essa folha de horas. Para obter mais informações, consulte [Criar uma folha de ponto de uso único](../../../timesheets/create-and-manage-timesheets/create-tmshts.md).
* Perfil da folha de horas: Ao optar por ocultar a caixa de horas extras no Perfil da folha de horas, todas as folhas de horas futuras criadas para os usuários atribuídos a esse perfil não visualizarão a caixa de horas extras. Para obter mais informações, consulte [Criar, editar e atribuir perfis de folha de ponto](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

Anteriormente, não era possível ocultar a caixa de horas extras nas folhas de horas.

## Expandir ou recolher itens na navegação estrutural

Para facilitar a visualização do caminho de navegação estrutural completo, adicionamos a funcionalidade de expandir e recolher.

Agora, quaisquer itens truncados são agrupados antes do Projeto com o texto &quot;mais&quot;. Por exemplo, &quot;mais 3&quot; indica que há 3 objetos que não estão sendo exibidos.

Anteriormente, era necessário clicar nas reticências para exibir todos os objetos truncados em um menu suspenso.

Para visualizar todos os itens na navegação estrutural, clique em &quot;mais&quot; no início da navegação estrutural para expandir os itens. Depois de expandido, você pode clicar em &quot;Menos&quot; para recolher os itens novamente.

## Nova aparência para navegação estrutural

Para ajudar os usuários a identificar melhor onde estão no Workfront e navegar mais facilmente entre objetos, fizemos as seguintes melhorias na navegação estrutural:

* Cada item na navegação estrutural agora inclui um rótulo de objeto.
* A página atual agora está incluída na navegação estrutural e está em itálico.
* Navegação por teclado e navegação por leitor de tela agora estão disponíveis para a navegação estrutural.
* Alterações adicionais no estilo secundário

