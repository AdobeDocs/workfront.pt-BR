---
title: Anexar um cartão de taxa a um projeto
description: Quando você anexa um cartão de taxa a um projeto, todas as funções por localização e suas taxas de cobrança associadas são adicionadas ao projeto.
author: Lisa
feature: Work Management
role: User
source-git-commit: 8dbb48e6aa2df874caa816468cf2e3ad408ebf7e
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Anexar um cartão de taxa a um projeto

{{highlighted-preview-article-level}}

Os cartões de taxa armazenam várias taxas de cobrança por função de trabalho, com base na localização. Você pode ter uma função de trabalho de Designer com base em Paris e um segundo Designer com base em Nova York, cada um com taxas de cobrança diferentes. No entanto, não é necessário um local para funções de trabalho em um cartão de taxa. Uma taxa de cobrança para uma função de trabalho (e possivelmente local) em um cartão de taxa também pode incluir datas de efetivação.

Quando você anexa um cartão de taxa a um projeto, todas as funções por localização e suas taxas de cobrança associadas são adicionadas ao projeto.

>[!NOTE]
>
>Anexar um cartão de taxa substitui todas as taxas de faturamento existentes no projeto.

Você pode editar as taxas de faturamento do cartão de taxa diretamente no projeto. Isso não afeta as taxas armazenadas no cartão de taxa padrão.

Para obter informações sobre como criar cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Para obter informações gerais sobre como substituir taxas de faturamento de função de trabalho para projetos e calcular a receita do projeto, consulte [Visão geral da substituição de Taxas de cobrança de função de trabalho e do cálculo de Receita em um projeto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Padrão</p><p>Ou</p><p>Plano herdado: plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Acesso administrativo para Funções de trabalho</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões do projeto com permissões para Gerenciar Finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Anexar um cartão de taxa a um projeto

1. Vá para o projeto.
1. Clique em **Taxas de cobrança** no painel esquerdo. Talvez seja necessário clicar primeiro **Mostrar mais**.
1. Clique em **Adicionar taxa de cobrança > Anexar um cartão de taxa**.

   A página Anexar um cartão de taxa é aberta. Para obter mais informações, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Selecione o cartão de taxa a ser adicionado ao projeto e clique em **Anexar**.

   O cartão de taxa e todas as suas taxas de função de trabalho são adicionados à lista de taxas de cobrança.

   ![Cartão de taxa adicionado ao projeto](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Na lista de taxas de cobrança, você pode remover uma ou mais funções de trabalho que vieram de um cartão de taxa. Remover uma taxa de cobrança de função de trabalho do projeto não a remove do cartão de taxa padrão.

