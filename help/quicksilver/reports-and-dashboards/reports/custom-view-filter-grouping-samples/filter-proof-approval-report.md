---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtro: relatório de aprovação de prova para omitir versões anteriores da prova'
description: Em um relatório Aprovação de prova, você pode usar o filtro É a versão atual do documento para incluir apenas as versões atuais das provas que estão aguardando sua aprovação.
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/0K5-65eWGsnej09HOH7yZKBDgANUPN1JThyGnkwt1kM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 378
ht-degree: 13%

---

# Filtro: relatório de aprovação de prova para omitir versões anteriores da prova

<!--Audited: 10/2024-->

Em um relatório de Aprovação de prova, você pode usar o filtro **É a versão atual do documento** para incluir apenas as versões atuais das provas que estão aguardando sua aprovação.

Isso é útil, por exemplo, se você foi solicitado a aprovar provas que têm várias versões. Quando você executa o relatório Aprovação de prova com o filtro É versão atual do documento, o relatório lista somente a versão atual de cada prova que está aguardando aprovação, omitindo versões anteriores nas quais você não precisa mais trabalhar.

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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Filtrar relatório Aprovação de prova para omitir versões de prova anteriores

É possível criar um filtro para um relatório Aprovação de prova.

1. Se você já tiver um relatório Aprovação de prova, abra-o.

   Ou

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   Para criar seu próprio relatório Aprovação de Prova, clique no **ícone do Menu Principal** ![ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito ou no **ícone do Menu Principal** ![linhas do Menu Principal](assets/lines-main-menu.png) no canto superior esquerdo, se disponível, e clique no **ícone Relatórios** ![Relatórios](assets/reports-in-main-menu.png).

1. Clique em **Novo Relatório**. A lista de tipos de objetos é exibida.
1. Clique em **Aprovação de prova** na lista.
O Report Builder é aberto.
1. Clique em **Filtros** e em **Adicionar uma Regra de Filtro**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. Clique dentro da caixa **Definir regras de filtro para seu relatório** e selecione **Aprovação de prova** na lista.
1. Clique em **Is Current Document Version** na lista sob o objeto **Aprovação de prova**.
1. Escolha Igual para o modificador de filtro e selecione True.
1. Clique em **Salvar + Fechar** no canto inferior esquerdo do Adobe Workfront e em **Aplicar** na caixa exibida.

   O relatório Aprovação de prova exibe somente as provas associadas às versões atuais de qualquer documento, se qualquer aprovação de prova corresponder a esse critério de filtragem.
