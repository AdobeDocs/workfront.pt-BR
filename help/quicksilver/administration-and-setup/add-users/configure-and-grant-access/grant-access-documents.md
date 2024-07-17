---
title: Conceder acesso a documentos
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a documentos no Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ba1d9a9b-7a1f-498b-a6e5-c548a11ac87c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 1%

---

# Conceder acesso a documentos

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário a documentos, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

Esse acesso também se aplica a pastas de documentos.

Para obter informações sobre o uso de níveis de acesso personalizados para gerenciar o acesso dos usuários a outros tipos de objetos na Workfront, consulte [Criar ou modifique os níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems plano da Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">licença da Adobe Systems Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.&gt;.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar usuário acesso a documentos usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone ![](assets/gear-icon-settings.png) de engrenagem na **Exibir** ou **na Editar** botão à direita dos Documentos, em seguida, selecione as habilidades que deseja conceder em **Ajustar suas configurações**.

   ![documento_access.png](assets/document-access.png)

   Você pode permitir que os usuários façam o seguinte em projetos, tarefas e problemas aos quais tenham acesso:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Criar</td> 
      <td>Carregar documentos.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Excluir</td> 
      <td> <p>Remover documentos carregados.</p> <p>A opção <b>Criar</b> é habilitada automaticamente quando essa opção é habilitada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar</td> 
      <td>Compartilhe documentos com usuários específicos, funções de trabalho e equipes.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar documentos publicamente</td> 
      <td>Compartilhe documentos com usuários externos (não tem uma licença da Workfront).</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhe com todo o sistema</td> 
      <td> <p>Disponibilize documentos para todos na sua instância da Workfront.</p> <p>Qualquer pessoa no sistema pode ver um documento compartilhado dessa forma se:</p> 
       <ul> 
        <li> <p>Você os envia uma link para os documentos página onde são enviados por upload.</p> </li> 
        <li> <p>Eles pesquisam por isso no Workfront</p> </li> 
       </ul> <p>A opção <b>Compartilhar</b> é habilitada automaticamente quando essa opção é habilitada.</p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Quando você define uma configuração de nível de acesso para um determinado tipo de objeto, essa configuração não afeta o acesso dos usuários aos objetos com uma classificação mais baixa. Por exemplo, você pode impedir que os usuários excluam projetos em seus níveis de acesso, mas isso não os impede de excluir documentos, que são classificações inferiores aos projetos. Para obter mais informações sobre a hierarquia de objetos, consulte a seção [Interdependência e hierarquia de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-interdependency-and-hierarchy-of-objects) no artigo [Entender os objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

1. (Opcional) Para restringir as permissões herdadas de documentos de objetos de classificação mais altos, clique **em Definir restrições** adicionais, em seguida, selecione **Nunca herdar documento acesso de projetos, tarefas, problemas etc**.
1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso à Adobe Systems Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) financeiros.
1. Quando terminar, clique **Salvar**.

   Depois que o nível de acesso é criado, você pode atribuí-lo a uma usuário. Para obter mais informações, consulte [Editar o perfil de uma usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Acesso a documentos por tipo de licença

Para obter mais informações sobre o que os usuários](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#document) de cada nível de acesso podem fazer com documentos, consulte a seção [Documentos no artigo [Funcionalidade disponível para cada tipo](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md) de objeto.

## Acesso a documentos compartilhados

Após carregar um documento no Workfront, você poderá compartilhá-lo com outros usuários concedendo a eles permissões, conforme explicado em [Compartilhar um documento](../../../workfront-basics/grant-and-request-access-to-objects/document-permissions.md).

<!--
If you make changes here, make them also in the "Grant access to" articles where this snippet had to be converted to text:
* reports, dashboards, and calendars
* financial data<
* issue
-->

Quando você compartilha qualquer objeto com outro usuário, os direitos do recipient sobre ele são determinados por uma combinação de dois itens:

* As permissões concedidas ao destinatário para o objeto
* As configurações de nível de acesso do destinatário para o tipo do objeto
