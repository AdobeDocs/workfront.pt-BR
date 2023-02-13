---
title: Conceder acesso a documentos
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário aos documentos no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# Conceder acesso a documentos

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário aos documentos, como explicado em [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Esse acesso também se aplica às pastas do documento.

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
   <td> <p>Você deve ser um administrador do Workfront.&gt;.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar o acesso do usuário aos documentos usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no **Exibir** ou **Editar** à direita de Documentos, em seguida, selecione as capacidades que deseja conceder em **Ajustar as configurações**.

   ![document_access.png](assets/document-access.png)

   Você pode permitir que os usuários façam o seguinte em projetos, tarefas e problemas aos quais tenham acesso:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Criar</td> 
      <td>Carregue documentos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir</td> 
      <td> <p>Remova os documentos carregados.</p> <p>O <b>Criar</b> é ativada automaticamente quando esta opção é ativada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar</td> 
      <td>Compartilhe documentos com usuários, funções de trabalho e equipes específicos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar documentos publicamente</td> 
      <td>Compartilhe documentos com usuários externos (não tem uma licença do Workfront).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhe com todo o sistema</td> 
      <td> <p>Disponibilize documentos para todos na sua instância do Workfront.</p> <p>Qualquer pessoa no sistema pode ver um documento compartilhado dessa maneira se:</p> 
       <ul> 
        <li> <p>Você envia um link para a página Documentos, onde é carregado.</p> </li> 
        <li> <p>Eles pesquisam no Workfront</p> </li> 
       </ul> <p>O <b>Compartilhar</b> é ativada automaticamente quando esta opção é ativada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Quando você configura uma configuração de nível de acesso para um determinado tipo de objeto, essa configuração não afeta o acesso dos usuários a objetos com uma classificação menor. Por exemplo, você pode impedir que usuários excluam projetos em seu nível de acesso, mas isso não os restringe de excluir documentos, que são de classificação inferior à dos projetos.Para obter mais informações sobre a hierarquia de objetos, consulte a seção [Interdependência e hierarquia de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Opcional) Para restringir as permissões herdadas para documentos de objetos de classificação superior, clique em **Definir restrições adicionais**, em seguida selecione **Nunca herdar o acesso ao documento de projetos, tarefas, problemas etc**.
1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

   Depois que o nível de acesso é criado, você pode atribuí-lo a um usuário. Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso a documentos por tipo de licença

Para obter mais informações sobre o que os usuários em cada nível de acesso podem fazer com documentos, consulte a seção [Documentos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).

## Acesso a documentos compartilhados

Após fazer upload de um documento para o Workfront, é possível compartilhá-lo com outros usuários, concedendo permissões a ele, como explicado em [Compartilhar um documento](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Quando você compartilha qualquer objeto com outro usuário, os direitos do recipient são determinados por uma combinação de dois itens:

* As permissões concedidas ao destinatário para o objeto
* As configurações de nível de acesso do recipient para o tipo do objeto
