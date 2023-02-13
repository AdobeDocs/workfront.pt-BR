---
title: Personalizar a terminologia da interface do usuário usando um modelo de layout
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador do Adobe Workfront, você pode usar um modelo de layout para alterar os rótulos de alguns objetos que aparecem em todo o Workfront para corresponder aos termos usados em sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3ab3ca43-d8e9-4545-a862-e6bf9419ef16
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 3%

---

# Personalizar a terminologia da interface do usuário usando um modelo de layout

Como administrador do Adobe Workfront, você pode usar um modelo de layout para alterar os rótulos de alguns objetos que aparecem em todo o Workfront para corresponder aos termos usados em sua organização.

Depois de salvar um modelo de layout em que a terminologia foi alterada, em seguida, saia do Workfront e entre novamente, os rótulos alterados são exibidos, onde os rótulos padrão são exibidos na maioria das áreas em todo o Workfront:

* Menu principal
* Todas as áreas acessadas do Menu Principal
* Todas as guias
* Todos os menus
* Report Builder e elementos de relatório (exibições, filtros e agrupamentos)
* Botões Salvar
* Arquivos exportados
* Emails
* Aplicativos móveis

>[!NOTE]
>
>* A área Suplemento do Outlook não exibe os rótulos personalizados.
>* Você pode encontrar gramática e outros problemas ao personalizar rótulos. Por exemplo, se você alterar &quot;Emitir&quot; para &quot;Solicitação&quot;, poderá haver lugares na interface do usuário onde você verá a frase &quot;Uma solicitação&quot;. Para obter mais informações, consulte [Implicações da personalização de nomes de objetos](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#implications-of-customizing-object-names) no artigo [Entender objetos no Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)
>


Para obter informações sobre modelos de layout para grupos, consulte [Criar e modificar modelos de layout de um grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

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
   <td> <p>Para executar essas etapas no nível do sistema, é necessário o nível de acesso Administrador do sistema.
Para executá-los para um grupo, você deve ser um gerente desse grupo.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalizar a terminologia da interface do usuário

1. Comece a trabalhar em um modelo de layout, conforme descrito em [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clique em **Definir Terminologia** próximo ao canto superior direito da página.
1. Siga um destes procedimentos:

   * Para usar um termo alternativo fornecido pelo Workfront, clique na seta para baixo  ![](assets/dropdown-arrow.png) ao lado do rótulo, clique no rótulo alternativo que deseja na lista suspensa.

      >[!NOTE]
      >
      >Rótulos alternativos fornecidos nas listas suspensas são compatíveis em versões do Workfront localizadas em idiomas diferentes do inglês.

   * Para fornecer sua própria alternativa personalizada para o rótulo exibido para um objeto, clique em **Definir nome personalizado** à direita do rótulo, em seguida, digite o **Singular** e **Plural** formas do termo personalizado. Você pode clicar em **Redefinir** se mudar de ideia.

      Você pode personalizar os seguintes nomes de objeto:

      <table style="table-layout:auto">
      <col>
      <col>
      <col>
      <tbody>
       <tr>
        <td role="rowheader"><p>Objetos Workfront</p></td>
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
        <td role="rowheader"><p>Objetos de metas do Workfront</p></td>
        <td>
         <ul>
          <p>Meta</p>
          <p>Resultado</p>
          <p>Atividade</p>
         </ul></td>
        <td><p>Esses objetos exigem uma licença adicional. Para obter mais informações, consulte <a href="../../../workfront-goals/goal-management/wf-goals-overview.md" class="MCXref xref">Visão geral das Metas da Adobe Workfront</a>.</p></td>
       </tr>
       <tr data-mc-conditions="">
        <td role="rowheader"><p>Objetos do Workfront Scenario Planner</p></td>
        <td>
         <ul>
          <p>Iniciativa</p>
          <p>Cenário</p>
          <p>Plano </p>
         </ul></td>
        <td><p>Esses objetos exigem uma licença adicional. Para obter mais informações, consulte <a href="../../../scenario-planner/get-started-with-scenario-planning.md" class="MCXref xref">Introdução ao Planejador de cenário</a>.</p></td>
       </tr>
      </tbody>
     </table>

1. Quando terminar, clique em **Concluído**.

   >[!TIP]
   >
   >Depois de clicar em Concluído (e mesmo depois de salvar seu modelo de layout), você sempre poderá retornar às configurações Definir terminologia e clicar em Redefinir ao lado de qualquer termo personalizado para retorná-los ao seu estado padrão.

1. Continue personalizando o modelo de layout.

   Ou

   Se tiver terminado de personalizar, clique em **Salvar**.

1. Para ver as alterações de terminologia:

   1. Faça logoff e volte no Workfront.
   1. Feche todas as guias do navegador abertas para seu ambiente Workfront.

   >[!IMPORTANT]
   >
   >Isso também é necessário para qualquer pessoa que usou o modelo de layout antes de fazer as alterações de terminologia.

Para obter mais informações sobre modelos de layout, consulte [Criar e gerenciar modelos de layout](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
