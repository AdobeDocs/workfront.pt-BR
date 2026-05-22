---
content-type: tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-basics
title: Como compartilhar objetos sem gerar notificações
description: Descubra como compartilhar objetos e impedir que notificações sobre essa alteração sejam enviadas. Isso é particularmente útil quando você compartilha objetos em massa.
author: Alina
feature: Get Started with Workfront
exl-id: 02106282-addb-4bdd-82d2-9da5a5f6a687
source-git-commit: 14b3bfaf16a4ab8749538b32100ce6363a3a9335
workflow-type: tm+mt
source-wordcount: '577'
ht-degree: 11%

---

# Como compartilhar objetos sem gerar notificações

<!--Audited: 12/2024-->

Quando você compartilha um objeto no Adobe Workfront, as pessoas com quem você está compartilhando o objeto recebem uma notificação por email sobre o compartilhamento.

Receber uma notificação por email quando alguém compartilhar um objeto com você é importante estar ciente dessa alteração. No entanto, muitas notificações podem ser muito confusas para os usuários. Se você quiser compartilhar um grande número de objetos com usuários de uma só vez, desativar as notificações temporariamente ajudará a evitar a confusão.

As pessoas recebem notificações por email quando as seguintes configurações são ativadas ao mesmo tempo:

* Uma ou ambas as notificações de eventos a seguir estão ativadas no nível do sistema ou do grupo:

   * Objeto - Compartilhar com o Usuário
   * O compartilhamento de objetos com a equipe está habilitado no nível do sistema ou do grupo.
* Uma ou ambas as notificações por email a seguir estão habilitadas no perfil do usuário:

   * Alguém compartilhar um objeto comigo
   * Alguém compartilhar um objeto com minha equipe

Se precisar compartilhar vários objetos com várias pessoas (em massa), mas não quiser que elas recebam notificações por email sobre essa alteração, faça o seguinte:

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Padrão</p>
   <p>Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Exibir o acesso ou superior aos objetos que você deseja compartilhar</p>
   <p>Editar acesso aos usuários</p>
   <p><b>Nota</b></p>
   <p> Você precisa ser um administrador do sistema ou do grupo para verificar o status das Notificações de eventos do sistema ou do grupo</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores aos objetos que você deseja compartilhar</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Compartilhar objetos sem gerar notificações

1. Verifique se as **Notificações de Eventos** a seguir estão habilitadas no nível do sistema ou do grupo:

   * **Compartilhamento de Objetos com o Usuário**
   * **O Compartilhamento de Objetos com a Equipe está habilitado no nível do sistema ou do grupo**.

   Para obter informações, consulte [Configurar notificações de eventos para todos no sistema](/help/quicksilver/administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   Se essas notificações de eventos não estiverem ativadas, as notificações sobre o compartilhamento de um objeto não serão enviadas aos usuários. Se um ou ambos estiverem ativados, continue com as etapas a seguir.

{{step-1-to-users}}

1. Selecione vários usuários na lista e clique em **Notificações** > **Diversos**.
1. Desative uma ou ambas as notificações a seguir (dependendo de quais estiverem ativadas no nível do sistema ou do grupo):

   * **Alguém compartilhar um objeto comigo**
   * **Alguém compartilhar um objeto com minha equipe**

   Certifique-se de que todos os usuários selecionados tenham essas notificações selecionadas antes de desativá-las. Dessa forma, você pode reativá-los em massa para todos eles depois de compartilhar os objetos.

1. Clique em **Salvar alterações**.
1. Vá para uma lista de objetos que você deseja compartilhar, selecione-os e clique no ícone **Compartilhar** na parte superior da lista.

   Para obter informações sobre como compartilhar objetos em massa, consulte [Compartilhar um objeto](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

1. Volte para a lista de usuários para os quais você desativou as notificações e selecione os mesmos usuários.
1. Selecione os mesmos usuários na lista e clique em **Notificações** > **Diversos**.
1. Ative uma ou ambas as notificações a seguir (dependendo de quais estiverem ativadas no nível do sistema ou do grupo):

   * **Alguém compartilhar um objeto comigo**
   * **Alguém compartilhar um objeto com minha equipe**

1. Clique em **Salvar alterações**.

   Os objetos foram compartilhados com os usuários selecionados e nenhum deles recebeu notificações por email sobre essa alteração.
