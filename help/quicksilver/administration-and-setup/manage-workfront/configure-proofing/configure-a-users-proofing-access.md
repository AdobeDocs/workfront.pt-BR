---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configurar o acesso à prova de um usuário
description: Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar o acesso de um usuário para criar e exibir provas no Workfront e na Workfront Proof.
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

Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar o acesso de um usuário para criar e exibir provas no Workfront e na Workfront Proof.

Para obter informações sobre a funcionalidade de prova disponível para provas básicas e integradas, consulte [Acesso à funcionalidade de prova no Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront ou do Workfront Proof. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Ativar e desativar a prova para um usuário (somente planos herdados) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Se sua organização estiver usando um Plano Workfront Premium ou Select herdado, como administrador do Workfront, você poderá ativar e desativar a funcionalidade de prova para o usuário.

Ao ativar a prova para um usuário, o Workfront ativa a opção para que as provas do usuário sejam geradas automaticamente.

Embora você possa ativar um usuário como prova, ele deve ter permissões de Administrador para navegar diretamente para a interface do Workfront Proof no Menu principal do Workfront. Para obter informações sobre como habilitar essa opção para todos os usuários de prova em seu sistema Workfront, consulte [Configurar o acesso à prova do Workfront por meio do Menu principal do Workfront para todos os usuários](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. No **Menu principal**, selecione **Usuários**.

1. Selecione um usuário e clique no botão **Editar** ícone .
1. No **Acesso** , selecione ou desmarque **O usuário pode gerar provas**.

## Configurar um perfil de permissão de prova do usuário

O perfil de permissão selecionado é concedido aos usuários para cada prova existente na organização.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).
1. Selecione um ou mais usuários e clique em **Editar**.

1. No **Acesso** clique em uma das seguintes opções de permissão de Prova do Workfront na seção **Perfil de permissão de prova** menu suspenso:

   >[!NOTE]
   >
   >Se você estiver em um plano Workfront herdado, verifique se **O usuário pode gerar provas** está ativada, conforme explicado acima na seção [Ativar e desativar a prova para um usuário (somente planos herdados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Os usuários podem gerenciar e exibir todas as provas criadas na conta de sua organização. Eles também podem editar revisores adicionados a essas provas. Os usuários com esse perfil de permissão não podem gerenciar usuários ou editar configurações do Workfront Proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gerente</strong> </td> 
      <td> <p> Os usuários podem gerenciar e exibir provas criadas ou de propriedade na conta da sua organização. Eles podem exibir as provas de outros usuários somente quando adicionadas como um revisor. Esta é uma configuração padrão. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador</strong> </td> 
      <td> Os usuários recebem permissões de Administrador no Workfront Proof e podem editar configurações da conta. Os usuários podem gerenciar e exibir todas as provas criadas na conta de sua organização. Isso inclui adicionar e remover revisores, provas e comentários.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Predefinido</strong> </td> 
      <td> <p>Disponível somente se você tiver configurado um perfil de permissão personalizado no Workfront Proof.</p> <p><b>Nota</b>:  <p>Certifique-se de que o perfil de permissão que você conceder aqui não forneça acesso maior do que a configuração Nível de acesso do usuário no Workfront (consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>). Se ele fornecer um acesso mais alto, o usuário poderá acessar provas dentro da Workfront de que não poderá acessar no Workfront.</p> <p>Isso é especialmente importante se você planeja permitir que todos os usuários do Workfront acessem o Workfront Proof diretamente da Workfront, conforme descrito em <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Acessar o Workfront Proof do Adobe Workfront</a>.</p> <p>Por padrão, somente os administradores do Workfront têm acesso a um link direto para o site da Workfront Proof na Barra de navegação global do Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   O perfil de permissão selecionado é concedido aos usuários para cada prova existente na organização.

1. Clique em **Salvar alterações** para concluir a atualização das configurações do usuário.

   >[!NOTE]
   >
   >Ao criar ou atualizar um usuário no Workfront e o endereço de email do Workfront do usuário corresponder ao de um usuário licenciado do Workfront Proof, o sistema ativa a verificação para o usuário no Workfront. Para obter mais informações, consulte [Sincronização de usuários entre o Adobe Workfront e a Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Considerações

Considere as seguintes informações ao definir permissões:

* Se você alterar o perfil de permissão de um usuário para um perfil com menos permissões, o usuário poderá perder visibilidade das provas existentes no Workfront. Isso pode ocorrer quando alguém compartilha uma tarefa com um usuário no Workfront, mas não compartilha a prova anexada à tarefa (consulte [Compartilhar uma prova no Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) em [Compartilhar uma prova no Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Você pode definir permissões de Workfront Proof no Workfront somente se o ambiente do Workfront estiver integrado a uma conta do Workfront Proof Premium . Se não puder usar a prova, conforme discutido nesta seção, entre em contato com o administrador do Workfront.
* Pelo menos um usuário em seu ambiente Workfront deve ter permissões de Administrador para prova. Uma mensagem de erro será exibida se você tentar remover permissões de Administrador para verificação de provas de todos os usuários.
* Quando você altera o nível de Acesso ao Workfront de um usuário para qualquer nível diferente de Administrador do sistema, o perfil de permissão do Workfront Proof do usuário assume o padrão de Gerente.

* Quando você altera o nível de Acesso à Workfront para Administrador do sistema, o perfil de Permissão de prova muda para Administrador.

## Configurar o acesso à prova do Workfront por meio do Menu principal do Workfront para todos os usuários {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

Por padrão, somente os usuários com direitos administrativos no Workfront podem acessar o Workfront Proof, conforme descrito  [Acessar o Workfront Proof do Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Você pode conceder acesso a todos os usuários ao botão Prova da Workfront no Menu principal da Workfront, entrando em contato com o Suporte da Workfront e enviando uma solicitação.

>[!IMPORTANT]
>
> Se você planeja permitir que todos os usuários do Workfront acessem a Workfront Proof diretamente da Barra de navegação global do Workfront, verifique se o perfil de permissão para cada usuário não fornece mais acesso do que o nível de acesso do usuário no Workfront. Isso impede que os usuários acessem provas no Workfront Proof que não podem acessar no Workfront. Para obter mais informações, consulte [Ativar e desativar a prova para um usuário (somente planos herdados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configurar o acesso do usuário ao Desktop Proofing Viewer

Se os usuários em sua organização preferirem usar o Desktop Proofing Viewer em vez do Web Proofing Viewer para revisar o conteúdo interativo, você pode configurar o Desktop Proofing Viewer para iniciar automaticamente quando os usuários abrirem provas de conteúdo interativo. Para obter informações sobre isso, consulte o Visualizador de prova de Desktop e como ele difere do Visualizador de prova de web, consulte [Entender o visualizador de prova de desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) e [Diferenças entre o Visualizador de Provas da Web e a visão geral do Visualizador de Provas de Desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. No Workfront, clique no ícone Workfront Proof na Barra de navegação global para acessar a Workfront Proof.

   ![](assets/proof-access-proofhq-350x39.png)

1. Clique em **Configurações da conta** próximo ao canto superior direito da Workfront Proof, clique no botão **Configurações** guia .

1. Em **Padrões de prova** no final do **Visualizador de prova de desktop para prova interativa** , clique em **Configuração**.

1. Modifique as configurações do Desktop Proofing Viewer, conforme descrito em [Visualizador de prova de desktop](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) no artigo [Definir configurações de prova para sua organização](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Clique em **Salvar**.

## Configurar dispositivos personalizados para provas interativas

Você pode adicionar qualquer dispositivo personalizado ao seu sistema, permitindo que os usuários revisem o conteúdo interativo e simulem como o conteúdo aparece em um dispositivo específico quando estão usando o Visualizador de Verificação de Verificação Linguística da Área de Trabalho. (Essa funcionalidade não está disponível no Web Proofing Viewer, onde os usuários podem revisar o conteúdo interativo, mas somente como ele aparece em várias resoluções, não em vários dispositivos.)

Para obter mais informações, consulte [Alterar resolução de prova interativa no visualizador de prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. No Workfront, acesse a interface da Workfront Proof , conforme descrito em [Acessar o Workfront Proof do Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifique as configurações do Desktop Proofing Viewer, conforme descrito em [Configurar dispositivos personalizados para provas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) no artigo [Definir configurações de prova para sua organização](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
