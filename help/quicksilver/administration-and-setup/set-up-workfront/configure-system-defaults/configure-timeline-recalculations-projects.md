---
user-type: administrator
product-area: system-administration;projects;setup
navigation-topic: configure-system-defaults
title: Configurar recálculos de cronograma de projetos
description: Recalcular linhas do tempo permite que os gerentes vejam como as forças fora do projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas para o projeto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 67028988-6ac3-48d4-957e-1b5202d33c48
source-git-commit: 4705c3fc76c1544f8c71e70a773432f164282abb
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 0%

---

# Configurar recálculos de cronograma de projetos

Recalcular linhas do tempo permite que os gerentes vejam como as forças fora do projeto estão afetando a linha do tempo do projeto. A linha do tempo de um projeto se refere às datas planejadas e projetadas para o projeto.

Como um [!DNL Adobe Workfront] administrador, você pode recalcular manualmente as linhas do tempo de todos os projetos no sistema. Os proprietários de projetos também podem recalcular manualmente as linhas do tempo de projetos individuais. Para obter mais informações, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

Este artigo descreve como você, como um [!DNL Workfront] pode determinar como e quando [!DNL Workfront] O calcula automaticamente as linhas do tempo do projeto configurando as preferências do projeto no [!UICONTROL Configuração] área.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Nível de acesso do administrador do sistema</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar recálculos automáticos

Como um [!DNL Adobe Workfront] administrador, você pode configurar quando [!DNL Workfront] recalcula automaticamente as linhas de tempo do projeto. [!DNL Workfront] O pode recalcular as linhas do tempo do projeto todas as noites, quando o escopo do projeto for alterado ou ambos.

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito, ou na guia [!UICONTROL **Menu principal**] ícone ![](assets/lines-main-menu.png) no canto superior esquerdo de [!DNL Workfront], se disponível, em seguida clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Preferências do projeto]** > **[!UICONTROL Projetos].**

1. No **[!UICONTROL Linhas de Tempo]** habilite ou desabilite uma ou ambas as configurações abaixo. Por padrão, ambas as configurações são ativadas.

   * **Todas as noites:** [!DNL Workfront&#x200B;&#x200B;&#x200B;] recalcula as linhas do tempo uma vez a cada 24 horas, à noite, somente para projetos com status de [!UICONTROL Atual] e que foram atualizadas nos últimos três meses. Dependendo da carga do sistema e de outros fatores, o tempo de recálculo pode ser atrasado em mais de 24 horas.

     Nesse caso, [!DNL Workfront] recalcula a linha do tempo para todos os projetos que possuem uma [!UICONTROL Tipo de atualização] de [!UICONTROL Automático] ou [!UICONTROL Automático e Mediante alteração].

   * **Quando o escopo de um projeto é alterado**: para obter informações sobre o que constitui uma alteração de escopo de projeto, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

     Nesse caso, [!DNL Workfront] recalcula a linha do tempo para todos os projetos que possuem um Tipo de atualização de [!UICONTROL Automático e Mediante alteração] ou [!UICONTROL Somente na alteração].
Para obter informações sobre Tipos de atualização de projeto, consulte [Visão geral do Tipo de atualização de projeto](../../../manage-work/projects/planning-a-project/project-update-type-overview.md).

1. Clique em **[!UICONTROL Salvar]**.

   A linha do tempo de todos os projetos no sistema é recalculada automaticamente com base no Tipo de atualização de cada projeto.

## Recalcular linhas do tempo para todo o [!DNL Workfront] instância

Você pode executar o [!UICONTROL Recalcular Linha de Tempo] diagnóstico para recalcular manualmente todas as linhas do tempo no [!DNL Workfront] sistema. Isso permite que todos os gerentes de projeto vejam a influência das alterações externas imediatamente nas datas planejadas e projetadas. Para obter mais informações, consulte [Usar diagnósticos para acionar processos automatizados](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
