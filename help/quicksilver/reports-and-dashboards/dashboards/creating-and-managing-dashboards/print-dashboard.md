---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Imprimir um painel
description: Você pode imprimir ou exportar um painel de controle para um arquivo .PDF. Para imprimir um painel, é necessário ter permissão para Visualizá-lo.
author: Nolan
feature: Reports and Dashboards
exl-id: 30f3481b-23b6-4dc9-be0d-9cffd5d4dfed
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Imprimir um painel

<!-- Audited: 1/2025 -->

Você pode imprimir ou exportar um painel de controle para um arquivo .PDF. Para imprimir um painel, é necessário ter permissão para Visualizá-lo.

>[!NOTE]
>
>Esse recurso deve ser usado somente com a exibição padrão do Painel. Não está disponível para painéis incorporados na área Projetos ou definidos como guias personalizadas.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença do Adobe Workfront</strong></td> 
      <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Trabalhar ou superior</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>Visualizar acesso a relatórios, painéis e calendários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong>/td&gt; 
   <td> <p>Exibir permissões para o painel</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

O painel deve ser criado antes que você possa imprimi-lo.

Para obter informações sobre como criar painéis, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Entender quais informações são impressas ao imprimir um painel

Ao imprimir um painel ou salvá-lo como um arquivo .PDF, algumas informações do painel, como exibidas no aplicativo web do Adobe Workfront, podem não aparecer no arquivo impresso ou exportado.

* [O que é exibido?](#what-is-displayed)
* [O que não é exibido?](#what-is-not-displayed)

### O que é exibido? {#what-is-displayed}

As seguintes informações estão incluídas no arquivo do painel impresso ou exportado:

* Título do painel
* Títulos do relatório
* Carimbo de data e hora de quando o relatório foi gerado pela última vez
* Todos os objetos no painel, incluindo exibições de lista, páginas da Web externas, relatórios e calendários
* O logotipo da sua empresa, se o administrador do Workfront o personalizou na Barra de navegação global. Para obter mais informações sobre como marcar o site do Workfront, consulte [Marcar sua instância do Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### O que não é exibido? {#what-is-not-displayed}

As seguintes informações não estão incluídas no arquivo do painel impresso ou exportado:

* A barra de navegação do Workfront
* Qualquer outra formatação específica do Workfront
* Dependendo do tamanho de seus relatórios e do número e da largura de colunas individuais, exportar e imprimir um painel pode resultar no corte de algumas colunas.

## Imprimir um painel

1. Vá para o painel que deseja imprimir.
1. Siga um destes procedimentos:

   * Clique em **Ações do Painel** > **Visualizar Impressão**

   * Pressione **Ctrl+P** (no Windows) ou **Command+P** (no Mac)

     >[!IMPORTANT]
     >
     >* Nenhuma dessas opções está disponível quando o painel é incorporado em uma guia personalizada. Para obter informações sobre como criar guias personalizadas, consulte [Criar guias ou seções personalizadas](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md).
     >* A opção de atalho de teclado não está disponível ao usar o navegador Internet Explorer.

1. No campo **Destino**, selecione uma das várias opções de impressão disponíveis.\
   As opções de impressão variam de acordo com o navegador e a versão do navegador usada.

1. (Opcional) Salve o painel como um arquivo .PDF e clique em **Salvar** para salvar o .PDF.\
   Para saber como salvar o painel como um arquivo .PDF, consulte [Exportar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/export-dashboard.md).

1. Clique em **Imprimir**.
