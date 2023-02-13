---
product-area: projects
navigation-topic: use-predecessors
title: Impor predecessores
description: Os antecessores são tarefas nas quais outras tarefas dependem para conclusão. As relações do antecessor afetam as Datas de início e conclusão das tarefas e, em última análise, afetam a linha do tempo do projeto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '530'
ht-degree: 0%

---

# Impor predecessores

Os antecessores são tarefas nas quais outras tarefas dependem para conclusão. As relações do antecessor afetam as Datas de início e conclusão das tarefas e, em última análise, afetam a linha do tempo do projeto.

Para obter informações sobre predecessores, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Ao definir relações de antecessor entre tarefas, você define como o início ou o término de uma tarefa dependente depende do início ou do término de suas tarefas antecessoras. Isso é feito usando Tipos de dependência diferentes.

Para obter informações sobre Tipos de Dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Visão geral dos antecessores forçados

>[!IMPORTANT]
>
>Você deve impor os antecessores para exigir que as relações dos antecessores sejam respeitadas. Sem impor os antecessores, as tarefas dependentes podem iniciar e terminar independentemente do início e do fim dos antecessores, independentemente dos Tipos de dependência.

Você pode aplicar a relação do antecessor ao definir antecessores em um projeto.

Se um antecessor for empregado, a tarefa sucessora não poderá ser iniciada antes que o antecessor seja concluído. Por exemplo, impor uma relação de Conclusão-Início entre a Tarefa A e a Tarefa B significa que a Tarefa B não pode iniciar (o Status deve permanecer Novo e a Porcentagem Concluída deve permanecer 0%) até que a Tarefa A seja marcada como concluída. A imposição de relações se aplica a todos os tipos de antecessores.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Tarefas e Projetos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para as tarefas e o projeto</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Impor um antecessor no nível da tarefa

1. Vá para a tarefa sucessora cujo antecessor deseja impor.
1. Clique em **Predecessores** no painel esquerdo, em seguida, clique em **Adicionar antecessor**. Talvez seja necessário clicar em **Mostrar mais**, em seguida **Predecessores**.
1. (Condicional) Se quiser adicionar um antecessor entre projetos, remova o nome do projeto na **Projeto pai** e substitua por outro projeto.
1. Especifique o nome da tarefa ou tarefas antecessora no **Tarefas** campo.
1. Especifique a **Tipo de dependência** entre estas duas tarefas.

   O padrão **Tipo de dependência** é **Finish-Start**.

1. Selecione o **Forçado** para aplicar o antecessor.
1. Clique em **Salvar**.

## Impor um antecessor em uma lista de tarefas

1. Vá para uma lista de tarefas em um projeto.
1. No **Exibir** selecione o menu suspenso **Exibição padrão**.

1. Anote o número de tarefas que você designará como antecessor.
1. Localize a tarefa sucessora cujo antecessor você deseja impor.
1. No **Predecessores** , comece a inserir o número da tarefa antecessora seguida de &quot;e&quot;. Por exemplo, digite &quot;1e&quot; para adicionar a tarefa número 1 como antecessora da tarefa selecionada.
1. Clique em Enter para salvar as informações do antecessor da tarefa.

   ![predecessor_forced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
