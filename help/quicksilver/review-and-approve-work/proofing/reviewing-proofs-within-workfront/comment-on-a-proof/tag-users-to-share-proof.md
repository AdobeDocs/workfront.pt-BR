---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: Marque usuários para compartilhar uma prova
description: Ao comentar uma prova no visualizador de prova, você pode marcar outros usuários para chamar a atenção para o seu comentário por email e adicioná-los ao fluxo de trabalho da prova.
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# Marque usuários para compartilhar uma prova

Ao comentar uma prova no visualizador de prova, você pode marcar outros usuários para chamar a atenção para o seu comentário por email e adicioná-los ao fluxo de trabalho da prova.

Ao marcar usuários em comentários em uma prova, os usuários que você pode marcar podem ser diferentes dependendo de vários fatores, como permissões de usuário individual e sua associação à organização:

* Se você for o criador, o proprietário ou tiver permissões específicas ativadas, é possível marcar usuários fora do fluxo de trabalho de prova e compartilhar a prova com eles.
* Se você tiver sido adicionado à prova como um usuário externo e for membro de outro ambiente com uma conta de prova diferente, poderá adicionar tags somente a esses usuários do ambiente original. <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## Requisitos de acesso {#access-requirements}

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Função de prova</td> 
   <td>Autor, Moderador</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Supervisor ou Administrador</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Marque usuários para compartilhar uma prova

Usuários com a função Perfil de permissão de prova ou Prova descrita na [Requisitos de acesso](#access-requirements) A seção acima pode marcar os usuários para compartilhar uma prova por padrão. Também é possível marcar usuários para compartilhar uma prova, independentemente da função Perfil de permissão de prova ou de Prova, se você for o proprietário ou criador da prova. Você pode permitir que usuários com funções de Perfil de permissão de prova ou de Prova menores marquem usuários para compartilhar uma prova ao criar uma prova. Para obter mais informações, consulte o [Configurar o fluxo de trabalho e adicionar revisores](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) na seção [Criar uma prova avançada com um workflow básico](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) artigo 10. o

>[!NOTE]
>
>Você pode marcar um colaborador externo usando seu endereço de email somente se um dos itens a seguir for verdadeiro:>
>* Um usuário na conta Workfront de sua organização adicionou o endereço de email do colaborador a uma prova anteriormente.
>* O colaborador usou o endereço de email para assinar uma prova na conta Workfront de sua organização anteriormente.
>


Para marcar alguém e compartilhar uma prova em um comentário:

1. Ao comentar em uma prova, digite um sinal de arroba (@) seguido do nome ou endereço de email da pessoa. Quando você começa a digitar, os nomes disponíveis são exibidos em uma lista suspensa.
1. Selecione o nome da pessoa quando você o vir na lista suspensa.

   >[!TIP]
   >
   >Se quiser fechar a lista suspensa sem selecionar ninguém, pressione a tecla **Esc** ou clique em qualquer lugar fora da lista.

1. Repita as etapas 1 a 2 para qualquer outro usuário que desejar adicionar uma tag ao comentário.
1. Termine o comentário e clique em **Post**.
1. (Condicional) Se você marcou alguém que ainda não foi adicionado à prova, especifique um **Função de prova** e **Alertas por email** configuração para cada usuário listado na caixa exibida, em seguida, clique em **Adicionar pessoas e postar comentários**.

   ![](assets/add-people-to-proof-350x220.png)

   Para obter informações sobre funções de prova, consulte . Para obter informações sobre alertas de email de prova, consulte a seção no artigo [Definir configurações de notificação de email no Workfront Proof](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   Se a prova tiver um Fluxo de trabalho automatizado, os usuários marcados serão adicionados ao palco em que você está. Para obter mais informações, consulte [Visão geral do fluxo de trabalho automatizado](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   Qualquer pessoa que você marcar recebe um email de notificação sobre seu comentário de prova, independentemente das configurações de alerta do email de prova que estiver usando:

   * Se o usuário receber um resumo diário ou um email de resumo por hora, o Workfront envia a notificação separadamente e inclui informações sobre seu comentário de prova no email de resumo.
   * Se o usuário receber alertas para todas as atividades ou para respostas feitas aos comentários, a notificação substituirá as notificações sobre esses comentários e respostas.

Para obter informações sobre outras maneiras de adicionar usuários a uma prova, consulte [Compartilhar uma prova no Adobe Workfront](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
