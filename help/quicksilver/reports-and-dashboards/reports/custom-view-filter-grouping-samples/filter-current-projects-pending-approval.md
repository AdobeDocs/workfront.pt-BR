---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: exibir seus projetos atuais pendentes de aprovação"
description: O filtro de projeto a seguir exibe projetos no status Atual - Aprovação pendente, onde o usuário conectado é o Patrocinador do projeto ou o Gerente de Portfolio.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 32045aec-acc5-44d2-bad5-7759dc797414
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 0%

---

# Filtro: exibir seus projetos atuais pendentes de aprovação

O filtro de projeto a seguir exibe projetos no status Atual - Aprovação pendente, onde o usuário conectado é o Patrocinador do projeto ou o Gerente de Portfolio.

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
   <td> <p>Solicitação para modificar um filtro </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Filtrar projetos atuais com aprovação pendente

Para aplicar esse filtro:

1. Ir para uma lista de projetos.
1. No **Filtro** selecione **Novo Filtro**.

1. Clique em **Alternar para modo de texto**.
1. No **Definir regras de filtro para seu relatório** , copie e cole o seguinte código:
   <pre>status=CUR:A<br>sponsorID=$$USER.ID<br>OU:a:status=CUR:A<br>OU:a:portfolio:ownerID=$$USER.ID</pre>

1. Clique em **Salvar Filtro**.
