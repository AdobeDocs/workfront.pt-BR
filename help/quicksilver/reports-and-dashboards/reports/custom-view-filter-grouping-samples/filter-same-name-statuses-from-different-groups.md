---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filtro: exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes'
description: Você pode ter um status de tarefa atribuído ao Grupo A chamado Novo Status com a chave de 3 letras NST. Você pode ter outro status de tarefa atribuído ao Grupo B também chamado Novo Status com a chave de 3 letras NES. Embora os nomes dos dois status possam ser idênticos, o código de 3 letras é sempre único. Para obter mais informações sobre status de grupo, consulte Criar ou editar um status de grupo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '471'
ht-degree: 0%

---

# Filtro: exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes

Você pode ter um status de tarefa atribuído ao Grupo A nomeado *Novo status* com a tecla de 3 letras *NST*. Você pode ter outro status de tarefa atribuído ao Grupo B também nomeado *Novo status* com a tecla de 3 letras *NES.* Embora os nomes dos dois status possam ser idênticos, o código de 3 letras é sempre único.\
Para obter mais informações sobre status de grupo, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Usando o construtor de filtros, não é possível identificar entre os dois status que têm o mesmo nome. Você deve usar o Modo de texto para distinguir entre os dois status.

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
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes

1. Vá para o filtro que deseja personalizar para obter uma lista de tarefas, por exemplo.\
   Isso também funciona para projetos e problemas.
1. Clique em **Adicionar uma regra de filtro** para **Status** do objeto da lista.\
   Por exemplo, em um relatório de tarefa, adicione **Status Igual a Novo Status**, se desejar exibir apenas tarefas que estão em um status de **Novo status**.

   >[!TIP]
   >
   >Observe que você tem apenas uma opção para um status chamado Novo status.

1. Clique em **Alternar para o modo de texto**.\
   O código a seguir deve ser exibido:

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Somente um status é exibido aqui. A linha de status exibe uma das chaves de 3 letras para um dos status.

1. Adicione as 2 linhas de código a seguir para adicionar o status que está faltando no filtro:

   <pre>OU:1:status=NES<br>OU:1:status_Mod=in</pre>

1. Clique em **Concluído**, em seguida **Salvar filtro**.

   A lista exibe ambas as tarefas com o status &quot;Novo status&quot; do Grupo A e com o status &quot;Novo status&quot; do Grupo B.
