---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Exibir: Objetos Resolvíveis em um Relatório de Tarefa ou Projeto"
description: Você pode exibir uma lista de todos os Objetos Resolvíveis em um projeto ou visualização de tarefa ou relatório.
author: Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Exibir: Objetos Resolvíveis em um relatório de tarefa ou de projeto

<!--Audited: 11/2024-->

Você pode exibir uma lista de todos os Objetos Resolvíveis em um projeto ou visualização de tarefa ou relatório.

Para obter mais informações sobre Objetos Resolvíveis, consulte o artigo [Visão Geral de Objetos Resolvíveis e Resolvíveis](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md).

![lista_de_contas_a_resolução_no_relatório.png](assets/list-of-resolvables-in-report-350x54.png)

A aplicação deste modo de exibição é idêntica para tarefas e projetos.

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

## Exibir Objetos Resolvíveis em um relatório de tarefa ou de projeto

1. Ir para uma lista de tarefas ou projetos que foram convertidos a partir de problemas.
1. No menu suspenso **Exibir**, clique em **Nova Exibição**.

1. Na área **Visualização da coluna**, clique em **Adicionar coluna**.

1. Clique no cabeçalho da nova coluna e em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. Clique em **Concluído** > **Salvar exibição**.\
   Uma lista de todos os Objetos Resolvíveis é exibida na nova coluna. Os nomes dos objetos na lista não podem ser vinculados diretamente aos objetos.
