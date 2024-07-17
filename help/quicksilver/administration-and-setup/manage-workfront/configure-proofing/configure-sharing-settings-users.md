---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Defina as configurações de compartilhamento para seus usuários
description: Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar as contas de usuário com as quais as provas podem ser compartilhadas, se os usuários podem ver todas as versões de uma prova e o tempo em que os usuários obtêm acesso aos itens compartilhados.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Defina as configurações de compartilhamento para seus usuários

Como administrador do Adobe Workfront ou administrador do Workfront Proof, você pode configurar as contas de usuário com as quais as provas podem ser compartilhadas, se os usuários podem ver todas as versões de uma prova e o tempo em que os usuários obtêm acesso aos itens compartilhados.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Premium ou Select</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>É necessário ter Administrador selecionado no seu Perfil de permissão de prova. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurar o acesso à prova de um usuário</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Configurar compartilhamento com outras contas

1. No Workfront, clique no Menu Principal ![](assets/main-menu-icon.png) e, em seguida, clique em Revisão ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. Clique em **Configurações** > **Configurações de conta** e na guia **Configurações**.

1. Na seção **Compartilhamento**, à direita de **Permitir compartilhamento com**, clique em **Configuração**.

1. Na lista suspensa exibida, selecione uma opção para especificar se deseja disponibilizar provas para qualquer pessoa, restringir o compartilhamento das provas somente para sua própria conta ou restringi-la a sua própria conta e a quaisquer contas de parceiros com as quais esteja colaborando.
1. Clique em **Salvar.**

## Configurar a visibilidade de todas as versões de uma prova compartilhada

1. No Workfront, clique no Menu Principal ![](assets/main-menu-icon.png) e, em seguida, clique em Revisão ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. Clique em **Configurações** > **Configurações de conta** e na guia **Configurações**.

1. Na seção **Compartilhamento**, à direita de **Os destinatários podem exibir todas as versões**, selecione **Habilitar** ou **Desabilitar** para indicar se você deseja permitir que os destinatários exibam todas as versões de uma prova no visualizador de provas quando a URL da Prova estiver habilitada.

## Configurar a visibilidade da prova com base na atividade do estágio do fluxo de trabalho

Você pode especificar quando as provas com um fluxo de trabalho automatizado estarão visíveis para os usuários associados a um determinado estágio.

>[!NOTE]
>
>* Essa opção está disponível somente ao usar o aplicativo Workfront Proof independente; não está disponível ao usar uma instância do Workfront Proof integrada ao Workfront ou ao fazer provas no Workfront.
>* Os usuários recebem uma notificação por email sobre a prova somente depois que ela entra no estágio ao qual o usuário está associado, independentemente dessa configuração.
>

Para configurar quando as provas com um fluxo de trabalho automatizado ficam visíveis para os usuários:

1. No Workfront, clique no Menu Principal ![](assets/main-menu-icon.png) e, em seguida, clique em Revisão ![](assets/proofing-in-main-menu.png) para acessar o Workfront Proof.

1. Clique em **Configurações** > **Configurações de conta** e na guia **Configurações**.

1. Na seção **Compartilhamento**, habilite ou desabilite a **Visibilidade de prova com base na ativação de preparo**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desabilitado</strong> (padrão)</td> 
      <td>As provas estão visíveis para os usuários no momento em que a prova é criada.<br><p>Qualquer usuário associado a um estágio no fluxo de trabalho para a prova pode ver a prova nos resultados da pesquisa imediatamente após a criação da prova.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Habilitado</strong> </td> 
      <td> <p>Provas ficam visíveis para usuários somente depois que o estágio ao qual estão associadas se torna <strong>ativo.</strong></p> <p><b>NOTA</b>:   
        <ul> 
         <li><em style="font-style: normal;">Após habilitar esta opção, as provas existentes ainda estarão visíveis para os usuários que poderiam exibi-la quando ela fosse criada.</em> </li> 
         <li>Depois que um usuário obtém acesso a uma versão de uma prova (porque o estágio ao qual o usuário está associado se torna ativo), ele pode ver somente a versão em que o estágio é ativado. Se uma versão anterior nunca atingiu o estágio ao qual o usuário está associado, o usuário não poderá ver essa versão da prova.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
