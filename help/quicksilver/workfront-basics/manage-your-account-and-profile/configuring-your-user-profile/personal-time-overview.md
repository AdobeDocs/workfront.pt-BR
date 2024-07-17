---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: Configurar folga pessoal
description: É importante indicar no Adobe Workfront quando a folga aprovada acontece, pois isso afeta sua programação e afeta as Datas de conclusão planejadas das tarefas às quais você está atribuído.
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 1%

---

# Configurar folga pessoal

<!-- Audited: 12/2023 -->

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

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> <p>Novo: Padrão (para configurar seu tempo livre pessoal)</p>
        <p>ou</p>
        <p>Atual: trabalha ou mais (para configurar seu tempo livre pessoal)</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Manager] com acesso a [!UICONTROL Editar Usuário] (para fazer alterações no calendário de folga de outros usuários)<br>
   <strong>OBSERVAÇÃO:</strong> se um gerente editar o calendário de folga pessoal de outro usuário, todas as entradas serão exibidas no fuso horário do usuário, e não no fuso horário do gerente.</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Configurar folga pessoal em [!DNL Workfront]

{{step1-click-profile-pic}}

1. No painel esquerdo, clique em **[!UICONTROL Folga]**.
1. Selecione a data desejada para sua folga pessoal.

   ![Calendário de folga pessoal](assets/personal-time-off-calendar.png)

1. Selecione **[!UICONTROL Todo o dia]**, se você estiver tirando um dia de folga.

   Deixe a caixa de seleção desmarcada se estiver tirando menos de um dia inteiro de folga e indique as horas de início e término de sua folga.

1. Clique em **[!UICONTROL Salvar]**.

   Sua folga agora está visível no sistema [!DNL Workfront] nas ferramentas de gerenciamento de recursos, como o Planejador de recursos e o Balanceador de carga de trabalho. Quando você recebe um trabalho durante esse período, uma dica de ferramenta informa ao usuário que você programou uma folga.
