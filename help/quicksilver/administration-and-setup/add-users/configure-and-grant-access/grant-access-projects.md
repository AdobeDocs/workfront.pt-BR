---
title: Conceder acesso aos projetos
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário aos projetos no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba6a9e68-68a1-4152-b024-cd39e06d556f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 0%

---

# Conceder acesso aos projetos

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário aos projetos, como explicado em [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Para obter informações sobre como usar níveis de acesso personalizados para gerenciar o acesso dos usuários a outros tipos de objetos no Workfront, consulte [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

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
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar o acesso do usuário a projetos usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no **Exibir** ou **Editar** à direita de Projetos, em seguida, selecione as habilidades que deseja conceder em **Ajustar as configurações**.

   ![](assets/planner-fine-tune-your-settings-with-copy-projects.png)

   >[!NOTE]
   >
   >* Os usuários com uma licença de Trabalho têm direitos de projeto limitados. Podem contribuir para um projeto, mas não gerenciá-lo.
   >* Os usuários com uma licença de Revisão têm direitos de Exibição em projetos de problemas convertidos, mas seus direitos de Exibição são limitados.
   >* Para obter informações sobre permissões que os usuários podem conceder ao compartilhar projetos com outras pessoas, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
   >* Quando você configura uma configuração de nível de acesso para um determinado tipo de objeto, essa configuração não afeta o acesso dos usuários a objetos com uma classificação menor. Por exemplo, você pode impedir que usuários excluam projetos em seu nível de acesso, mas isso não os restringe de excluir tarefas, que são de classificação inferior à dos projetos.Para obter mais informações sobre a hierarquia de objetos, consulte a seção [Interdependência e hierarquia de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).


1. (Opcional) Clique em **definir padrões de compartilhamento** à direita da opção Criar , em seguida **Adicionar regra** para adicionar uma regra de compartilhamento para novos projetos.

   Quando o usuário com esse nível de acesso cria um projeto, o projeto é compartilhado automaticamente com os usuários selecionados no menu à esquerda.

   ![](assets/project-sharing-menu.png)

   No menu à direita, especifique como deseja que o projeto seja compartilhado com esses usuários:

   ![](assets/project-sharing-right-menu.png)

   >[!NOTE]
   >
   >Se um usuário com esse nível de acesso estiver usando um modelo de acesso a projeto, o modelo substituirá as configurações de compartilhamento no nível de acesso. Para obter informações sobre modelos de acesso a projetos, consulte [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

   É possível repetir essa etapa para adicionar quantas regras de compartilhamento de projeto forem necessárias para o nível de acesso.

1. Clique no X para fechar o **Ajustar as configurações** caixa.
1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

   Depois que o nível de acesso é criado, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso a relatórios, painéis e calendários por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com problemas, consulte a seção [Projetos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#projects) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso a projetos compartilhados

Como proprietário ou criador de um problema, você pode compartilhar com outros usuários, concedendo permissões a eles, como explicado em [Compartilhar um projeto no Adobe Workfront](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data
* issue
-->

Quando você compartilha qualquer objeto com outro usuário, os direitos do recipient são determinados por uma combinação de dois itens:

* As permissões concedidas ao destinatário para o objeto
* As configurações de nível de acesso do recipient para o tipo do objeto
