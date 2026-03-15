---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes'
description: Você pode ter um status de tarefa atribuído ao Grupo A com o nome Novo status com a chave de três letras NST. Você pode ter outro status de tarefa atribuído ao Grupo B, também chamado Novo status com a chave de três letras NES. Embora os nomes dos dois status possam ser idênticos, o código de três letras é sempre exclusivo. Para obter mais informações sobre status de grupo, consulte Criar ou editar um status de grupo.
author: Courtney
feature: Reports and Dashboards
exl-id: 8ddcd8b1-44a9-4341-80c7-76ba70d2953b
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 11%

---

# Filtro: exibir itens por status de mesmo nome quando os status estão associados a grupos diferentes

<!--Audited: 10/2024-->

Você pode ter um status de tarefa atribuído ao Grupo A chamado *Novo Status* com a chave de três letras *NST*. Você pode ter outro status de tarefa atribuído ao Grupo B também chamado *Novo Status* com a chave de três letras *NES.* Embora os nomes dos dois status possam ser idênticos, o código de três letras é sempre exclusivo.

Para obter mais informações sobre status de grupo, consulte [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

Usando o construtor de filtros, você não pode identificar entre os dois status que têm o mesmo nome. Você deve usar o Modo de texto em um filtro personalizado para distinguir entre os dois status.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a filtros, exibições e agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir itens por status de mesmo nome quando os status estiverem associados a grupos diferentes

1. Vá para o menu suspenso **Filtro** do filtro que você deseja personalizar para uma lista de tarefas, por exemplo.\
   Isso funciona do mesmo modo em projetos e problemas.
1. Clique em **Novo filtro**.
1. Na primeira lista suspensa no canto superior esquerdo, selecione Tarefa > Status.
1. Selecione **Igual a** para o modificador e selecione um dos status sobre o qual deseja gerar um relatório.

   Por exemplo, em um relatório de tarefas, adicione **Status Igual a Novo Status**, se você deseja exibir apenas tarefas que estão em um status de **Novo Status**.

   >[!TIP]
   >
   >Observe que você tem apenas uma opção para um status chamado Novo status.

1. Clique em **Modo de Texto**.\
   O seguinte código deve ser exibido no espaço fornecido:

   <pre>OR:1:status=NST<br>OR:1:status_Mod=in </pre>

   >[!NOTE]
   >
   >Apenas um status é exibido aqui. A linha de status exibe uma das chaves de 3 letras para um dos status.

1. Adicione as 2 linhas de código a seguir para adicionar o status que está ausente no filtro:

   <pre>OR:2:status=NES<br>OR:2:status_Mod=in</pre>

1. Clique em **Aplicar** e em **Salvar como novo**.

   A lista exibe ambas as tarefas com um status de “Novo Status” do Grupo A e com um status de “Novo Status” do Grupo B.
