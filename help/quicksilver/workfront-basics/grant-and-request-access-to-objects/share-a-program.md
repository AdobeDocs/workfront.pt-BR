---
title: Compartilhar um programa
product-area: projects
keywords: compartilhar,programa,permissões
navigation-topic: grant-and-request-access-to-objects
description: O administrador do Adobe Workfront pode conceder acesso para visualizar ou editar programas ao atribuir seu nível de acesso. Você deve ter uma licença de Plano para ter acesso para editar um programa.
author: Courtney
feature: Get Started with Workfront
exl-id: bfa6ce97-24ad-44b3-9c2f-7fac6b748f94
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '892'
ht-degree: 3%

---

# Compartilhar um programa


O administrador do Adobe Workfront pode conceder acesso para visualizar ou editar programas ao atribuir seu nível de acesso. Você deve ter uma licença de Plano para ter acesso para editar um programa. Para obter mais informações, consulte [Conceder acesso aos programas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md).

Além do nível de acesso concedido, você também pode receber permissões para exibir ou gerenciar programas específicos de usuários que podem compartilhá-los com você. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

As permissões são específicas para cada item no Workfront e definem quais ações os usuários podem realizar nesse item.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p> 
   <p>Trabalho ou maior</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir o acesso ou superior aos objetos que você deseja compartilhar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores aos objetos que você deseja compartilhar</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre o compartilhamento de um programa

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

* Por padrão, o criador de um programa tem Permissões de gerenciamento.

* Você pode compartilhar programas individualmente ou vários deles de cada vez.

  Para obter mais informações sobre como compartilhar itens no Workfront, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Você só pode conceder permissões de Exibir ou Gerenciar em programas:

* Quando você compartilha um programa, os usuários herdam as mesmas permissões para todos os objetos secundários associados ao programa, por padrão.

  Para obter mais informações sobre a hierarquia de objetos no Workfront, consulte [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Você pode remover permissões herdadas do programa. Para obter mais informações sobre como remover permissões de objetos, consulte   [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Compartilhar um programa

{{step1-to-programs}}

1. Na página **Programas**, selecione o programa que deseja compartilhar. A página do programa é aberta.

1. À direita do nome do programa, clique em **Compartilhar**. A caixa de diálogo **Compartilhar [Nome do Programa]** é aberta.

   ![Botão Compartilhar programa](assets/share-program-button.png)

1. No campo **Conceder acesso ao programa para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar o programa e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar um programa com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso do programa:

   * **Somente pessoas convidadas podem acessá-lo:** Somente usuários convidados para o programa podem acessá-lo (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir o programa sem um convite.


1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para este programa:

   * **Exibir**: o usuário pode revisar e compartilhar o programa.
   * **Gerenciar**: o usuário tem acesso total ao programa sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no programa.

   ![Opções avançadas de permissão configuradas](assets/advanced-options-icon.png)

1. (Opcional) Para desativar as permissões herdadas para os objetos filho do programa, clique em **Desativar** embutido com **Permissões herdadas**.

1. (Opcional) Para compartilhar o programa rapidamente usando um link, clique em **Copiar link** e encaminhe-o para o destinatário.

1. Clique em **Salvar**.

## Compartilhar programas em massa

{{step1-to-programs}}

1. Na página **Programas**, selecione a caixa à esquerda de cada programa que você deseja compartilhar e clique no ícone **Compartilhar** ![Ícone Compartilhar](assets/share-icon.png) na parte superior da página. O modal de compartilhamento é aberto.

   ![Programas de compartilhamento em massa](assets/bulk-share-programs.png)

1. No campo **Conceder acesso ao programa para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar os programas e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar programas com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso dos programas:

   * **Somente pessoas convidadas podem acessá-las:** Somente usuários convidados para os programas podem acessá-las (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir os programas sem um convite.


1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para os programas:

   * **Exibir**: o usuário pode revisar e compartilhar os programas.
   * **Gerenciar**: o usuário tem acesso total aos programas sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas nos programas.

   ![Opções avançadas de permissão configuradas](assets/advanced-options-icon.png)

1. Clique em **Salvar**.

## Permissões do programa

A tabela a seguir mostra quais permissões você pode conceder aos usuários ao permitir que eles exibam ou gerenciem um programa:

| **Ações** | **Gerenciar** | **Exibir** |
|---|---|---|
| Editar detalhes do programa | ✓ |   |
| Exibir um programa | ✓ | ✓ |
| Excluir um programa | ✓ |   |
| Anexar um formulário personalizado | ✓ |   |
| Editar um campo personalizado | ✓ |   |
| Adicionar ou remover um projeto&#42; | ✓ |   |
| Aprovar um projeto | ✓ |   |
| Adicionar uma pasta de documentos&#42; | ✓ | ✓ |
| Adicionar um documento | ✓ | ✓ |
| Adicionar atualizações/comentários | ✓ | ✓ |
| Compartilhar | ✓ | ✓ |
| Compartilhar em todo o sistema |   | ✓ |

*Essas permissões são controladas pelo nível de acesso e por permissões em outros objetos, como projetos.


