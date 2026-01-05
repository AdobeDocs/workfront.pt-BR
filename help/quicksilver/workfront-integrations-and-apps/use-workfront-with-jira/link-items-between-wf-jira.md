---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]
description: Você pode vincular [!DNL Jira] problemas a [!DNL Adobe Workfront] tarefas ou problemas automática ou manualmente.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 1c37f361-e866-4ac6-b672-408848a80ed6
source-git-commit: e06713b8871ba5e7bfae58f67ee246c9c1163a63
workflow-type: tm+mt
source-wordcount: '1378'
ht-degree: 1%

---

# Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]

<!-- Audited: 5/2025 -->

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Jira não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Jira.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Jira, consulte [módulos do Software Jira](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-modules-new).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Você pode vincular [!DNL Jira] problemas a [!DNL Adobe Workfront] tarefas ou problemas automática ou manualmente.

Somente um item em [!DNL Workfront] pode ser vinculado a um item em [!DNL Jira]. Você nunca pode vincular um item [!DNL Workfront] a vários problemas [!DNL Jira], nem um problema [!DNL Jira] a vários itens [!DNL Workfront].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão </p>
       <p>Plano </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Acesso à Jira</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no Jira e no Workfront para se dedicar a essa integração, em vez de usar as existentes que podem ser anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Instalar o [!DNL Workfront] para [!DNL Jira]

A instalação do [!DNL Workfront] for [!DNL Jira] OnDemand é idêntica à instalação dele em uma instância do Servidor [!DNL Jira].

Você deve ser um administrador [!DNL Jira] para instalar o complemento [!DNL Workfront].

Se você não for um administrador do [!DNL Jira], poderá procurar o complemento [!DNL Workfront] e solicitar que ele seja instalado. Sua solicitação é enviada ao administrador do [!DNL Jira] para aprovação e instalação.

Para obter mais informações sobre como solicitar a instalação de um complemento no aplicativo [!DNL Jira], consulte [Gerenciando solicitações de usuários para complementos.](https://confluence.atlassian.com/upm/managing-user-requests-for-add-ons-781394968.html)

Para instalar [!DNL Workfront for Jira]:

1. Faça logon em [!DNL Jira] como administrador [!DNL Jira].
1. Localize o complemento **[!DNL Workfront for Jira]** em [[!DNL Atlassian Marketplace]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview).

1. Clique em **[!UICONTROL Obter agora]** para instalá-lo.

   Após a conclusão da instalação, faça logon no [!DNL Workfront] a partir do [!DNL Jira] e configure sua integração.

   Para obter mais informações, consulte [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Pré-requisitos

Antes de vincular itens entre [!DNL Workfront] e [!DNL Jira], é necessário fazer o seguinte:

* Instalar o [!DNL Workfront] para [!DNL Jira].

  Para obter instruções, consulte [Instalar o Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront] para Jira.

  Para obter instruções, consulte [Configurar Adobe Workfront para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Vincular automaticamente [!DNL Workfront] itens a [!DNL Jira] problemas

Como administrador do [!DNL Workfront], você pode definir acionadores que criarão automaticamente um problema no [!DNL Jira] sempre que determinadas condições forem atendidas em uma tarefa ou um problema no [!DNL Workfront]. O Workfront e [!DNL Jira] itens se tornam vinculados.

Após concluir a configuração do [!DNL Workfront] para Jira, quando um item for criado ou atualizado no [!DNL Workfront] para corresponder aos seus acionadores, um novo item será criado automaticamente no [!DNL Jira].

Os usuários do Workfront que criam e atualizam itens do Workfront não precisam de uma licença do [!DNL Jira] para acionar a criação de itens no [!DNL Jira].

Para obter mais informações, consulte [Configurar [!DNL Adobe Workfront] para Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

>[!NOTE]
>
>Você pode criar [!DNL Jira] itens automaticamente anexando um modelo a um projeto. Se o modelo contiver tarefas com atribuições que atendam aos [!DNL Jira] acionadores, as novas tarefas gerarão novos [!DNL Jira] problemas.

Vincular automaticamente um problema do [!DNL Workfront] a um problema do [!DNL Jira] é idêntico a vincular automaticamente uma tarefa do [!DNL Workfront] a um problema do [!DNL Jira].

Para vincular automaticamente uma tarefa [!DNL Workfront] a um problema [!DNL Jira]:

1. Verifique se o administrador do sistema do [!DNL Jira] configurou acionadores para criar automaticamente [!DNL Jira] problemas quando [!DNL Workfront] itens forem atribuídos e faça logon em [!DNL Workfront] com um nível de acesso que permita criar uma tarefa.

   Para obter mais informações sobre o acesso a tarefas, consulte [Conceder acesso a tarefas](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md).

{{step1-to-projects}}

1. Na página **Projetos**, selecione um projeto.

1. No painel esquerdo do projeto, selecione **[!UICONTROL Tarefas]**.

1. Clique em **+ Nova tarefa**.

   >[!NOTE]
   >
   >Para vincular um item existente do Workfront a um problema do Jira, selecione **Editar** no menu **Mais** ![Ícone Mais](assets/more-icon.png) do item.

1. Especifique ou atualize qualquer um dos campos disponíveis para a tarefa.
1. No campo **[!UICONTROL Atribuições]**, procure e selecione o usuário, a função ou a equipe especificada como um acionador na integração [!DNL Jira].

1. Clique em **Criar tarefa**. A tarefa é criada no Workfront, e um novo comentário aparece na guia **Atualizações** da tarefa para indicar que um novo problema também foi criado em [!DNL Jira].

1. (Opcional) Na área **[!UICONTROL Integrações]** da seção **[!UICONTROL Detalhes]** do cabeçalho da tarefa ou do problema, clique no link **[!UICONTROL Ir para Jira]** para abrir o problema no Jira.

   O administrador do sistema ou do grupo deve adicionar o campo [!UICONTROL Integrações] ao modelo de layout para exibi-lo no cabeçalho da tarefa ou do problema. Para obter informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   Qualquer usuário do [!DNL Jira] pode começar a trabalhar imediatamente em itens criados automaticamente do [!DNL Workfront] e suas atualizações serão transferidas para o [!DNL Workfront] sem precisar de uma licença do [!DNL Workfront] para fazer isso.

   Somente os campos que você, como administrador do [!DNL Workfront], configurou durante a configuração do complemento [!DNL Workfront] são atualizados.

   Para obter mais informações sobre como sincronizar campos entre o Workfront e o Jira, consulte a seção Configurar o Workfront para o Jira em [Configurar o Adobe Workfront para o Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

   >[!NOTE]
   >
   >O problema [!DNL Jira] não é atribuído a ninguém em [!DNL Jira] quando é criado automaticamente no Workfront.

## Vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] itens

Depois que os itens forem criados em [!DNL Jira] e [!DNL Workfront] independentemente uns dos outros, você poderá vincular manualmente um problema [!DNL Jira] a uma tarefa ou problema [!DNL Workfront] existente.

Você não pode vincular manualmente um item [!DNL Workfront] de [!DNL Workfront] a um item [!DNL Jira] existente.

>[!NOTE]
>
>Se o problema [!DNL Jira] não estiver em um projeto que não esteja identificado como um acionador na Integração [!DNL Workfront], você não poderá vinculá-lo manualmente a um item do Workfront ao usar a integração com o [!DNL Jira] No Local.\
>Para obter mais informações sobre como configurar acionadores para o fluxo de trabalho Workfront para Jira, consulte [Vincular automaticamente itens do Workfront a problemas do Jira](#automatically-link-workfront-items-to-jira-issues).

Quando [!DNL Workfront] e [!DNL Jira] itens são vinculados, determinados campos de um item podem ser atualizados automaticamente no outro.\
Para obter mais informações sobre como atualizar itens vinculados, consulte [Atualizar itens vinculados entre Jira e Adobe Workfront](../../workfront-integrations-and-apps/use-workfront-with-jira/update-linked-items-between-jira-wf.md).

Para vincular manualmente [!DNL Jira] problemas a [!DNL Workfront] itens:

1. (Condicional) Faça logon em [!DNL Workfront] e encontre um problema ou uma tarefa que você deseja vincular a um problema de [!DNL Jira].
1. (Condicional) Na seção **Informações básicas** da guia **Detalhes da tarefa** ou **Detalhes do problema**, copie o **[!UICONTROL Número de referência]** do item no Workfront.

   Ou

   Na barra de endereços do item, copie a **URL** do item no Workfront.

   >[!IMPORTANT]
   >
   >Se sua organização foi integrada à Experiência unificada do Adobe, você deve usar o **Número de referência** para vincular itens do Workfront ao Jira. (A opção URL está disponível, mas retornará um erro se você usá-la.) Para obter informações sobre a Experiência unificada, consulte [Experiência unificada da Adobe para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
   >
   >Para organizações que não fazem parte da Experiência unificada da Adobe, não é recomendável usar a opção de URL, pois os URLs podem ser alterados.

   >[!NOTE]
   >
   >Você deve ter uma licença do [!DNL Workfront] para fazer logon no [!DNL Workfront]. Caso contrário, um usuário do [!DNL Workfront] deverá fornecer essas informações a você.

1. Em [!DNL Jira], navegue até um problema que você deseja vincular manualmente ao item [!DNL Workfront].
1. No painel direito [!DNL Workfront], cole o **[!UICONTROL Número de Referência]** ou a **URL** do item [!DNL Workfront] ao qual você deseja vinculá-lo.

1. Clique em **[!UICONTROL Link]**. Os dois itens se tornam vinculados e o painel direito [!DNL Workfront] é preenchido com informações do item [!DNL Workfront].

   Por padrão, os seguintes campos [!DNL Workfront] estão visíveis em [!DNL Jira] no painel direito [!DNL Workfront]:

   * O **[!UICONTROL Nome]** do item. Você pode acessar o item [!DNL Workfront] clicando no nome no painel.
   * O **[!UICONTROL Nome Do Projeto]**.
   * O **[!UICONTROL Status]** do item.
   * A **[!UICONTROL Prioridade]** do item.
   * A data em que foi criado em [!DNL Workfront].
   * As **[!UICONTROL Horas Planejadas]** do item.
   * O **[!UICONTROL Número De Referência]**. Você pode acessar o item [!DNL Workfront] clicando no **Número de Referência** no painel.

   Para obter mais informações sobre como habilitar campos adicionais a serem exibidos no painel direito, consulte a seção Configurar sincronização de campo entre [!DNL Jira] e [!DNL Workfront] Itens em [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md). Um comentário do administrador [!DNL Workfront] associado à integração é postado na guia **[!DNL Workfront]** do problema [!DNL Jira] para confirmar que um novo item [!DNL Jira] foi criado. O comentário contém um link para o problema [!DNL Jira].

## Desvincular itens entre [!DNL Jira] e [!DNL Workfront]

Itens vinculados entre [!DNL Jira] e [!DNL Workfront] podem ser desvinculados manualmente em [!DNL Jira]. Você não pode desvincular um item [!DNL Workfront] do correspondente [!DNL Jira] em [!DNL Workfront].

Você precisa do seguinte acesso para desvincular o item vinculado manualmente:

* Você é o usuário que vinculou os itens manualmente.
* Você é o administrador do sistema [!DNL Jira].

>[!NOTE]
>
>Somente um administrador [!DNL Workfront] pode desvincular itens que foram vinculados automaticamente.

Para desvincular um problema [!DNL Jira] de um item [!DNL Workfront]:

1. Faça logon no Jira.
1. Navegue até o problema que está vinculado a uma tarefa ou problema do [!DNL Workfront].
1. Vá para o painel direito **Workfront**.
1. Clique no ícone **[!UICONTROL Desvincular]** e em **[!UICONTROL Desvincular]**. Os itens [!DNL Jira] e [!DNL Workfront] vinculados anteriormente desvinculam.

   Qualquer um de seus campos, comentários ou documentos que forem atualizados no futuro não será atualizado em sua contraparte anterior na outra aplicação.
