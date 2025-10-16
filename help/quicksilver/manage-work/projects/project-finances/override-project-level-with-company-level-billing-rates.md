---
product-area: projects
navigation-topic: financials
title: Sobrepor Taxas de Cobrança no Nível do Projeto com Taxas de Cobrança no Nível da Empresa
description: Sobrepor Taxas de Cobrança no Nível do Projeto com Taxas de Cobrança no Nível da Empresa
author: Lisa
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '453'
ht-degree: 1%

---

# Sobrepor Taxas de Cobrança no Nível do Projeto com Taxas de Cobrança no Nível da Empresa

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Você pode configurar um projeto para usar taxas de cobrança no nível da empresa em vez de taxas de cobrança no nível do projeto.

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
   <td>Editar acesso a Projetos e Dados Financeiros</td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões do projeto com permissões para Gerenciar Finanças</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Habilitar a opção de substituição de Taxas de Cobrança no Nível da Empresa

Quando uma empresa está associada a um projeto e essa opção está habilitada, as alterações feitas nas taxas de cobrança no nível da empresa substituem a taxa de cobrança definida no projeto.

Quando um usuário recalcula manualmente as finanças do projeto, qualquer alteração nas taxas de cobrança no nível da empresa é aplicada. Os cálculos de receita histórica também são substituídos, a menos que estejam marcados como faturados.

1. Ir para um projeto.
1. Clique no menu **Mais** ![Mais menu](assets/qs-more-icon-on-an-object.png) ao lado do nome do projeto no cabeçalho e clique em **Editar**.
1. Na seção **Finanças**, habilite **Permitir que taxas de cobrança no nível da empresa substituam taxas de cobrança no nível do projeto**.

   >[!CAUTION]
   >
   >Ativar essa opção substitui os cálculos de receita históricos, a menos que estejam marcados como faturados. Você pode preservar os cálculos de receita históricos criando um registro de faturamento. Para obter mais informações, consulte o artigo [Criar registros de cobrança](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Clique em **Salvar alterações**.

## Atualizar taxas de cobrança no nível da empresa e aplicá-las a um projeto

Depois que você ativou a opção de substituição de taxas de cobrança no nível da empresa em um projeto, as alterações feitas nas taxas de cobrança da empresa se aplicam ao projeto sempre que as finanças são recalculadas.

>[!NOTE]
>
>Os usuários devem ter acesso a Empresas em seu nível de acesso para atualizar as taxas de cobrança no nível da empresa.

{{step-1-to-setup}}

1. Clique em **Empresas**.
1. Clique no nome da empresa associada ao projeto para o qual você ativou a substituição de taxas de cobrança no nível da empresa.
1. Clique em **Taxas de cobrança** no painel esquerdo.
1. Atualize a **Taxa de Cobrança da Empresa** e as datas de início/término de uma função de trabalho existente, em seguida, pressione Enter.

   Para adicionar uma nova taxa de cobrança da empresa de data efetiva, selecione uma taxa de cobrança para a função de trabalho e clique em **Editar**. Para obter mais informações sobre taxas de cobrança da empresa de data efetiva, consulte [Substituir taxas de cobrança de função de trabalho no nível da empresa](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

1. Para atualizar as taxas da empresa para um ou mais projetos, siga um destes procedimentos:

   * Vários projetos:

      1. Ir para uma lista de projetos.
      1. Marque a caixa de seleção de acordo com os projetos que deseja atualizar.
      1. Clique em **Editar**.
      1. Na seção Configurações, habilite a opção **Recalcular Custos e Receitas**.
      1. Clique em **Salvar alterações**.

   * Um único projeto:

      1. Vá para o projeto para o qual você ativou a substituição de taxas de cobrança no nível da empresa.
      1. Clique no menu **Mais** ![Mais menu](assets/qs-more-icon-on-an-object.png) ao lado do nome do projeto no cabeçalho e clique em **Recalcular Finanças**.
