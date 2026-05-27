---
title: Compartilhar um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode configurar o acesso de um formulário personalizado para controlar quem pode exibi-lo, compartilhá-lo e editá-lo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: bb5e1d1df73ecb4ae9749c5e0960b824bf2e6eda
workflow-type: tm+mt
source-wordcount: '980'
ht-degree: 5%

---

# Compartilhar um formulário personalizado

{#preview-fast-release-general}

É possível configurar o acesso para um formulário personalizado para controlar quem — pessoa, função, grupo, equipe, empresa, perfil de negócios — pode exibi-lo, compartilhá-lo e editá-lo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Acesso a formulários personalizados {#access-to-custom-forms}

Por padrão, quando você cria um novo formulário personalizado e alguém o anexa a um objeto, qualquer usuário atribuído ao objeto pode visualizar e preencher o formulário. Isso inclui usuários com licenças de Colaborador ou Solicitação e usuários externos.

No entanto, em um objeto em que o formulário personalizado ainda não está anexado, um usuário (mesmo que tenha um nível de acesso de Planejador) não pode anexá-lo pelo menu suspenso Forms personalizado, a menos que uma das seguintes opções seja verdadeira:

* <span class="preview">Alguém compartilhou o formulário personalizado como &quot;Todos no sistema podem exibir e anexar&quot;</span>
* Alguém compartilhou o formulário personalizado com o usuário ou com sua equipe, função de trabalho, grupo, empresa ou perfil de negócios que concede pelo menos a permissão Exibir com a opção Anexar aos dados personalizados selecionada
* O usuário tem uma licença Padrão ou de Plano e seu nível de acesso permite acesso administrativo a formulários personalizados

<!--

## Share a custom form from the list of forms

Rather than leaving a custom form in the default sharing state (described in [Access to custom forms](#access-to-custom-forms) in this article), you can configure specific levels of access to the form for certain users, job roles, groups, teams, and companies.

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Select the custom form, then click ![Share icon](assets/share-icon.png).
1. In the box that displays, under **Give custom form access to**, start typing the name of the user, team, job role, group, company, or business profile you want to share the custom form with, then press **Enter** when the name displays.
1. To adjust access for the user, team, job role, group, company, or business profile you just added, click the drop-down menu to the right of the name, then configure one of the following available options and any of its advanced settings:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">View it</td> 
      <td> <p>This option provides the ability to view and fill out the custom form on objects. At the object level, users must also have at least Contribute access with the <strong>Edit custom form</strong> advanced setting enabled. For example, if the form is attached to a project, users must have Contribute access to that project, or they will not be able to fill out the form.</p>
      
      <p><b>NOTE</b>: For users with Light and Contributor licenses (or Work, Review, and Request licenses), this is the highest available option.</p>
      
      <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow the following:</p> 
       <ul> 
        <li><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</li> 
        <li> <p><strong>Share</strong>: Ability to share the custom form with others in the system</p> <p>Users with a Light or Contributor license (or Work, Review, or Request license) can share a custom form only through the API or a custom forms report.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Manage it</td> 
      <td> <p>This option available only for users with a Standard or Plan license. </p> <p>In addition to being able to add the form to objects they have access to edit, users can also fully edit the custom form, including adding, editing, and deleting fields.</p> <p>Click <strong>Advanced Settings</strong> to specify whether you want to allow following:</p> 
       <ul> 
        <li> <p><strong>Attach to custom data</strong>: Ability to attach the custom form to projects, tasks, and issues for which they have Manage access</p> </li> 
        <li><strong>Delete</strong>: Delete the custom form from the system</li> 
        <li><strong>Share</strong>: Share the custom form with others in the system</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Optional) Repeat Steps 4-5 to add other names to the list and configure their options.
1. (Optional) If you want to limit access to the custom form (on objects where it's attached) to those you have specified in the previous steps, click the gear icon ![](assets/gear-icon-settings-with-dn-arrow.jpg) in the upper right corner of the sharing box, then click **Remove system-wide access**.

   If you change your mind, you can click **Make this visible system-wide** (the default option).

   >[!NOTE]
   >
   >* When you make a custom form visible system-wide, you allow users only to see and fill it out on objects they are assigned to, not to attach it to other objects. You can grant the ability to attach the custom form to objects using the option "Attach to custom data" explained under step 5.
   >* Most organizations want to ensure that everyone in the system can fill out a custom form when it's attached to objects they work on and view its data in reports. If this is true for your organization, we recommend that you use **Make this visible system-wide**. When the option is configured this way, "Visible System-Wide" displays in the dialog box:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >If you are concerned about a custom form where users might enter sensitive data when it is attached to certain objects, limiting sharing for those *objects* might be better rather than limiting access to the form itself.

1. Click **Save**.

-->

## Compartilhar um formulário personalizado

Em vez de deixar um formulário personalizado no estado de compartilhamento padrão (descrito em [Acesso a formulários personalizados](#access-to-custom-forms) neste artigo), você pode configurar níveis específicos de acesso ao formulário para determinados usuários, funções de trabalho, grupos, equipes, empresas e perfis comerciais.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Selecione o formulário personalizado na lista e clique em ![Ícone Compartilhar](assets/share-icon.png).

   Ou

   Abra um formulário personalizado ou crie um novo formulário personalizado. Em seguida, clique em **Compartilhar** na parte superior direita do designer do formulário.

1. Na caixa de compartilhamento, em **Conceder acesso ao formulário personalizado**, comece digitando o nome do usuário, da equipe, da função de trabalho, do grupo, da empresa ou do perfil de negócios com o qual deseja compartilhar o formulário personalizado e pressione **Enter** quando o nome for exibido.
1. Para ajustar o acesso do usuário, equipe, função de trabalho, grupo, empresa ou perfil comercial que você acabou de adicionar, clique no menu suspenso à direita do nome e configure uma das seguintes opções disponíveis e qualquer uma de suas configurações avançadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exibir</td> 
      <td> <p>Essa opção fornece a capacidade de exibir e preencher o formulário personalizado em objetos. No nível do objeto, os usuários também devem ter pelo menos acesso ao Contribute com a configuração avançada <strong>Editar formulário personalizado</strong> ativada. Por exemplo, se o formulário estiver anexado a um projeto, os usuários devem ter acesso ao Contribute a esse projeto, ou não poderão preencher o formulário.</p>

   <p><b>OBSERVAÇÃO</b>: para usuários com licenças Light e de Colaborador (ou licenças de Trabalho, Revisão e Solicitação), esta é a opção mais alta disponível.</p> <p>Clique em <strong>Configurações Avançadas</strong> para especificar se deseja permitir o seguinte:</p> 
       <ul> 
        <li><strong>Anexar a dados personalizados</strong>: capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</li> 
        <li> <p><strong>Compartilhar</strong>: capacidade de compartilhar o formulário personalizado com outras pessoas no sistema</p> <p>Os usuários com uma licença Light ou de Colaborador (ou licença de Trabalho, Revisão ou Solicitação) podem compartilhar um formulário personalizado somente por meio da API ou de um relatório de formulários personalizado.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar</td> 
      <td> <p>Essa opção está disponível somente para usuários com uma licença Padrão ou de Plano. </p> <p>Além de poder adicionar o formulário aos objetos que eles têm acesso para editar, os usuários também podem editar totalmente o formulário personalizado, incluindo adicionar, editar e excluir campos.</p> <p>Clique em <strong>Configurações Avançadas</strong> para especificar se deseja permitir o seguinte:</p> 
       <ul> 
        <li> <p><strong>Anexar a dados personalizados</strong>: capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</p> </li> 
        <li><strong>Excluir</strong>: excluir o formulário personalizado do sistema</li> 
        <li><strong>Compartilhar</strong>: compartilhar o formulário personalizado com outras pessoas no sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita as etapas 5 a 6 para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Se quiser limitar o acesso ao formulário personalizado (nos objetos ao qual ele está anexado) àqueles que você especificou nas etapas anteriores, clique na seta suspensa em **Quem tem acesso** e selecione **Somente pessoas convidadas podem acessar**.

   Se mudar de ideia, você pode selecionar **Todos no sistema podem visualizar**.

   >[!NOTE]
   >
   >* Ao tornar um formulário personalizado visível em todo o sistema, você permite que os usuários o vejam e preencham apenas nos objetos aos quais estão atribuídos, e não anexem a outros objetos. Você pode conceder a capacidade de anexar o formulário personalizado a objetos usando a opção &quot;Anexar a dados personalizados&quot; explicada na etapa 6.
   >* A maioria das organizações quer garantir que todos no sistema possam preencher um formulário personalizado quando ele estiver anexado a objetos nos quais trabalham e visualizar seus dados em relatórios. Se isso for verdadeiro para sua organização, recomendamos que você use o **Todos no sistema podem visualizar**.
   >* <span class="preview">Se você selecionar **Todos no sistema podem exibir e anexar**, todos os usuários poderão anexar o formulário a outros objetos.</span>
   >
   ><span class="preview">Imagem de exemplo no ambiente de Visualização:</span>
   >![Compartilhar formulário personalizado](assets/share-custom-forms-all-can-attach.png)
   >   
   >Imagem de amostra no ambiente de produção:
   >![Compartilhar formulário personalizado](assets/share-custom-form-in-designer.png)
   >   
   >Se você estiver preocupado com um formulário personalizado em que os usuários podem inserir dados confidenciais quando ele é anexado a determinados objetos, limitar o compartilhamento para esses *objetos* pode ser mais eficaz, em vez de limitar o acesso ao próprio formulário.

1. Clique em **Salvar**.

## Remover o acesso a um formulário personalizado

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Selecione o formulário personalizado na lista e clique em ![Ícone Compartilhar](assets/share-icon.png).
1. Na caixa de compartilhamento, clique no menu suspenso à direita do nome do usuário, equipe, função, grupo, empresa ou perfil comercial que você não deseja mais ter acesso especial ao formulário e selecione **Remover**.
1. (Opcional) Repita a etapa anterior para outros nomes que você deseja remover.
1. Clique em **Salvar**.

