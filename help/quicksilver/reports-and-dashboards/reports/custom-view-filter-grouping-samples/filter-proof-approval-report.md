---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Filtro: relatório Aprovação de prova para omitir versões de prova anteriores"
description: Em um relatório Aprovação de prova, você pode usar o filtro É a versão atual do documento para incluir apenas as versões atuais das provas que estão aguardando sua aprovação.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '356'
ht-degree: 0%

---

# Filtro: relatório Aprovação de prova para omitir versões de prova anteriores

Em um relatório Aprovação de prova, você pode usar o **É a versão atual do documento** filtro para incluir somente as versões atuais das provas que estão aguardando sua aprovação.

Isso é útil, por exemplo, se você foi solicitado a aprovar provas que têm várias versões. Quando você executa o relatório Aprovação de prova com o filtro É versão atual do documento, o relatório lista somente a versão atual de cada prova que está aguardando aprovação, omitindo versões anteriores nas quais você não precisa mais trabalhar. 

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

## Filtrar relatório Aprovação de prova para omitir versões de prova anteriores

1. Se você já tiver um relatório Aprovação de prova, abra-o.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Para criar seu próprio relatório Aprovação de prova, clique no menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em **Relatórios** ![](assets/reports-in-main-menu.png). Clique em **Novo Relatório**. Na lista exibida, role até e clique em **Aprovação da prova**. Clique em **Salvar + Fechar**, digite um **Nome do relatório** (opcional) e clique em **Salvar relatório**.

1. Clique em **Ações de Relatório > Editar**.
1. Clique em **Filtros** e, em seguida, clique em **Adicionar uma regra de filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Clique em **Aprovação da prova**.
1. Na lista exibida, clique em **É a versão atual do documento**.
1. Clique em **Salvar + Fechar** no canto inferior esquerdo do Adobe Workfront, clique em **Salvar relatório** na caixa exibida.
