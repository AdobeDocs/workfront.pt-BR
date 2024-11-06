---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "View: Exibir o Relacionamento Pai-Filho em uma Tarefa Recuando as Tarefas"
description: Você pode manter a distinção de relacionamentos pai-filho em uma lista de tarefas exportada adicionando um modo de exibição personalizado à lista de tarefas e garantindo que esse modo de exibição seja selecionado antes de exportar a lista.
author: Nolan
feature: Reports and Dashboards
exl-id: 4987501f-a1d9-47cd-bfbe-83acfc225204
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 0%

---

# Exibição: exibir o relacionamento pai-filho em uma tarefa recuando as tarefas

<!--Audited: 11/2024-->

Você pode manter a distinção de relacionamentos pai-filho em uma lista de tarefas exportada adicionando um modo de exibição personalizado à lista de tarefas e garantindo que esse modo de exibição seja selecionado antes de exportar a lista.

![](assets/parent-child-indented-custom-view-350x94.png)

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p> Atual: 
   <ul>
   <li>Solicitação para modificar uma exibição</li> 
   <li>Planejar a modificação de um relatório</li>
   </ul>
     </p>
     <p> Novo: 
   <ul>
   <li>Colaborador para modificar uma visualização</li> 
   <li>Padrão para modificar um relatório</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir a relação pai-filho em uma tarefa recuando as tarefas

1. Vá para o projeto com a lista de tarefas que deseja exportar.
1. Clique no menu suspenso **Exibir** e selecione **Nova Exibição**.
1. Clique no cabeçalho da coluna **Nome da tarefa**.
1. Selecione **Alternar para Modo de Texto** no canto superior direito.
1. Clique em **Editar Modo de Texto** e remova todo o texto existente.
1. Cole o seguinte texto:


   ```
   displayname=
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(" - ",{name}),IF({indent}<3,CONCAT(" - - ",{name}),IF({indent}<4,CONCAT(" - - - ",{name}),CONCAT(" - - - - ",{name})))))
   valueformat=HTML
   ```

1. Clique em **Concluído** > **Salvar exibição**.
