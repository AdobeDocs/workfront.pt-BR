---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Visão geral das conexões
description: Para a maioria dos aplicativos, é necessário criar uma conexão, por meio da qual o [!DNL Adobe Workfront Fusion]  pode se comunicar com o serviço de terceiros fornecido de acordo com as configurações do cenário específico.
author: Becky
feature: Workfront Fusion
exl-id: 2d5cf083-9893-45e8-8f7d-0f8f5a74eef3
source-git-commit: b90343eab40e91c6f5cddeaa960ce9c9c97b1d29
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 0%

---

# Visão geral das conexões

<!-- Audited: 3/2024-->

Para a maioria dos aplicativos, o [!DNL Workfront Fusion] requer uma conexão, por meio da qual ele pode se comunicar com o serviço de terceiros especificado de acordo com as configurações do cenário específico.

Por exemplo, se você deseja criar um cenário que recupere informações de [!DNL Workfront], você deve conceder permissão de acesso para [!DNL Workfront Fusion] acessar sua conta [!DNL Workfront].

Uma conexão representa a autorização e as permissões que o Fusion usa para acessar o aplicativo. É possível criar uma ou mais conexões para cada aplicativo e usar a mesma conexão em vários módulos ou cenários.

A maioria das conexões é usada somente para um único aplicativo. Por exemplo, uma conexão [!DNL Workfront] não pode ser usada em um módulo [!UICONTROL Salesforce]. Alguns aplicativos do [!DNL Adobe] podem compartilhar conexões. Para obter detalhes, consulte os artigos desses aplicativos, listados em [Aplicativos e seus módulos](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

As conexões são gerenciadas no nível da equipe. Todos os membros de uma equipe têm acesso às conexões da equipe e os usuários fora de uma equipe não têm acesso às conexões da equipe.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p><p>Ou</p><p>Atual: [!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td>
   <p>Atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Herdados: Qualquer um </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Novo:</p> <ul><li>[!UICONTROL Select] ou [!UICONTROL Prime] [!DNL Workfront] Plano: sua organização deve comprar [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plano: [!DNL Workfront Fusion] está incluído.</li></ul>
   <p>Ou</p>
   <p>Atual: sua organização deve comprar o [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Direitos de acesso

Para cada conexão, [!DNL Workfront Fusion] requer somente os direitos de acesso necessários para concluir com êxito um determinado cenário. Por exemplo, se você criar um cenário para listar documentos de [!DNL Google Docs], [!DNL Workfront Fusion] não solicitará permissão para obter o conteúdo dos documentos. Posteriormente, se você achar que precisa acessar o conteúdo dos documentos, poderá atualizar a conexão ou criar uma nova que possa acessar esse conteúdo.

Nem todos os serviços permitem limitar o acesso a tarefas específicas. Nesses casos, [!DNL Workfront Fusion] deve exigir direitos de acesso totais. Para obter mais informações sobre como restringir o acesso do [!DNL Workfront Fusion] à sua conta registrada para esses serviços, consulte a documentação específica do aplicativo listada em [Aplicativos e seus módulos](/help/quicksilver/workfront-fusion/apps-and-their-modules/apps-and-their-modules.md).

## Gerenciar conexões

Você pode gerenciar todas as conexões da área [!UICONTROL Conexões].

>[!NOTE]
>
>As conexões são de propriedade de equipes. Se não conseguir encontrar a conexão que você está procurando, verifique se você está vendo o grupo correto.
>
>Para selecionar uma nova equipe:
>
>* Clique no nome do grupo no menu de navegação esquerdo e selecione um novo grupo.
>
>    Ou
>
>* Clique em Visão geral da equipe no menu de navegação esquerdo e, em seguida, clique na seta suspensa ao lado do nome da equipe, próximo à parte superior da página. Selecione uma nova equipe.

1. Para abrir a área [!UICONTROL Conexões], clique em <b>[!UICONTROL Conexões]</b> no painel de navegação esquerdo.
1. (Opcional) Indique o ambiente e o tipo de conexão, clicando na lista suspensa Ambiente e tipo e selecionando uma opção.
1. (Opcional) Para exibir quais permissões foram fornecidas a [!DNL Workfront Fusion] para uma conexão, clique no ícone Exibir ![Exibir permissões de conexão](assets/view-connection-permissions.png) para essa conexão.
1. (Opcional) Para renomear uma conexão, realce o nome da conexão e digite o novo nome.
1. (Opcional) Para reautorizar uma conexão, clique em **Reautorizar** para essa conexão.
1. (Opcional) Para excluir uma conexão, clique em **Excluir** dessa conexão.
1. (Opcional) Para verificar se a conexão com o serviço foi estabelecida com êxito, clique em **Verificar** para a conexão.



## Renovar uma conexão

[!DNL Workfront Fusion] geralmente obtém direitos de acesso a um determinado serviço por um período ilimitado. Alguns aplicativos exigem que a permissão de acesso seja renovada após um determinado período. Nesses casos, o [!DNL Workfront Fusion] o notifica por email pouco antes da expiração dos direitos de acesso.

Para renovar uma conexão:

1. Clique no botão **[!UICONTROL Reautorizar]** na área **[!UICONTROL Conexões]**.
