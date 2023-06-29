---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Gerenciar cartões de taxa
description: Cartões de tarifa permitem definir várias taxas de cobrança por função, com base na localização.
author: Lisa
feature: System Setup and Administration
role: Admin
source-git-commit: 1517e3e28fe536a8a72d2802919c8b8819e9ea1a
workflow-type: tm+mt
source-wordcount: '532'
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
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Plano herdado: [!UICONTROL Plan]</p>
       <p>Plano atual: [!UICONTROL Padrão]</p></td> 
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
1. Clique em [!UICONTROL **Novo cartão de taxa**] e, em seguida, digite o nome e a descrição do cartão de taxa na lista.
1. Para adicionar taxas de cobrança, clique no nome do cartão de taxa na lista.
1. Na tela do cartão, clique em [!UICONTROL **Nova taxa de cobrança**].
1. Na caixa de diálogo Novo preço, selecione um [!UICONTROL **Função de trabalho**] para definir taxas de faturamento.

   A Taxa de Faturamento Padrão exibe a taxa no nível do sistema para esta função de trabalho.

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
1. (Opcional) Para adicionar outra taxa de cobrança, para a mesma função de trabalho em outro local ou para uma função de trabalho separada, clique em [!UICONTROL **Nova taxa de cobrança**].

## Copiar um cartão de taxa

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Cartões de taxa**].
1. Marque a caixa de seleção ao lado do cartão de taxa na lista e clique no **Copiar** ícone ![Ícone Copiar](assets/copy-icon.png).

   Um cartão de taxa duplicado é adicionado. Clique no nome do cartão de taxa na lista para alterar seu nome.

## Excluir um cartão de taxa

{{step-1-to-setup}}

1. No painel esquerdo, clique em [!UICONTROL **Cartões de taxa**].
1. Marque a caixa de seleção ao lado do cartão de taxa na lista e clique no **Excluir** ícone ![Ícone Excluir](assets/delete.png).

   >[!NOTE]
   >
   >Um cartão de taxa anexado a um projeto será excluído do projeto.
