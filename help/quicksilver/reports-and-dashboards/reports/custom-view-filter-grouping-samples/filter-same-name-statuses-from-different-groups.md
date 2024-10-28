---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes"
description: Você pode ter um status de tarefa atribuído ao Grupo A com o nome Novo status com a chave de 3 letras NST. Você pode ter outro status de tarefa atribuído ao Grupo B, também chamado Novo status com a chave de 3 letras NES. Embora os nomes dos dois status possam ser idênticos, o código de 3 letras é sempre exclusivo. Para obter mais informações sobre status de grupos, consulte Criar ou editar um status de grupo.
author: Nolan
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 0%

---

# Filtro: exibe itens por status de mesmo nome quando os status são associados a grupos diferentes

<!--Audited: 10/2024-->

Você pode ter um status de tarefa atribuído ao Grupo A chamado *Novo status* com a chave de 3 letras *NST*. Você pode ter outro status de tarefa atribuído ao Grupo B também chamado *Novo status* com a chave de 3 letras *NES.* Embora os nomes dos 2 status possam ser idênticos, o código de 3 letras é sempre exclusivo.

Para obter mais informações sobre status de grupo, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Com o construtor de filtros, não é possível identificar entre os dois status que têm o mesmo nome. Você deve usar o Modo de texto em um filtro personalizado para distinguir os dois status.

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador para modificar um filtro </p></li>
   <li><p>Padrão para modificar um relatório</p></li> </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação para modificar um filtro </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes

1. Vá para o menu suspenso **Filtro** do filtro que você deseja personalizar para uma lista de tarefas, por exemplo.\
   Isso funciona do mesmo modo em projetos e problemas.
1. Clique em **Novo filtro**.
1. Na primeira lista suspensa no canto superior esquerdo, selecione Tarefa > Status.
1. Selecione **Igual** para o modificador e selecione um dos status que deseja relatar.

   Por exemplo, em um relatório de tarefa, adicione **Status Igual a Novo Status**, se desejar exibir somente tarefas que estejam no status **Novo Status**.

   >[!TIP]
   >
   >Observe que você tem apenas uma opção para um status chamado Novo status.

1. Clique em **Modo de texto**.\
   O código a seguir deve ser exibido no espaço fornecido:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Somente um status é exibido aqui. A linha de status exibe uma das chaves de 3 letras para um dos status.

1. Adicione as 2 linhas de código a seguir para adicionar o status que está ausente no filtro:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Clique em **Aplicar** e em **Salvar como novo**.

   A lista exibe ambas as tarefas com um status de &quot;Novo status&quot; do Grupo A e com um status de &quot;Novo status&quot; do Grupo B.
