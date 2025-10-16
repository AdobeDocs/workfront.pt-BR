---
title: Anexar um cartão de taxa a um projeto
description: Quando você anexa um cartão de taxa a um projeto, todas as funções por localização e suas taxas de cobrança associadas são adicionadas ao projeto.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '377'
ht-degree: 0%

---

# Anexar um cartão de taxa a um projeto

{{highlighted-preview-article-level}}

Os cartões de taxa armazenam várias taxas de cobrança por função de trabalho, com base na localização. Você pode ter uma função de trabalho de Designer com base em Paris e uma segunda Designer com base em Nova York, cada uma com taxas de cobrança diferentes. No entanto, não é necessário um local para funções de trabalho em um cartão de taxa. Uma taxa de cobrança para uma função de trabalho (e possivelmente local) em um cartão de taxa também pode incluir datas de efetivação.

Quando você anexa um cartão de taxa a um projeto, todas as funções por localização e suas taxas de cobrança associadas são adicionadas ao projeto.

>[!NOTE]
>
>Anexar um cartão de taxa substitui todas as taxas de faturamento existentes no projeto.

Você pode editar as taxas de faturamento do cartão de taxa diretamente no projeto. Isso não afeta as taxas armazenadas no cartão de taxa padrão.

Para obter informações sobre como criar cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

Para obter informações gerais sobre substituição de taxas de cobrança de função de trabalho para projetos e cálculo de receita do projeto, consulte [Visão geral da substituição de Taxas de cobrança de função de trabalho e cálculo de Receita em um projeto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Acesso administrativo para funções de trabalho</p></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto que inclui Editar Dados Financeiros </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anexar um cartão de taxa a um projeto

1. Vá para o projeto.
1. Clique em **Taxas de cobrança** no painel esquerdo.
1. Clique em **Adicionar taxa de cobrança > Anexar um cartão de taxa**.

   A página Anexar um cartão de taxa é aberta. Para obter mais informações, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).

1. Selecione o cartão de taxa a ser adicionado ao projeto e clique em **Anexar**.

   O cartão de taxa e todas as suas taxas de função de trabalho são adicionados à lista de taxas de cobrança.

   ![Cartão de taxa adicionado ao projeto](assets/billing-rates-added-from-rate-card.png)

   >[!NOTE]
   >
   >Na lista de taxas de cobrança, você pode remover uma ou mais funções de trabalho que vieram de um cartão de taxa. Remover uma taxa de cobrança de função de trabalho do projeto não a remove do cartão de taxa padrão.
