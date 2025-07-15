---
title: Personalizar a terminologia da interface do usuário usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront, você pode usar um modelo de layout para alterar os rótulos de alguns objetos que aparecem em todo o Workfront para corresponder aos termos usados em sua organização.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 2%

---

# Personalizar a terminologia da interface de usuário usando um modelo de layout

Como administrador do Adobe Workfront, você pode usar um modelo de layout para alterar os rótulos de alguns objetos que aparecem em todo o Workfront para corresponder aos termos usados em sua organização.

Depois de salvar um modelo de layout no qual você alterou a terminologia e, em seguida, fazer logout do Workfront e fazer logon novamente, os rótulos alterados aparecerão onde os rótulos padrão apareceriam na maioria das áreas em todo o Workfront:

* Menu principal
* Todas as áreas acessadas no menu principal
* Todas as guias
* Todos os menus
* Elementos do Report Builder e de relatórios (exibições, filtros e agrupamentos)
* Botões Salvar
* Arquivos exportados
* Emails
* Aplicativos móveis

>[!NOTE]
>
>* A área de Suplemento do Outlook não exibe os rótulos personalizados.
>* Você pode encontrar problemas gramaticais e outros ao personalizar rótulos. Por exemplo, se você alterar &quot;Problema&quot; para &quot;Solicitação&quot;, poderá haver locais na interface do usuário onde você verá a frase &quot;Uma solicitação&quot;. Para obter mais informações, consulte [Implicações da personalização de nomes de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).

Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Após configurar um modelo de layout, você deve atribuí-lo aos usuários para que as alterações feitas fiquem visíveis para outros usuários. Para obter informações sobre como atribuir um modelo de layout aos usuários, consulte [Atribuir usuários a um modelo de layout](../use-layout-templates/assign-users-to-layout-template.md).

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
  <p> Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalizar a terminologia da interface do usuário

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique em **Definir terminologia** próximo ao canto superior direito da página.
1. Siga um destes procedimentos:

   * Para usar um termo alternativo fornecido pelo Workfront, clique na seta para baixo ![ao lado do rótulo e clique no rótulo alternativo desejado na lista suspensa.](assets/dropdown-arrow.png)

     >[!NOTE]
     >
     >Os rótulos alternativos fornecidos nas listas suspensas são compatíveis com as versões do Workfront localizadas para idiomas que não sejam o inglês.

   * Para fornecer sua própria alternativa personalizada para o rótulo exibido para um objeto, clique em **Definir nome personalizado** à direita do rótulo e digite as formas **Singular** e **Plural** do termo personalizado. Você pode clicar em **Redefinir** se mudar de ideia.

     Você pode personalizar os seguintes nomes de objeto:

     <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Objetos do Workfront</p></td>
        <td>
          <p>Portfólio</p>
          <p>Programa</p>
          <p>Projeto</p>
          <p>Tarefa</p>
          <p>Problema</p>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Atividade</p>
         </ul></td>
        <td><p>Para obter mais informações sobre esses objetos, consulte <a href="../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Entender objetos no Adobe Workfront</a>.</p></td>
       </tr>
       <tr>
        <td role="rowheader"><p>Objetos do Workfront Goals</p></td>
        <td>
         <ul>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Atividade</p>
         </ul></td>
        <td><p>Esses objetos exigem uma licença adicional. Para obter mais informações, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">visão geral das Metas do Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Objetos do Planejador de cenários do Workfront</p></td>
        <td>
         <ul>
          <p>Iniciativa</p>
          <p>Cenário</p>
          <p>Plano </p>
         </ul></td>
        <td><p>Esses objetos exigem uma licença adicional. Para obter informações, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Introdução ao Scenario Planner</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Quando terminar, clique em **Concluído**.

   >[!TIP]
   >
   >Depois de clicar em Concluído (e mesmo depois de salvar o modelo de layout), você sempre pode retornar às configurações Definir terminologia e clicar em Redefinir ao lado de qualquer termo personalizado para retorná-lo ao estado padrão.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

1. Para ver as alterações de terminologia:

   1. Faça logout e logon novamente no Workfront.
   1. Feche todas as guias do navegador abertas no ambiente do Workfront.

   >[!IMPORTANT]
   >
   >Isso também é necessário para qualquer pessoa que tenha usado o modelo de layout antes de você fazer as alterações de terminologia.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
