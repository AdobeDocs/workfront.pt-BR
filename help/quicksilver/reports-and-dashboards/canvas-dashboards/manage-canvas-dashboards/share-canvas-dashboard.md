---
product-area: Canvas Dashboards
navigation-topic: manage-canvas-dashboards
title: Compartilhar um painel da tela
description: Você pode compartilhar um painel do Canvas com outros usuários do Adobe Workfront para que eles possam exibi-lo ou editá-lo.
author: Jenny
feature: Reports and Dashboards
exl-id: 5cb03113-35b0-49aa-86ec-ec800cd3f4dc
source-git-commit: d76ad0d51f28191cbd04af950e10a2247414830e
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 0%

---

# Compartilhar um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

Você pode compartilhar um painel do Canvas com outros usuários do Adobe Workfront para que eles possam visualizá-lo ou editá-lo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso. 
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> 
<p>Atual: Plano </p> 
<p>Novo: Padrão</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurações de nível de acesso</p></td> 
   <td><p>Visualizar acesso a relatórios, painéis e calendários</p>
  </td> 
  </tr>  
    </tr>  
        <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Exibir permissões para o painel compartilhar o painel</p>
   <p>Gerenciar permissões para que o painel atribua permissões de painel</p>
  </td> 
  </tr>
</tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Considerações sobre o compartilhamento de painéis

* Os painéis podem ser compartilhados com usuários, equipes, grupos, funções de trabalho ou recursos da empresa.

* Por padrão, o criador de um painel tem Permissões de gerenciamento para o painel.

* Administradores de sistema e usuários com permissão Gerenciar podem conceder acesso a Exibir ou Gerenciar a um painel.

* Os usuários com permissão de Exibição em um painel podem conceder acesso de Exibição a um painel.

* Ao compartilhar um painel, os recursos com os quais ele é compartilhado herdarão permissões para os relatórios exibidos no painel.

* Quando um painel é distribuído por meio de um modelo de layout, uma permissão de Exibição automática para o painel (e seus relatórios) é concedida a todos os recursos atribuídos ao modelo de layout.


## Compartilhar um painel da tela


{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Na página **Painéis da Tela**, selecione o painel que deseja compartilhar.

1. No canto superior direito da página, clique no botão **Compartilhar**. A caixa de diálogo **Compartilhamento de Painel** é exibida.

1. No campo **Conceder acesso a**, comece digitando o nome de um usuário, equipe, função, grupo ou empresa específico com o qual deseja compartilhar o Painel da Tela, em seguida, selecione-o quando ele aparecer na lista suspensa.

1. (Opcional) Para editar o acesso de um recurso ao painel, clique em **Exibir** ao lado do nome e selecione **Gerenciar** na lista suspensa exibida.

   >[!NOTE]
   >
   > Quando os usuários não têm as permissões Editar para um painel atribuído por meio de seu nível de acesso, elas não podem receber as permissões Gerenciar para um painel.

1. Repita as etapas 5 a 6 para cada recurso com o qual deseja compartilhar o painel.

1. Clique no botão **Compartilhar**. Os destinatários recebem uma notificação por email informando que o painel foi compartilhado com eles, que agora eles podem acessar em **Painéis** > **Painéis do Canvas** > **Painéis compartilhados**.

   >[!NOTE]
   >
   > As preferências individuais do usuário e exclusões de sistema para notificações por email podem ser aplicadas. <br>
   > As notificações só são enviadas quando compartilhadas diretamente com um usuário. O compartilhamento para grupos, funções, empresas e equipes não gera notificações por email.<br>
   > As permissões herdadas de um modelo de layout não gerarão uma notificação por email sobre o acesso ao painel.
