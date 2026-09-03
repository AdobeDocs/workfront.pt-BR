---
product-area: projects
navigation-topic: financials
title: Substituir as taxas de faturamento no nível do projeto pelas taxas de faturamento no nível da empresa
description: Substituir as taxas de faturamento no nível do projeto pelas taxas de faturamento no nível da empresa
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
TQID: https://experienceleague.adobe.com/GQSQGGHBZsBLtI8IEUltVXzxmEtOxue0iE6fpHmYWP4
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 8c08e110aeccdf6d6416fd1070fbcbd40fd46983
workflow-type: tm+mt
source-wordcount: 480
ht-degree: 13%

---

# Substituir as taxas de faturamento no nível do projeto pelas taxas de faturamento no nível da empresa

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Você pode configurar um projeto para usar taxas de cobrança no nível da empresa em vez de taxas de cobrança no nível do projeto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Editar acesso a Projetos e Dados Financeiros</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto com permissões para Editar Taxas de Cobrança e Finanças Gerais</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ativar a opção de substituição de Taxas de Cobrança no Nível da Empresa

Quando uma empresa está associada a um projeto e essa opção está ativada, as alterações feitas nas taxas de cobrança no nível da empresa substituem a taxa de cobrança definida no projeto.

Quando um usuário recalcula manualmente as finanças do projeto, qualquer alteração nas taxas de cobrança no nível da empresa é aplicada. Os cálculos de receita histórica também são substituídos, a menos que estejam marcados como faturados.

1. Ir para um projeto.
1. Clique no menu **Mais** ![Mais menu](assets/qs-more-icon-on-an-object.png) ao lado do nome do projeto no cabeçalho e clique em **Editar**.
1. Na seção **Finanças**, selecione **Permitir que taxas de cobrança no nível da empresa substituam taxas de cobrança no nível do projeto**.

   >[!CAUTION]
   >
   >Ativar essa opção substitui os cálculos de receita históricos, a menos que estejam marcados como faturados. Você pode preservar os cálculos de receita históricos criando um registro de faturamento. Para obter mais informações, consulte o artigo [Criar registros de cobrança](../../../manage-work/projects/project-finances/create-billing-records.md).

1. Clique em **Salvar**.

## Atualizar taxas de cobrança no nível da empresa e aplicá-las a um projeto

Depois que você ativou a opção de substituição de taxas de cobrança no nível da empresa em um projeto, as alterações feitas nas taxas de cobrança da empresa se aplicam ao projeto sempre que as finanças são recalculadas.

>[!NOTE]
>
>Os usuários devem ter acesso a Empresas em seu nível de acesso para atualizar as taxas de cobrança no nível da empresa.

{{step-1-to-setup}}

1. Clique em **Empresas**.
1. Clique no nome da empresa associada ao projeto para o qual você ativou a substituição de taxas de cobrança no nível da empresa.
1. Clique em **Taxas de cobrança** no painel esquerdo.
1. Selecione a taxa de funções de trabalho a ser atualizada e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png).

   Atualize a taxa de cobrança e as datas de efetivação conforme necessário, e clique em **Salvar**. Para obter mais informações sobre taxas de cobrança da empresa de data efetiva, consulte [Substituir taxas de cobrança de função de trabalho no nível da empresa](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Para atualizar as taxas da empresa para um ou mais projetos, siga um destes procedimentos:

   * Vários projetos:

     1. Ir para uma lista de projetos.
     1. Marque as caixas de seleção dos projetos que deseja atualizar.
     1. Clique no menu **Mais** ![Mais menu](assets/qs-more-icon-on-an-object.png) na parte superior da lista e em **Recalcular Finanças**.

   * Um único projeto:

     1. Vá para o projeto para o qual você ativou a substituição de taxas de cobrança no nível da empresa.
     1. Clique no menu **Mais** ![Mais menu](assets/qs-more-icon-on-an-object.png) ao lado do nome do projeto no cabeçalho e clique em **Recalcular Finanças**.

     Para obter mais informações sobre como recalcular finanças para um ou mais projetos, consulte [Recalcular finanças do projeto](/help/quicksilver/manage-work/projects/project-finances/recalculate-project-finances.md).

