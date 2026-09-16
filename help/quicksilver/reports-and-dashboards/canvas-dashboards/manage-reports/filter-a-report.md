---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrar um relatório em um painel da tela
description: Adicione ou edite um filtro em um relatório para controlar quais dados são exibidos em um Painel da tela.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 15%
---
# Filtrar um relatório em um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Falar com o suporte ao cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

Você pode filtrar um relatório para controlar quais dados são exibidos ao criar o relatório e a qualquer momento depois. As opções de filtragem e o comportamento são os mesmos em ambos os casos.

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
<p>Padrão</p> 
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

Você deve ter um relatório em um painel, ou estar criando um, antes de poder filtrá-lo. Para obter mais informações, consulte [Criar um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Adicionar ou editar um filtro de relatório

Para adicionar ou editar um filtro em um relatório:

1. Abra o painel de filtro do relatório:

   * Se você estiver criando um relatório, clique no ícone **Filtro** no painel esquerdo da caixa de diálogo **Configurar**.
   * Se você estiver editando um relatório existente, clique no ícone **Mais** no canto superior direito, selecione **Editar** e clique no painel **Filtros** na caixa de diálogo **Configurar**.

1. Clique em **Editar filtro**.

1. Clique em **Adicionar condição** e defina a condição:

   * Clique em **Escolher campo** e selecione o campo pelo qual deseja filtrar.
   * Selecione o modificador que define que tipo de condição o campo deve atender.
   * Digite ou selecione o valor para avaliar, se o modificador exigir um.

   ![Adicionar condição](assets/add-condition.png)

1. (Opcional) Repita a etapa anterior para adicionar mais condições.

1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

>[!NOTE]
>
>Para obter a lista completa de campos, operadores, curingas e regras de filtragem especiais, consulte [Referência de filtro de relatório para Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

1. Clique em **Salvar**.
