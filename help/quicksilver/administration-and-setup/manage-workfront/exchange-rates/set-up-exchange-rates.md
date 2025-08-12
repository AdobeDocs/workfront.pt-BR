---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Configurar Taxas de Câmbio
description: As taxas de câmbio afetam todos os elementos financeiros no Workfront. A moeda base é a moeda padrão para todos os projetos no sistema.
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: cb12c715d6b20dd4737e2d2e29d9849f08ce67e9
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 2%

---

# Configurar taxas de câmbio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador do Adobe Workfront, você pode configurar taxas de câmbio de moeda no Workfront. Isso inclui o seguinte:

* Definição da moeda padrão do sistema Workfront
* Atualizando taxas de câmbio no Workfront para corresponder às taxas de câmbio atuais
* Configurar as taxas de câmbio para várias moedas (isso permite que os usuários escolham uma moeda padrão para projetos individuais)

As taxas de câmbio afetam todos os elementos financeiros no Workfront. A moeda base é a moeda padrão para todos os projetos em todo o sistema, a menos que seja substituída para um determinado projeto ou função de trabalho. A moeda base ou padrão atual é indicada por um ícone ![Ícone de moeda padrão](assets/default-icon.png) na lista. Você também pode optar por exibir informações financeiras em moedas disponíveis no sistema que sejam diferentes da moeda base ou da moeda do projeto ao exibi-las em um relatório ou lista. Para obter mais informações, consulte [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obter mais informações sobre como substituir a moeda base no Workfront para projetos e funções de trabalho, consulte os seguintes artigos:

* [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

A maneira como você configura as taxas de câmbio afeta se os usuários podem modificar as taxas de câmbio de um determinado projeto.

>[!IMPORTANT]
>
>As taxas de câmbio no Workfront não são dinâmicas; o valor definido deve ser atualizado quando ocorrerem alterações nas taxas de câmbio.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Novo: Padrão</p>
       <p>Ou</p>
       <p>Atual: Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar taxas de câmbio

{{step-1-to-setup}}

1. Clique em **Preferências do Projeto** > **Taxas de Câmbio**.

1. Clique em **Adicionar moeda**.
1. Na caixa **Adicionar moeda**, comece digitando o nome da moeda e, em seguida, clique nele quando ele aparecer na lista suspensa.
1. No campo **Taxa de câmbio**, insira a taxa da moeda selecionada em comparação à moeda definida como moeda base no sistema.
1. Clique em **Adicionar** para adicionar a nova moeda e sua taxa de câmbio.
1. (Opcional) Para alterar a moeda base (padrão), siga um destes procedimentos:

   * Marque a caixa de seleção ao lado do nome da moeda e selecione **Tornar padrão** na barra de ações, na parte inferior da tela.
   * Passe o mouse sobre o nome da moeda e clique no menu **Mais** que aparece. Em seguida, selecione **Tornar Padrão**.

     A nova moeda padrão é atualizada com o ícone.

1. (Opcional) Para excluir uma moeda, marque a caixa de seleção ao lado do nome da moeda e selecione **Excluir** na barra de ações na parte inferior da tela. Não é possível excluir a moeda padrão.

## Permitir que os usuários modifiquem a moeda padrão de um projeto

Os usuários podem modificar a moeda padrão de um projeto quando as seguintes condições são atendidas:

* O usuário tem uma licença Padrão ou Plano com acesso administrativo a Taxas de Câmbio.

  Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em um determinado projeto, consulte [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que os usuários modifiquem a moeda padrão de uma função de trabalho

Os usuários podem modificar a moeda de uma função de trabalho quando as seguintes condições forem atendidas:

* O usuário tem uma licença Padrão ou de Plano com acesso administrativo às Funções de trabalho.

  Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em uma determinada função de trabalho, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).


<!--The default currency is the currency that is used as the default for all projects and reports throughout the system. The current default is indicated with an icon ![Default currency icon](assets/default-icon.png).-->
