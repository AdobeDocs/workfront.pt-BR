---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Gerencie as licenças disponíveis em seu sistema
description: Como administrador da Adobe Workfront, você pode acessar informações sobre sua conta da Workfront, incluindo o número de licenças compradas para sua organização, bem como o número dessas licenças em uso no momento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 5ec772260c965b83824ff307bc84755fe06e1ba0
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 0%

---

# Gerencie as licenças disponíveis em seu sistema

Como administrador da Adobe Workfront, você pode acessar informações sobre sua conta da Workfront, incluindo o número de licenças compradas para sua organização, bem como o número dessas licenças em uso no momento.

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
   <td> <p>Você deve ser um administrador do Workfront. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Exibir as licenças de sua organização

O número de licenças usadas em uso é atualizado automaticamente à medida que você atribui níveis de acesso aos usuários adicionados ao Workfront. Para obter mais informações, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para exibir informações de licença no seu sistema:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Na parte inferior do painel esquerdo, clique em **Sistema** > **Licenças**.

   Para obter mais informações sobre as licenças listadas nesta página, consulte [Visão geral das licenças do Adobe Workfront](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Licenças de prova estão disponíveis somente para clientes que compraram o complemento Workfront Proof pago além da licença Workfront. Para obter informações sobre este complemento, consulte [Workfront Proof](../../workfront-proof/workfront-proof.md).

1. (Condicional) Se você vir a mensagem **Para definir um máximo, você deve adicionar um Grupo Doméstico**, adicione um grupo doméstico ao seu sistema, conforme explicado na seção [Adicionar ou remover um grupo doméstico da página Licenças](#add-or-remove-a-home-group-to-the-licenses-page) neste artigo.

## Exibição de informações sobre licenças para complementos do Workfront

Na imagem abaixo, **5 de 10 certificados de prova** indica que essa organização tem o complemento pago Workfront Proof e está usando atualmente 5 das 10 licenças Workfront Proof adquiridas.

![](assets/updated-licenses-page.png)

Se sua organização adquiriu o Workfront Metas, as informações de licença desse produto também serão exibidas aqui. Nesse caso, você pode exibir as seguintes informações:

* O número total de licenças do Workfront Metas que sua empresa comprou
* O número de licenças do Workfront Metas associadas aos usuários. Esse é o número de usuários aos quais deve ter concedido pelo menos o acesso de Exibição às Metas em seus níveis de acesso.

Para obter informações sobre as Metas da Workfront, consulte [Visão geral das Metas da Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Para obter informações sobre o acesso às Metas da Workfront, consulte [Conceder acesso às Metas da Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)

>[!NOTE]
>
>O Workfront permite atribuir mais licenças do Workfront Metas que você comprou. No entanto, quando você atribui mais licenças do que o permitido pelo seu contrato do Workfront Metas, um gerente de conta da Workfront entrará em contato com você para saber que você excedeu seu número contratual.

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Os usuários sem acesso administrativo podem usar um relatório de Grupo para visualizar a contagem de licenças. Na guia Relatório , crie um novo relatório de grupo e adicione as seguintes colunas:>
>* Limite do tipo de licença: Limite do trabalhador
>* Limite do tipo de licença: Limite do Planejador
>
>Para saber mais sobre como criar um relatório, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Adicionar ou remover um grupo doméstico da página Licenças {#add-or-remove-a-home-group-to-the-licenses-page}

É necessário um Plano Workfront de Negócios ou de Empresas para usar esse recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos da Workfront.](https://www.workfront.com/plans)

Cada usuário pode ser atribuído a apenas um Grupo Doméstico. A Workfront fornece uma contagem de licenças orientada a grupos, calculando quantas licenças são alocadas e usadas atualmente em cada Grupo Doméstico.

Caso veja a mensagem **Para definir um máximo, você deve adicionar um Grupo Doméstico** na página Licenças, é necessário adicionar pelo menos um Grupo Doméstico à página Licenças.

>[!IMPORTANT]
>
>* Para gerenciar licenças com eficácia com grupos domésticos, recomendamos configurar grupos domésticos específicos para unidades de negócios antes de atualizar a contagem máxima de licenças. Para obter mais informações, consulte [Visão geral dos grupos domésticos](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Você pode adicionar somente grupos de nível superior como Grupos iniciais, não subgrupos. Se um usuário tiver um subgrupo atribuído como Grupo doméstico, sua licença será adicionada à contagem de licenças do grupo de nível superior acima desse subgrupo.
>


Para adicionar ou remover um Grupo Doméstico à página Licenças:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Na parte inferior do painel esquerdo, clique em **Sistema** > **Licenças**.

1. Clique em **Gerenciar lista de grupos**.
1. Comece a digitar o nome do grupo de nível superior no **Grupos Iniciais** caixa.
1. Para adicionar o grupo, clique em seu nome quando ele for exibido.

   Ou

   Para remover o grupo, clique no ícone X à direita do nome.

1. Clique em **Salvar**.

Como administrador do Workfront, você pode definir contagens máximas de licença para os Grupos Domésticos para impedir que uma unidade comercial use licenças Workfront compradas para outras unidades comerciais. Para obter instruções, consulte [Definir a contagem máxima de licenças para um Grupo Doméstico](#set-the-maximum-license-count-for-a-home-group) neste artigo.

## Definir a contagem máxima de licenças para um Grupo Doméstico {#set-the-maximum-license-count-for-a-home-group}

Como administrador do Workfront, você pode definir contagens máximas de licença para os Grupos Domésticos de nível superior em seu sistema. Isso permite impedir que uma unidade comercial use licenças da Workfront adquiridas para outras unidades comerciais em sua organização.

Por padrão, a contagem máxima de licenças é definida como N/A, o que significa que não há limite.

Os administradores de grupo podem visualizar o número de licenças alocadas e usadas em um Grupo doméstico gerenciado por eles. Para obter mais informações, consulte [Exibir o número de licenças alocadas e usadas em um grupo na nova experiência do Adobe Workfront](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Para definir a contagem máxima de licenças para um Grupo Doméstico:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Na parte inferior do painel esquerdo, clique em **Sistema** > **Licenças**.

1. Localize o Grupo inicial na lista.
1. No **Max** do grupo, clique no valor para o qual deseja definir um máximo.
1. Digite o número máximo e pressione Enter.

   ![](assets/updated-max.png)

   >[!NOTE]
   >
   >Para definir o valor máximo de licença de um grupo de volta ao padrão, não digite 0. Em vez disso, exclua o número na caixa . Definir o valor máximo de licença como 0 indica que não há licenças alocadas para esse grupo.
