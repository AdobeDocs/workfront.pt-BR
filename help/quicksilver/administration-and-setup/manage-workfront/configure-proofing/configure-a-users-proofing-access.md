---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configurar o acesso à prova de um usuário
description: Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar o acesso de um usuário para criar e exibir provas no Workfront e no Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# Configurar o acesso à prova de um usuário

Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar o acesso de um usuário para criar e exibir provas no Workfront e no Workfront Proof.

Para obter informações sobre a funcionalidade de revisão de texto disponível para revisões básicas e integradas, consulte [Acesso à funcionalidade de revisão de texto no Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront ou do Workfront Proof. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Habilitar e desabilitar revisões para um usuário (somente planos herdados) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Se sua organização estiver usando um Select ou Premium Workfront Plan herdado, como administrador do Workfront, você poderá ativar e desativar a funcionalidade de comprovação para o usuário.

Quando você ativa a prova para um usuário, o Workfront ativa a opção para que as provas do usuário sejam geradas automaticamente.

Embora seja possível habilitar um usuário como usuário de comprovação, ele deve ter permissões de Administrador para navegar diretamente para a interface do Workfront Proof no Menu principal do Workfront. Para obter informações sobre como você pode habilitar esta opção para todos os usuários de revisão no sistema Workfront, consulte [Configurar o acesso ao Workfront Proof por meio do Menu Principal do Workfront para todos os usuários](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. No **Menu principal**, selecione **Usuários**.

1. Selecione um usuário e clique no ícone **Editar**.
1. Na seção **Acesso**, marque ou desmarque **O usuário pode gerar provas**.

## Configurar o perfil de permissão de prova de um usuário

O perfil de permissão selecionado é concedido aos usuários para cada prova existente em sua organização.

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito do Adobe Workfront e clique em **Usuários** ![](assets/users-icon-in-main-menu.png).
1. Selecione um ou mais usuários e clique em **Editar**.

1. Na seção **Access**, clique em uma das seguintes opções de permissão de Workfront Proof no menu suspenso **Perfil de Permissão de Prova**:

   >[!NOTE]
   >
   >Se você estiver em um plano herdado do Workfront, verifique se a opção **O usuário pode gerar provas** está habilitada, conforme explicado acima na seção [Habilitar e desabilitar provas para um usuário (somente planos herdados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Os usuários podem gerenciar e visualizar todas as provas criadas na conta da sua organização. Eles também podem editar revisores adicionados a essas provas. Os usuários com este perfil de permissão não podem gerenciar usuários nem editar configurações do Workfront Proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gerente</strong> </td> 
      <td> <p> Os usuários podem gerenciar e visualizar provas criadas ou próprias na conta da sua organização. Eles podem exibir as provas de outros usuários somente quando adicionados como revisores. Esta é uma configuração padrão. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador</strong> </td> 
      <td> Os usuários recebem permissões de Administrador no Workfront Proof e podem editar configurações da conta. Os usuários podem gerenciar e visualizar todas as provas criadas na conta da sua organização. Isso inclui adicionar e remover revisores, provas e comentários.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personalizado</strong> </td> 
      <td> <p>Disponível somente se você tiver configurado um perfil de permissão personalizado no Workfront Proof.</p> <p><b>NOTA</b>:  <p>Certifique-se de que o perfil de permissão concedido aqui não forneça acesso superior à configuração Nível de Acesso do usuário no Workfront (consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>). Se ele fornecer maior acesso, o usuário poderá acessar provas no Workfront Proof que não poderá acessar no Workfront.</p> <p>Isso é especialmente importante se você planeja permitir que todos os usuários do Workfront acessem o Workfront Proof diretamente da Workfront, conforme descrito em <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Acessar o Workfront Proof pela Adobe Workfront</a>.</p> <p>Por padrão, somente os administradores do Workfront têm acesso a um link direto para o site do Workfront Proof na Barra de navegação global da Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   O perfil de permissão selecionado é concedido aos usuários para cada prova existente em sua organização.

1. Clique em **Salvar alterações** para concluir a atualização das configurações do usuário.

   >[!NOTE]
   >
   >Quando você cria ou atualiza um usuário no Workfront e o endereço de email do Workfront do usuário corresponde ao de um usuário licenciado do Workfront Proof, o sistema ativa a prova para o usuário no Workfront. Para obter mais informações, consulte [Sincronização de usuário entre o Adobe Workfront e o Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerações

Considere as seguintes informações ao definir permissões:

* Se você alterar o perfil de permissão de um usuário para um perfil com menos permissões, o usuário poderá perder a visibilidade das provas existentes no Workfront. Isso pode ocorrer quando alguém compartilha uma tarefa com um usuário no Workfront, mas não compartilha a prova anexada à tarefa (consulte [Compartilhar uma prova no Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) em [Compartilhar uma prova no Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Você pode definir permissões do Workfront Proof no Workfront somente se o ambiente do Workfront estiver integrado a uma conta do Workfront Proof Premium. Se não conseguir usar provas como discutido nesta seção, entre em contato com o administrador do Workfront.
* Pelo menos um usuário no seu ambiente do Workfront deve ter permissões de Administrador para revisões. Uma mensagem de erro será exibida se você tentar remover permissões de Administrador para revisão de todos os usuários.
* Quando você altera o nível de Acesso ao Workfront de um usuário para qualquer nível que não seja o de Administrador do Sistema, o perfil de permissão Workfront Proof do usuário é padronizado como Gerente.

* Quando você altera o nível de acesso do Workfront para Administrador do sistema, o perfil Permissão de prova muda para Administrador.

## Configuração do acesso ao Workfront Proof pelo menu principal do Workfront para todos os usuários {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Por padrão, somente usuários com direitos administrativos no Workfront podem acessar o Workfront Proof conforme descrito [Acessar o Workfront Proof pelo Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Você pode conceder a todos os usuários acesso ao botão Workfront Proof no Menu principal do Workfront, entrando em contato com o Suporte da Workfront e enviando uma solicitação.

>[!IMPORTANT]
>
> Se você planeja permitir que todos os usuários do Workfront acessem o Workfront Proof diretamente da Barra de navegação global da Workfront, verifique se o perfil de permissão para cada usuário não fornece mais acesso do que o nível de acesso do usuário no Workfront. Isso impede que os usuários acessem provas no Workfront Proof que não podem acessar no Workfront. Para obter mais informações, consulte [Habilitar e desabilitar revisões para um usuário (somente planos herdados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configurar o acesso do usuário ao Desktop Proofing Viewer

Se os usuários em sua organização preferirem usar o Visualizador de provas de desktop em vez do Visualizador de provas de web para revisar o conteúdo interativo, você poderá configurar o Visualizador de provas de desktop para ser iniciado automaticamente quando os usuários abrirem provas de conteúdo interativo. Para obter informações sobre este o Desktop Proofing Viewer e como ele difere do Web Proofing Viewer, consulte [Entender o Desktop Proofing Viewer](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) e [Diferenças entre o Web Proofing Viewer e a visão geral do Desktop Proofing Viewer](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. No Workfront, clique no ícone Workfront Proof na Barra de navegação global para acessar o Workfront Proof.

   ![](assets/proof-access-proofhq-350x39.png)

1. Clique em **Configurações da conta** próximo ao canto superior direito do Workfront Proof e clique na guia **Configurações**.

1. Em **Padrões de Prova**, no final da linha **Visualizador de Provas de Área de Trabalho para Prova Interativa**, clique em **Configurar**.

1. Modifique as configurações do Desktop Proofing Viewer, conforme descrito no [Desktop Proofing Viewer](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) do artigo [Definir configurações de prova para sua organização](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Clique em **Salvar**.

## Configurar dispositivos personalizados para provas interativas

Você pode adicionar qualquer dispositivo personalizado ao seu sistema, permitindo que os usuários revisem o conteúdo interativo e simulem como o conteúdo aparece em um dispositivo específico quando estão usando o Visualizador de provas de desktop. (Essa funcionalidade não está disponível no Visualizador de provas da Web, onde os usuários podem revisar o conteúdo interativo, mas somente como ele aparece em várias resoluções, não em vários dispositivos.)

Para obter mais informações, consulte [Alterar resolução de prova interativa no visualizador de provas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. No Workfront, acesse a interface do Workfront Proof, conforme descrito em [Acessar o Workfront Proof do Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifique as configurações do Desktop Proofing Viewer, conforme descrito em [Configurar dispositivos personalizados para provas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) no artigo [Definir configurações de prova para sua organização](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
