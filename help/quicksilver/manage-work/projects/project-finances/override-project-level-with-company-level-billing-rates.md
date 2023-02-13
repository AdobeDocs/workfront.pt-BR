---
product-area: projects
navigation-topic: financials
title: Substituir as taxas de faturamento no nível do projeto por taxas de faturamento no nível da empresa
description: Substituir as taxas de faturamento no nível do projeto por taxas de faturamento no nível da empresa
author: Alina
feature: Work Management
exl-id: 02ea4c7c-0473-4cc4-913c-3baa613767b7
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 0%

---

# Substituir as taxas de faturamento no nível do projeto por taxas de faturamento no nível da empresa

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN THE EDIT PROJECT MODAL)</p>
-->

Você pode configurar um projeto para usar taxas de faturamento em nível de empresa, em vez de taxas de faturamento em nível de projeto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões do projeto com permissões para Gerenciar finanças</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Ativar a opção Substituição de Taxas de Faturamento no Nível da Empresa

Quando uma empresa está associada a um projeto e essa opção está ativada, as alterações feitas nas taxas de faturamento no nível da empresa substituem a taxa de faturamento definida no projeto.

Quando um usuário recalcula manualmente as finanças no projeto, quaisquer alterações nas taxas de faturamento no nível da empresa são aplicadas. Os cálculos de receita histórica também são substituídos, a menos que sejam marcados como faturados.

1. Vá para um projeto.
1. Clique no botão **Mais** menu ![](assets/qs-more-icon-on-an-object.png) ao lado do nome do projeto no cabeçalho, clique em **Editar**.
1. No **Finanças** ative a **Permitir que as taxas de faturamento em nível de empresa substituam as taxas de faturamento em nível de projeto**.

   >[!CAUTION]
   >
   >Ativar essa opção substitui os cálculos de receita histórica, a menos que sejam marcados como faturados. Você pode preservar os cálculos de receita históricos criando um registro de faturamento. Para obter mais informações, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md)

1. Clique em **Salvar alterações**.

## Atualizar as Taxas de Faturamento no nível da Empresa e aplicá-las a um projeto

Após ativar a opção de substituição de taxas de faturamento em nível de empresa em um projeto, as alterações feitas nas taxas de faturamento da empresa se aplicam ao projeto sempre que as finanças são recalculadas.

>[!NOTE]
>
>Os usuários devem ter acesso às Empresas em seu nível de acesso para atualizar as taxas de faturamento da empresa.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração**.
1. Clique em **Empresas**.
1. Clique no nome da empresa associada ao projeto para o qual você ativou a substituição das taxas de faturamento no nível da empresa.
1. Clique em **Taxas de Faturamento** no painel esquerdo.
1. Informe a nova taxa de faturamento para uma função de cargo existente no **Taxa de Faturamento da Empresa** e pressione Enter.
1. Para atualizar as taxas da empresa para um ou mais projetos, execute um dos seguintes procedimentos:

   * Vários projetos:
   1. Acesse uma lista de projetos.
   1. Marque a caixa de seleção de acordo com os projetos que deseja atualizar.
   1. Clique em **Editar**.
   1. Na seção Configurações , habilite o **Recalcular Custos E Receitas** opção.
   1. Clique em **Salvar alterações**.
   * Projeto único:

      1. Vá para o projeto para o qual você ativou a substituição das taxas de faturamento no nível da empresa.
      1. Clique no botão **Mais** menu ![](assets/qs-more-icon-on-an-object.png) ao lado do nome do projeto no cabeçalho, em seguida, clique em **Recalcular Finanças**.
