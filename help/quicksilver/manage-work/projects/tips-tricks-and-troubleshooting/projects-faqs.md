---
title: Perguntas frequentes sobre projetos
description: Perguntas frequentes sobre projetos
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 0%

---

# Perguntas frequentes sobre projetos

As perguntas a seguir são frequentes sobre projetos.

## Por que a tarefa Inserir acima / abaixo está ausente quando eu clico com o botão direito do mouse em uma tarefa na lista de tarefas?

### Resposta

Para usar as opções de inserção, a lista de tarefas deve ser classificada por número. Para classificar a coluna por número, clique em **#** no cabeçalho da coluna à esquerda de **Nome da tarefa** para reordenar a tarefa por número.

## Qual é a Data de conclusão real?

### Resposta

A Data de Conclusão Real representa a data e a hora em que o trabalho é concluído. Para obter mais informações, consulte [Visão geral da data de conclusão real do projeto](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## Por que o botão de recuo/recuo está ausente?

### Resposta

Para usar o botão recuo/recuo, verifique se as tarefas são classificadas pelo número da tarefa e se não há Agrupamentos aplicados.

## Por que não posso alterar o status do projeto para Concluído?

Recebo a seguinte mensagem de erro quando tento marcar meu projeto como concluído:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Resposta

Não é possível alterar o status de um projeto para ser concluído se você tiver uma das opções a seguir no projeto:

* Tarefas ou problemas incompletos
* Tarefa ou problemas no status de aprovação pendente

## Por que não posso alterar o status do projeto de Concluído para Atual?

### Resposta

Se o projeto tiver o Modo de conclusão definido como Automático, depois que todas as tarefas e problemas forem concluídos, o status do projeto automaticamente será Concluído e você não poderá modificá-lo para qualquer outro status. O Modo de conclusão do projeto deve ser definido como Manual para poder transformar um projeto completo em Atual. Para obter mais informações, consulte [O status do projeto não será alterado de Concluído para Atual](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## Por que não posso adicionar um Projeto a um Portfolio, embora eu tenha as permissões corretas para fazer isso?

Embora eu tenha as permissões corretas, o botão Adicionar projetos está ausente na guia Projetos do Portfolio.

### Resposta

Isso é causado pelo status do Portfolio sendo Inativo. Para alterar o status do Portfolio:

1. Clique em **Detalhes do Portfolio > Visão geral**.
1. Altere o **Status** para **Ativo.**

1. Clique em **Salvar**.\
   O **Adicionar projetos** O botão deve estar visível no **Projetos** guia .

## Que acesso um Gerenciador de recursos recebe quando adicionado a um projeto?

### Resposta

Os Gerentes de recursos recebem automaticamente o acesso de Gerenciar aos projetos. Remover o usuário da função do Gerenciador de Recursos não remove o acesso de gerenciamento de compartilhamento.

## Por que o status do projeto muda quando eu adiciono um grupo?

### Resposta

Os status do projeto são alterados por causa dos status padrão do Grupo. Ao adicionar um grupo a um projeto, ele altera a lista de status para os status padrão definidos para o grupo.

Para obter mais informações, consulte o artigo [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## O que é Status do Orçamento?

### Resposta

O Status do Orçamento mostrará se o projeto está ou não adicionado ao Planejador de Capacidade e se o cálculo do orçamento foi concluído.

A seguir estão os Status do Orçamento:

* Não Incluído - O projeto não é adicionado ao planejador de capacidade.
* Incluído, mas não calculado - o projeto é adicionado ao Planejador de Capacidade, mas é excluído do cálculo de orçamento.
* Incluído e Calculado - O projeto é adicionado ao Planejador de Capacidade e incluído no cálculo do orçamento.

## Por que não posso compartilhar um projeto do qual sou o Proprietário e onde tenho permissões de Gerenciar com uma Equipe? Simplesmente não consigo encontrar a equipe na caixa de diálogo de compartilhamento do projeto.

### Resposta

O administrador do Adobe Workfront restringiu você a visualizar somente Empresas, Grupos e Equipes aos quais você pertence em seu Nível de acesso do. A equipe que você está procurando não é uma das equipes às quais você pertence.

![](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Para obter informações sobre como permitir que um usuário exiba todas as equipes no sistema, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
