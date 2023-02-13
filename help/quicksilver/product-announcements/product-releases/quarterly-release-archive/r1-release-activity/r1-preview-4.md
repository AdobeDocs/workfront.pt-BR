---
content-type: release-notes
navigation-topic: product-releases-archive
title: R1 Pré-visualização 4
description: Esta página descreve todas as alterações disponíveis no ambiente de Visualização com a versão R1.4. A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 15 de fevereiro de 2017.
author: Luke
feature: Product Announcements
exl-id: 2945e058-74dd-4cc3-9d6c-e5618ee7041c
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# R1 Pré-visualização 4

Esta página descreve todas as alterações disponíveis no ambiente de Visualização com a versão R1.4. A funcionalidade nesta página foi disponibilizada no ambiente de Visualização em 15 de fevereiro de 2017.

Para obter uma lista de todas as alterações feitas em R1, consulte [A versão Workfront R1](../../../../product-announcements/product-releases/quarterly-release-archive/r1-release-activity/workfront-r1-release.md).

## Aprovações de projeto, tarefa e ocorrência atualizadas

Ao criar processos de aprovação para aprovações de projeto, tarefa e emissão, os seguintes aprimoramentos e alterações agora estão disponíveis: 

* As &quot;Etapas&quot; de aprovação agora são chamadas de aprovação &quot;Etapas&quot;.
* Incluir vários tipos de aprovadores por estágio.\
   Isso inclui usuários, equipes e funções de trabalho.\
   Antes dessa alteração, você podia incluir vários aprovadores do mesmo tipo somente. Por exemplo, você pode incluir várias funções de trabalho, mas não uma função de trabalho e uma equipe.

* As seguintes limitações pré-existentes relacionadas à modificação de processos de aprovação global existentes foram removidas:

   * O processo de aprovação modificado reflete-se apenas em objetos em todo o sistema em que o processo de aprovação ainda não foi iniciado ou em que o processo de aprovação não foi modificado. Os objetos em que o processo de aprovação já foi iniciado ou em que o processo de aprovação foi modificado não são atualizados com as alterações.
   * Não é possível modificar o status que determina quando a aprovação começa.

* Aparência e comportamento atualizados.

Para obter mais informações sobre a criação de processos de aprovação, consulte [Criar um processo de aprovação para itens de trabalho](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Ao associar um processo de aprovação a um projeto, tarefa ou problema, os seguintes aprimoramentos e alterações estão disponíveis:

* Aparência e comportamento atualizados.
* O diagrama de aprovação é exibido na guia Aprovações , mostrando uma representação visual das etapas de aprovação anteriores, atuais e futuras.

Para obter mais informações sobre como associar aprovações a projetos, tarefas e emissões, consulte [Associar um processo de aprovação novo ou existente ao trabalho](../../../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## Alterar o status de um projeto diretamente da página do projeto

Não é mais necessário editar um projeto para alterar o status do projeto. Agora é possível alterar o status de um projeto diretamente da página principal do projeto.

Para obter mais informações, consulte [Alterar o status de um projeto](../../../../manage-work/projects/manage-projects/change-project-status.md).

## Agendar usuários para desativação

Agora é possível agendar a desativação de usuários em uma data futura.

Antes dessa melhoria, você só podia desativar manualmente um usuário imediatamente.

Agendar um usuário para ser desativado pode ser útil em vários cenários. Por exemplo, se você criar usuários no Workfront que são contratados temporariamente, você poderá configurá-los para serem desativados quando o contrato terminar.

Esse recurso também está disponível ao editar usuários em massa. 

Para obter mais informações sobre como programar usuários para desativação, consulte [Desativar ou reativar um usuário](../../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md) e [Adicionar usuários](../../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Novas opções de resumo de email para &quot;Ações necessárias&quot;

A opção Daily Digest delivery está disponível na área &quot;Action Needed&quot; das configurações de Notificações.

Para obter mais informações, consulte [Ativar ou desativar suas próprias notificações de evento](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

Lembre-se de atualizar o endereço de email associado à sua conta para poder testar essa funcionalidade. Isso é necessário porque a sandbox de visualização limpa os endereços de email de todos os usuários.

## Melhoria da Lixeira: Registrado na atualização de fluxo e na notificação por email de recebimento

Os seguintes aprimoramentos foram adicionados ao restaurar projetos, tarefas e problemas excluídos:

* Agora você recebe uma notificação por email após restaurar um objeto.\
   Como administrador do Workfront, agora você recebe uma notificação por email após restaurar um projeto, tarefa ou problema que foi excluído anteriormente. A notificação por email informa sobre o status do processo de restauração.\
   Para obter mais informações sobre como restaurar objetos no Workfront, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

* Quando o objeto é restaurado, a exclusão e a restauração do objeto agora são registradas no fluxo de atualização do próprio objeto e no fluxo de atualização do objeto pai.\
   Anteriormente, somente a exclusão era registrada no fluxo de atualização do objeto pai.\
   Por exemplo, quando a tarefa é restaurada, uma mensagem é adicionada ao fluxo de atualização do projeto e da própria tarefa, indicando que a tarefa foi restaurada. (As exclusões e restaurações não são registradas em subtarefas. As informações sobre exclusões e restaurações de subtarefas estão disponíveis somente em tarefas pai.)\
   Para obter mais informações, consulte [Restaurar itens excluídos](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

 

## Caixa de diálogo atualizada para gerenciar associação de grupo

Há uma nova interface para o gerenciamento de grupos e subgrupos que oferece uma experiência mais fácil e fácil de usar.

O campo Proprietários do grupo e o campo Membros do grupo agora são combinados em um único campo, com uma lista de membros do grupo listada abaixo. Além disso, você pode filtrar a lista de membros do grupo e alterar se eles são Proprietário ou Membro. 

Para obter mais informações sobre como adicionar subgrupos a grupos, bem como designar usuários como membros ou proprietários de grupos, consulte [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) e [Criar um grupo](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md). 

 

## Copiar texto no aplicativo móvel

Você pode copiar o texto nos seguintes campos de todos os objetos que estão visíveis no aplicativo móvel:

* Nome
* Descrição
* Número de Referência
* Comentários

Essa funcionalidade deve ser lançada nas lojas de aplicativos iOS e Android na semana de 13 de fevereiro.
