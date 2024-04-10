---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gerenciar cartões de taxa
description: Cartões de tarifa permitem definir várias taxas de cobrança por função, com base na localização.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: a61635022da9eed7c2fc61bad1cbca0f7f23d7ec
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Gerenciar cartões de taxa

{{highlighted-preview-article-level}}

Cartões de tarifa permitem definir várias taxas de cobrança por função, com base na localização. Você pode ter uma função de trabalho de Designer com base em Paris e um segundo Designer com base em Nova York, cada um com taxas de cobrança diferentes. No entanto, não é necessário um local para funções de trabalho em um cartão de taxa. Uma taxa de cobrança para uma função de trabalho (e possivelmente local) em um cartão de taxa também pode incluir datas de efetivação.

## Requisitos de acesso

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
   <td><p>Novo plano: [!UICONTROL Padrão] </p>
       <p>ou</p> 
       <p>Plano atual: [!UICONTROL Plan] </p>
   </td>    
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a [!UICONTROL Dados Financeiros]</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Para editar um cartão de taxa compartilhado com você, é necessário ter permissões de gerenciamento para o cartão de taxa.</td> 
  </tr> 
 </tbody> 
</table>

## Adicionar um cartão de taxa

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Cartões de taxa**].
1. Clique em [!UICONTROL **Novo cartão de taxa**], em seguida, digite um nome para o cartão de taxa na [!UICONTROL Novo cartão de taxa] para substituir &quot;Cartão de tarifa sem título&quot;.
1. (Opcional) Na tela Detalhes do cartão de tarifa, adicione uma [!UICONTROL **Descrição**].
1. (Opcional) Para anexar um formulário personalizado ao cartão de taxa, clique no [!UICONTROL **Adicionar formulário personalizado**] no canto superior direito e selecione um formulário personalizado na lista exibida.

   Para obter mais informações sobre como anexar um formulário personalizado, consulte [Adicionar um formulário personalizado a um objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Clique em [!UICONTROL **Funções e taxas de trabalho**] no painel de navegação esquerdo.
1. Na tela Funções e Taxas de Cartão de Taxa, clique em [!UICONTROL **Adicionar função de trabalho**].
1. Na caixa de diálogo, selecione uma [!UICONTROL **Função de trabalho**] para definir taxas de faturamento.

   A Taxa de Faturamento Padrão exibe a taxa no nível do sistema para essa função de trabalho, se houver uma definida.

   ![Caixa de diálogo Nova taxa de cobrança](assets/location-rate-for-rate-card.png)

1. Selecione um [!UICONTROL **Moeda**] para a função de trabalho.
1. (Opcional) Selecione um [!UICONTROL **Localização**] para a função de trabalho.
1. No [!UICONTROL **Taxa de cobrança 1**] insira a taxa de faturamento para este local. Em seguida, clique em [!UICONTROL **Salvar**] para substituir a taxa de faturamento uma vez.

   Ou

   Clique em [!UICONTROL **Adicionar taxa**] para adicionar taxas de cobrança específicas do local com datas de efetivação.

1. (Condicional) Se você estiver adicionando mais de uma taxa de faturamento para este local, especifique as seguintes informações:

   * **[!UICONTROL Taxa de cobrança 1], 2, etc.:** O valor da taxa de cobrança do período.
   * **[!UICONTROL Data de início]:** A data em que a substituição de taxa começa.
   * **[!UICONTROL Data final]:** A data em que a substituição de taxa termina.

     A Taxa de Cobrança 1 não terá uma data inicial e a última taxa de cobrança não terá uma data final. Algumas datas são adicionadas automaticamente. Por exemplo, se a Taxa de cobrança 1 não tiver uma data final e você adicionar a Taxa de cobrança 2 com uma data inicial de 1º de maio de 2023, uma data final de 30 de abril de 2023 será adicionada à Taxa de cobrança 1 para que não haja lacunas.

1. Clique em [!UICONTROL **Salvar**].
1. (Opcional) Para adicionar outra taxa de cobrança, para a mesma função de trabalho em outro local ou para uma função de trabalho separada, clique em [!UICONTROL **Adicionar função de trabalho**].
1. (Opcional) Para editar um cartão de taxa, clique no nome do cartão de taxa na lista Cartões de taxa em Configurar. Para editar uma taxa de faturamento, clique em [!UICONTROL **Funções e taxas de trabalho**] no painel de navegação esquerdo do cartão de taxa. Em seguida, selecione a taxa e clique no botão **Editar** ícone ![Ícone Editar](assets/edit-icon.png).

## Copiar um cartão de taxa

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Cartões de taxa**].
1. Marque a caixa de seleção ao lado do cartão de taxa na lista e clique no **Copiar** ícone ![Ícone Copiar](assets/copy-icon.png).
1. Digite um nome para o cartão de tarifa na [!UICONTROL Copiar cartão de taxa] para substituir &quot;Cartão de tarifa sem título&quot;. Em seguida, clique em **Salvar**.

   O novo cartão de taxa é salvo. Edite os detalhes do cartão de classificação, as funções de trabalho e as taxas conforme necessário.

## Excluir um cartão de taxa inteiro

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Cartões de taxa**].
1. Marque a caixa de seleção ao lado do cartão de taxa na lista e clique no **Excluir** ícone ![Ícone Excluir](assets/delete.png).

   >[!NOTE]
   >
   >Um cartão de taxa anexado a um projeto será excluído do projeto.
