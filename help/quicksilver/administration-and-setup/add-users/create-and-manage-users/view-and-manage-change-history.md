---
user-type: administrator
product-area: system-administration;setup
title: Exibir e gerenciar o histórico de alterações
description: O histórico de alterações permite exibir um log de alterações em objetos e campos do Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 100b900bd7419d78a3135358026ec5e27755fdeb
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 6%

---

# Exibir e gerenciar o histórico de alterações

{{preview-fast-release-general}}

O histórico de alterações permite configurar e rastrear alterações em objetos e campos específicos no Adobe Workfront. A configuração flexível permite definir quais objetos e campos exatamente você deseja rastrear.

O histórico de alterações pode rastrear os seguintes tipos de dados definidos:

* Atividade na área Configuração, como criar ou excluir um nível de acesso ou uma função de trabalho
* Atualizações em nível de campo, como edição de uma descrição de projeto ou alteração do modelo de layout de um usuário
* Atualizações de objeto, como atualização de um status de projeto ou anexação de um formulário personalizado a uma tarefa
* <span class="preview">Atividade unificada de fluxo de trabalho de revisão e aprovação, incluindo participantes e decisões</span>

Para obter informações sobre como definir quais objetos e campos são rastreados, consulte [Configurar campos para rastrear no histórico de alterações](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/configure-fields-in-change-history.md).

Na Lista de Histórico de Alterações, você pode exibir o log de alterações para objetos do Workfront, incluindo atributos como:

* Nome do objeto
* Tipo de objeto
* Tipo de alteração (operação)
* Data e hora da alteração
* Source da alteração, como usuários específicos, APIs, Workfront Fusion, AI LLMs ou o sistema Workfront

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Padrão]</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td><span class="preview">Acesso administrativo ao histórico de alterações</span></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
## View the Configuration area for change tracking

>[!NOTE]
>
>In the Production environment, Configuration is currently available only as information and cannot be changed. The ability to change which fields are tracked will be available in the near future.

To view the types of changes that are tracked: 

{{step-1-to-setup}}

1. In the left panel, click **Change Tracking > Configuration**.
   
   Fields are displayed grouped by object type.

1. To display fields under a specific object, click the dropdown arrow next to the object type.
-->


## Exibir a Lista de Histórico de Alterações

Você pode exibir os logs do histórico de alterações na área Configuração.

A Lista do histórico de alterações é uma lista aprimorada com filtros, colunas, altura da linha, um seletor de datas e uma barra de pesquisa.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações > Lista do histórico de alterações**.

   A Lista do histórico de alterações é aberta.

1. Para ajustar as datas para as quais as alterações são exibidas, clique no seletor de datas e selecione as novas datas.

   As alterações estão disponíveis para os últimos 90 dias.

1. Para pesquisar um termo específico, clique na caixa de pesquisa e insira o termo. Os resultados são destacados na lista à medida que você digita.
1. (Opcional) Para filtrar por coluna, consulte [Filtrar itens em lista aprimorada](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) no artigo [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Opcional) Para ocultar, exibir ou reordenar colunas, consulte [Personalizar colunas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) no artigo [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Opcional) Para adicionar ou remover colunas, consulte [Adicionar e remover colunas com o Gerenciador de colunas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) no artigo [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).
1. (Opcional)Para ajustar a altura da linha, consulte [Alterar a altura da linha em uma exibição](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) no artigo [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Exportar histórico de alterações

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações > Lista do histórico de alterações**.
1. Filtre a lista para exibir os itens que deseja exportar.
1. Clique no ícone **Exportar** ![Ícone Exportar](assets/export-icon.png) e selecione se deseja salvar no formato XLSX ou CSV.

   A caixa Salvar arquivo é aberta e você pode salvar o arquivo exportado em seu computador.
   Termine de salvar o arquivo exportado. Agora você pode encontrá-lo em seu computador e compartilhá-lo com outras pessoas.



