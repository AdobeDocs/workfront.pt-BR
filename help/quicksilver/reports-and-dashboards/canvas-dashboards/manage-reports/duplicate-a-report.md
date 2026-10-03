---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Copiar e mover relatórios nos Painéis do Canvas
description: Você pode copiar ou mover um relatório entre Painéis do Canvas.
author: Courtney
feature: Reports and Dashboards
exl-id: e0f9d091-bb89-4c5b-a18d-b1e339084e67
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/5ioNl-M-KgnYE0huAbxMmLlE-qIrnwwKp-eeTRRiYLo'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: c6dd2ac5-f5bd-4e59-9101-25b156918623
    internal-label: Reports and dashboards
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 45491118778279522358f87c1c4185c4cf824829
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 12%
---
# Copiar e mover relatórios nos Painéis do Canvas

{{highlighted-preview}}

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Falar com o suporte ao cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

Você pode duplicar um relatório de KPI, tabela ou gráfico em um Painel da tela após sua criação. Após a duplicação, é possível editar o relatório conforme necessário antes de salvar.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> 
<p>Padrão </p> 
<p>Plano</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurações de nível de acesso</p></td> 
   <td><p>Editar acesso a relatórios, painéis e calendários</p>
  </td> 
  </tr>  
      <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Gerenciar permissões do painel</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

É necessário adicionar um relatório a um painel antes de duplicá-lo.

Para obter mais informações, consulte [Criar um painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Duplicação de um relatório na produção

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.
1. Na página **Painéis da Tela**, clique no ícone **Mais** ![Mais](assets/more-icon.png) no canto superior direito do relatório que você deseja duplicar e selecione **Duplicar**.

   ![Botão duplicado](assets/duplicate-button.png)

1. (Opcional) Na caixa **Configurar** exibida, insira um novo relatório **Nome** na guia **Detalhes**.

1. (Opcional) Faça os ajustes necessários nas configurações usando as guias no lado esquerdo.

   >[!NOTE]
   >
   >Essas guias variam dependendo se você duplicou um relatório de KPI, tabela ou gráfico.  Para obter mais informações, consulte [Criar um relatório de KPI em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md), [Criar um relatório de gráfico em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) e [Criar um relatório de tabela em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

1. Clique em **Salvar**. O relatório duplicado é exibido no painel.

<div class="preview">

## Copiar ou mover um relatório na Visualização

Você pode copiar um relatório para o painel atual, copiá-lo para outro painel ou movê-lo para outro painel. Copiar cria uma duplicata do relatório no destino; mover realoca-o do painel atual.

>[!IMPORTANT]
>
>* Para copiar um relatório, você precisa de permissões de Gerenciamento para o painel de destino.
>* Para mover um relatório, você precisa do acesso de Gerenciar aos painéis de origem e destino.
>* Se o relatório tiver uma configuração Executar como usuário e você não for um Administrador do sistema ou o Executar como usuário, você ainda poderá copiá-lo ou movê-lo, mas a opção Executar como usuário será removida do relatório resultante.


Para copiar ou mover um relatório:

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.
1. Abra o painel que contém o relatório.
1. Clique no ícone do **Mais** ![Mais botão](assets/more-icon.png) no canto superior direito do relatório e selecione **Copiar relatório**.

   ![Opção Copiar relatório](assets/copy-report-button.png)

1. Na caixa de diálogo **Copiar relatório**, escolha uma das seguintes opções:

   <table>
   <tr>
   <td><strong>Copiar</strong></td>
   <td>Clique em <strong>Copiar</strong> na parte inferior da tela para copiar o relatório. O painel atual é selecionado por padrão. Você precisa de acesso de Gerenciar ao painel para copiar um relatório.</td>
   </tr>
   <tr>
   <td><strong>Copiar e mover</strong></td>
   <td>Selecione um painel de destino diferente para copiar o relatório e movê-lo para um novo painel. O relatório original permanece no painel atual.Você precisa de acesso de Gerenciamento ao painel de destino para copiar e mover um relatório. </td>
   </tr>
   <tr>
   <td><strong>Mover</strong></td>
   <td>Selecione um painel de destino diferente para o qual mover o relatório. Isso realoca o relatório no painel de destino e o remove do painel atual. Você precisa de acesso de Gerenciar aos painéis de origem e destino para mover um relatório.</td>
   </tr>
   </table>

   >[!NOTE]
   >
   >Se o relatório tiver uma configuração Executar como usuário e você não for um Administrador do sistema ou o usuário definido como Executar como usuário, você ainda poderá copiar ou mover o relatório. A opção Executar como usuário é removida do relatório resultante.

1. Clique em **Salvar**.

   ![copiar e mover](assets/copy-and-move.png)

</div>
