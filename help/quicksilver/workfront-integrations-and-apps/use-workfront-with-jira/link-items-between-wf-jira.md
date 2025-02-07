---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]
description: Você pode vincular [!DNL Jira] problemas a [!DNL Adobe Workfront] tarefas ou problemas automática ou manualmente.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '1231'
ht-degree: 0%

---

# Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]

Você pode vincular [!DNL Jira] problemas a [!DNL Adobe Workfront] tarefas ou problemas automática ou manualmente.

Somente um item em [!DNL Workfront] pode ser vinculado a um item em [!DNL Jira]. Você nunca pode vincular um item [!DNL Workfront] a vários problemas [!DNL Jira], nem um problema [!DNL Jira] a vários itens [!DNL Workfront].

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plano]</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] visão geral das licenças</a>*</td> 
   <td> <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acesso à Jira</td> 
   <td> <p>Acesso de administrador do sistema</p> <p><b>IMPORTANTE</b>

Recomendamos que você crie contas de administrador do sistema separadas no [!DNL Jira] e no [!DNL Workfront] para se dedicar a essa integração, em vez de usar contas existentes que possam estar anexadas a usuários.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter informações sobre administradores do [!DNL Workfront], consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Pré-requisitos

Antes de vincular itens entre [!DNL Workfront] e [!DNL Jira], é necessário

* Instalar o [!DNL Workfront] para [!DNL Jira]

  Para obter instruções sobre como instalar o Workfront para Jira, consulte [Instalar o Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront] para Jira

  Para obter instruções sobre como configurar o Workfront para Jira, consulte [Configurar o Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Vincular automaticamente [!DNL Workfront] itens a [!DNL Jira] problemas

Como administrador do [!DNL Workfront], você pode definir acionadores que podem criar automaticamente um problema no [!DNL Jira] sempre que determinadas condições forem atendidas em uma tarefa ou um problema no [!DNL Workfront]. O Workfront e [!DNL Jira] itens se tornam vinculados.

Após concluir a configuração do [!DNL Workfront] para Jira, quando um item for criado ou atualizado no [!DNL Workfront] para corresponder aos seus acionadores, um novo item será criado automaticamente no [!DNL Jira].\
Os usuários do Workfront que criam e atualizam itens do Workfront não precisam de uma licença do [!DNL Jira] para acionar a criação de itens no [!DNL Jira].

Para obter mais informações sobre como definir acionadores para criar problemas do Jira automaticamente, consulte [Configurar [!DNL Adobe Workfront] para o Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Você pode criar [!DNL Jira] itens automaticamente anexando um modelo a um projeto. Se o modelo contiver tarefas com atribuições que atendam aos [!DNL Jira] acionadores, as novas tarefas gerarão novos [!DNL Jira] problemas.

Vincular automaticamente um problema do [!DNL Workfront] a um problema do [!DNL Jira] é idêntico a vincular automaticamente uma tarefa do [!DNL Workfront] a um problema do [!DNL Jira].

Para vincular automaticamente uma tarefa [!DNL Workfront] a um problema [!DNL Jira]:

1. Verifique se o administrador do sistema do [!DNL Jira] configurou acionadores para criar automaticamente [!DNL Jira] problemas quando [!DNL Workfront] itens forem atribuídos e faça logon em [!DNL Workfront] com um nível de acesso que permita criar uma tarefa.

   Para obter mais informações sobre o acesso a tarefas, consulte [Conceder acesso a tarefas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

1. Vá para um projeto e selecione **[!UICONTROL Tarefas]** ![Ícone Tarefas](assets/tasks-icon-in-left-panel-14x14.png) no painel esquerdo.

1. Clique em **[!UICONTROL Nova tarefa]**

   Ou

   Selecione uma tarefa existente e clique em **Editar**.

1. Especifique ou atualize qualquer um dos campos disponíveis para a tarefa.
1. Clique em **[!UICONTROL Atribuições]** e atribua a tarefa a um usuário, função ou equipe que esteja especificado como um acionador na integração [!DNL Jira].

1. Clique em **Salvar alterações**.

   Uma nova tarefa é criada no Workfront.

   Na área **[!UICONTROL Atualizações]** da nova tarefa, há um comentário para indicar que um novo problema também foi criado em [!DNL Jira].

1. (Opcional) Clique no link para o problema Jira para abri-lo no Jira.

   Ou

   Clique no link **[!UICONTROL Ir para Jira]** na área **[!UICONTROL Integrações]** da seção **[!UICONTROL Detalhes]** ou no cabeçalho da tarefa ou do problema, para abrir o problema [!DNL Jira].

   O administrador do sistema ou do grupo deve adicionar o campo [!UICONTROL Integrações] ao modelo de layout para exibi-lo no cabeçalho da tarefa ou do problema. Para obter informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Qualquer usuário do [!DNL Jira] pode começar a trabalhar imediatamente em itens criados automaticamente do [!DNL Workfront] e suas atualizações serão transferidas para o [!DNL Workfront] sem precisar de uma licença do [!DNL Workfront] para fazer isso.

   Somente os campos que você, como administrador do [!DNL Workfront], configurou durante a configuração do complemento [!DNL Workfront] são atualizados.

   Para obter mais informações sobre como sincronizar campos entre o Workfront e o Jira, consulte a seção [Configurar o Workfront para o Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#configuring-the-add-on-for-jira) em [Configurar o Adobe Workfront para o Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >O problema [!DNL Jira] não é atribuído a ninguém em [!DNL Jira] quando é automaticamente criado a partir do Workfront.

## Vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] itens

Depois que os itens forem criados em [!DNL Jira] e [!DNL Workfront], independentemente uns dos outros, você poderá vincular manualmente um problema [!DNL Jira] a uma tarefa ou problema [!DNL Workfront] existente.\
Você não pode vincular manualmente um item [!DNL Workfront] de [!DNL Workfront] a um item [!DNL Jira] existente.

>[!NOTE]
>
>Se o problema [!DNL Jira] não estiver em um projeto que não esteja identificado como um acionador na Integração [!DNL Workfront], você não poderá vinculá-lo manualmente a um item do Workfront ao usar a integração com o [!DNL Jira] No Local.\
>Para obter mais informações sobre como configurar acionadores para o fluxo de trabalho Workfront para Jira, consulte [Vincular automaticamente itens do Workfront a problemas do Jira](#automatically-link-workfront-items-to-jira-issues).

Quando [!DNL Workfront] e [!DNL Jira] itens são vinculados, determinados campos de um item podem ser atualizados automaticamente no outro.\
Para obter mais informações sobre como atualizar itens vinculados, consulte [Atualizar itens vinculados entre Jira e Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Para vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] itens:

1. (Condicional) Faça logon em [!DNL Workfront] e encontre um problema ou uma tarefa que você deseja vincular a [!DNL Jira] problema(s).
1. (Condicional) Na área [!UICONTROL Detalhes], copie o **[!UICONTROL Número de Referência]** do item no Workfront.

   Ou

   Na barra de endereços do item, copie a **URL** do item no Workfront.

   >[!IMPORTANT]
   >
   >Se sua organização foi integrada à Experiência unificada do Adobe, você deve usar o **Número de referência** para vincular itens do Workfront ao Jira. (A opção URL está disponível, mas retornará um erro se você usá-la.) Para obter informações sobre a Experiência unificada, consulte [Experiência unificada do Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Para organizações que não estão na Experiência unificada do Adobe, não é recomendável usar a opção de URL, pois os URLs podem ser alterados.

   >[!NOTE]
   >
   >Você deve ter uma licença do [!DNL Workfront] para fazer logon no [!DNL Workfront]. Caso contrário, um usuário do [!DNL Workfront] deverá fornecer essas informações a você.

1. Em [!DNL Jira], navegue até um problema que você deseja vincular manualmente ao item [!DNL Workfront].
1. No painel direito [!DNL Workfront], cole o **[!UICONTROL Número de Referência]** ou a **URL** do item [!DNL Workfront] que você deseja vincular a ele.

1. Clique em **[!UICONTROL Link]**.

   Os dois itens se tornam vinculados e o painel direito [!DNL Workfront] é preenchido com informações do item [!DNL Workfront].

   Os seguintes campos [!DNL Workfront] estão visíveis em [!DNL Jira], por padrão, no painel direito [!DNL Workfront]:

   * O **[!UICONTROL Nome]** do item: você pode acessar o item [!DNL Workfront] clicando no nome no painel.
   * **[!UICONTROL Nome do projeto]**
   * O **[!UICONTROL Status]** do item
   * A **[!UICONTROL Prioridade]** do item
   * A data em que ele foi criado em [!DNL Workfront]
   * As **[!UICONTROL Horas Planejadas]** do item
   * O **[!UICONTROL Número de Referência]**: Você pode acessar o item [!DNL Workfront] clicando no [!UICONTROL Número de Referência] no painel.

Para obter mais informações sobre como habilitar campos adicionais a serem exibidos no painel direito, consulte a seção [Configurar sincronização de campo entre [!DNL Jira] e [!DNL Workfront] Itens](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md#setting-up-field-synchronization) em [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Um comentário do administrador [!DNL Workfront] associado à integração é postado na guia **[!DNL Workfront]** do problema [!DNL Jira] para confirmar que um novo item [!DNL Jira] foi criado. O comentário contém um link para o problema [!DNL Jira].

## Desvincular itens entre [!DNL Jira] e [!DNL Workfront]

Itens vinculados entre [!DNL Jira] e [!DNL Workfront] podem ser desvinculados manualmente de [!DNL Jira].\
Você não pode desvincular um item [!DNL Workfront] do correspondente [!DNL Jira] em [!DNL Workfront].

Você precisa do seguinte acesso para desvincular o item vinculado manualmente:

* Você é o usuário que vinculou os itens manualmente
* Você é o administrador do sistema [!DNL Jira]

Somente um administrador [!DNL Workfront] pode desvincular itens que foram vinculados automaticamente.

Para desvincular um problema [!DNL Jira] de um item [!DNL Workfront]:

1. Em [!DNL Jira], navegue até um problema que esteja vinculado a uma tarefa ou problema do [!DNL Workfront].
1. Vá para o painel direito [!DNL Workfront], clique no ícone **[!UICONTROL Desvincular]** e clique em **[!UICONTROL Desvincular]**.

   Os itens [!DNL Jira] e [!DNL Workfront] vinculados anteriormente estão agora desvinculados. Quaisquer campos, comentários ou documentos que possam ser atualizados individualmente no futuro não serão atualizados em sua contraparte anterior no outro aplicativo.
