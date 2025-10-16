---
product-area: workfront-integrations;projects
keywords: google,doc,documento,planilha,slide
navigation-topic: workfront-for-g-suite
title: Exibir e gerenciar  [!DNL Adobe Workfront] detalhes do objeto do Google Workspace
description: Você pode exibir e gerenciar os detalhes de um item de trabalho sem sair do Google Workspace. Por exemplo, você pode ler a descrição de uma tarefa, exibir seu objeto pai, alterar seu status e marcá-la como concluída, tudo dentro de [!DNL Adobe Workfront] para o Google Workspace.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 0f15b05f-3b4a-4f0b-9d9a-21a0f97de1ea
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Exibir e gerenciar detalhes do objeto [!DNL Adobe Workfront] de [!DNL Google Workspace]

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a seguinte funcionalidade do Workfront para Google Workspace não estará disponível após **28 de fevereiro de 2026**:
>
>* Acesso à funcionalidade Google Workspace no Workfront
>
>* Exibir e gerenciar tarefas do Workfront no Gmail ou no painel do site Calendário do Google
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Google Workspace.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Google Workspace, consulte [módulos do Gmail](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules) e [módulos do Google Calendar](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules).

Você pode exibir e gerenciar os detalhes de um item de trabalho sem sair de [!DNL Google Workspace]. Por exemplo, você pode ler a descrição de uma tarefa, exibir seu objeto pai, alterar seu status e marcá-la como concluída, tudo dentro de [!DNL Adobe Workfront for Google Workspace].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Standard</p><p>Trabalhar ou superior</p>
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de exibir e gerenciar os detalhes do item de trabalho no [!DNL Google Workspace], você deve

* Instalar [!DNL Workfront for Google Workspace]\
   Para obter instruções, consulte [Instalar [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md).

## Exibir e gerenciar detalhes do item de trabalho em [!DNL Google Workspace]

1. Se o painel [!UICONTROL Workfront para Google Workspace] não for exibido, clique no [!DNL Workfront] ícone ![Workfront ícone](assets/wf-lion-icon.png) na barra lateral de complementos [!DNL Google Workspace] na extremidade direita da página.
1. Vá para a tarefa ou problema [!DNL Workfront] em [!DNL Google Workspace], conforme descrito em [Acesso [!DNL Adobe Workfront] [!UICONTROL Residência] conteúdo de [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/access-wf-home-content-from-g-suite.md).

   Quando você seleciona uma tarefa ou problema, a guia **[!UICONTROL Detalhes]** está aberta. A área acima da guia **[!UICONTROL Detalhes]** exibe o nome do objeto pai, o nome da tarefa ou problema e a [!UICONTROL Data de vencimento] (se for uma tarefa) ou a [!UICONTROL Data de prioridade] (se for um problema).


   Você pode fazer várias tarefas nesta guia sem sair de [!DNL Google Workspace], incluindo as seguintes:

   * Exiba a **[!UICONTROL Descrição]** do objeto e outros detalhes, como os usuários atribuídos ao objeto, a **[!UICONTROL Prioridade]**, o solicitante, a **[!UICONTROL Data de conclusão planejada]** e quaisquer campos e formulários personalizados anexados ao objeto.

     Os formulários personalizados exibem apenas os campos nos quais foram adicionadas informações.

   * Clique na área **[!UICONTROL Projeto pai]** para exibir os detalhes do objeto pai.

     >[!TIP]
     >
     >Isso pode ser útil quando você tem tarefas e problemas com o mesmo nome e precisa diferenciá-los.

   * Aceite o trabalho atribuído a você clicando em **[!UICONTROL Trabalhar nisto]**.
   * Edite várias opções, como a opção **[!UICONTROL Concluído]**, o **[!UICONTROL Status]** e a **[!UICONTROL Porcentagem concluída]**.

     Em **[!UICONTROL Percentual concluído]**, digite números e (opcionalmente) o sinal de porcentagem % para indicar seu progresso em um item.
   * Exibir informações sobre uma solicitação de aprovação, incluindo o proprietário, o tamanho e quaisquer anexos.
   * **[!UICONTROL Aprovar]** ou **[!UICONTROL Rejeitar]** solicitações de aprovação e documentos.

   * **[!UICONTROL Conceder]** ou **[!UICONTROL Ignorar]** solicitações de acesso.

1. (Opcional) Clique em **[!UICONTROL Exibir em[!DNL Workfront]]** para ir para o item de trabalho atual em [!DNL Workfront].

* Para obter informações sobre como usar a guia [!UICONTROL Atualizações] em [!DNL Workfront for Google Workspace], consulte [Atualizar um [!DNL Adobe Workfront] objeto de [!DNL Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/update-a-workfront-object-in-gsuite.md).
* Para obter informações sobre como usar a guia [!UICONTROL Documentos] em [!DNL Workfront for Google Workspace], consulte [Exibir e gerenciar documentos do [!DNL G Suite]](../../workfront-integrations-and-apps/workfront-for-g-suite/view-and-manage-documents-in-gsuite.md).
