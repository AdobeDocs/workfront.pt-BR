---
title: Perguntas frequentes de Projetos
description: Perguntas frequentes de Projetos
author: Alina
draft: Probably
feature: Work Management
exl-id: be262d72-f4e4-4426-a6bc-23499667fc97
source-git-commit: 15ddf6b4d82ccc694ec7a6c60d8e2d5b6b3645d6
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 1%

---

# Perguntas frequentes de Projetos

Veja a seguir perguntas frequentes sobre projetos.

## Por que a opção Inserir Tarefa Acima/ Abaixo está ausente quando eu clico com o botão direito do mouse em uma tarefa na lista de tarefas?

### Responder

Para usar as opções de inserção, a lista de tarefas deve ser classificada por número. Para classificar a coluna por número, clique em **#** no cabeçalho da coluna à esquerda de **Nome da Tarefa** para classificar a tarefa por número.

## Qual é a Data de Término Efetivo?

### Responder

A Data de Término Efetivo representa a data e a hora em que o trabalho foi concluído. Para obter mais informações, consulte [Visão geral da Data de Término Efetivo do projeto](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md).

## Por que o botão recuar/ recuar está faltando?

### Responder

Para usar o botão recuar/ recuar, certifique-se de que as tarefas estejam ordenadas pelo número da tarefa e que não haja Agrupamentos aplicados.

## Por que não posso alterar o status do projeto para Concluído?

Quando tento marcar meu projeto como concluído, recebo a seguinte mensagem de erro:

![Project_FAQ_Complete_Error_message.png](assets/project-faq-complete-error-message-350x138.png)

### Responder

Não é possível alterar o status de um projeto para concluído se você tiver uma das seguintes opções no projeto:

* Tarefas ou problemas incompletos
* Tarefa ou problemas com status de aprovação pendente

## Por que não posso alterar o status do projeto de Concluído para Atual?

### Responder

Se o modo de conclusão do projeto estiver definido como Automático, quando todas as tarefas e problemas forem concluídas, o status do projeto automaticamente se tornará Concluído e você não poderá modificá-lo para nenhum outro status. O Modo de conclusão do projeto deve ser definido como Manual para poder transformar um projeto completo em Atual. Para obter informações, consulte [O status do projeto não será alterado de Concluído para Atual](../../../manage-work/projects/tips-tricks-and-troubleshooting/project-status-does-not-change-from-complete-to-current.md).

## Por que não posso adicionar um projeto a uma Portfolio, embora tenha as permissões corretas para fazer isso?

Embora eu tenha as permissões corretas, o botão Adicionar projetos não aparece na guia Projetos do Portfolio.

### Responder

Isso é causado pelo Status de Portfolio estar Inativo. Para alterar o status da Portfolio:

1. Clique em **Detalhes do Portfolio > Visão geral**.
1. Alterar o **Status** para **Ativo.**

1. Clique em **Salvar**.\
   O botão **Adicionar Projetos** agora deve estar visível na guia **Projetos**.

## Que acesso um Gerenciador de recursos recebe quando adicionado a um projeto?

### Responder

Os gerentes de recursos recebem automaticamente o acesso Gerenciar aos projetos. Remover o usuário da função Gerenciador de Recursos não remove seu acesso Gerenciar compartilhamento.

## Por que o status do projeto muda quando adiciono um grupo?

### Responder

Os status do projeto mudam devido aos status padrão do Grupo. Quando você adiciona um grupo a um projeto, ele altera a lista de status para os status padrão definidos para o grupo.

Para obter mais informações, consulte o artigo [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

## O que é Status do Orçamento?

### Responder

O Status do Orçamento mostrará se o projeto foi adicionado atualmente ao Planejador de Capacidade e se o cálculo do orçamento foi concluído.

A seguir estão os Status de Orçamento:

* Não incluído - O projeto não é adicionado ao planejador de capacidade.
* Incluído mas Não Calculado - O projeto é adicionado ao Planejador de Capacidade, mas é excluído do cálculo do orçamento.
* Incluído e Calculado - O projeto é adicionado ao Planejador de Capacidade e incluído no cálculo do orçamento.

## Por que não posso compartilhar um projeto para o qual sou o Proprietário e onde tenho permissões de Gerenciamento com uma Equipe? Eu simplesmente não consigo encontrar a equipe na caixa de diálogo de compartilhamento do projeto.

### Responder

O administrador do Adobe Workfront restringiu você a visualizar somente Empresas, Grupos e equipes aos quais você pertence em seu Nível de acesso do. A equipe que você está procurando não é uma das equipes às quais você pertence.

![Exibir apenas equipes, grupos e empresas às quais pertencem](assets/view-only-team-groups-companies-they-belong-to-350x141.png)

Para obter informações sobre como permitir que um usuário visualize todas as equipes no sistema, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
