---
title: Compartilhar um portfólio
description: Você pode compartilhar um portfólio com outros usuários se tiver permissões para acessá-lo.
author: Courtney
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: 883ec4eaa2258de2e464acf14b6b4083db05b99a
workflow-type: tm+mt
source-wordcount: '870'
ht-degree: 0%

---

# Compartilhar um portfólio

O administrador do Adobe Workfront pode conceder acesso para visualizar ou editar portfólios ao atribuir seu nível de acesso. Você deve ter uma licença de Plano para ter acesso para editar um portfólio. Para obter mais informações, consulte [Conceder acesso aos portfólios](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md).

Além do nível de acesso concedido, você também pode receber permissões para exibir ou gerenciar portfólios específicos de usuários que podem compartilhá-los com você. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

As permissões são específicas a um item no Workfront e definem quais ações os usuários podem realizar nesse item.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

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
   <td> <p>Standard</p> 
   <p>Trabalhar ou superior</p> 
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

## Considerações sobre o compartilhamento de portfólios

Além das considerações abaixo, consulte também [Visão geral das permissões de compartilhamento em objetos](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

* Por padrão, o criador de um portfólio tem Permissões de gerenciamento.
* Você pode compartilhar um portfólio individualmente ou vários portfólios ao mesmo tempo. O compartilhamento de um portfólio é idêntico ao compartilhamento de outros objetos no Workfront. Para obter informações, consulte [Compartilhar um objeto](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* Você só pode conceder permissões de Visualização ou Gerenciamento em Portfólios.
</span>
* Quando você compartilha um portfólio, os usuários herdam as mesmas permissões para todos os objetos secundários associados ao portfólio por padrão.

Para obter mais informações sobre a hierarquia de objetos no Workfront, consulte [Entender objetos no Adobe Workfront](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* Você pode remover permissões herdadas do Portfolio. Para obter mais informações sobre como remover permissões de objetos, consulte [Remover permissões de objetos](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## Compartilhar um portfólio

{{step1-to-portfolios}}

1. Na página **Portfólios**, selecione o portfólio que deseja compartilhar. A página do portfólio é aberta.

1. À direita do nome do portfólio, clique em **Compartilhar**. A caixa de diálogo **Compartilhar [Nome do Portfolio]** é aberta.

   ![Botão Compartilhar portfólio](assets/share-portfolio-button.png)

1. No campo **Conceder acesso ao portfólio para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar o portfólio e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar um portfólio com usuários, equipes, funções ou empresas ativos.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso do portfólio:

   * **Somente pessoas convidadas podem acessá-lo:** Somente usuários convidados para o portfólio podem acessá-lo (Padrão).
   * **Todos no sistema podem visualizar**: todos os usuários no sistema podem visualizar o portfólio sem um convite.

1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para este portfólio:

   * **Exibir**: o usuário pode revisar e compartilhar o portfólio.
   * **Gerenciar**: o usuário tem acesso total ao portfólio sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de exibição).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas no portfólio.

   ![Opções avançadas de permissão configuradas](assets/advanced-options-icon.png)

1. (Opcional) Para compartilhar rapidamente o portfólio usando um link, clique em **Copiar link** e encaminhe-o para o destinatário.

1. Clique em **Salvar**.

## Compartilhar portfólios em massa

{{step1-to-portfolios}}

1. Na página **Portfólios**, marque a caixa à esquerda de cada portfólio que você deseja compartilhar e clique no ícone **Compartilhar** ![Ícone Compartilhar](assets/share-icon.png) na parte superior da página. O modal de compartilhamento é aberto.

   ![Portfólios de compartilhamento em massa](assets/bulk-share-portfolios.png)

1. No campo **Conceder acesso ao portfólio para**, comece digitando o nome do usuário, da equipe, da função, do grupo ou da empresa com a qual deseja compartilhar os portfólios e clique no nome quando ele aparecer na lista suspensa.

   >[!TIP]
   >
   >Você só pode compartilhar portfólios com usuários, equipes, funções ou empresas ativas.


1. (Opcional) Selecione o menu suspenso **Quem tem acesso** e selecione o nível de acesso dos portfólios:

   * **Somente pessoas convidadas podem acessá-las:** Somente usuários convidados para os portfólios podem acessá-las (Padrão).
   * **Todos no sistema podem exibir**: todos os usuários do sistema podem exibir os portfólios sem um convite.


1. Clique na lista suspensa à direita do nome do usuário e selecione o nível de permissão para os portfólios:

   * **Exibir**: o usuário pode revisar e compartilhar os portfólios.
   * **Gerenciar**: o usuário tem acesso total aos portfólios sem direitos administrativos, que são concedidos no nível de acesso (também inclui todas as permissões de Exibição).

1. (Opcional) Clique no ícone de opções avançadas ao lado do nível de permissão que você concedeu para configurar permissões específicas nos portfólios.

   ![Opções avançadas de permissão configuradas](assets/advanced-options-icon.png)

1. Clique em **Salvar**.


## Permissões do Portfolio

A tabela a seguir mostra quais permissões você pode conceder aos usuários ao permitir que eles visualizem ou gerenciem uma Portfolio:

| **Ações** | **Gerenciar** | **Exibir** |
|---|---|---|
| Editar detalhes do Portfolio | ✓ |   |
| Exibir uma Portfolio | ✓ | ✓ |
| Excluir uma Portfolio | ✓ |   |
| Anexar um formulário personalizado | ✓ |   |
| Editar um campo personalizado | ✓ |   |
| Adicionar ou remover um programa&#42; | ✓ |   |
| Adicionar ou remover um projeto&#42; | ✓ |   |
| Aprovar um projeto | ✓ |   |
| Otimização do Portfolio&#42; | ✓ |   |
| Adicionar uma pasta de documentos&#42; | ✓ | ✓ |
| Adicionar um documento | ✓ | ✓ |
| Atualizações/comentários | ✓ | ✓ |
| Compartilhar | ✓ | ✓ |
| Compartilhar em todo o sistema |   | ✓ |

*Essas permissões são controladas pelo nível de acesso e permissões em outros objetos, como projetos, programas e documentos.
