---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibição: exibir o relacionamento pai-filho em uma tarefa recuando as tarefas"
description: Você pode manter a distinção de relacionamentos pai-filho em uma lista de tarefas exportada adicionando um modo de exibição personalizado à lista de tarefas e garantindo que esse modo de exibição seja selecionado antes de exportar a lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 1%

---

# Exibição: exibir o relacionamento pai-filho em uma tarefa recuando as tarefas

Você pode manter a distinção de relacionamentos pai-filho em uma lista de tarefas exportada adicionando um modo de exibição personalizado à lista de tarefas e garantindo que esse modo de exibição seja selecionado antes de exportar a lista.

![](assets/parent-child-indented-custom-view-350x94.png)

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
   <td> <p>Solicitação para modificar uma exibição </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Exibir a relação pai-filho em uma tarefa recuando as tarefas

1. Vá para o projeto com a lista de tarefas que deseja exportar.
1. Clique em **Exibir** e selecione **Nova visualização**.

1. Nomeie o filtro no canto superior esquerdo da tela.
1. Clique em **Nome da tarefa** cabeçalho da coluna.

1. Selecionar **Alternar para modo de texto** no canto superior direito.
1. Clique em qualquer lugar na caixa de texto para editar o texto e remover todo o texto existente.
1. Cole o seguinte texto:

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Clique em **Salvar**.
1. Clique em **Salvar visualização**.
