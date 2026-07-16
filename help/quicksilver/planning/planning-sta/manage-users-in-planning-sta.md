---
title: Gerenciar Usuários no Adobe Workfront Planning como um produto independente
description: Este artigo descreve como é possível gerenciar usuários e equipes no Adobe Workfront Planning quando o Planning é adquirido como um produto independente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
source-git-commit: b186900d58f6a422c787cef881a4d06d6cd7feed
workflow-type: tm+mt
source-wordcount: '835'
ht-degree: 1%

---


# Gerenciar usuários no Adobe Workfront Planning como um produto independente

>[!IMPORTANT]
>
>As informações neste artigo se referem ao Adobe Workfront Planning, quando adquirido como um produto independente. Consulte este artigo quando sua empresa comprou um pacote somente do Adobe Workfront Planning e não comprou um pacote do Workfront Workflow.
>
>Para obter informações sobre o Adobe Workfront Planning quando adquirido junto com um pacote do Workfront, consulte [Introdução ao Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).
>

É possível gerenciar usuários no Adobe Workfront Planning como um produto independente de uma maneira semelhante à que você gerencia no Adobe Workfront.

Existem algumas limitações nos níveis de acesso que você pode atribuir aos usuários no Workfront Planning.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront Planning como um pacote independente</p>

</td> </tr>
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Administrador de planejamento</p>
   </td> 
  </tr>

</tbody> 
</table>

Para obter mais informações sobre o acesso necessário ao Workfront como um pacote independente, consulte [Acesso necessário ao Adobe Workfront Planning como um produto independente](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).
+++    

## Níveis de acesso no Adobe Workfront Planning

Você pode atribuir os seguintes níveis de acesso aos usuários no Workfront Planning quando eles forem comprados como um produto independente:

* Administrador de planejamento
* Planejamento padrão

Para obter mais informações sobre os recursos incluídos em cada acesso, consulte [Acesso necessário ao Adobe Workfront Planning como um produto independente](/help/quicksilver/planning/planning-sta/access-needed-for-planning-sta.md).

Considere o seguinte ao trabalhar com níveis de acesso no Workfront Planning como um produto independente:

* Não é possível criar ou modificar níveis de acesso no Workfront Planning. Eles são pré-configurados.

* Depois de adicionar um usuário ao Adobe Admin Console como Administrador do produto Workfront, ele é automaticamente atribuído a esse nível de acesso no Workfront Planning e seu nível de acesso não pode ser editado no Planning.
* Você só pode atribuir um nível de acesso do Planning Standard a usuários no Planning depois de adicionar os usuários ao Admin Console. Esse é o único nível de acesso que você pode atribuir manualmente a um usuário.

## Gerenciar usuários no Workfront Planning como um produto independente

1. Como Administrador do Planning, execute uma das seguintes ações:

   * Se você for um novo cliente do Workfront Planning, receberá um email da Adobe Workfront alertando que agora tem uma conta na Adobe Workfront. Use o link no email para fazer logon na Admin Console.

   * Se você já for um Administrador do Workfront Planning e quiser adicionar outras pessoas à sua conta, faça logon no Admin Console.

   Para obter informações, consulte [Gerenciar usuários na Adobe Admin Console](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/admin-console.md).

1. No Admin Console, comece a adicionar usuários em uma das seguintes guias:

   * **Administradores**: os usuários são criados automaticamente como um usuário Administrador do Planning no Planning.
   * **Usuários**: você deve atribuir um Nível de Acesso no Workfront Planning.

1. (Condicional) Faça logon no Workfront a partir da página inicial do Adobe CX Enterprise.

   O Workfront Planning é aberto.
1. Clique em **Menu Principal** > **Usuários** > **Novo Usuário**.

   ![Caixa Novo Usuário no Planning independente](assets/new-user-box-planning-sta.png)

1. Na caixa **Novo usuário**, atualize as seguintes informações:

   * **Nome(s)**: mesmo nome que você adicionou à Admin Console.
   * **Sobrenome**: o mesmo nome que você adicionou à Admin Console.
   * **Endereço de email (nome de usuário)**: Mesmo email que você adicionou à Admin Console.
   * **O usuário está ativo**: para indicar que o usuário está ativo e pode fazer logon no Workfront Planning e pode ser atribuído a registros, ative a configuração.
   * **Nível de acesso**: selecione Planning Standard para um usuário não administrador. É a única opção.

     >[!TIP]
     >
     >Adicionar um usuário que já foi configurado como Administrador no Admin Console adiciona automaticamente o nível de acesso Administrador do Planning ao usuário. Não é possível editar.

   * **Equipes**: no menu suspenso, selecione equipes para associar ao usuário. As equipes devem ser criadas antes de você poder atribuí-las aos usuários.

     Para obter informações, consulte [Gerenciar equipes](/help/quicksilver/planning/planning-sta/manage-teams-in-planning-sta.md).

1. Clique em **Carregar agora** para adicionar uma imagem de perfil e em **Salvar**.

1. Clique em **Salvar** ou **Adicionar pessoa e iniciar outra** para salvar o usuário e adicionar outra pessoa.

   Os usuários são adicionados e receberão um email para fazer logon no Workfront Planning.
1. (Opcional) Para editar um usuário existente, siga um destes procedimentos:

   * Passe o mouse sobre o nome do usuário na lista, em seguida, clique no menu **Mais** ![Mais menus](assets/more-menu.png) > **Editar Usuário**
   * Selecione o usuário na lista e clique em **Editar usuário** na barra de ferramentas azul na parte inferior da página.
1. (Opcional) Para excluir um usuário, siga um destes procedimentos:

   * Passe o mouse sobre o nome do usuário na lista, em seguida, clique no menu **Mais** ![Mais menus](assets/more-menu.png) > **Excluir usuário**
   * Selecione a equipe na lista e clique em **Excluir usuário** na barra de ferramentas azul na parte inferior da página
1. Clique em **Excluir** para confirmar.
1. (Opcional) Para desativar um usuário, siga um destes procedimentos:

   * Passe o mouse sobre o nome do usuário na lista, em seguida, clique no menu **Mais** ![Mais menus](assets/more-menu.png) > **Desativar**
   * Selecione a equipe na lista e clique em **Desativar** na barra de ferramentas azul na parte inferior da página
1. Clique em **Desativar** para confirmar.

   Para manter registros históricos do seu trabalho, recomendamos desativar os usuários, em vez de excluí-los.



