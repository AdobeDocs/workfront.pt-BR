---
product-area: home
navigation-topic: use-the-home-area
title: Gerencie seu trabalho com o widget Meu trabalho
description: O widget Meu trabalho exibe todas as tarefas, problemas e solicitações atribuídas a você em um único local. Aqui, você pode filtrar e organizar seu trabalho, registrar horas, fazer atualizações e marcar itens de trabalho como concluídos.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 09dd8d24d021e8a25b3a7a63fe93d074f8a8ee0c
workflow-type: tm+mt
source-wordcount: '704'
ht-degree: 5%

---


# Gerencie seu trabalho com o widget Meu trabalho

O widget Meu trabalho exibe todas as tarefas, problemas e solicitações atribuídas a você em um único local. Aqui, você pode filtrar e organizar seu trabalho, registrar horas, fazer atualizações e marcar itens de trabalho como concluídos.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença</strong></td> 
   <td> <p>Atual: Contribute</p>
   <p>Ou</p> 
   <p>Novo:[!UICONTROL Light] ou superior<p> 
  </td> 
  </tr> </ul>
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso a Projetos, Tarefas, Problemas e Documentos</p> </td> 
  </tr>  
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>permissões do Contribute ou superiores às tarefas e problemas nos quais você precisa trabalhar</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Encontre seu trabalho com filtros

Você pode ajustar os filtros Meu trabalho para se concentrar em itens específicos na lista de trabalho:

![](assets/filter-my-work-widget.png)

### Detalhes do filtro

<table>
  <tbody>
    <tr>
      <td>Trabalhando em</td>
      <td>Exibe itens nos quais você está trabalhando no momento</td>
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
      <li>A Data de Início Planejada mais de duas semanas no futuro</li>
      </ul>
       </td>
    </tr>
    <tr>
      <td>Solicitado</td>
      <td>Exibe problemas nos quais você não começou a trabalhar</td>
    </tr>
    <tr>
      <td>Delegado por mim</td>
      <td>Exibe itens que você delegou a outros usuários</td>
    </tr>
    <tr>
      <td>Delegado a mim</td>
      <td>Exibe itens que os usuários delegaram a você</td>
    </tr>
    <tr>
      <td>Concluídos</td>
      <td>Exibe o trabalho concluído nas últimas duas semanas. Essa opção de filtro não inclui aprovações.</td>
    </tr>
  </tbody>
</table>

>[!TIP]
>
>Se estiver procurando opções de filtragem mais específicas, você pode usar os widgets Minha tarefa ou Meu problema. Para obter mais informações sobre os filtros Minha tarefa e Meu problema, consulte [Visão geral dos novos filtros de widget da Página inicial](/help/quicksilver/workfront-basics/using-home/new-home/widget-filter-overview-new-home.md).

## Organize o seu trabalho

Você pode usar a classificação e os recursos de grupo do widget Meu trabalho para organizar seu trabalho de uma forma que faça sentido para você.

### Ordenar

Você pode classificar a lista de trabalho por

* Prazo
Os itens vencidos exibem um ícone de aviso ao lado da data. O Workfront usa a Data de conclusão planejada para determinar se as tarefas e os problemas estão vencidos.
* Nome
* Percentual concluído
* Status

>[!TIP]
>
>Para criar uma lista que exiba todos os itens em atraso na parte superior do widget Meu trabalho, classifique por Data de vencimento e não aplique um agrupamento.


![](assets/sort-my-work-widget.png)

### Grupo

Você pode agrupar a lista de trabalho por

* Projeto
* Status
* Prazo
A Data de vencimento é determinada pela Data de conclusão planejada.

>[!NOTE]
>
>Quando você aplica um agrupamento, sua seleção no menu Classificar determina a ordem dentro do agrupamento.


![](assets/group-my-work-widget.png)

## Atualizar informações do item de trabalho no Resumo

Você pode abrir o painel Resumo para atualizar rapidamente as informações em uma tarefa ou problema. No Resumo, é possível

* Atualizar o percentual concluído
* Adicionar uma atualização
* Navegue até a área Documento para fazer upload de um documento
* Exibir detalhes do item de trabalho e atualizar campos personalizados
Os administradores do Workfront podem personalizar quais campos aparecem no Resumo no modelo de layout. Para obter mais informações, consulte [Personalizar Início e Resumo usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md).
* Alterar o status do item de trabalho
* Exibir subtarefas
* Registrar de tempo
* Exibir processos de aprovação anexados

Para abrir o Resumo, passe o mouse sobre o item de trabalho e clique no ícone ![](assets/open-summary-new-home.png) de **Resumo**.

Para obter informações adicionais sobre como usar o painel Resumo, consulte [Visão geral do resumo](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md).

## Usar ações rápidas para atualizar itens de trabalho

Você pode usar o menu de ações rápidas para

* Registrar de tempo
* Adicionar uma atualização
* Atualizar um formulário personalizado
* Carregar um arquivo

Para localizar o menu de ações rápidas, passe o mouse sobre o item de trabalho. A lista de ações rápidas é exibida próximo ao botão **Trabalhar nisto** ou **Concluído**.

![](assets/quick-actions-new-home.png)


## Exibir aprovações e solicitações de equipe

Aprovações e solicitações de equipe não são exibidas no widget Meu trabalho. Se você trabalha regularmente com aprovações e solicitações de equipe, recomendamos adicionar os seguintes widgets à Nova página inicial:

* Aguardando minha aprovação
* Todas as aprovações
* Solicitações de equipe

Para obter informações sobre como adicionar widgets à Nova Página Inicial, consulte [Adicionar, editar ou remover widgets na Nova Página Inicial](/help/quicksilver/workfront-basics/using-home/new-home/add-edit-remove-widgets-in-new-home.md).




