---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: exibir apenas itens em status de aprovação'
description: Você pode exibir somente itens em um determinado status que esteja atualmente em Aprovação Pendente. Isso funciona da mesma forma para qualquer outro objeto com um status de aprovação.
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 22%

---

# Filtro: exibir apenas itens em status de aprovação

<!--Audited: 10/2024-->

Você pode exibir somente itens em um determinado status que esteja atualmente em Aprovação Pendente. Isso funciona da mesma forma para qualquer outro objeto com um status de aprovação.

Você pode colocar os seguintes objetos em um status de aprovação:

* Tarefas
* Problemas
* Projetos

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
   <p>Colaborador ou solicitação para modificar um filtro </p>
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

## Exibir somente itens no status de aprovação

1. Ir para uma lista de projetos.
1. No menu suspenso **Filtro**, selecione **Novo filtro**.
1. Escolha filtrar por **Projeto: Status** e selecione o status pelo qual deseja filtrar na lista.

   Por exemplo, em um relatório de projeto, adicione **Status Igual ao Planning**, se desejar exibir apenas projetos com status **Planejamento - Aprovação Pendente**.
1. Clique em **Modo de texto**.
1. Modifique a linha `status` adicionando **:A** à chave de 3 letras do status:
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. Clique em **Aplicar** > **Salvar como novo**.

   A lista exibe apenas os projetos que estão no status Planejamento - Aprovação Pendente.
