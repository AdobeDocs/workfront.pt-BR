---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Definir as configurações de exibição do Calendário da página inicial
description: Você pode definir as configurações do Calendário da página inicial para integrar-se a uma versão do Outlook baseada na Web e ajudá-lo a controlar sua carga de trabalho em relação às horas de trabalho disponíveis.
author: Nolan
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 1%

---

# Configurar as configurações de exibição do [!UICONTROL Calendário da página inicial]

<!--Audited: 01/2024-->

Você pode definir as configurações do [!UICONTROL Calendário da página inicial] para fazer o seguinte:

* Integre com uma versão do [!DNL Outlook] baseada na web no [!DNL Office 365] hospedado na nuvem ou [!DNL Outlook Live]. Você pode exibir todos os eventos do seu calendário do Outlook e de qualquer calendário associado selecionado no seu [!UICONTROL Calendário da Página Inicial] no Adobe Workfront.
* Ajudar a controlar sua carga de trabalho em relação ao horário disponível na barra [!UICONTROL Alocação].

Para saber mais sobre o Calendário da página inicial, consulte a [[!UICONTROL exibição do Calendário da página inicial]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

Este artigo descreve como você pode definir as configurações do Calendário da página inicial e integrar o Calendário da página inicial ao seu calendário externo do Outlook.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>Atual: [!UICONTROL Trabalho] ou superior</p> 
   Ou
   <p>Novo: [!UICONTROL Padrão]</p> 
   </td> 
  </tr> 
   </tbody> 
</table>

*Para saber que tipo de plano ou licença você tem, contate o administrador do [!DNL Workfront]. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sobre a integração de calendários do [!DNL Microsoft Outlook]

Considere o seguinte ao configurar seu Calendário da página inicial com seu calendário do [!DNL Microsoft Outlook]:

* Você pode integrar apenas uma versão baseada na Web de [!DNL Outlook] no [!DNL Office 365] ou [!DNL Outlook Live] hospedado na nuvem.

  Não há suporte para [!DNL Outlook] e [!DNL Outlook] locais em um servidor [!DNL Exchange] corporativo baseado em nuvem.

  Se sua organização usa logon único, você precisa de [!DNL Microsoft 365 E3] ou [!DNL E5].

* Os anexos associados aos eventos do [!DNL Outlook] não estão anexados aos eventos do [!DNL Outlook] no Calendário da Página Inicial.
* A integração com um calendário [!DNL Outlook] deve ser concluída para cada usuário individualmente.
* Os eventos exibidos na barra [!UICONTROL Conclusão] não aparecem no calendário [!DNL Microsoft], a menos que você os tenha arrastado da [!UICONTROL Lista de Trabalho] para o Calendário [!DNL Adobe Workfront]. Para obter mais informações, consulte [[!UICONTROL Barra de vencimento]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) e [Lista de trabalho no [!UICONTROL Calendário da página inicial]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) no modo de exibição [[!UICONTROL Calendário da página inicial]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Ao habilitar a integração com [!DNL Outlook], somente os itens de trabalho arrastados para o [!UICONTROL Calendário da Página Inicial] desse ponto serão sincronizados. Os itens que estavam no Calendário da página inicial antes da habilitação da integração não serão exibidos, e você deve arrastá-los para o Calendário da página inicial novamente se quiser que eles apareçam em [!DNL Outlook].
* Quando você compartilha (ou cancela o compartilhamento) um calendário do [!DNL Outlook] com outras pessoas, ou quando você altera o nível de permissão de um calendário que você compartilha com outras pessoas, essa alteração não afeta seus calendários por cerca de 30 minutos. Para obter mais informações, consulte a documentação do [!DNL Microsoft Outlook].\
   Consequentemente, quando você integra o Calendário do [!DNL Workfront] a um calendário do [!DNL Outlook] que você compartilha com outros usuários, eles não verão os itens do Calendário do [!DNL Workfront] por cerca de 30 minutos.

>[!NOTE]
>
>A configuração do calendário [!DNL Outlook] é completamente separada do Suplemento [!DNL Outlook] ([!UICONTROL [!DNL Outlook] Integração] ou [!DNL Workfront Outlook]). Não é necessária nenhuma instalação para configurar o calendário, mas há uma instalação necessária para o Suplemento [!DNL Outlook]. Para obter mais informações sobre o Suplemento [!DNL Outlook], consulte [Configurar [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configure suas configurações de exibição do [!UICONTROL Calendário da Página Inicial] e integre-o aos calendários do Outlook

1. No modo de exibição [!UICONTROL Calendário da página inicial], clique no ícone de engrenagem **[!UICONTROL Configurações]** ![Calendário_Configurações_ícone_de_engrenagem.png](assets/calendar-settings-gear-icon.png), no canto superior direito, para abrir o painel **[!UICONTROL Configurações do calendário]**, à direita.

   Se precisar de informações sobre como acessar o modo de exibição [!UICONTROL Calendário da Página Inicial], consulte [Exibir o [!UICONTROL Calendário da Página Inicial]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Opcional) Para integrar seu calendário do [!DNL Microsoft Outlook], clique em **[!UICONTROL Adicionar conta]** no canto superior direito do painel **[!UICONTROL Configurações do calendário]**. Em seguida, se for solicitado, insira suas informações de logon do [!DNL Microsoft Outlook]. Você pode repetir esta etapa para adicionar várias contas do [!DNL Outlook].

   >[!NOTE]
   >
   >Você deve dar permissão [!DNL Workfront] para acessar seu calendário [!DNL Outlook]. Conceder permissão permite que o [!DNL Workfront] mantenha o acesso aos dados do calendário, leia o perfil do [!DNL outlook] e leia e atualize o calendário do [!DNL Microsoft].

1. Atualize a janela do navegador para ver informações da sua conta do [!DNL Outlook] no calendário e no painel [!UICONTROL Configurações do calendário].
1. Clique no ícone de engrenagem **[!UICONTROL Configurações]** novamente no canto superior direito para abrir o painel **[!UICONTROL Configurações do calendário]**. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (Opcional) Em cada conta do [!DNL Microsoft] adicionada na etapa anterior, selecione **[!UICONTROL Exibir]** ou **[!UICONTROL Sincronizar]**:

   * **[!UICONTROL Exibir]**: esta é uma opção somente leitura que exibe [!DNL Microsoft] eventos de calendário no [!UICONTROL Calendário da Página Inicial].
   * **[!UICONTROL Sincronizar]**: esta opção permite uma sincronização bidirecional entre os calendários do [!DNL Microsoft] e da [!UICONTROL Página Inicial]. Em outras palavras, os itens do [!DNL Workfront] [!UICONTROL Calendário da página inicial] são exportados para o calendário [!DNL Microsoft] e os itens do calendário [!DNL Microsoft] são importados para o [!UICONTROL Calendário da página inicial] da Workfront em tempo real.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Opcional) Em sua conta do [!DNL Workfront] ou em uma conta integrada, selecione os calendários associados que você deseja exibir em seu [!UICONTROL Calendário da página inicial] (como seu calendário de PTO, Aniversários ou Feriados) e clique no botão [!UICONTROL Atualizar] ou [!UICONTROL Recarregar] do navegador para ver suas alterações.

1. (Opcional) Na seção **[!UICONTROL Geral]** em **[!UICONTROL Iniciar Semana em]**, selecione o dia que deseja exibir como o primeiro dia da semana de trabalho no Calendário da Página Inicial.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configure as seguintes opções:

   * **[!UICONTROL Meus Dias Úteis]:** Selecione os dias em que você trabalha.
   * **[!UICONTROL Meu horário de início habitual]:** Selecione o horário em que você inicia seu dia de trabalho.
   * **[!UICONTROL Meu horário de término habitual]:** Selecione o horário em que você encerra seu dia de trabalho.

   O [!DNL Workfront] usa essas três configurações para calcular o número de horas que você trabalha em uma semana. Este número afeta a barra [!UICONTROL Alocação], que ajuda a controlar sua carga de trabalho em relação às horas de trabalho disponíveis. Para obter mais informações, consulte a [[!UICONTROL Barra de alocação]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) no artigo [[!UICONTROL exibição do ] Calendário da página inicial](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Clique fora da área **[!UICONTROL Configurações do calendário]** para fechá-la.

   [!DNL Workfront] salva suas alterações automaticamente.

Para obter informações sobre como usar o modo de exibição [!UICONTROL Calendário] para gerenciar suas atribuições de trabalho e eventos de calendário integrados, consulte [Usar o modo de exibição [!UICONTROL Calendário da página inicial]](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
