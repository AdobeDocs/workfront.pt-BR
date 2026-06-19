---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Histórico de alterações
description: O histórico de alterações permite exibir um log de alterações em objetos do Workfront
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 44292bc9cf8654d1ecfb398b0f118a6c001f544f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 7%

---

# Exibir e gerenciar o histórico de alterações

Você pode exibir o histórico de alterações, incluindo logs de auditoria, na área Rastreamento de alterações da Configuração.

* **Logs de Auditoria** são alterações acionadas por usuários.
Para obter mais informações sobre Logs de auditoria e a área Logs de auditoria, consulte [Visão geral dos Logs de auditoria](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/audit-logs.md)
* **A configuração** exibe quais campos estão sendo acompanhados para a Lista de Histórico de Alterações.
No momento, a configuração está disponível somente como informação e não pode ser alterada. A capacidade de alterar quais campos são rastreados estará disponível em breve.
* A Lista de histórico de alterações permite exibir um log de alterações para objetos do Workfront, incluindo atributos como:

   * Objeto
   * Tipo de objeto
   * Tipo de alteração (operação)
   * Source da alteração, como usuários específicos, APIs, Workfront Fusion, AI LLMs ou o sistema Workfront

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Padrão]</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Você precisa ser um administrador do Workfront para visualizar o Histórico de alterações</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir e gerenciar logs de auditoria

Para exibir e gerenciar logs de auditoria, consulte [Exibir e exportar logs de auditoria](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md).

## Exibir a área Configuração para controle de alterações

>[!NOTE]
>
>No momento, a configuração está disponível somente como informação e não pode ser alterada. A capacidade de alterar quais campos são rastreados estará disponível em breve.

Para exibir os tipos de alterações que são rastreadas:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações** ![Ícone Alterar histórico](assets/change-history-icon.png).
1. Clique em **Configuração**.

   Os campos são exibidos agrupados por tipo de objeto.

1. Para exibir campos sob um objeto específico, clique na seta suspensa ao lado do tipo de objeto.

## Exibir a Lista de Histórico de Alterações

Os administradores do Workfront podem exibir o histórico de alterações na área Configuração.

A Lista do histórico de alterações é uma lista aprimorada com filtros, colunas, altura da linha, um seletor de datas e uma barra de pesquisa.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Controle de alterações** ![Ícone Alterar histórico](assets/change-history-icon.png).
1. Clique em **Lista do Histórico de Alterações**.

   A Lista do histórico de alterações é aberta.

1. Para ajustar as datas para as quais as alterações são exibidas, clique no seletor de datas e selecione as novas datas.

   As alterações estão disponíveis para os últimos 90 dias.
1. Para pesquisar um termo específico, clique na barra de pesquisa e insira o termo. Os resultados são filtrados à medida que você digita.
1. (Opcional) Para filtrar por uma coluna, consulte [Filtrar itens em uma lista aprimorada](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#filter-items-in-an-enhanced-list) no artigo Usar listas aprimoradas.
1. (Opcional) Para ocultar, exibir ou reordenar colunas, consulte [Personalizar colunas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#customize-columns) no artigo Usar listas aprimoradas.
1. Para adicionar ou remover colunas, consulte [Adicionar e remover colunas com o Gerenciador de colunas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) no artigo Usar listas aprimoradas.
1. Para ajustar a altura da linha, consulte [Alterar a altura da linha em uma exibição](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#change-the-row-height-in-a-view) no artigo Usar listas aprimoradas.





