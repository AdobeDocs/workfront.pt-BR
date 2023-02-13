---
title: Compartilhar um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode configurar o acesso de um formulário personalizado para controlar quem (pessoa, função, grupo, equipe, empresa) pode visualizá-lo, compartilhá-lo e editá-lo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '884'
ht-degree: 1%

---

# Compartilhar um formulário personalizado

Você pode configurar o acesso de um formulário personalizado para controlar quem (pessoa, função, grupo, equipe, empresa) pode visualizá-lo, compartilhá-lo e editá-lo.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com o administrador da Workfront.

## Acesso a formulários personalizados {#access-to-custom-forms}

Por padrão, quando um novo formulário personalizado é criado e alguém o anexa a um objeto, qualquer usuário atribuído a ele pode exibir e preencher o formulário. Isso inclui usuários com licenças de solicitação e usuários externos.

No entanto, em um objeto no qual o formulário personalizado ainda não está anexado, um usuário (mesmo que ele tenha um nível de acesso de Planejador) não poderá anexá-lo a partir do menu suspenso Forms Personalizado, a menos que uma das opções a seguir seja verdadeira:

* Alguém compartilhou o formulário personalizado com o usuário ou com sua equipe, função de trabalho, grupo ou empresa, concedendo pelo menos a permissão Exibir com a opção Anexar dados personalizados selecionada
* O usuário tem uma licença de Plano e seu nível de acesso permite acesso administrativo a formulários personalizados

## Compartilhar um formulário personalizado

Em vez de deixar um formulário personalizado no estado de compartilhamento padrão (descrito em [Acesso a formulários personalizados](#access-to-custom-forms) neste artigo), é possível configurar níveis específicos de acesso ao formulário para determinados usuários, funções, grupos, equipes e empresas.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizada**.
1. Selecione o formulário personalizado e clique em **Compartilhar**.
1. Na caixa exibida, em **Conceder acesso ao formulário personalizado para**, comece digitando o nome do usuário, equipe, função de trabalho, grupo ou empresa com quem deseja compartilhar o formulário personalizado e pressione **Enter** quando o nome for exibido.
1. Para ajustar o acesso do usuário, da equipe, da função de trabalho, do grupo ou da empresa que acabou de adicionar, clique no menu suspenso à direita do nome e, em seguida, defina uma das seguintes opções disponíveis e qualquer uma de suas configurações avançadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizar o projeto</td> 
      <td> <p>Capacidade de exibir e preencher o formulário personalizado em objetos.</p> <p><b>OBSERVAÇÃO</b>: Para usuários com licenças de Trabalho, Revisão e Solicitação, essa é a opção mais alta disponível.</p> <p>Clique em <strong>Configurações avançadas</strong> para especificar se você deseja permitir o seguinte:</p> 
       <ul> 
        <li><strong>Anexar a dados personalizados</strong>: Capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</li> 
        <li> <p><strong>Compartilhar</strong>: Capacidade de compartilhar o formulário personalizado com outras pessoas no sistema</p> <p>Os usuários com uma licença de Trabalho, Revisão ou Solicitação podem compartilhar um formulário personalizado somente por meio da API ou de um relatório de formulários personalizado. Para obter mais informações, consulte .</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar o projeto</td> 
      <td> <p>Disponível somente para usuários com uma licença do Plano. </p> <p>Além de poder adicionar o formulário aos objetos que têm acesso para editar, os usuários também podem editar totalmente o formulário personalizado, incluindo adicionar, editar e excluir campos.</p> <p>Clique em <strong>Configurações avançadas</strong> para especificar se você deseja permitir o seguinte:</p> 
       <ul> 
        <li> <p><strong>Anexar a dados personalizados</strong>: Capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</p> </li> 
        <li><strong>Excluir</strong>: Excluir o formulário personalizado do sistema</li> 
        <li><strong>Compartilhar</strong>: Compartilhar o formulário personalizado com outras pessoas no sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita as Etapas 4-5 para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Se você quiser limitar o acesso ao formulário personalizado (em objetos aos quais ele está anexado) aos especificados nas etapas anteriores, clique no ícone de engrenagem ![](assets/gear-icon-settings-with-dn-arrow.jpg) no canto superior direito da caixa de compartilhamento, clique em **Remova o acesso em todo o sistema**.

   Se mudar de ideia, você pode clicar em **Tornar esse sistema visível** (a opção padrão).

   >[!NOTE]
   >
   >* Quando um formulário personalizado é visível em todo o sistema, é possível que os usuários o vejam e preencham apenas os objetos aos quais estão atribuídos, não para anexá-lo a outros objetos. É possível conceder a capacidade de anexar o formulário personalizado a objetos usando a opção &quot;Anexar a dados personalizados&quot;, descrita na etapa 5.
   >* A maioria das organizações deseja garantir que todos no sistema possam preencher um formulário personalizado quando ele estiver anexado a objetos em que trabalham e exibir seus dados em relatórios. Se isso for verdade para sua organização, recomendamos que você use &quot;**Tornar esse sistema visível**.&quot; Quando a opção é configurada dessa forma, &quot;Sistema visível&quot; é exibido na caixa de diálogo:

   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Se você estiver preocupado com um formulário personalizado em que os usuários possam inserir dados confidenciais quando eles estiverem anexados a determinados objetos, limitando o compartilhamento desses objetos *objetos* pode ser melhor do que limitar o acesso ao próprio formulário.

1. Clique em **Salvar**.

## Remover acesso a um formulário personalizado

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizada**.
1. Selecione o formulário personalizado e clique em **Compartilhar**.
1. Na caixa exibida, clique no X à direita do nome do usuário, da equipe, da função, do grupo ou da empresa que você não deseja mais ter acesso especial ao formulário.
1. (Opcional) Repita a etapa anterior para para outros nomes que deseja remover.
1. Clique em **Salvar**.
