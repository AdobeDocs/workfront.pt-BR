---
title: Anexar um cartão de taxa a um projeto
description: Quando você anexa um cartão de taxa a um projeto, todas as funções por localização e suas taxas de cobrança associadas são adicionadas ao projeto.
author: Lisa
feature: Work Management
role: User
exl-id: 97c33c5a-e42d-4015-841f-69dc44a0599d
source-git-commit: 58d3f084c343bcc404f30edd270017fa5f86eb58
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 8%

---

# Anexar um cartão de tarifas a um projeto

{{highlighted-preview-article-level}}

Os cartões de taxa armazenam várias taxas de cobrança por função de trabalho, com base nos atributos. Por exemplo, você pode ter uma função de trabalho de Designer com base em Paris para a Agência A, outra Designer com base em Paris para a Agência B e uma terceira Designer com base em Nova York não atribuída a uma agência, cada uma com taxas de faturamento diferentes. No entanto, os atributos não são necessários para funções de trabalho em um cartão de taxa. Os atributos servem como ferramentas para estabelecer taxas mais granulares. Uma taxa de cobrança em um cartão de taxa também pode ter data de efetivação, de modo que a taxa comece e termine em datas especificadas.

Quando você anexa um cartão de taxa a um projeto, todas as funções e suas taxas de cobrança associadas são adicionadas ao projeto.

>[!NOTE]
>
>Anexar um cartão de taxa sobrepõe quaisquer taxas de faturamento existentes no cartão de taxa do projeto. As sobreposições de taxa de cobrança que foram adicionadas diretamente ao projeto não são removidas.

Para obter informações sobre como criar cartões de taxa, consulte [Gerenciar cartões de taxa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

Para obter informações gerais sobre substituição de taxas de cobrança de função de trabalho para projetos e cálculo de receita do projeto, consulte [Visão geral sobre substituição de taxas de cobrança e cálculo de receita em um projeto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>Padrão</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a projetos, dados financeiros e cartões de taxa</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto com permissões para Editar Taxas de Cobrança</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Anexar um cartão de tarifas a um projeto

1. Vá para o projeto.
1. Clique em **Taxas** no painel esquerdo e selecione **Faturamento**.
1. Clique em **Adicionar taxa de cobrança > Anexar um cartão de taxa**.

   A caixa **Anexar um cartão de taxa** é aberta. Você pode procurar por um cartão de tarifa na lista.

   ![Anexar uma caixa de cartão de taxa](assets/attach-rate-card-dialog.png)

   >[!NOTE]
   >
   >O Grupo e a Empresa nos cartões de taxa são usados como filtros nesta lista. Como os projetos também incluem campos de Grupo e Empresa, a Workfront usa esses valores para restringir a lista de cartões de taxa disponíveis àqueles relevantes para o contexto do projeto e não a todos os cartões de taxa no sistema.
   >
   >A correspondência não precisa ser exata. Cartões de tarifas com valores em branco de Grupo e/ou Empresa ainda podem aparecer, dependendo da configuração de Grupo/Empresa do projeto. Por exemplo, se um projeto tiver um Grupo selecionado, mas a Empresa estiver em branco, você poderá ver cartões de taxa associados a esse Grupo, mesmo se a Empresa do cartão de taxa for diferente ou estiver em branco.

1. Selecione o cartão de taxa a ser adicionado ao projeto e clique em **Anexar**.

   O cartão de taxa e todas as suas taxas de função de trabalho são adicionados à lista de taxas de cobrança.

   ![Cartão de taxa adicionado ao projeto](assets/rate-card-on-project.png)

## Remover um cartão de taxa de um projeto

Quando você remove um cartão de taxas de um projeto, todas as suas taxas de função de trabalho são removidas. Você não pode remover uma taxa individual do projeto que vem de um cartão de taxa.

As substituições de taxa de cobrança para usuários ou funções de trabalho que foram adicionadas diretamente ao projeto podem ser removidas sem remover todo o cartão de taxa.

1. Vá para o projeto.
1. Clique em **Taxas** no painel esquerdo e selecione **Faturamento**.
1. Clique no ícone **Remover** ![Ícone Remover](assets/remove-icon.png).
1. Clique em **Confirmar** na mensagem de confirmação para remover o cartão de taxa.

