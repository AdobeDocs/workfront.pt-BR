---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurar folga pessoal
description: É importante indicar no Adobe Workfront quando a folga aprovada acontece, pois isso afeta sua programação e afeta as Datas de conclusão planejadas das tarefas às quais você está atribuído.
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 4%

---

# Configurar folga pessoal

<!-- Audited: 12/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment, and is being released in a phased rollout to Production.</span>-->

O [!DNL Adobe Workfront] não foi projetado para replicar ou substituir seus sistemas existentes para gerenciar, acumular e rastrear o tempo livre pessoal.

No entanto, é importante indicar quando ocorre a folga aprovada, pois isso afeta seu agendamento e as [!UICONTROL Datas de conclusão planejadas] das tarefas às quais você está atribuído.

Por exemplo, se você estiver atribuído a uma tarefa com duração de duas semanas e planeja três dias de folga durante esse período, o [!DNL Workfront] adiciona três dias à linha do tempo da tarefa para considerar o tempo de folga.

As ferramentas de Gerenciamento de Recursos também usam sua folga pessoal para indicar quando você está disponível para ser programado para o trabalho.

>[!NOTE]
>
>Para garantir que não ocorram inconsistências com as datas para as quais você agenda a folga, recomendamos que o fuso horário do seu perfil de usuário corresponda ao da sua agenda. Para obter mais informações, consulte os seguintes artigos:
>
>* [Criar um agendamento](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td> <p>Para configurar suas folgas pessoais, você deve ter:</p>
        <p>Padrão (para configurar seu tempo livre pessoal)</p>
        <p>Trabalhar ou mais (para configurar seu tempo livre pessoal)</p> </td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td><p>Para fazer alterações no calendário de folga de outro usuário, você deve ser o gerente desse usuário e ter acesso para Editar usuário.</p>
   <p><strong>OBSERVAÇÃO:</strong> se um gerente editar o calendário de folga pessoal de outro usuário, todas as entradas serão mostradas no fuso horário do usuário e não no fuso horário do gerente.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar folga pessoal em [!DNL Workfront]

{{step1-click-profile-pic}}

>[!NOTE]
>
>Se sua organização estiver na Experiência unificada da Adobe, clique no menu de conta do **Adobe** (sua imagem de perfil) no canto superior direito da área de navegação superior e clique em **Perfil do Workfront**.
>
>![perfil do workfront](assets/aue-profile.png)

1. No painel esquerdo, clique em **[!UICONTROL Folga]**.
1. Selecione a data desejada para sua folga pessoal.

   ![Calendário de folga pessoal](assets/personal-time-off-calendar-0925.png)

   <!--Sample image in the Production environment:
   ![Personal time off calendar](assets/personal-time-off-calendar.png)-->

1. Selecione **[!UICONTROL Todo o dia]**, se você estiver tirando um dia de folga.

   Deixe a caixa de seleção desmarcada se estiver tirando menos de um dia inteiro de folga e indique as horas de início e término de sua folga.

1. Clique em **[!UICONTROL Salvar]**.

   Sua folga agora está visível no sistema [!DNL Workfront] nas ferramentas de gerenciamento de recursos, como o Planejador de recursos e o Balanceador de carga de trabalho. Quando você recebe um trabalho durante esse período, uma dica de ferramenta informa ao usuário que você programou uma folga.
