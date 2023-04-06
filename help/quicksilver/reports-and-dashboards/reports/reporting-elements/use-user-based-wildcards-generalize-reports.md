---
product-area: reporting
navigation-topic: reporting-elements
title: Usar curingas baseadas em usuário para generalizar relatórios
description: Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: 216e2869-b4f8-4cc7-9497-a12ebe00fe49
source-git-commit: 302771f4d64b386149623f87a3436d0c40f421d5
workflow-type: tm+mt
source-wordcount: '508'
ht-degree: 0%

---

# Usar curingas baseadas em usuário para generalizar relatórios

Você pode generalizar um relatório usando curingas em vez de informações específicas ao criar determinados elementos de relatório. Por exemplo, se você quiser criar um relatório que mostre as tarefas atribuídas a um usuário específico, poderá usar o nome do usuário no campo Atribuído a do filtro. No entanto, se você quiser criar um relatório que mostre as tarefas atribuídas ao usuário conectado, independentemente de quem seja esse usuário, poderá usar um curinga que indica que, quando alguém exibir o relatório, exibirá informações pertencentes somente a ele. Dessa forma, você cria o relatório uma vez, mas, como você usa um curinga no filtro, ele produz resultados diferentes sempre que outra pessoa o ler.

Você pode usar curingas com base no usuário ao criar os seguintes elementos de relatório:

* Filtros
* Solicitações personalizadas
* Exibições ao adicionar regras para colunas

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para editar elementos de relatório em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para editar elementos de relatório em um relatório</p> <p>Gerencie permissões em uma visualização ou filtro para editá-las</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Você deve criar um relatório antes de poder adicionar uma variável curinga a ele.

Para obter instruções sobre como criar relatórios, consulte [Criar um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md).

## Etapas de instruções

Para inserir um curinga baseado em usuário em um relatório:

1. Vá para um relatório para o qual deseja inserir um curinga baseado em usuário.
1. Clique em **Ações de Relatório**, em seguida **Editar**.

1. Clique no botão **Filtros** guia .
1. Clique em **Adicionar uma regra de filtro**.
1. Comece digitando o nome do campo que deseja filtrar.\
   Você deve digitar campos que fazem referência ao objeto do usuário ou informações sobre usuários.
1. Selecionar **Igual** no menu suspenso da variável de filtro.

   >[!TIP]
   >
   >Você sempre deve selecionar a variável **Igual** variável de filtro ao trabalhar com curingas no Adobe Workfront.

1. No **Começar a digitar nome ...** caixa, tipo: `$$USER.ID` ou `$$USER.name` se desejar que o relatório exiba informações sobre o usuário que faz logon, com base em seu nome. Você pode inserir outros curingas que se referem ao Grupo, Equipe, Empresa ou outras informações do usuário conectado.

   Para obter uma lista completa de curingas com base em usuários, consulte [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

   ![](assets/user-based-wildcard-in-project-filter-350x74.png)

1. Clique em **Salvar + Fechar**.

## Informações adicionais

Consulte também:

* [Programa básico de criação de relatórios](https://one.workfront.com/s/basic-report-creation-program)
* [Variáveis de filtro curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md)
* [Criar ou editar filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
* [Visão geral dos filtros no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
* [Adicionar um prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md)
* [Usar formatação condicional em exibições](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md)
