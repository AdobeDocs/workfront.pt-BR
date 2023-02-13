---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filtro: eliminar itens em uma lista comparando dois campos'''
description: Você pode filtrar itens fora de uma lista comparando dois de seus campos. Por exemplo, você pode exibir apenas tarefas em que a Data de conclusão real da tarefa é maior que a Data de conclusão planejada.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '273'
ht-degree: 0%

---

# Filtro: eliminar itens em uma lista comparando dois campos

Você pode filtrar itens fora de uma lista comparando dois de seus campos. Por exemplo, você pode exibir apenas tarefas em que a Data de conclusão real da tarefa é maior que a Data de conclusão planejada.

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

## Filtrar itens comparando dois campos

1. Vá para uma lista de tarefas.
1. No **Filtro** , selecione **Novo filtro**.

1. Clique em **Adicionar regra de filtro** e adicionar **Data de conclusão real** >**Maior que** > **Selecionar uma data**.

   >[!TIP]
   >
   >Escolha o modificador de filtro que deseja usar para o campo selecionado, se disponível.

1. Clique em **Alternar para o modo de texto**.
1. No **Definir regras de filtro para seu relatório** , adicione o seguinte código:

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. Clique em **Concluído**, em seguida **Salvar filtro**.
