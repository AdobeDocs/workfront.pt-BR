---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filtro: exibir os projetos atuais com aprovação pendente'''
description: O filtro de projeto a seguir exibe os projetos no status Atual - Aprovação pendente , onde o usuário conectado é o Patrocinador do projeto ou o Gerente de Portfolio.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 0%

---

# Filtro: exibir os projetos atuais com aprovação pendente

O filtro de projeto a seguir exibe os projetos no status Atual - Aprovação pendente , onde o usuário conectado é o Patrocinador do projeto ou o Gerente de Portfolio.

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

## Filtrar projetos atuais pendentes de aprovação

Para aplicar este filtro:

1. Acesse uma lista de projetos.
1. No **Filtro** , selecione **Novo filtro**.

1. Clique em **Alternar para o modo de texto**.
1. No **Definir regras de filtro para seu relatório** , copie e cole o seguinte código:
   <pre>status=CUR:A<br>patrosorID=$$USER.ID<br>OU:a:status=CUR:A<br>OU:a:portfólio:ownerID=$$USER.ID</pre>

1. Clique em **Salvar filtro**.
