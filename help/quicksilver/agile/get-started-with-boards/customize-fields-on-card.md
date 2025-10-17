---
product-area: agile-and-teams
navigation-topic: customize-fields-on-card
title: Personalizar quais campos são exibidos em um cartão
description: Você pode personalizar quais campos são exibidos em um cartão desativando um campo para que ele não seja exibido no cartão completo ou na exibição condensada, ou ocultando um campo na exibição de cartão condensada.
author: Jenny
feature: Agile
exl-id: 28fa6455-04dd-4115-9ead-cb3e7c26289e
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 0%

---

# Personalizar quais campos são exibidos em um cartão

Por padrão, todos os campos disponíveis são exibidos em um cartão, tanto na exibição completa quando o cartão está aberto quanto na exibição condensada do cartão no quadro. Você pode personalizar quais campos serão exibidos ao:

* Desabilitação de um campo para que ele não seja exibido em nenhuma exibição
* Ocultar um campo na exibição de cartão condensado

Se um campo contiver um valor e você desativar o campo, o valor será retido se você ativar o campo novamente mais tarde.

As seções (que aparecem como as opções de navegação à esquerda nos detalhes do cartão) também estão disponíveis para exibição e ocultação.

Você também pode exibir campos personalizados criados anteriormente. Não é possível projetar e criar novos campos personalizados em um quadro.

>[!NOTE]
>
>As personalizações de campo que você fizer se aplicam somente ao painel em que está trabalhando.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou superior</p> 
   <p>Solicitação ou superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar cartões {#configure-cards}

{{step1-to-boards}}

1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em [!UICONTROL **Configurar**] à direita do quadro para abrir o painel Configurar.
1. Expanda [!UICONTROL **Cartões**].

   A maioria dos campos e seções é ativada por padrão.

1. Desative um campo ou seção para desativá-lo nas duas visualizações de cartão.
1. Clique no ícone Ocultar ![ícone Ocultar](assets/eye-hide-icon.png) ao lado de um campo ou seção para ocultá-lo no modo de exibição condensado.
1. Para exibir todos os campos e seções em ambos os modos de exibição, clique em [!UICONTROL **Restaurar todos os campos para o padrão**].
1. Clique em [!UICONTROL **Ocultar configuração**] para fechar o painel Configurar.

## Adicionar campos personalizados a cartões

Campos personalizados estão disponíveis em cartões conectados. Eles só são visíveis na exibição de cartão completo, não na exibição condensada no quadro.

Os dados em campos personalizados podem ser editados no cartão, embora alguns elementos personalizados possam estar disponíveis apenas para edição no campo original e não no cartão.

1. Acesse um quadro e clique em [!UICONTROL **Configurar**] para abrir o painel Configurar.
1. Expanda [!UICONTROL **Cartões**].
1. Em [!UICONTROL Campos de Cartão], clique em [!UICONTROL **Adicionar campo personalizado**].
1. Selecione [!UICONTROL **Tarefa**] ou [!UICONTROL **Problema**].

   As categorias de campos disponíveis para tarefas ou problemas são exibidas. Expanda uma categoria para ver todos os campos. Também é possível pesquisar por um campo.

   ![Pesquisar campo personalizado](assets/boards-search-for-custom-field.png)

   >[!NOTE]
   >
   >Os seguintes tipos de campo não estão disponíveis para adicionar a cartões: Adobe XD, Image, PDF, Video.

1. Selecione o nome do campo.
1. (Opcional) Clique no campo **[!UICONTROL Valor do campo]** para alterar este campo personalizado para outro.
1. (Opcional) Altere o **[!UICONTROL Rótulo do campo]** para o nome do campo que você deseja que apareça nos cartões.
1. Quando terminar de fazer alterações, clique em [!UICONTROL **Salvar campo**].

   ![Rótulo e valor de campo personalizado](assets/save-custom-field-value-label.png)

   O campo personalizado é adicionado à lista de campos disponíveis e é ativado por padrão. Você pode desabilitar o campo personalizado seguindo as etapas da seção [Configurar cartões](customize-fields-on-card.md#configure-cards) acima, editar o campo ou excluí-lo de todos os cartões.

>[!NOTE]
>
>Posteriormente, se você renomear o campo personalizado no Workfront, deverá editar o rótulo do campo no painel Configurar para corresponder, ou o campo não será exibido nos cartões.

## Exibir ou ocultar cartões arquivados

Você deve ativar uma definição de configuração para exibir cartões arquivados em uma placa.

1. Acesse um quadro e clique em [!UICONTROL **Configurar**] para abrir o painel Configurar.
1. Expanda [!UICONTROL **Cartões**].
1. Ative [!UICONTROL **Exibir cartões arquivados no quadro**].

   Agora, você pode filtrar o quadro para mostrar todos os cartões que foram arquivados. Para obter detalhes, consulte [Filtrar e pesquisar em um quadro](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

1. Clique em [!UICONTROL **Ocultar configuração**] para fechar o painel Configurar.

## Configurar queda de cartão

Para remover automaticamente cartões do quadro após um período, consulte [Configurar fallout de cartão](/help/quicksilver/agile/use-boards-agile-planning-tools/configure-card-falloff.md).
