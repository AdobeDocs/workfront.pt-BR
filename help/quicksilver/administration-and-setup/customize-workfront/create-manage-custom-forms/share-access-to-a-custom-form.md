---
title: Compartilhar um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: É possível configurar o acesso para um formulário personalizado para controlar quem — pessoa, função, grupo, equipe, empresa — pode visualizá-lo, compartilhá-lo e editá-lo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 6c43d836c24f893d1b7d7d01c1dd0b1cc3fba357
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 1%

---

# Compartilhar um formulário personalizado

É possível configurar o acesso para um formulário personalizado para controlar quem — pessoa, função, grupo, equipe, empresa — pode visualizá-lo, compartilhá-lo e editá-lo.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Acesso a formulários personalizados {#access-to-custom-forms}

Por padrão, quando você cria um novo formulário personalizado e alguém o anexa a um objeto, qualquer usuário atribuído ao objeto pode visualizar e preencher o formulário. Isso inclui usuários com licenças de Solicitação e usuários externos.

No entanto, em um objeto em que o formulário personalizado ainda não está anexado, um usuário (mesmo que tenha um nível de acesso de Planejador) não pode anexá-lo pelo menu suspenso Forms personalizado, a menos que uma das seguintes opções seja verdadeira:

* Alguém compartilhou o formulário personalizado com o usuário ou com sua equipe, função de trabalho, grupo ou empresa, concedendo pelo menos a permissão Exibir com a opção Anexar aos dados personalizados selecionada
* O usuário tem uma licença de Plano e seu nível de acesso permite acesso administrativo a formulários personalizados

## Compartilhar um formulário personalizado da lista de formulários

Em vez de deixar um formulário personalizado no estado de compartilhamento padrão (descrito em [Acesso a formulários personalizados](#access-to-custom-forms) neste artigo), você pode configurar níveis específicos de acesso ao formulário para determinados usuários, funções de trabalho, grupos, equipes e empresas.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms personalizado**.
1. Selecione o formulário personalizado e clique em ![Ícone Compartilhar](assets/share-icon.png).
1. Na caixa exibida, em **Conceder acesso ao formulário personalizado a**, comece digitando o nome do usuário, da equipe, da função de trabalho, do grupo ou da empresa com a qual deseja compartilhar o formulário personalizado e pressione **Enter** quando o nome é exibido.
1. Para ajustar o acesso do usuário, equipe, função de trabalho, grupo ou empresa que você acabou de adicionar, clique no menu suspenso à direita do nome e configure uma das seguintes opções disponíveis e qualquer uma de suas configurações avançadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizar o projeto</td> 
      <td> <p>Capacidade de visualizar e preencher o formulário personalizado em objetos.</p> <p><b>NOTA</b>: para usuários com licenças Light e Contributor (ou licenças de Trabalho, Revisão e Solicitação), esta é a opção mais alta disponível.</p> <p>Clique em <strong>Configurações avançadas</strong> para especificar se deseja permitir o seguinte:</p> 
       <ul> 
        <li><strong>Anexar aos dados personalizados</strong>: capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</li> 
        <li> <p><strong>Compartilhar</strong>: capacidade de compartilhar o formulário personalizado com outras pessoas no sistema</p> <p>Os usuários com uma licença Light ou de Colaborador (ou licença de Trabalho, Revisão ou Solicitação) podem compartilhar um formulário personalizado somente por meio da API ou de um relatório de formulários personalizado.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar o projeto</td> 
      <td> <p>Disponível somente para usuários com uma licença Padrão ou de Plano. </p> <p>Além de poder adicionar o formulário aos objetos que eles têm acesso para editar, os usuários também podem editar totalmente o formulário personalizado, incluindo adicionar, editar e excluir campos.</p> <p>Clique em <strong>Configurações avançadas</strong> para especificar se deseja permitir o seguinte:</p> 
       <ul> 
        <li> <p><strong>Anexar aos dados personalizados</strong>: capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</p> </li> 
        <li><strong>Excluir</strong>: exclua o formulário personalizado do sistema</li> 
        <li><strong>Compartilhar</strong>: compartilhe o formulário personalizado com outras pessoas no sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita as etapas 4 a 5 para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Se desejar limitar o acesso ao formulário personalizado (nos objetos aos quais ele está anexado) aos especificados nas etapas anteriores, clique no ícone de engrenagem ![](assets/gear-icon-settings-with-dn-arrow.jpg) no canto superior direito da caixa de compartilhamento e clique em **Remover acesso a todo o sistema**.

   Se mudar de ideia, você pode clicar em **Tornar isto visível em todo o sistema** (a opção padrão).

   >[!NOTE]
   >
   >* Ao tornar um formulário personalizado visível em todo o sistema, você permite que os usuários o vejam e preencham apenas nos objetos aos quais estão atribuídos, e não anexem a outros objetos. Você pode conceder a capacidade de anexar o formulário personalizado a objetos usando a opção &quot;Anexar a dados personalizados&quot; explicada na etapa 5.
   >* A maioria das organizações quer garantir que todos no sistema possam preencher um formulário personalizado quando ele estiver anexado a objetos nos quais trabalham e visualizar seus dados em relatórios. Se isso for verdadeiro para sua organização, recomendamos que você use **Tornar isto visível em todo o sistema**. Quando a opção é configurada dessa maneira, &quot;Visível em todo o sistema&quot; é exibido na caixa de diálogo:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Se você estiver preocupado com um formulário personalizado em que os usuários podem inserir dados confidenciais quando anexado a determinados objetos, limitando o compartilhamento para esses *objetos* pode ser melhor do que limitar o acesso ao próprio formulário.

1. Clique em **Salvar**.

## Compartilhar um formulário personalizado do designer de formulário

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms personalizado**.
1. Abra um formulário personalizado ou crie um novo formulário personalizado.
1. Clique em **Compartilhar** na parte superior direita do designer do formulário quando estiver pronto para compartilhar o formulário.
1. Na caixa exibida, em **Conceder acesso ao formulário personalizado a**, comece digitando o nome do usuário, da equipe, da função de trabalho, do grupo ou da empresa com a qual deseja compartilhar o formulário personalizado e pressione **Enter** quando o nome é exibido.
1. Para ajustar o acesso do usuário, equipe, função de trabalho, grupo ou empresa que você acabou de adicionar, clique no menu suspenso à direita do nome e configure uma das seguintes opções disponíveis e qualquer uma de suas configurações avançadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizar o projeto</td> 
      <td> <p>Capacidade de visualizar e preencher o formulário personalizado em objetos.</p> <p><b>NOTA</b>: para usuários com licenças Light e Contributor (ou licenças de Trabalho, Revisão e Solicitação), esta é a opção mais alta disponível.</p> <p>Clique em <strong>Configurações avançadas</strong> para especificar se deseja permitir o seguinte:</p> 
       <ul> 
        <li><strong>Anexar aos dados personalizados</strong>: capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</li> 
        <li> <p><strong>Compartilhar</strong>: capacidade de compartilhar o formulário personalizado com outras pessoas no sistema</p> <p>Os usuários com uma licença Light ou de Colaborador (ou licença de Trabalho, Revisão ou Solicitação) podem compartilhar um formulário personalizado somente por meio da API ou de um relatório de formulários personalizado.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar o projeto</td> 
      <td> <p>Disponível somente para usuários com uma licença Padrão ou de Plano. </p> <p>Além de poder adicionar o formulário aos objetos que eles têm acesso para editar, os usuários também podem editar totalmente o formulário personalizado, incluindo adicionar, editar e excluir campos.</p> <p>Clique em <strong>Configurações avançadas</strong> para especificar se deseja permitir o seguinte:</p> 
       <ul> 
        <li> <p><strong>Anexar aos dados personalizados</strong>: capacidade de anexar o formulário personalizado a projetos, tarefas e problemas para os quais eles têm acesso de Gerenciamento</p> </li> 
        <li><strong>Excluir</strong>: exclua o formulário personalizado do sistema</li> 
        <li><strong>Compartilhar</strong>: compartilhe o formulário personalizado com outras pessoas no sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita as etapas 5 a 6 para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Se quiser limitar o acesso ao formulário personalizado (nos objetos aos quais ele está anexado) aos especificados nas etapas anteriores, clique na seta suspensa em **Quem tem acesso** e selecione **Somente pessoas convidadas podem acessar**.

   Se mudar de ideia, você pode selecionar **Todos no sistema podem visualizar**.

   >[!NOTE]
   >
   >* Ao tornar um formulário personalizado visível em todo o sistema, você permite que os usuários o vejam e preencham apenas nos objetos aos quais estão atribuídos, e não anexem a outros objetos. Você pode conceder a capacidade de anexar o formulário personalizado a objetos usando a opção &quot;Anexar a dados personalizados&quot; explicada na etapa 6.
   >* A maioria das organizações quer garantir que todos no sistema possam preencher um formulário personalizado quando ele estiver anexado a objetos nos quais trabalham e visualizar seus dados em relatórios. Se isso for verdadeiro para sua organização, recomendamos que você use **Todos no sistema podem visualizar**. Quando a opção é configurada dessa maneira, &quot;Visível em todo o sistema&quot; é exibido na caixa de diálogo:
   >   
   >![Compartilhar formulário personalizado](assets/share-custom-form-in-designer.png)
   >   
   >Se você estiver preocupado com um formulário personalizado em que os usuários podem inserir dados confidenciais quando anexado a determinados objetos, limitando o compartilhamento para esses *objetos* pode ser melhor do que limitar o acesso ao próprio formulário.

1. Clique em **Salvar**.

## Remover acesso a um formulário personalizado da lista de formulários

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms personalizado**.
1. Selecione o formulário personalizado e clique em ![Ícone Compartilhar](assets/share-icon.png).
1. Na caixa exibida, clique no X à direita do nome do usuário, da equipe, da função, do grupo ou da empresa a quem você não deseja mais ter acesso especial ao formulário.
1. (Opcional) Repita a etapa anterior para para outros nomes que você deseja remover.
1. Clique em **Salvar**.
