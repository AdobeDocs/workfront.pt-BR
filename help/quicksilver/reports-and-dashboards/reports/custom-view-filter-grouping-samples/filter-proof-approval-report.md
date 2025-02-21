---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filtro: relatório de aprovação de prova para omitir versões anteriores da prova'
description: Em um relatório Aprovação de prova, você pode usar o filtro É a versão atual do documento para incluir apenas as versões atuais das provas que estão aguardando sua aprovação.
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# Filtro: relatório Aprovação de prova para omitir versões de prova anteriores

<!--Audited: 10/2024-->

Em um relatório de Aprovação de prova, você pode usar o filtro **É a versão atual do documento** para incluir apenas as versões atuais das provas que estão aguardando sua aprovação.

Isso é útil, por exemplo, se você foi solicitado a aprovar provas que têm várias versões. Quando você executa o relatório Aprovação de prova com o filtro É versão atual do documento, o relatório lista somente a versão atual de cada prova que está aguardando aprovação, omitindo versões anteriores nas quais você não precisa mais trabalhar.

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
