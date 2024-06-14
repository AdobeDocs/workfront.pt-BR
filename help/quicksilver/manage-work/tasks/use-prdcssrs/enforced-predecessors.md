---
product-area: projects
navigation-topic: use-predecessors
title: Forçar predecessores
description: Predecessoras são tarefas das quais outras tarefas dependem para serem concluídas. As relações predecessoras afetam as datas de início e conclusão das tarefas e afetam a linha do tempo do projeto.
author: Alina
feature: Work Management
exl-id: c3242b92-9036-4770-a073-2a9c393b97fd
source-git-commit: 5cb07cb42c3264c6629bc0a038c0e70ffc2cb509
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# Forçar predecessores

<!-- Audited: 2/2024 -->

Predecessoras são tarefas das quais outras tarefas dependem para serem concluídas. As relações predecessoras afetam as datas de início e conclusão das tarefas e afetam a linha do tempo do projeto.

Para obter informações sobre predecessores, consulte [Visão geral das predecessoras da tarefa](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Ao definir as relações de predecessoras entre tarefas, você define como o início ou o término de uma tarefa dependente depende do início ou do término de suas tarefas predecessoras. Isso é feito usando diferentes Tipos de dependência.

Para obter informações sobre Tipos de Dependência, consulte [Visão geral dos tipos de dependência de tarefa](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).

## Visão geral de predecessores aplicados

>[!IMPORTANT]
>
>Você deve impor predecessores para exigir que as relações predecessoras sejam respeitadas. Sem impor as predecessoras, as tarefas dependentes podem iniciar e terminar independentemente do início e do fim de suas predecessoras, independentemente de seus Tipos de Dependência.

Você pode impor a relação da predecessora ao definir predecessores em um projeto.

Se uma predecessora for imposta, a tarefa sucessora não poderá ser iniciada antes que a predecessora seja concluída. Por exemplo, impor uma relação Término-Início entre a Tarefa A e a Tarefa B significa que a Tarefa B não pode iniciar (o Status deve permanecer Novo e a Porcentagem Concluída deve permanecer 0%) até que a Tarefa A seja marcada como concluída. A imposição de relacionamentos se aplica a todos os tipos de predecessores.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
      <p>Novo: Padrão</p> 
      <p>OU</p>
      <p>Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a tarefas e projetos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td><p>Gerenciar permissões para as tarefas e o projeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Forçar um predecessor no nível da tarefa

1. Vá para a tarefa sucessora cujo antecessor você deseja impor.
1. Clique em **Predecessores** no painel esquerdo e clique em **Adicionar predecessor**. Talvez seja necessário clicar em **Mostrar mais**, depois **Predecessores**.
1. (Condicional) Se quiser adicionar um predecessor de projeto cruzado, remova o nome do projeto na **Projeto pai** e substitua-o por outro projeto.
1. Especifique o nome da(s) tarefa(s) predecessora(s) na **Tarefas** campo.
1. Especifique a **Tipo de Dependência** entre essas duas tarefas.

   O padrão **Tipo de Dependência** é **Término-Início**.

1. Selecione o **Reforçado** para aplicar o antecessor.
1. Clique em **Salvar**.

## Forçar um predecessor em uma lista de tarefas

1. Ir para uma lista de tarefas em um projeto.
1. No **Exibir** selecione a variável **Visualização Padrão**.

1. Tome nota mental do número de tarefas que você vai designar como o antecessor.
1. Localize a tarefa sucessora cujo antecessor você deseja impor.
1. No **Predecessores** , comece inserindo o número da tarefa predecessora seguido por &quot;e&quot;. Por exemplo, digite &quot;1e&quot; para adicionar a tarefa número 1 como predecessora da tarefa selecionada.
1. Clique em Enter para salvar as informações de sua predecessora da tarefa.

   ![predecessor_enforced_in_list.png](assets/predecessor-enforced-in-list-350x308.png)
