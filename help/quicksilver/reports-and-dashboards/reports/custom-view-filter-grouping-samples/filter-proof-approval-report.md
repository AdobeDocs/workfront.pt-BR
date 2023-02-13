---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '"Filtro: Relatório de aprovação de prova para omitir versões de prova anteriores'''
description: Em um relatório de Aprovação de prova, você pode usar o filtro É versão atual do documento para incluir apenas as versões atuais das provas que aguardam a aprovação.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# Filtro: relatório de aprovação de prova para omitir versões de prova anteriores

Em um relatório de Aprovação de prova , é possível usar a variável **É Versão do Documento Atual** filtro para incluir apenas as versões atuais das provas aguardando sua aprovação.

Isso é útil, por exemplo, se você tiver sido solicitado a aprovar provas que tenham várias versões. Quando você executa o relatório de Aprovação de prova com o filtro É a versão atual do documento, o relatório lista apenas a versão atual de cada prova aguardando sua aprovação, omitindo as versões anteriores nas quais você não precisa mais trabalhar. 

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

## Filtrar relatório de aprovação de prova para omitir versões de prova anteriores

1. Se você já tiver um relatório de Aprovação de prova, abra-o.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Para criar seu próprio relatório de Aprovação de prova, clique no Menu principal ![](assets/main-menu-icon.png), depois clique em **Relatórios** ![](assets/reports-in-main-menu.png). Clique em **Novo relatório**. Na lista exibida, procure e clique em **Aprovação de prova**. Clique em **Salvar + Fechar**, digite a **Nome do relatório** (opcional), em seguida, clique em **Salvar relatório**.

1. Clique em **Ações de relatório > Editar**.
1. Clique em **Filtros**, depois clique em **Adicionar uma regra de filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Clique em **Aprovação de prova**.
1. Na lista que aparece, clique em **É Versão do Documento Atual**.
1. Clique em **Salvar + Fechar** no canto inferior esquerdo do Adobe Workfront, em seguida, clique em **Salvar relatório** na caixa exibida.
