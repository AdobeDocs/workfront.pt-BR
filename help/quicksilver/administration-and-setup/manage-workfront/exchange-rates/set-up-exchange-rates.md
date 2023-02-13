---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: Como administrador do Adobe Workfront, você pode configurar taxas de câmbio no Workfront.
description: Configurar taxas de câmbio
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# Configurar taxas de câmbio

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador do Adobe Workfront, você pode configurar taxas de câmbio no Workfront. Isso inclui o seguinte:

* Configuração da moeda padrão para o sistema Workfront
* Atualização das taxas de câmbio no Workfront para corresponder às taxas de câmbio atuais
* Configurar as taxas de câmbio para várias moedas (isso permite que os usuários escolham uma moeda padrão para projetos individuais)

As taxas de câmbio afetam todos os elementos financeiros no Workfront. A Moeda de base é a moeda padrão para todos os projetos em todo o sistema, a menos que seja substituída para um determinado projeto ou função de cargo. Você também pode optar por exibir informações financeiras em moedas disponíveis no sistema que sejam diferentes da moeda base ou da do projeto ao exibi-las em um relatório ou lista. Para obter mais informações, consulte [Criar relatórios de dados financeiros com taxas de câmbio exclusivas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

Para obter mais informações sobre a substituição da Moeda de base no Workfront para projetos e funções de jobs, consulte os seguintes artigos:

* [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md)
* [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

A forma como você configura as taxas de câmbio afeta se os usuários podem modificar as taxas de câmbio de um determinado projeto.

>[!IMPORTANT]
>
>As taxas de câmbio no Workfront não são dinâmicas; o valor definido deve ser atualizado quando ocorrerem alterações nas taxas de câmbio.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar taxas de câmbio

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Preferências do projeto** > **Taxas De Câmbio.**

1. Clique em **Adicionar Moeda.**
1. Comece digitando o nome da moeda e clique nela quando ela for exibida na lista suspensa.

1. No campo fornecido, especifique a taxa para a moeda selecionada, pois está relacionada à moeda definida como a moeda base no sistema.
1. (Opcional) Defina a moeda como a moeda base (padrão) para o Workfront.

   Essa é a moeda usada como padrão para todos os projetos e relatórios em todo o sistema.

1. Clique em **Salvar** para salvar as alterações.

## Permitir que os usuários modifiquem a moeda padrão de um projeto

Os usuários podem modificar a moeda padrão de um projeto quando as seguintes condições forem atendidas:

* O usuário tem uma licença de Plano com acesso administrativo a Taxas de Troca.

   Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em um determinado projeto, consulte [Alterar a moeda do projeto](../../../manage-work/projects/project-finances/change-project-currency.md).

## Permitir que os usuários modifiquem a moeda padrão de uma função de trabalho

Os usuários podem modificar a moeda de uma função de cargo quando as seguintes condições forem atendidas:

* O usuário tem uma licença de Plano com acesso administrativo a Funções de Trabalho.

   Para obter mais informações, consulte [Conceder aos usuários acesso administrativo a determinadas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Mais de uma moeda está ativada no sistema Workfront.

Para obter informações sobre como os usuários podem alterar a moeda padrão em uma determinada função de trabalho, consulte [Criar e gerenciar funções de trabalho](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
