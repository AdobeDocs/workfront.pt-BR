---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: exibir seus projetos atuais pendentes de aprovação'
description: O filtro de projeto a seguir exibe projetos no status Atual - Aprovação pendente, onde o usuário conectado é o Patrocinador do projeto ou o Gerente do Portfolio.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '197'
ht-degree: 0%

---

# Filtro: exibir seus projetos atuais pendentes de aprovação

<!--Audited: 10/2024-->

O filtro de projeto a seguir exibe projetos no status Atual - Aprovação pendente, onde o usuário conectado é o Patrocinador do projeto ou o Gerente do Portfolio.

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

## Filtrar projetos atuais com aprovação pendente

Para aplicar esse filtro:

1. Ir para uma lista de projetos.
1. No menu suspenso **Filtro**, selecione **Novo filtro**.

1. Clique em **Modo de texto**.
1. Na área exibida, copie e cole o seguinte código:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OR:a:status=CUR:A<br>OR:a:portfolio:ownerID=$$USER.ID</pre>

1. Clique em **Aplicar** > **Salvar como novo**.
