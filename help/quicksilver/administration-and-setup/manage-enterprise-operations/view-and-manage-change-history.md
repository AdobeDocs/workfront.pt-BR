---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Histórico de alterações
description: O histórico de alterações permite exibir um log de alterações em objetos do Workfront
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: de1f426630b8c99cfaca07dafb9c2de0f16f263f
workflow-type: tm+mt
source-wordcount: '737'
ht-degree: 4%

---

# Exibir e gerenciar o histórico de alterações

{{preview-fast-release-general}}

Você pode exibir o histórico de alterações, incluindo logs de auditoria, na área Rastreamento de alterações da Configuração.

* **Logs de Auditoria** são alterações acionadas por usuários.
Para obter mais informações sobre Logs de Auditoria e a área Logs de Auditoria, consulte [Visão geral dos Logs de Auditoria](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md) e [Exibir e exportar logs de auditoria](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).
* A **Configuração** exibe quais campos estão sendo acompanhados para a Lista de Histórico de Alterações.
  <span class="preview">Como administrador do Workfront, você pode configurar quais campos de objeto e ações o Workfront rastreia. Por exemplo, você pode fazer com que o Workfront rastreie todas as alterações que os usuários fazem nos nomes de problemas em todo o sistema. Qualquer alteração de nome de problema aparece como uma entrada no log de histórico de alterações.</span>

* **A Lista do Histórico de Alterações** permite que você exiba um log de alterações para objetos do Workfront, incluindo atributos como:

  * Objeto
  * Tipo de objeto
  * Tipo de alteração (operação)
  * Source da alteração, como usuários específicos, APIs, Workfront Fusion, AI LLMs ou o sistema Workfront

  <span class="preview">A atividade de fluxo de trabalho de revisão e aprovação unificada é acompanhada no Histórico de Alterações, incluindo participantes e decisões.</span>

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
   <td><p>Administrador do sistema</p>
       <p><span class="preview">Para exibir o histórico de alterações: Acesso administrativo ao histórico de alterações</span></p>
       <p><span class="preview">Para configurar campos rastreados: Administrador do sistema</span></p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<div class="preview">

## Adicionar campos que você deseja rastrear

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações > Configuração**.
1. Na tela Configuração, clique em **Adicionar campo**.
1. Na caixa **Adicionar campos**, selecione um objeto. Você pode começar a digitar o nome do objeto e, em seguida, selecioná-lo quando ele aparecer na lista.
1. Em seguida, selecione os nomes de campo que deseja rastrear para esse objeto. Você pode digitar o nome do campo e, em seguida, selecioná-lo quando ele aparecer na lista.

   Tanto os campos personalizados quanto os campos nativos estão disponíveis para o objeto.
   Os campos que já estão sendo rastreados são mostrados como selecionados na lista.

   ![Adicionar campos para controle de alterações](assets/change-history-config-add-fields.png)

1. Depois de selecionar todos os campos que deseja rastrear, clique em **Adicionar**.

   Os campos são adicionados à lista Campos rastreados.

## Remova os campos que não deseja mais rastrear

Você pode remover campos que não deseja que o sistema rastreie para um tipo específico de objeto em toda a interface do Workfront.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações > Configuração**.
1. Na tela Configuração, selecione o campo ou os campos que deseja interromper o rastreamento.

   Você pode ver o mesmo nome de campo mais de uma vez. Os campos são agrupados por objeto para que você possa localizar o campo correto. Você também pode usar a caixa de pesquisa na parte superior da tela.

1. Selecione **Excluir** na barra de ações na parte inferior da tela.
1. Clique em **Remover** na mensagem de confirmação.

   Os campos são removidos da lista Campos rastreados.

</div>

## Exibir a área Configuração para controle de alterações

>[!NOTE]
>
>No ambiente de Produção, a Configuração está disponível atualmente somente como informação e não pode ser alterada. A capacidade de alterar quais campos são rastreados estará disponível em breve.

Para exibir os tipos de alterações que são rastreadas:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações >** Configuração**.

   Os campos são exibidos agrupados por tipo de objeto.

1. Para exibir campos sob um objeto específico, clique na seta suspensa ao lado do tipo de objeto.

## Exibir a Lista de Histórico de Alterações

Os administradores do Workfront podem exibir o histórico de alterações na área Configuração.

A Lista do histórico de alterações é uma lista aprimorada com filtros, colunas, altura da linha, um seletor de datas e uma barra de pesquisa.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações > Lista do histórico de alterações**.

   A Lista do histórico de alterações é aberta.

1. Para ajustar as datas para as quais as alterações são exibidas, clique no seletor de datas e selecione as novas datas.

   As alterações estão disponíveis para os últimos 90 dias.

1. Para pesquisar um termo específico, clique na barra de pesquisa e insira o termo. Os resultados são destacados na lista à medida que você digita.
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



