---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: exibir a relação pai-filho em uma tarefa recuando as tarefas'''
description: É possível manter a distinção de relações pai-filho em uma lista de tarefas exportada adicionando uma exibição personalizada à lista de tarefas e garantindo que essa exibição seja selecionada antes de exportar a lista.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '161'
ht-degree: 1%

---

# Exibir: exibir a relação pai-filho em uma tarefa recuando as tarefas

É possível manter a distinção de relações pai-filho em uma lista de tarefas exportada adicionando uma exibição personalizada à lista de tarefas e garantindo que essa exibição seja selecionada antes de exportar a lista.  

![](assets/parent-child-indented-custom-view-350x94.png)

1. Vá para o projeto com a lista de tarefas que deseja exportar.
1. Clique no botão **Exibir** e selecione **Nova exibição**.

1. Nomeie o filtro no canto superior esquerdo da tela.
1. Clique no botão **Nome da tarefa** cabeçalho da coluna.

1. Selecionar **Alternar para o modo de texto** no canto superior direito.
1. Clique em qualquer lugar na caixa de texto para editar o texto e remover todo o texto existente.
1. Cole o seguinte texto:

   ```
   displayname=<br>linkedname=direct<br>namekey=name<br>querysort=name<br>textmode=true<br>valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))<br>valueformat=HTML
   ```

1. Clique em **Salvar**.
1. Clique em **Salvar exibição**.
