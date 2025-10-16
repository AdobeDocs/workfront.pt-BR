---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: exibir somente itens em um status de aprovação'
description: Você pode exibir somente itens em um determinado status que está atualmente em Aprovação pendente. Isso funciona da mesma forma para qualquer outro objeto com status de aprovação.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '265'
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
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
