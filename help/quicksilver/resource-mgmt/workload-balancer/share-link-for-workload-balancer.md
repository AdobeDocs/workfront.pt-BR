---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Compartilhar o Balanceador de Carga de Trabalho com um link
description: Você pode compartilhar o Balanceador de Carga de Trabalho com outros usuários que talvez não tenham a área de Recursos disponível para eles. Para obter informações sobre o uso do Balanceador de Carga de Trabalho, consulte Navegar no Balanceador de Carga de Trabalho.
author: Alina
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: a74cc358c547e11a55cce728ad5330712ed0bd49
workflow-type: tm+mt
source-wordcount: '711'
ht-degree: 0%

---

# Compartilhar o Balanceador de Carga de Trabalho com um link

Você pode compartilhar o Balanceador de Carga de Trabalho com outros usuários que talvez não tenham a área de Recursos disponível para eles. Para obter informações sobre como usar o Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Planejar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso ao seguinte:</p> 
    <ul> 
     <li> <p>Gerenciamento de recursos</p> </li> 
     <li> <p>Projetos</p> </li> 
     <li> <p>Tarefas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Visualizar ou exibir permissões mais altas para projetos, tarefas e problemas </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Informações incluídas no Balanceador de Carga de Trabalho ao visualizá-lo a partir de um link compartilhado

Quando você compartilha um link para o Balanceador de carga de trabalho com outros usuários, as seguintes informações são incluídas com o link compartilhado:

* A área Trabalho Atribuído do Balanceador de Carga de Trabalho.
* Projeto, tarefa, informações do usuário. Isso inclui as informações de alocação do usuário.
* As informações são exibidas de acordo com o filtro selecionado.

   >[!IMPORTANT]
   >
   >Se você excluir os filtros depois de compartilhar o link, os usuários que visualizam o Balanceador de carga de trabalho do link receberão um aviso de que os filtros foram excluídos. Eles exibem todos os usuários na área de Trabalho atribuído. Esta é a exibição padrão do Balanceador de Carga de Trabalho.

* O número de semanas selecionadas anteriormente.

As seguintes opções estão disponíveis para o usuário que visualiza o Balanceador de carga de trabalho de um link compartilhado para se atualizar:

* As seguintes seleções de linha do tempo:

   * Hoje
   * Ícones de trás e de frente
   * Seleção de calendário

* Os ícones Dia, Semana e Mês
* O ícone Configurações
* O ícone Mostrar alocações

   Para obter informações sobre como usar essas opções, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* O ícone Mostrar alocações de função

   Isso está disponível somente para o Balanceador de Carga de Trabalho de um projeto.

O usuário que recebe o link compartilhado não pode fazer o seguinte no Balanceador de Carga de Trabalho deste link:

* Atribuir itens de trabalho aos usuários
* Gerenciar alocações de usuário
* Criar filtros novos ou atualizar filtros aplicados originalmente

## Acesso necessário para exibir informações no Balanceador de Carga de Trabalho a partir de um link compartilhado

Você precisa do seguinte acesso para exibir informações no Balanceador de Carga de Trabalho de um link compartilhado:

* Uma licença válida do Adobe Workfront e você deve estar conectado ao Workfront.
* Pelo menos, visualize o acesso ao Gerenciamento de recursos em seu Nível de acesso. Para obter informações sobre a concessão de acesso ao Gerenciamento de Recursos, consulte [Conceder acesso ao gerenciamento de recursos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Exiba permissões para projetos, tarefas, problemas e usuários exibidos no Balanceador de Carga de Trabalho.

## Compartilhar o Balanceador de Carga de Trabalho com outros usuários de um link

1. Vá para o Balanceador de Carga de Trabalho

   Para obter informações sobre como acessar o Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Opcional) Siga um ou mais destes procedimentos:

   * Atualizar a seleção do período de tempo.
   * Clique em **Dia, Semana** ou **Mês** para exibir informações diárias, semanais ou mensais.

      ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Aplique filtros às áreas de Trabalho Atribuído e Não Atribuído.

      Para obter informações sobre filtragem no Balanceador de Carga de Trabalho, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Clique no botão **ícone de link** ![](assets/wb-shearable-link-icon-small.png).

   Isso adiciona o link à área de transferência.

1. Siga um destes procedimentos para compartilhar o link com outras pessoas:

   * Cole-o em um email, mensagem de bate-papo ou qualquer outro aplicativo e compartilhe-o com outros usuários.
   * Adicione-a a uma seção personalizada como uma página externa, adicione a seção personalizada ao perfil de um usuário ou a um Modelo de layout e, em seguida, compartilhe o Modelo de layout com usuários, equipes, funções de trabalho ou grupos.

      Para obter informações sobre como criar uma Página Externa, consulte [Incorporar uma página da Web externa em um painel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Para obter informações sobre como adicionar seções personalizadas a um modelo de layout, consulte [Personalizar o painel esquerdo usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

      >[!IMPORTANT]
      >
      >Quando você adiciona o Balanceador de Carga de Trabalho à seção personalizada de um objeto, as informações no Balanceador de Carga de Trabalho não são filtradas pelo objeto. O Balanceador de Carga de Trabalho exibe as informações filtradas pelos filtros aplicados originalmente.
