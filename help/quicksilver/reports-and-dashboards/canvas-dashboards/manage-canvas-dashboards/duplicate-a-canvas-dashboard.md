---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Copiar um painel da tela
description: Você pode Copiar um painel da tela para criar uma variação dele, como uma cópia específica de um público-alvo, sem recriá-lo do zero.
author: Courtney
feature: Reports and Dashboards
source-git-commit: b66f6931ee2fe83688fb8910861af6e958d1f74f
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 15%

---

# Copiar um painel da tela

{{highlighted-preview-article-level}}

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Falar com o suporte ao cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

É possível copiar um Painel da tela para criar uma variação dele para um público-alvo diferente, como uma cópia em nível de diretor de um painel executivo, sem recriá-lo do zero.

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
   <td><p>Editar ou criar acesso a painéis</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Visualizar acesso ao painel</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

Você deve criar um painel antes de duplicá-lo.

Para obter mais informações, consulte [Criar um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Copiar um painel

>[!NOTE]
>
>As preferências de compartilhamento não são copiadas para o novo painel. Se um widget tiver uma configuração **Executar como usuário**, essa configuração será preservada na cópia somente se você for o usuário designado ou um Administrador do Sistema.

Para copiar um painel:

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Na página **Painéis da Tela**, abra o painel que deseja copiar.

1. No canto superior direito, selecione o ícone **Mais** ![Mais](assets/more-icon.png) e selecione **Copiar**.
   ![Opção de menu Copiar painel](assets/duplicate-dashboard.png)

1. Na caixa de diálogo **Copiar painel**, digite um **Nome** para o novo painel, que assume como padrão o nome do painel de origem seguido por &quot;(Copiar)&quot;.

1. (Opcional) Na guia **Detalhes do painel**, atualize a **Descrição** ou a **Moeda** para o novo painel.
   ![Copiar painel - guia de detalhes do painel](assets/duplicate-details.png)

1. (Opcional) Clique na guia **Widgets** e desmarque todos os widgets que não deseja incluir no painel duplicado.
   ![Copiar painel - Guia Dispositivos](assets/copy-widgets.png)

1. (Opcional) Clique na guia **Filtros e Prompts** e desative a opção **Copiar filtros do painel** ou **Copiar prompts do painel** para excluí-los do painel duplicado.
   ![Copiar painel - guia Filtros e Solicitações](assets/copy-filters.png)

1. Clique em **Copiar painel**.

Uma mensagem de confirmação é exibida, com um link para o novo painel.
