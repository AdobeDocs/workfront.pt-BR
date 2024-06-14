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

# Configurar o [!UICONTROL Calendário da página inicial] configurações de visualização

<!--Audited: 01/2024-->

Você pode configurar o [!UICONTROL Calendário da página inicial] configurações para fazer o seguinte:

* Integre com uma versão do [!DNL Outlook] baseada na web no [!DNL Office 365] hospedado na nuvem ou [!DNL Outlook Live]. Você pode exibir todos os eventos do seu calendário do Outlook e qualquer calendário associado que você selecionar no seu [!UICONTROL Calendário da página inicial] no Adobe Workfront.
* Ajudar a controlar a carga de trabalho em relação às horas de trabalho disponíveis na [!UICONTROL Alocação] barra.

Para saber mais sobre o Calendário da página inicial, consulte [[!UICONTROL Calendário da página inicial] exibir](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

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

*Para descobrir que tipo de plano ou licença você tem, entre em contato com o [!DNL Workfront] administrador. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sobre a integração [!DNL Microsoft Outlook] calendários

Considere o seguinte ao configurar seu Calendário da página inicial com [!DNL Microsoft Outlook] calendário:

* É possível integrar somente uma versão baseada na Web do [!DNL Outlook] em nuvem [!DNL Office 365] ou [!DNL Outlook Live].

  No local [!DNL Outlook] e [!DNL Outlook] em uma empresa baseada em nuvem [!DNL Exchange] servidor não são compatíveis.

  Se sua organização usa logon único, é necessário [!DNL Microsoft 365 E3] ou [!DNL E5].

* Anexos associados ao seu [!DNL Outlook] os eventos não estão anexados à [!DNL Outlook] eventos no Calendário da página inicial.
* Integração com um [!DNL Outlook] o calendário deve ser preenchido individualmente para cada usuário.
* Eventos que aparecem na variável [!UICONTROL Vencimento] não aparecem na sua [!DNL Microsoft] calendário, a menos que você os tenha arrastado da [!UICONTROL Lista de trabalho] ao seu [!DNL Adobe Workfront] Calendário. Para obter mais informações, consulte [[!UICONTROL Vencimento] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) e [Lista de trabalho na [!UICONTROL Calendário da página inicial]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) in [[!UICONTROL Calendário da página inicial] exibir](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Ao habilitar a integração com o [!DNL Outlook], somente itens de trabalho que são arrastados para o [!UICONTROL Calendário da página inicial] a partir desse ponto, será sincronizado. Os itens que estavam no Calendário da página inicial antes de habilitar a integração não serão exibidos, e você deve arrastá-los para o Calendário da página inicial novamente se quiser que eles sejam exibidos no [!DNL Outlook].
* Ao compartilhar (ou cancelar o compartilhamento) de um [!DNL Outlook] calendário com outras pessoas, ou quando você altera o nível de permissão de um calendário que você compartilha com outras pessoas, essa alteração não afeta seus calendários por cerca de 30 minutos. Para obter mais informações, consulte o [!DNL Microsoft Outlook] documentação.\
   Consequentemente, ao integrar [!DNL Workfront] Calendário com um [!DNL Outlook] que você compartilha com outros usuários, eles não verão seu [!DNL Workfront] Itens de calendário por cerca de 30 minutos.

>[!NOTE]
>
>A variável [!DNL Outlook] a configuração do calendário é completamente separada da variável [!DNL Outlook] Suplemento ([!UICONTROL [!DNL Outlook] Integração] ou [!DNL Workfront Outlook]). Não é necessária nenhuma instalação para configurar o calendário, mas há uma instalação necessária para o [!DNL Outlook] suplemento. Para obter mais informações sobre o [!DNL Outlook] Consulte Suplemento [Configurar [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configurar o [!UICONTROL Calendário da página inicial] exibir configurações e integrá-las aos calendários do Outlook

1. No [!UICONTROL Calendário da página inicial] clique no link **[!UICONTROL Configurações]** ícone de engrenagem ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png) no canto superior direito para abrir a **[!UICONTROL Configurações do calendário]** à direita.

   Se precisar de informações sobre como acessar o [!UICONTROL Calendário da página inicial] exibir, consulte [Exibir o [!UICONTROL Calendário da página inicial]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Opcional) Para integrar sua [!DNL Microsoft Outlook] calendário, clique em **[!UICONTROL Adicionar conta]** no canto superior direito da **[!UICONTROL Configurações do calendário]** painel. Em seguida, se for solicitado, insira o [!DNL Microsoft Outlook] informações de logon. Você pode repetir essa etapa para adicionar vários [!DNL Outlook] contas.

   >[!NOTE]
   >
   >Você deve dar [!DNL Workfront] permissão para acessar seu [!DNL Outlook] calendário. Conceder permissão permite [!DNL Workfront] para manter o acesso aos dados do calendário, leia [!DNL outlook] perfil, além de ler e atualizar o [!DNL Microsoft] calendário.

1. Atualize a janela do navegador para ver as informações do [!DNL Outlook] conta no calendário e no [!UICONTROL Configurações do calendário] painel.
1. Clique em **[!UICONTROL Configurações]** ícone de engrenagem novamente no canto superior direito para abrir a **[!UICONTROL Configurações do calendário]** painel. ![Calendar_Settings_gear_icon.png](assets/calendar-settings-gear-icon.png)

1. (Opcional) Em cada [!DNL Microsoft] conta adicionada na etapa anterior, selecione **[!UICONTROL Exibir]** ou **[!UICONTROL Sincronizar]**:

   * **[!UICONTROL Exibir]**: essa é uma opção somente leitura exibida [!DNL Microsoft] eventos do calendário em seu [!UICONTROL Calendário da página inicial].
   * **[!UICONTROL Sincronizar]**: essa opção permite uma sincronização bidirecional entre as [!DNL Microsoft] e [!UICONTROL Início] calendários. Em outras palavras, [!DNL Workfront] [!UICONTROL Calendário da página inicial] itens são exportados para o seu [!DNL Microsoft] calendário e [!DNL Microsoft] importação de itens do calendário para o Workfront [!UICONTROL Calendário da página inicial] em tempo real.

     ![](assets/view-sync-checkboxes-qs.png)

1. (Opcional) Em seu [!DNL Workfront] ou uma conta integrada, selecione os calendários associados que deseja visualizar no seu [!UICONTROL Calendário da página inicial] (como seu calendário de PTO, Aniversários ou Feriados) e clique no link do seu navegador [!UICONTROL Atualizar] ou [!UICONTROL Recarregar] botão para ver as alterações.

1. (Opcional) Na **[!UICONTROL Geral]** seção em **[!UICONTROL Iniciar Semana em]**, selecione o dia que deseja exibir como o primeiro dia da semana de trabalho no Calendário da página inicial.

   ![](assets/general-section-home-calendar-settings-panel.png)

1. Configure as seguintes opções:

   * **[!UICONTROL Meus Dias de Trabalho]:** Selecione os dias de trabalho.
   * **[!UICONTROL Meu horário de início habitual]:** Selecione a hora em que você iniciou seu dia de trabalho.
   * **[!UICONTROL Meu horário de término habitual]:** Selecione a hora em que você encerra seu dia de trabalho.

   [!DNL Workfront] O usa essas três configurações para calcular o número de horas trabalhadas em uma semana. Esse número afeta o [!UICONTROL Alocação] que ajuda a controlar sua carga de trabalho em relação às horas de trabalho disponíveis. Para obter mais informações, consulte [[!UICONTROL Alocação] barra](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) no artigo [[!UICONTROL Calendário da página inicial] exibir](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Clique fora da **[!UICONTROL Configurações do calendário]** área para fechá-la.

   [!DNL Workfront] O salva as alterações automaticamente.

Para obter informações sobre como usar o [!UICONTROL Calendário] para gerenciar suas atribuições de trabalho e eventos de calendário integrados, consulte [Use o [!UICONTROL Calendário da página inicial] exibir](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
