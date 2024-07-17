---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: elimine itens em uma lista comparando dois campos"
description: É possível filtrar itens de uma lista comparando dois de seus campos. Por exemplo, você pode exibir somente tarefas em que a Data de Término Efetivo da tarefa seja maior que a Data de Término Planejada.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 0%

---

# Filtro: elimine itens em uma lista comparando dois campos

É possível filtrar itens de uma lista comparando dois de seus campos. Por exemplo, você pode exibir somente tarefas em que a Data de Término Efetivo da tarefa seja maior que a Data de Término Planejada.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
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
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Filtrar itens comparando dois campos

1. Ir para uma lista de tarefas.
1. No menu suspenso **Filtro**, selecione **Novo Filtro**.

1. Clique em **Adicionar Regra de Filtro** e adicione **Data de Término Efetivo** >**Maior que** > **Selecione uma data**.

   >[!TIP]
   >
   >Escolha o modificador de filtro que deseja usar para o campo selecionado, se disponível.

1. Clique em **Alternar para Modo de Texto**.
1. Na área **Definir Regras de Filtro para seu Relatório**, adicione o seguinte código:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Clique em **Concluído** e em **Salvar filtro**.
