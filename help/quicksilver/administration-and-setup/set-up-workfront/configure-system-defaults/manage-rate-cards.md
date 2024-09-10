---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gerenciar cartões de tarifa
description: Cartões de tarifa permitem definir várias taxas de cobrança por função, com base na localização.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Gerenciar cartões de taxa

{{highlighted-preview-article-level}}

Cartões de tarifa permitem definir várias taxas de cobrança por função, com base na localização. Você pode ter uma função de trabalho de Designer com base em Paris e uma segunda Designer com base em Nova York, cada uma com taxas de cobrança diferentes. No entanto, não é necessário um local para funções de trabalho em um cartão de taxa. Uma taxa de cobrança para uma função de trabalho (e possivelmente local) em um cartão de taxa também pode incluir datas de efetivação.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
   Ou
   <p>Atual: [!UICONTROL Plano]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Editar acesso a [!UICONTROL Dados Financeiros]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Para editar um cartão de taxa compartilhado com você, é necessário ter permissões de gerenciamento para o cartão de taxa.</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Adicionar um cartão de taxa

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Clique em [!UICONTROL **Novo cartão de taxa**] e digite um nome para o cartão de taxa na caixa [!UICONTROL Novo cartão de taxa], para substituir &quot;Cartão de taxa sem título&quot;.
1. (Opcional) Na tela Detalhes do Cartão de Taxa, adicione uma [!UICONTROL **Descrição**].
1. (Opcional) Para anexar um formulário personalizado ao cartão de taxa, clique no campo [!UICONTROL **Adicionar formulário personalizado**] no canto superior direito e selecione um formulário personalizado na lista que é exibida.

   Para obter mais informações sobre como anexar um formulário personalizado, consulte [Adicionar um formulário personalizado a um objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Clique em [!UICONTROL **Funções e taxas de trabalho**] no painel de navegação esquerdo.
1. Na tela Taxas e Funções de Trabalho do Cartão de Taxa, clique em [!UICONTROL **Adicionar função de trabalho**].
1. Na caixa de diálogo, selecione uma [!UICONTROL **Função de trabalho**] para definir taxas de cobrança.

   A Taxa de Faturamento Padrão exibe a taxa no nível do sistema para essa função de trabalho, se houver uma definida.

   ![Caixa de diálogo Nova Taxa de Cobrança](assets/location-rate-for-rate-card.png)

1. Selecione uma [!UICONTROL **Moeda**] para a função de trabalho.
1. (Opcional) Selecione um [!UICONTROL **Local**] para a função de trabalho.
1. No campo [!UICONTROL **Taxa de Cobrança 1**], insira a taxa de cobrança para esta localização. Em seguida, clique em [!UICONTROL **Salvar**] para substituir a taxa de cobrança uma vez.

   Ou

   Clique em [!UICONTROL **Adicionar taxa**] para adicionar taxas de cobrança específicas da localização com datas de efetivação.

1. (Condicional) Se você estiver adicionando mais de uma taxa de faturamento para este local, especifique as seguintes informações:

   * **[!UICONTROL Taxa de Cobrança 1], 2, etc.:** O valor da taxa de cobrança para o período.
   * **[!UICONTROL Data de Início]:** A data em que a substituição de taxa começa.
   * **[!UICONTROL Data Final]:** A data em que a substituição de taxa termina.

     A Taxa de Cobrança 1 não terá uma data inicial e a última taxa de cobrança não terá uma data final. Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de cobrança 1 não tiver uma data final e você adicionar a Taxa de cobrança 2 com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de cobrança 1 para que não haja lacunas.

1. Clique em [!UICONTROL **Salvar**].
1. (Opcional) Para adicionar outra taxa de cobrança, para a mesma função de trabalho em outro local ou para uma função de trabalho separada, clique em [!UICONTROL **Adicionar função de trabalho**].
1. (Opcional) Para editar um cartão de taxa, clique no nome do cartão de taxa na lista Cartões de taxa em Configurar. Para editar uma taxa de cobrança, clique em [!UICONTROL **Funções e Taxas de Trabalho**] no painel de navegação esquerdo do cartão de taxa. Em seguida, selecione a taxa e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png).

## Copiar um cartão de taxa

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Marque a caixa de seleção ao lado do cartão de taxa na lista e clique no ícone **Copiar** ![Copiar ícone](assets/copy-icon.png).
1. Digite um nome para o cartão de taxa na caixa [!UICONTROL Copiar cartão de taxa], para substituir &quot;Cartão de Taxa sem Título&quot;. Em seguida, clique em **Salvar**.

   O novo cartão de taxa é salvo. Edite os detalhes do cartão de classificação, as funções de trabalho e as taxas conforme necessário.

## Excluir um cartão de taxa inteiro

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Classificar cartões**].
1. Marque a caixa de seleção ao lado do cartão de taxa na lista e clique no ícone **Excluir** ![Excluir](assets/delete.png).

   >[!NOTE]
   >
   >Um cartão de taxa anexado a um projeto será excluído do projeto.
