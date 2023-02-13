---
product-area: calendars;setup
navigation-topic: use-the-home-area
title: Definir as configurações de exibição do Calendário doméstico
description: Você pode configurar as configurações do Calendário Doméstico para integrar com uma versão baseada na Web do Outlook e ajudá-lo a rastrear sua carga de trabalho em relação às horas de trabalho disponíveis.
author: Lisa
feature: Get Started with Workfront
exl-id: 2acd930b-5923-452e-9d8d-a6121d8d37ac
source-git-commit: d1babaf52c4035c20bf3990272af5a2f401b7fcb
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 0%

---

# Configure seu [!UICONTROL Calendário doméstico] configurações de exibição

Você pode configurar o [!UICONTROL Calendário doméstico] configurações para fazer o seguinte:

* Integrar a uma versão baseada na Web de [!DNL Outlook] na nuvem hospedada [!DNL Office 365] ou [!DNL Outlook Live]. Você pode exibir todos os eventos do calendário do Outlook e qualquer calendário associado selecionado, como calendários de Aniversários e Feriados, em seu [!UICONTROL Calendário doméstico].
* Ajude você a rastrear sua carga de trabalho em relação às horas de trabalho disponíveis no [!UICONTROL Alocação] bar.

Para saber mais sobre o Calendário inicial, consulte [[!UICONTROL Calendário doméstico] exibir](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Trabalho] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano ou tipo de licença você possui, entre em contato com seu [!DNL Workfront] administrador.

## Sobre a integração [!DNL Microsoft Outlook] calendários

Considere o seguinte ao configurar seu Calendário doméstico com o [!DNL Microsoft Outlook] calendário:

* É possível integrar somente uma versão baseada na Web de [!DNL Outlook] na nuvem hospedada [!DNL Office 365] ou [!DNL Outlook Live].

   No local [!DNL Outlook] e [!DNL Outlook] em uma empresa baseada em nuvem [!DNL Exchange] não são suportados.

   Se sua organização usar logon único, será necessário [!DNL Microsoft 365 E3] ou [!DNL E5].

* Anexos associados à [!DNL Outlook] não são anexados ao [!DNL Outlook] em seu Calendário doméstico.
* Integração com um [!DNL Outlook] o calendário deve ser preenchido para cada usuário individualmente.
* Eventos que aparecem no [!UICONTROL Vencimento] a barra não aparece na sua [!DNL Microsoft] calendário, a menos que você os tenha arrastado do [!UICONTROL Lista de Trabalho] para [!DNL Adobe Workfront] Calendário. Para obter mais informações, consulte [[!UICONTROL Vencimento] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#viewing-the-due-bar) e [Lista de trabalho na [!UICONTROL Calendário doméstico]](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#using-the-left-panel-of-the-home-view) em [[!UICONTROL Calendário doméstico] exibir](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

* Ao habilitar a integração com o [!DNL Outlook], somente itens de trabalho que são arrastados para o [!UICONTROL Calendário doméstico] desse ponto em diante será sincronizado. Os itens que estavam no Calendário inicial antes de habilitar a integração não aparecerão e você deve arrastá-los para o Calendário inicial novamente se desejar que apareçam em [!DNL Outlook].
* Quando você compartilha (ou cancela o compartilhamento) uma [!DNL Outlook] calendário com outras pessoas ou quando você altera o nível de permissão de um calendário que compartilha com outras pessoas, essa alteração não afeta os calendários por cerca de 30 minutos (para obter mais informações, consulte o [!DNL Microsoft Outlook] documentação).\
   Consequentemente, ao integrar [!DNL Workfront] Calendário com um [!DNL Outlook] calendário compartilhado com outros usuários, eles não visualizarão seu [!DNL Workfront] Itens de calendário por cerca de 30 minutos.

>[!NOTE]
>
>O [!DNL Outlook] a configuração do calendário é completamente separada da [!DNL Outlook] Suplemento ([!UICONTROL [!DNL Outlook] Integração] ou [!DNL Workfront Outlook]). Não é necessária nenhuma instalação para configurar o calendário, mas há uma instalação necessária para o [!DNL Outlook] Suplemento. Para obter mais informações sobre o [!DNL Outlook] Consulte o suplemento [Configurar [!DNL Adobe Workfront for Outlook]](../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md).

## Configure seu [!UICONTROL Calendário doméstico] configurações de exibição

1. No [!UICONTROL Calendário doméstico] , clique no botão **[!UICONTROL Configurações]** ícone de engrenagem ![Calendar_Settings_évez_icon.png](assets/calendar-settings-gear-icon.png) no canto superior direito para abrir o **[!UICONTROL Configurações do calendário]** no lado direito da janela.

   Se precisar de informações sobre como acessar o [!UICONTROL Calendário doméstico] exibir, consulte [Visualize o [!UICONTROL Calendário doméstico]](../../../workfront-basics/using-home/using-the-home-area/view-home-calendar.md).

1. (Opcional) Para integrar o [!DNL Microsoft Outlook] calendário, clique em **[!UICONTROL Adicionar conta]** no canto superior direito do **[!UICONTROL Configurações do calendário]** painel. Em seguida, se você for solicitado a fazer isso, insira [!DNL Microsoft Outlook] informações de logon. Você pode repetir esta etapa para adicionar vários [!DNL Outlook] contas.

   >[!NOTE]
   >
   >Você deve dar [!DNL Workfront] permissão para acessar seu [!DNL Outlook] calendário. Concessão de permissão permite [!DNL Workfront] para manter o acesso aos dados do calendário, leia seu [!DNL outlook] e leia e atualize seu [!DNL Microsoft] calendário.

1. Atualize a janela do navegador para ver informações de seu [!DNL Outlook] no calendário e no [!UICONTROL Configurações do calendário] painel.
1. Clique no botão **[!UICONTROL Configurações]** ícone de engrenagem novamente no canto superior direito para abrir o **[!UICONTROL Configurações do calendário]** painel. ![Calendar_Settings_évez_icon.png](assets/calendar-settings-gear-icon.png)

1. (Opcional) Em cada [!DNL Microsoft] conta que você adicionou na etapa anterior, selecione **[!UICONTROL Exibir]** ou **[!UICONTROL Sincronizar]**:

   * **[!UICONTROL Exibir]**: Esta é uma opção somente leitura que é exibida [!DNL Microsoft] eventos de calendário em seu [!UICONTROL Calendário doméstico].
   * **[!UICONTROL Sincronizar]**: Essa opção permite uma sincronização bidirecional entre os [!DNL Microsoft] e [!UICONTROL Início] calendários. Por outras palavras, [!DNL Workfront] [!UICONTROL Calendário doméstico] exportar itens para o seu [!DNL Microsoft] calendário e [!DNL Microsoft] itens do calendário importados para a sua Workfront [!UICONTROL Calendário doméstico] em tempo real.

      ![](assets/view-sync-checkboxes-qs.png)

1. (Opcional) Em [!DNL Workfront] ou uma conta integrada, selecione os calendários associados que deseja visualizar em sua [!UICONTROL Calendário doméstico] (como seu PTO, aniversário ou calendário de Feriados) e clique no navegador [!UICONTROL Atualizar] ou [!UICONTROL Recarregar] para visualizar as alterações.

1. (Opcional) Na seção **[!UICONTROL Geral]** seção sob **[!UICONTROL Iniciar Semana em]**, selecione o dia que deseja exibir como o primeiro dia da semana de trabalho no Calendário inicial.

1. Configure as seguintes opções:

   * **[!UICONTROL Meus Dias de Trabalho]:** Selecione os dias de trabalho.
   * **[!UICONTROL Hora de início habitual]:** Selecione a hora em que você inicia o dia de trabalho.
   * **[!UICONTROL Hora de término normal]:** Selecione a hora em que você termina seu dia de trabalho.

   [!DNL Workfront] O usa essas três configurações para calcular o número de horas de trabalho em uma semana. Esse número afeta a função [!UICONTROL Alocação] bar, o que ajuda a rastrear sua carga de trabalho em relação ao horário de trabalho disponível. Para obter mais informações, consulte [[!UICONTROL Alocação] bar](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md#understanding-the-allocation-of-time) no artigo [[!UICONTROL Calendário doméstico] exibir](../../../workfront-basics/using-home/using-the-home-area/home-calendar-view.md).

1. Clique fora do **[!UICONTROL Configurações do calendário]** área para rejeitá-la.

   [!DNL Workfront] salva as alterações automaticamente.

Para obter informações sobre como usar o [!UICONTROL Calendário] para gerenciar suas atribuições de trabalho e eventos de calendário integrados, consulte [Use o [!UICONTROL Calendário doméstico] exibir](../../../workfront-basics/using-home/using-the-home-area/use-home-calendar-view.md).

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(NOTE: from Courtney: [step #] Type your weekly work hours under How many hours a week do you work?This number affects the Allocation bar, which helps you track your workload against your available work hours. For more information, see "Allocation Bar" in the article "Understanding the Home Calendar View.")
</MadCap:conditionalText>
-->
