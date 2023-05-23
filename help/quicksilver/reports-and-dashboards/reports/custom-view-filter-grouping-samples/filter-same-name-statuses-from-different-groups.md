---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes"
description: Você pode ter um status de tarefa atribuído ao Grupo A com o nome Novo status com a chave de 3 letras NST. Você pode ter outro status de tarefa atribuído ao Grupo B, também chamado Novo status com a chave de 3 letras NES. Embora os nomes dos dois status possam ser idênticos, o código de 3 letras é sempre exclusivo. Para obter mais informações sobre status de grupos, consulte Criar ou editar um status de grupo.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 0%

---

# Filtro: exibe itens por status de mesmo nome quando os status são associados a grupos diferentes

Você pode ter um status de tarefa atribuído ao Grupo A com nome *Novo Status* com a chave de 3 letras *NST*. Você pode ter outro status de tarefa atribuído ao Grupo B também chamado *Novo Status* com a chave de 3 letras *NES.* Embora os nomes dos dois status possam ser idênticos, o código de 3 letras é sempre exclusivo.\
Para obter mais informações sobre status de grupos, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Com o construtor de filtros, não é possível identificar entre os dois status que têm o mesmo nome. Você deve usar o Modo de texto para distinguir entre os dois status.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar um filtro </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes

1. Vá para o filtro que deseja personalizar para uma lista de tarefas, por exemplo.\
   Isso funciona do mesmo modo em projetos e problemas.
1. Clique em **Adicionar uma regra de filtro** para o **Status** do objeto da lista.\
   Por exemplo, em um relatório de tarefa, adicione **Status Igual a Novo Status**, se quiser exibir somente tarefas com status de **Novo Status**.

   >[!TIP]
   >
   >Observe que você tem apenas uma opção para um status chamado Novo status.

1. Clique em **Alternar para modo de texto**.\
   O código a seguir deve ser exibido:

   <pre xml:space="preserve">status=NST<br>status_Mod=in </pre>

   >[!NOTE]
   >
   >Somente um status é exibido aqui. A linha de status exibe uma das chaves de 3 letras para um dos status.

1. Adicione as 2 linhas de código a seguir para adicionar o status que está ausente no filtro:

   <pre>OU:1:status=NES<br>OU:1:status_Mod=in</pre>

1. Clique em **Concluído**, depois **Salvar Filtro**.

   A lista exibe ambas as tarefas com um status de &quot;Novo status&quot; do Grupo A e com um status de &quot;Novo status&quot; do Grupo B.
