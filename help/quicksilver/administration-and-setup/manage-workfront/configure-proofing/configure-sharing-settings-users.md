---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Definir configurações de compartilhamento para seus usuários
description: Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar as contas de usuário com as quais as provas podem ser compartilhadas, se os usuários podem ver todas as versões de uma prova e o momento em que os usuários ganham acesso aos itens compartilhados.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Definir configurações de compartilhamento para seus usuários

Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar as contas de usuário com as quais as provas podem ser compartilhadas, se os usuários podem ver todas as versões de uma prova e o momento em que os usuários ganham acesso aos itens compartilhados.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Premium ou Selecionar</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ter o Administrador selecionado em seu Perfil de permissão de prova. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurar o acesso à prova de um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Configurar compartilhamento com outras contas

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. Clique em **Configurações** > **Configurações da conta**, em seguida, clique no botão **Configurações** guia .

1. No **Compartilhamento** à direita de **Permitir compartilhamento com**, clique em **Configuração**.

1. Na lista suspensa que é exibida, selecione uma opção para especificar se deseja disponibilizar provas para qualquer pessoa, restringir o compartilhamento das provas somente em sua própria conta ou restringi-las a sua própria conta e quaisquer contas de parceiros com as quais você está colaborando.
1. Clique em **Salvar.**

## Configurar visibilidade para todas as versões de uma prova compartilhada

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. Clique em **Configurações** > **Configurações da conta**, em seguida, clique no botão **Configurações** guia .

1. No **Compartilhamento** à direita de **Os recipients podem exibir todas as versões**, selecione **Habilitar** ou **Desativar** para indicar se você deseja permitir que os recipients visualizem todas as versões de uma prova no visualizador de prova quando o URL de prova estiver ativado.

## Configurar visibilidade de prova com base na atividade do estágio de fluxo de trabalho

Você pode especificar quando provas com um fluxo de trabalho automatizado ficam visíveis para usuários associados a um determinado estágio.

>[!NOTE]
>
>* Essa opção está disponível somente ao usar o aplicativo Workfront Proof independente; não está disponível ao usar uma instância da Workfront Proof integrada ao Workfront ou ao fazer prova no Workfront.
>* Os usuários recebem uma notificação por email sobre a prova somente depois que ela entra no estágio ao qual o usuário está associado, independentemente dessa configuração.
>


Para configurar quando as provas com um fluxo de trabalho automatizado estiverem visíveis para os usuários:

1. No Workfront, clique no Menu principal ![](assets/main-menu-icon.png)e, em seguida, clique em Verificação ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. Clique em **Configurações** > **Configurações da conta**, em seguida, clique no botão **Configurações** guia .

1. No **Compartilhamento** seção, ativar ou desativar **Prova de visibilidade com base na ativação do estágio**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desabilitado</strong> (padrão)</td> 
      <td>As provas estão visíveis para os usuários no momento em que a prova é criada.<br><p>Qualquer usuário associado a um estágio no fluxo de trabalho da prova pode ver a prova nos resultados da pesquisa imediatamente após a criação da prova.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Ativado</strong> </td> 
      <td> <p>As provas são visíveis para os usuários somente após o estágio ao qual estão associadas se tornar <strong>ativo.</strong></p> <p><b>Nota</b>:   
        <ul> 
         <li><em style="font-style: normal;">Após habilitar essa opção, as provas existentes ainda estarão visíveis para os usuários que poderão visualizá-la quando ela for criada.</em> </li> 
         <li>Depois que um usuário recebe acesso a uma versão de uma prova (porque o estágio ao qual o usuário está associado se torna ativo), ele pode ver somente a versão em que o estágio foi ativado. Se uma versão anterior nunca tiver atingido o estágio ao qual o usuário está associado, ele não poderá ver essa versão da prova.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
