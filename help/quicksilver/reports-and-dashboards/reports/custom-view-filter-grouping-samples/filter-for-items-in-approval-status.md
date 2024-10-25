---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: exibir somente itens em um status de aprovação"
description: Você pode exibir somente itens em um determinado status que está atualmente em Aprovação pendente. Isso funciona da mesma forma para qualquer outro objeto com status de aprovação.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 1%

---

# Filtro: exibir somente itens em um status de aprovação

<!--Audited: 10/2024-->

Você pode exibir somente itens em um determinado status que está atualmente em Aprovação pendente. Isso funciona da mesma forma para qualquer outro objeto com status de aprovação.

Você pode colocar os seguintes objetos em um status de aprovação:

* Tarefas
* Problemas
* Projetos

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

## Exibir somente itens no status de aprovação

1. Ir para uma lista de projetos.
1. No menu suspenso **Filtro**, selecione **Novo filtro**.
1. Escolha filtrar por **Projeto: Status** e selecione o status que deseja filtrar na lista.

   Por exemplo, em um relatório de projeto, adicione **Status Igual a Planejamento**, se desejar exibir somente projetos com status **Planejamento - Aprovação Pendente**.
1. Clique em **Modo de texto**.
1. Modifique a linha `status` adicionando **:A** à chave de 3 letras do status:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Clique em **Aplicar** > **Salvar como novo**.

   A lista exibe somente projetos com status Planejamento - Aprovação Pendente.
