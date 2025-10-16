---
title: Conceder acesso a relatórios, painéis e calendários
user-type: administrator
product-area: system-administration;dashboards;calendars
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a relatórios, painéis e calendários no Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 776bb223-3481-4ea9-8049-276b2dec95c5
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# Conceder acesso a relatórios, painéis e calendários

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a relatórios, painéis e calendários, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Esse acesso também inclui o acesso a Páginas Externas. Para obter informações sobre Páginas Externas, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

>[!NOTE]
>
>* Se quiser conceder aos usuários acesso a relatórios, painéis e calendários, você também deverá conceder a esses usuários acesso a filtros, visualizações e agrupamentos. Para obter instruções, consulte [Conceder acesso a filtros, visualizações e agrupamentos](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md).
>* Quando alguém compartilha um relatório, painel ou calendário com outro usuário, os direitos do recipient nele são determinados por uma combinação de dois fatores: A configuração de nível de acesso do recipient para relatórios, painéis e calendários _e_ todas as permissões que o compartilhador concedeu ao relatório, painel ou calendário
>
>Para obter informações sobre permissões que os usuários podem conceder a um relatório, painel ou calendário durante o compartilhamento, consulte [Compartilhar relatórios, painéis e calendários](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o acesso do usuário a relatórios, painéis e calendários usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, conforme explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no botão **Exibir** ou **Editar** à direita de Relatórios e selecione as capacidades que deseja conceder em **Ajustar suas configurações**.

   ![reports_access.png](assets/reports-access.png)

   As seguintes opções são ativadas por padrão:

   * **Criar**
   * **Excluir**
   * **Exibir relatórios internos**: esta opção precisa ser selecionada para que os relatórios criados pela Workfront possam ser vistos.
   * **Compartilhar**
   * **Compartilhar Relatórios Publicamente**: os relatórios podem ser compartilhados publicamente, compartilhando um link público com o relatório com qualquer pessoa que não tenha uma conta do Workfront. Essa opção deve ser selecionada para permitir esse nível de compartilhamento.
   * **Compartilhar em todo o sistema**: os relatórios podem ser compartilhados com qualquer pessoa no sistema que tenha uma licença do Workfront. Essa opção deve ser selecionada para permitir esse nível de compartilhamento.

     Para obter informações sobre como compartilhar relatórios, painéis e calendários, consulte [Compartilhar relatórios, painéis e calendários](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

   Após criar o nível de acesso, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso a relatórios, painéis e calendários por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com problemas, consulte a seção [Relatórios](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#reports) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso a relatórios, painéis e calendários compartilhados

Como proprietário ou criador de um relatório, painel ou calendário, você pode compartilhá-lo com outros usuários concedendo a eles permissões, conforme explicado em [Compartilhar relatórios, painéis e calendários](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:</p>
<p>* reports, dashboards, and calendars</p>
<p>* financial data</p>
<p>* issue</p>
</div>
-->

Quando você compartilha qualquer objeto com outro usuário, os direitos do recipient sobre ele são determinados por uma combinação de dois itens:

* As permissões concedidas ao destinatário para o objeto
* As configurações de nível de acesso do destinatário para o tipo do objeto
