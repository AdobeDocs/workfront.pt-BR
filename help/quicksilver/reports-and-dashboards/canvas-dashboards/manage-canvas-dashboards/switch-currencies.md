---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Usar campos de moeda nos Painéis do Canvas
description: É possível usar os campos de moeda em um Painel da tela de desenho.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 3e4ab2dfc66efd262c0c2ad30a9c62758084f8ce
workflow-type: tm+mt
source-wordcount: '622'
ht-degree: 4%

---


# Usar campos de moeda nos Painéis do Canvas

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Contate o Suporte ao Cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

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
   <p>Exibir acesso a Dados Financeiros</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Gerenciar permissões do painel</p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

1. Você deve ter vários tipos de moeda configurados na instância do Workfront para usar a funcionalidade descrita neste artigo. Para obter mais informações, consulte [Configurar taxas de câmbio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   >[!IMPORTANT]
   >
   >A funcionalidade descrita neste artigo se aplica somente aos campos de moeda nativa. O suporte para campos de moeda personalizados será disponibilizado em breve.


## Definir uma moeda padrão para um Painel da Tela

Ao criar um Painel de controle do Canvas, você pode definir uma moeda padrão para o painel. Essa moeda será usada para exibir todos os campos de moeda nativos em relatórios no painel, a menos que o campo de moeda esteja bloqueado no nível do relatório.

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**,

1. Especifique o seguinte:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Nome</strong></td>
      <td><p>Insira um nome para o painel. Recomendamos usar somente caracteres UTF-8 para evitar problemas de compatibilidade.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Descrição (opcional)</strong></td>
      <td>Insira uma descrição do painel.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Moeda</strong></td>
      <td>Escolha o tipo de moeda padrão para o painel. <br>
      <br>Os usuários podem alternar entre diferentes tipos de moeda ao filtrar o painel.</td>
     </tr>
    </tbody>
   </table>


## Alternar entre moedas em um Painel de Controle da Tela

Você pode alternar entre diferentes tipos de moeda no nível do painel. Os relatórios que contêm campos de moeda serão atualizados para refletir o tipo de moeda selecionado.

Os campos de moeda podem ser bloqueados no nível do relatório. Se um campo de moeda estiver bloqueado, o tipo de moeda para esse relatório não será alterado quando você alterar o tipo de moeda para o painel.

Para alterar o tipo de moeda do painel,

1. Clique no menu suspenso currency no canto superior direito da página de detalhes do painel.
1. Selecione o tipo de moeda desejado na lista.

   ![alterar lista suspensa de moedas](assets/filter-by-currency.png)


## Limitações

A tabela a seguir descreve as limitações quando as moedas são definidas na área Taxas de Câmbio em Configuração.

<table> 
<tr>
<td></td>
<td>Os usuários podem</td>
<td>Usuários não podem</td>
</tr>
<tr> 
<td>Uma única moeda está definida</td>
<td>
<ul>
<li>Usar campos de moeda nativa em gráficos de tela, KPI e relatórios de tabela</li>
<li>Usar campos de moeda personalizados em relatórios de gráfico de tela, KPI e gráfico</li>
</ul>
</td>
<td>
<ul>
<li>Atribuir uma moeda padrão ao painel (na criação ou edição do painel)</li>
<li>Ver e usar a alternância de moeda no nível do painel</li>
<li>Bloquear uma moeda específica para exibição em um gráfico de tela, KPI ou relatório de tabela</li>
<li>Usar campos de moeda do Planning em um gráfico de tela, KPI e relatórios de tabela</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>Várias moedas estão definidas</td>
<td>
<ul>
  <li>Usar campos de moeda nativa em gráficos de tela, KPI e relatórios de tabela</li>
  <li>Definir uma moeda padrão para o painel (na criação ou edição do painel)</li>
  <li>Ver e usar a alternância de moeda no nível do painel</li>
  <li>Bloqueie uma moeda específica para exibição em um gráfico de tela, KPI ou relatório de tabela para ignorar a preferência de alternância de moeda do painel</li>
</ul>
</td>
<td><ul>
  <li>Usar campos de moeda de dados personalizados em relatórios de gráfico de tela, KPI e tabela</li>
  <li>Usar campos de moeda do Planning em um gráfico de tela, KPI e relatórios de tabela</li>
</ul>
</td>
</tr></table>





