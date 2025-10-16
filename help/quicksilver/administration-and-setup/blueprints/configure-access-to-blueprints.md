---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: Configurar acesso a blueprints
description: Como administrador do sistema, você pode habilitar o acesso para que os usuários solicitem a instalação de blueprints configurando uma fila de solicitações para armazenar as solicitações. Você tem um único local para rastrear e atualizar solicitações.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: 5fd855bec596926a4361fd07a1a763c7956e5e61
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Configurar acesso a blueprints

Todos os usuários [!DNL Adobe Workfront] podem navegar pelo catálogo de blueprints.

Como administrador do sistema, você pode:

* Adicione [!UICONTROL Blueprints] ao menu principal nos modelos de layout e atribua o modelo de layout aos usuários ou grupos. Para obter mais informações, consulte [Personalizar o [!UICONTROL Menu Principal] usando um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) e [Atribuir usuários a um modelo de layout](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

  >[!NOTE]
  >
  >* Os usuários que não tiverem um modelo de layout atribuído a eles verão o ícone [!UICONTROL Blueprints] no [!UICONTROL Menu Principal].
  >* Ao criar um novo modelo de layout, o ícone [!UICONTROL Blueprints] é incluído na lista [!UICONTROL Itens Ativos] do [!UICONTROL Menu Principal] por padrão.


* Habilite o acesso para que os usuários solicitem a instalação de blueprints configurando uma fila de solicitações para armazenar as solicitações. Você tem um único local para rastrear e atualizar solicitações. Para obter mais informações, siga o procedimento abaixo.
* Instalar blueprints. Para obter informações, consulte [Instalar um blueprint](../../administration-and-setup/blueprints/blueprints-install.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>administrador do Workfront </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos {#prerequisites}

* Você deve usar uma fila de solicitações existente para armazenar solicitações de blueprint. O projeto deve ser salvo como uma fila de solicitações e deve estar no status [!UICONTROL Atual].
* A fila de solicitações deve ser pública. Nos detalhes da fila de solicitações, &quot;[!UICONTROL Quem pode adicionar solicitações a esta fila?] deve ser definido como **[!UICONTROL Qualquer]**.

>[!TIP]
>
>Se quiser criar uma nova fila de solicitações para solicitações de blueprint, você deve criá-la antes de configurar o acesso a blueprints. Para obter informações sobre como criar uma fila de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Selecione a fila de solicitações para armazenar solicitações de blueprint

Antes que os usuários possam solicitar que você instale blueprints para eles, você deve selecionar uma fila de solicitações para essas solicitações. Até que a fila de solicitações seja definida, os usuários só poderão navegar pelo catálogo de blueprints.

{{step1-to-blueprints}}

1. Clique em **[!UICONTROL Configurar solicitações de blueprint]** na parte superior direita da tela do catálogo.

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. Na caixa de diálogo **[!UICONTROL Configurar blueprints]**, comece digitando o nome de uma fila de solicitações ativa e selecione-a quando ela aparecer nos resultados da pesquisa.

   >[!IMPORTANT]
   >
   >Somente as filas de solicitações públicas aparecem nesta lista. Para tornar sua fila de solicitações pública, consulte a seção [Pré-requisitos](#prerequisites) acima.

   A preferência de fila de solicitações está definida e os usuários agora podem solicitar a instalação do blueprint.

   ![Configurar fila de solicitações](assets/Blueprints_access_setup_request_queue.png)

1. (Opcional) Para fazer alterações na fila de solicitações real, clique em **[!UICONTROL Editar esta fila de solicitações]**.

   O projeto de fila de solicitações é aberto em uma nova guia do navegador e você pode atualizá-lo conforme necessário.

1. (Opcional) Se a fila de solicitações contiver grupos de tópicos ou tópicos da fila, você pode selecioná-los na lista.
1. Para retornar ao catálogo de blueprints, clique em **[!UICONTROL Fechar]**.

>[!NOTE]
>
>Ao instalar um blueprint solicitado, você deve alterar o status do problema para **[!UICONTROL Fechado]** ou **[!UICONTROL Resolvido]** na fila de solicitações para que o solicitante seja notificado. Para obter informações sobre como instalar um blueprint, consulte [Instalar um blueprint](../../administration-and-setup/blueprints/blueprints-install.md).
