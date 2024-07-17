---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Configurar taxas de câmbio
description: Como administrador do Adobe Workfront, você pode configurar taxas de câmbio de moeda no Workfront.
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: b0cf0a5ec6b932267c8714b966638d8da93331b8
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 3%

---

# Configurar taxas de câmbio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador do Adobe Workfront, você pode configurar taxas de câmbio de moeda no Workfront. Isso inclui o seguinte:

* Definição da moeda padrão do sistema Workfront
* Atualizando taxas de câmbio no Workfront para corresponder às taxas de câmbio atuais
* Configurar as taxas de câmbio para várias moedas (isso permite que os usuários escolham uma moeda padrão para projetos individuais)

As taxas de câmbio afetam todos os elementos financeiros no Workfront. A Moeda Base é a moeda padrão para todos os projetos em todo o sistema, a menos que seja substituída para um determinado projeto ou função de trabalho. Você também pode optar por exibir informações financeiras em moedas disponíveis no sistema que sejam diferentes da moeda base ou da moeda do projeto ao exibi-las em um relatório ou lista. Para obter mais informações, consulte [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obter mais informações sobre como substituir a Moeda base no Workfront para projetos e funções de trabalho, consulte os seguintes artigos:

* [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

A maneira como você configura as taxas de câmbio afeta se os usuários podem modificar as taxas de câmbio de um determinado projeto.

>[!IMPORTANT]
>
>As taxas de câmbio no Workfront não são dinâmicas; o valor definido deve ser atualizado quando ocorrerem alterações nas taxas de câmbio.

## Requisitos de acesso

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar taxas de câmbio

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Preferências do Projeto** > **Taxas de Câmbio.**

1. Clique em **Adicionar moeda.**
1. Comece digitando o nome da moeda e clique nele quando ele aparecer na lista suspensa.

1. No campo fornecido, especifique a taxa da moeda selecionada, pois ela está relacionada à moeda definida como a moeda base no sistema.
1. (Opcional) Defina a moeda como a moeda base (padrão) do Workfront.

   Essa é a moeda usada como padrão para todos os projetos e relatórios no sistema.

1. Clique em **Salvar** para salvar as alterações.

## Permitir que os usuários modifiquem a moeda padrão de um projeto

Os usuários podem modificar a moeda padrão de um projeto quando as seguintes condições são atendidas:

* O usuário tem uma licença de Plano com acesso administrativo a Taxas de Câmbio.

  Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em um determinado projeto, consulte [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que os usuários modifiquem a moeda padrão de uma função de trabalho

Os usuários podem modificar a moeda de uma função de trabalho quando as seguintes condições forem atendidas:

* O usuário tem uma licença de Plano com acesso administrativo a Funções de trabalho.

  Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em uma determinada função de trabalho, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
