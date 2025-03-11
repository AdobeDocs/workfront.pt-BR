---
title: Compartilhar exibições
description: Você pode compartilhar uma visualização com outras pessoas para garantir a colaboração ao usar o Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 673dd888-3135-48b0-8198-c8d6d6706ddf
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '1600'
ht-degree: 1%

---


# Compartilhar exibições

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode compartilhar uma exibição com outras pessoas para garantir a colaboração ao trabalhar com registros no Adobe Workfront Planning.

>[!IMPORTANT]
>
>* Conceder permissões a um espaço de trabalho não concede a outros usuários permissões para as exibições nas páginas do tipo de registro. Você deve conceder permissões a exibições individuais em uma página de tipo de registro para compartilhá-las com outros usuários.
>
>* A concessão de permissões para uma exibição não altera as permissões de exibição dos registros. As permissões de registro são concedidas por espaços de trabalho de compartilhamento.
>
>* Ao compartilhar uma exibição, você concede a outras pessoas permissões para acessar todos os elementos da exibição. Por exemplo, se você conceder a eles permissões Gerenciar para uma exibição, eles poderão modificar a aparência do agrupamento, do filtro, da classificação ou da barra.


Você pode compartilhar uma exibição com as seguintes entidades:

* Internamente, com usuários, grupos, <span class="preview">equipes, empresas e funções de trabalho da Workfront</span>
* Publicamente, com usuários fora do Workfront

<!--
This article describes how you can share a view with others. For information about requesting, granting, or denying permissions to a view, see [Request permissions to a view or a workspace](/help/quicksilver/planning/access/request-permissions.md). -->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

<!--at GA, check that the Workfront plans article linked below has Planning info-->

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Sua organização deve estar integrada à Adobe Unified Experience para que os usuários possam solicitar e conceder permissões para uma exibição a partir de uma solicitação de permissão. </p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  <p>Gerenciar permissões para uma exibição</p>  
   <p>Somente usuários com permissões para Gerenciar um espaço de trabalho podem compartilhar uma visualização publicamente.</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações ao compartilhar visualizações

* Para obter informações gerais sobre o compartilhamento de objetos no Workfront Planning, consulte também [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).
* É possível conceder permissões de Visualização ou Gerenciamento a uma visualização para usuários internos da Workfront.

* Os usuários com permissões para Gerenciar podem modificar, compartilhar, duplicar ou excluir as configurações de exibição.

* Você pode compartilhar visualizações com pessoas de fora da sua organização usando um link público.

* Quando você compartilha uma visualização publicamente, o link é acessível por qualquer pessoa fora da sua empresa por um tempo limitado, indicado pela data de expiração. Não é necessário fazer logon para exibir a exibição compartilhada.

* As pessoas de fora da organização que têm acesso a uma exibição não podem criar outras exibições, editar a exibição compartilhada ou adicionar, excluir ou editar informações de registro na exibição.

## Compartilhar permissões para uma exibição internamente

Você pode compartilhar exibições que criou ou exibições para as quais tem permissões de gerenciamento com usuários, grupos, <span class="preview">equipes, empresas e funções de trabalho</span> no Workfront Planning.

>[!NOTE]
>
>Os administradores do sistema não podem exibir ou compartilhar exibições que não foram criadas por eles mesmos. Eles só podem acessar ou compartilhar exibições compartilhadas com eles.
>
>Os administradores do sistema só podem ter permissões de Gerenciamento para uma exibição.

{{step1-to-planning}}

1. Abra o espaço de trabalho cuja exibição você deseja compartilhar e clique em um cartão de tipo de registro.

   Isso abre a página do tipo de registro.

1. Na guia de exibição, passe o mouse sobre o modo de exibição que você deseja compartilhar e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do modo de exibição e clique em **Compartilhar**.

   ![Mais menus para exibições expandidas com a opção de compartilhamento](assets/more-menu-for-views-expanded-with-share-option.png)

   A guia **Compartilhamento interno** deve ser selecionada por padrão.

1. (Opcional) Na área **Quem tem acesso**, selecione uma das seguintes opções:

   * **Somente pessoas convidadas podem acessar**: você deve especificar usuários, grupos, <span class="preview">equipe, empresa ou função de trabalho</span> com os quais deseja compartilhar a exibição. Esta é a opção padrão.
   * **Todos no espaço de trabalho podem exibir**: todos os usuários que têm permissões de Exibição ou superiores para espaços de trabalho podem acessar a exibição.

1. No campo **Conceder acesso a este modo de exibição**, comece digitando o nome de um usuário, grupo, <span class="preview">equipe, empresa ou função de trabalho</span> e clique nele quando ele for exibido na lista.

   ![Compartilhando um modo de exibição com grupos](assets/sharing-a-view-ui-with-groups.png)

1. Selecione um dos seguintes níveis de permissão no menu suspenso:
   * Exibir
   * Gerenciar

     Para obter informações sobre níveis de permissão e quais ações os usuários podem executar para cada nível, consulte [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

     Os administradores do sistema sempre recebem permissões de Gerenciamento para exibições compartilhadas com eles.

1. Clique em **Copiar link** para copiar um link para o modo de exibição para a área de transferência.
1. Clique em **Salvar**.

   A exibição é atualizada com um ícone de pessoas ![Exibir compartilhado com outros ícones](assets/view-shared-with-others-people-icon.png) para indicar que a exibição agora está compartilhada com outros usuários.

   >[!TIP]
   >
   >Visualizações sem um ícone de pessoas ou global são visualizações que você criou e não são compartilhadas com outras pessoas. As exibições não compartilhadas só estão visíveis para você.

1. Compartilhar o link copiado com outras pessoas. Os usuários que recebem o link devem ser usuários ativos e fazer logon no Workfront para acessar a página de tipo de registro e exibi-la na exibição selecionada.

## Compartilhar permissões para uma exibição pública

É possível compartilhar os modos de exibição criados ou os modos de exibição nos quais você tem permissões de gerenciamento com pessoas que não têm uma licença da Workfront e que podem ser externas à organização.

>[!IMPORTANT]
>
>Somente usuários com permissões para Gerenciar um espaço de trabalho podem compartilhar as exibições do espaço de trabalho publicamente.


Para compartilhar uma exibição publicamente no Workfront Planning:

{{step1-to-planning}}

1. Abra o espaço de trabalho cuja exibição você deseja compartilhar e clique em um cartão de tipo de registro.

   Isso abre a página do tipo de registro.

1. Na guia de exibição, passe o mouse sobre o modo de exibição que você deseja compartilhar e clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do modo de exibição e clique em **Compartilhar**.

   ![Mais menus para exibições expandidas com a opção de compartilhamento](assets/more-menu-for-views-expanded-with-share-option.png)

1. Clique em **Compartilhamento público**.

   ![Guia de compartilhamento público para exibições](assets/public-sharing-tab-for-views.png)

1. Habilitar a configuração **Criar link público**.

   Um link fica disponível. Este é um link público. Quando compartilhados, qualquer pessoa com o link, incluindo pessoas de fora da organização, pode acessar a página de tipo de registro e exibir registros e campos na página.

1. Clique no ícone **Copiar link** ![Copiar exibição de link](assets/copy-link-view.png) para copiar o link para a área de transferência.

1. Insira uma data manualmente ou use o calendário no campo **Data de expiração do link** para selecionar uma data de expiração para o link público. A exibição de página de registro não estará acessível após a data selecionada.

1. Clique em **Salvar**.

   A exibição é atualizada com um ícone global ![Ícone de exibição pública compartilhada](assets/public-shared-view-icon-highlighted.png) para indicar que a exibição é compartilhada publicamente.

   >[!TIP]
   >
   >Visualizações sem um ícone de pessoas ou global são visualizações que você criou e não são compartilhadas com outras pessoas. As exibições não compartilhadas só estão visíveis para você.


1. (Opcional) Cole o link copiado em um email, mensagem de chat, documento ou comentário do Workfront para compartilhá-lo com outras pessoas.

## Conceder permissões para uma exibição a partir de uma solicitação de permissão

Os usuários que acessam um link para uma exibição para a qual não têm permissões podem solicitar permissões para a exibição. Todos os usuários com permissões para Gerenciar a exibição recebem a solicitação de permissão e podem conceder ou negar as permissões.

1. (Condicional) Se você for o gerente de uma view, poderá receber uma solicitação de outro usuário para acessar a view nas seguintes áreas:

   * Uma notificação no aplicativo
     ![Notificação no aplicativo para solicitação de acesso para exibição](assets/in-app-notification-for-access-request-for-view.png)
   * Uma notificação por email
     ![Notificação no aplicativo para solicitação de acesso para exibição](assets/in-app-notification-for-access-request-for-view.png)
1. (Condicional) Na área de notificação do Workfront, clique no link de notificação no aplicativo
Ou
Na notificação por email, clique em **Exibir todas as notificações** e clique na notificação na lista.

   A caixa **Solicitações de acesso pendentes** é exibida.

   ![Caixa de aprovação da lista de notificações](assets/notifications-list-approval-box.png)
1. (Opcional) Para o usuário cujas permissões você deseja aprovar, selecione uma das seguintes opções no menu suspenso à direita do nome do usuário:
   * **Exibir**
   * **Gerenciar**
1. Selecione o usuário para o qual você deseja aprovar ou negar a permissão e clique em **Aprovar tudo** ou **Negar tudo**.
1. Clique na seta à esquerda de **Solicitações de acesso pendentes** e clique em **Salvar**.

   Se você aprovou a solicitação, os usuários são adicionados à caixa de compartilhamento da visualização. O usuário que solicita a permissão recebe uma confirmação por email de que sua solicitação foi aprovada. <!--will they also get an in-app notification??-->

## Remover permissões para uma exibição

{{step1-to-planning}}

1. Abra o espaço de trabalho cuja exibição você deseja interromper o compartilhamento e clique em um cartão de tipo de registro. Isso abre a página do tipo de registro.
1. Passe o cursor do mouse sobre o nome da guia do modo de exibição do qual deseja remover o compartilhamento e clique no menu **Mais** ![Mais menu](assets/more-menu.png), depois clique em **Compartilhar**.
1. Para remover o compartilhamento interno de uma exibição, faça o seguinte:

   1. Verifique se a guia **Compartilhamento interno** está selecionada.
   1. Localize o usuário, grupo, <span class="preview">equipe, empresa ou função de trabalho</span> o que deseja remover, expanda o menu suspenso de permissões à direita do nome da entidade com a qual você está compartilhando o modo de exibição e clique em **Remover**.

1. Para remover o compartilhamento público de uma exibição, faça o seguinte:

   1. Clique na guia **Compartilhamento público**.
   1. Desmarque a opção **Criar link público**.

1. Clique em **Salvar**.

   As pessoas não têm mais acesso à visualização. Não há notificação para os usuários que foram removidos do acesso à visualização de que eles não têm mais esse acesso.
