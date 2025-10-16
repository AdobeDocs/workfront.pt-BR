---
navigation-topic: get-started-with-workfront
title: Gerenciar seu trabalho no calendário Prioridades
description: Acompanhe seu trabalho com um calendário visual e claro.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: d24ad7d1-3a88-479e-beaf-69f8264c9a6b
source-git-commit: 0940e4c89de6cd3518cd98a1e06dc726f434846b
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 4%

---

# Gerenciar seu trabalho no calendário Prioridades

Acompanhe facilmente seu trabalho com um calendário visual claro. Com o calendário Prioridades, você pode

* Use filtros para encontrar seu trabalho
* Aplique campos personalizados como status e nível de foco para identificar trabalhos de alta prioridade
* Aplicar cores para organização rápida

>[!IMPORTANT]
>
>Os projetos devem estar no status Atual ou em um status que seja igual a atual para que possam exibir os projetos, bem como suas tarefas e problemas secundários.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Revisor ou superior</p>
   <p>Leve ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de Visualização ou Edição para o objeto no qual a atualização está</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar acesso ao objeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir seu trabalho no calendário

Prioridades exibe os itens de trabalho atribuídos a você. Não é possível ver os itens de trabalho atribuídos à sua equipe no calendário de Prioridades.

{{step1-to-priorities}}

1. Clique no ícone **Calendário** na parte superior da lista de trabalho.
   ![ícone do calendário](assets/calendar-tab.png)
1. Selecione um ou mais filtros para restringir seus itens de trabalho.

   +++Expanda para ver informações detalhadas sobre filtros disponíveis
   <table>
    <tbody>
    <tr>
    <th>Filtro</th>
    <th>Descrição</th>
    </tr>
        <tr>
        <td>Em desenvolvimento</td>
        <td>Exibe itens nos quais você está trabalhando no momento.</td>
        </tr>
        <tr>
        <td>Pronto para iniciar</td>
        <td>Exibe itens com 
        <ul>
        <li>Sem predecessores incompletos ou restrições de tarefa</li>
        <p>e</p>
        <li>A Data de Início Planejada está no passado ou em até duas semanas no futuro</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Não está pronto</td>
        <td>Exibe itens que possuem
        <ul>
        <li>Predecessoras incompletas ou restrições de tarefa que impedem o trabalho no item</li>
        <p>ou</p>
        <li>A Data de Início Planejada mais de duas semanas no futuro.</li>
        </ul>
        </td>
        </tr>
        <tr>
        <td>Solicitado</td>
        <td>Exibe problemas nos quais você não começou a trabalhar.</td>
        </tr>
        <td>Concluído</td>
        <td>Exibe o trabalho concluído nas últimas duas semanas. Essa opção de filtro não inclui aprovações.</td>
        </tr>
        <tr>
        <td>Projeto</td>
        <td>Exibe projetos que contêm tarefas ou problemas aos quais você foi atribuído.</td>
        </tr>
        <tr>
        <td>Data final</td>
        <td>Exibe o trabalho pela Data de conclusão planejada.</td>
        </tr>
        <tr>
        <td>Status</td>
        <td>Exibe tarefas ou problemas nos status novo, em andamento e concluído.</td>
        </tr>
        <tr>
        <td>Meu foco</td>
        <td>Exibe tarefas ou problemas no que têm níveis de foco atribuídos. Os níveis de foco são atribuídos e gerenciados pelo usuário individual.</td>
        </tr>
    </tbody>
    </table>

   +++

1. Clique na barra de itens de trabalho no calendário para abrir o resumo lateral. O resumo lateral permite

   * Exibir e editar detalhes do projeto e do item de trabalho
   * Fazer e exibir comentários
   * Visualizar e carregar documentos
   * Criar uma prova
   * Acesse a página do projeto no Workfront
   * Navegue até a página de detalhes do item de trabalho em Prioridades
   * Registrar de tempo
   * Adicionar links rápidos

1. (Opcional) Clique em **Criar novo** para adicionar um novo item de trabalho ao calendário. Para obter mais informações, consulte [Criar uma nova tarefa ou problema em Prioridades](/help/quicksilver/workfront-basics/priorities/create-task-issue-priorities.md).

## Configurar o calendário

{{step1-to-priorities}}

1. Clique no ícone **Calendário** na parte superior da lista de trabalho.
   ![ícone do calendário](assets/calendar-tab.png)
1. Clique no ícone **Configurações** no canto direito do calendário.

1. Na guia **Estilo da barra**, escolha até 5 campos para exibir na barra de itens de trabalho do calendário.
   ![barra de exemplo](assets/sample-task-for-field-config.png)

1. Na guia **Cor**, escolha como deseja que seus itens de trabalho sejam exibidos. Por exemplo, se você escolher **Projeto**, seus itens de trabalho serão exibidos de acordo com a cor atribuída ao projeto na lista de trabalho.
   ![projeto de cores de amostra](assets/sample-calendar-projects.png)
