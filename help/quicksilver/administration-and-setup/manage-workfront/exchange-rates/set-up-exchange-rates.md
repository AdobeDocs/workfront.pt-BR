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
source-git-commit: b16523bf6c37747702efe3b5ecfcc33801526af1
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 5%

---

# Configurar taxas de câmbio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

{{highlighted-preview}}

Como administrador do Adobe Workfront, você pode configurar taxas de câmbio de moeda no Workfront. Isso inclui o seguinte:

* Definição da moeda padrão do sistema Workfront
* Atualizando taxas de câmbio no Workfront para corresponder às taxas de câmbio atuais
* Configurar as taxas de câmbio para várias moedas (isso permite que os usuários escolham uma moeda padrão para projetos individuais)

As taxas de câmbio afetam todos os elementos financeiros no Workfront. A moeda base é a moeda padrão para todos os projetos e relatórios em todo o sistema, a menos que seja substituída por um determinado projeto ou função de trabalho. A moeda base ou padrão atual é indicada por um ícone ![Ícone de moeda padrão](assets/default-icon.png) na lista. Você também pode optar por exibir informações financeiras em moedas disponíveis no sistema que sejam diferentes da moeda base ou da moeda do projeto ao exibi-las em um relatório ou lista. Para obter mais informações, consulte [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obter mais informações sobre como substituir a moeda base no Workfront para projetos e funções de trabalho, consulte os seguintes artigos:

* [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

A maneira como você configura as taxas de câmbio afeta se os usuários podem modificar as taxas de câmbio de um determinado projeto.

>[!IMPORTANT]
>
>As taxas de câmbio no Workfront não são dinâmicas; o valor definido deve ser atualizado quando ocorrerem alterações nas taxas de câmbio.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Para configurar taxas de câmbio: Qualquer pacote de Workfront ou Workflow</p>
       <p>Para aplicar datas de efetivação às taxas de câmbio: pacote Ultimate do workflow</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador de sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

     A nova moeda padrão é atualizada com o ícone ![Ícone de moeda padrão](assets/default-icon.png).

     >[!NOTE]
     >
     >A moeda padrão sempre aparece primeiro na lista, independentemente de como a lista é classificada.

1. (Opcional) Para excluir uma moeda, marque a caixa de seleção ao lado do nome da moeda e selecione **Excluir** na barra de ações na parte inferior da tela. Não é possível excluir a moeda padrão.

<div class="preview">

## Definir datas de efetivação nas taxas de câmbio de uma moeda

As datas de efetivação das taxas de câmbio de uma moeda são configuradas de forma que um valor de taxa termine em uma data específica e outra taxa comece. A taxa de câmbio para a data correta é então usada nos cálculos financeiros.

{{step-1-to-setup}}

1. Clique em **Preferências do Projeto** > **Taxas de Câmbio**.
1. Selecione uma moeda na lista e clique em **Gerenciar datas** na barra de ações.
1. Na caixa de diálogo de **(nome da moeda) taxas em vigor de data**, escolha uma **Data Final** para a taxa de câmbio atual.

   Ou

   Escolha uma **Data de Início** para a nova taxa de câmbio.

   A primeira taxa de câmbio não terá uma data inicial e a última taxa não terá uma data final. Algumas datas são adicionadas automaticamente. Por exemplo, se a primeira taxa não tiver uma data final e você adicionar uma taxa de câmbio com uma data inicial de 1º de dezembro de 2025, uma data final de 30 de novembro de 2025 será adicionada à primeira taxa para que não haja lacunas.

   ![Caixa de diálogo de datas de taxas de câmbio efetivas](assets/euro-date-effective-rates.png)

1. Digite o novo valor de **Taxa de câmbio**.
1. (Opcional) Clique em **Adicionar taxa de efetivação de data** para adicionar mais taxas de câmbio com datas de efetivação para esta moeda.
1. Clique em **Salvar**.

</div>

## Permitir que os usuários modifiquem a moeda padrão de um projeto

Os usuários podem modificar a moeda padrão de um projeto quando as seguintes condições são atendidas:

* O usuário tem uma licença Padrão ou de Plano com acesso administrativo às Taxas de Câmbio.

  Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em um determinado projeto, consulte [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que os usuários modifiquem a moeda padrão de uma função de trabalho

Os usuários podem modificar a moeda de uma função de trabalho quando as seguintes condições forem atendidas:

* O usuário tem uma licença Padrão ou de Plano com acesso administrativo às Funções de trabalho.

  Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em uma determinada função de trabalho, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).



