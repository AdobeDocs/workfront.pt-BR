---
navigation-topic: get-started-with-workfront
title: Personalizar as colunas da lista de trabalho de prioridades
description: Você pode personalizar as colunas na lista de trabalho em Prioridades para respaldar a maneira como você trabalha.
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: e4232fbe-1b5c-4614-8613-3b0e25ffee46
TQID: https://experienceleague.adobe.com/YIqeZbiTZH00yXJ6LnQrpEZuHvW4Y5QZVkYU3OquWqE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 10%

---

# Personalizar as colunas da lista de trabalho de prioridades

{{preview-fast-release-general}}

<!--I think this article can point to the Enhanced lists article for managing the view-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


Você pode personalizar as colunas na lista de trabalho em Prioridades para respaldar a maneira como você trabalha.

Prioridades exibe os itens de trabalho atribuídos a você. Não é possível ver os itens de trabalho atribuídos à sua equipe.

<!--
>[!NOTE]
>
>You cannot add custom data to columns at this time.
-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Pacote do Adobe Workfront</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença do Adobe Workfront</strong></td> 
   <td> 
   <p>Revisor ou superior</p>
   <p>Leve ou superior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso</strong></td> 
   <td> <p>Acesso de Visualização ou Edição para o objeto no qual a atualização está</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Visualizar acesso ao objeto</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar as colunas da lista de trabalho de prioridades

### Ativar ou desativar colunas

{{step1-to-priorities}}

1. Clique em **Colunas** no lado esquerdo da tela.

   <span class="preview">Imagem de exemplo no ambiente de Visualização:</span>
   ![Colunas](assets/columns-new-060226.png)

   Imagem de amostra no ambiente de produção:
   ![Colunas](assets/columns-new.png)

1. Use os botões para exibir ou ocultar colunas na lista de trabalho.

### Reordenar as colunas

{{step1-to-priorities}}

1. Clique em **Colunas** no lado esquerdo da tela.
1. Clique no ícone **Arrastar** e mova a coluna para o local desejado. A movimentação de colunas atualiza a lista de trabalho automaticamente.
   ![Reordenar colunas](assets/reorder-columns-new.png)

>[!NOTE]
>
>A coluna Name está fixa e não pode ser movida.

<div class="preview">

### Adicionar e remover colunas com o Gerenciador de colunas

{{step1-to-priorities}}

1. Clique no ícone + no canto superior direito da lista para abrir a caixa **Gerenciador de colunas**.
1. Adicione ou remova colunas, em seguida, clique em **Salvar**.

   >[!NOTE]
   >
   >Você pode adicionar somente campos existentes à exibição de lista. Campos nativos e personalizados para tarefas e problemas estão disponíveis para serem adicionados como colunas.

Para obter mais informações sobre o Gerenciador de colunas, consulte a seção [Adicionar e remover colunas com o Gerenciador de colunas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager) no artigo [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

</div>

### Alterar a altura da linha na lista de prioridades

{{step1-to-priorities}}

1. Clique no ícone **Altura da linha**.

   Isso atualiza o comprimento vertical de uma linha. Escolha entre as seguintes opções:

   * Pequena
   * Padrão. Esta é a opção padrão.
   * Médio
   * Alta

   A lista é atualizada imediatamente.

<div class="preview">

## Gerenciar exibições para a lista de prioridades

Uma exibição define as colunas, os filtros e os agrupamentos na lista com as configurações predefinidas.

Uma exibição padrão é atribuída à lista de prioridades. Você também pode criar e compartilhar suas próprias visualizações.

{{step1-to-priorities}}

1. Expanda o menu suspenso de modos de exibição no canto superior esquerdo da lista para selecionar outro modo de exibição ou clique em **Novo modo de exibição** para criar outro.
1. Atualize as colunas, os filtros e os agrupamentos que deseja incluir no modo de exibição.

   As alterações nas exibições são salvas automaticamente. Na próxima vez que você aplicar essa visualização, as configurações de coluna e filtro permanecerão da maneira definida.

Para obter mais informações sobre exibições, consulte a seção [Atualizar elementos da lista aprimorada](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#update-enhanced-list-elements) no artigo [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

</div>
