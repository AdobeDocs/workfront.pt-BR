---
product-area: timesheets;setup
navigation-topic: configure-timesheet-preferences
title: Configurar se a hora é registrada em horas ou dias
description: Como usuário com uma licença do Plan, você pode configurar se deseja efetuar logon no Adobe Workfront em horas ou dias. Os administradores do sistema podem configurar essa configuração para usuários individuais ou para vários usuários em sua organização. Por padrão, os usuários registram o tempo em horas.
author: Alina
feature: Timesheets
exl-id: 4f801a13-182d-4e06-98ea-f6863f6a8edf
source-git-commit: b4ab350af22afa44774f06d82daf1c3fb266d2b9
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Configurar se a hora é registrada em horas ou dias

Como usuário com uma licença do Planejador, você pode configurar se deseja fazer logon no Adobe Workfront em horas ou dias. Os administradores do sistema podem configurar essa configuração para usuários individuais ou para vários usuários em sua organização. Por padrão, os usuários registram o tempo em horas. Para obter informações sobre como registrar o tempo no Workfront, consulte [Tempo de registro](../../timesheets/create-and-manage-timesheets/log-time.md).

>[!NOTE]
>
>Recomendamos registrar o tempo da mesma maneira, horas ou dias, em toda a organização para garantir a precisão dos relatórios.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Os planejadores podem configurar o tempo para si mesmos. Somente um administrador do Workfront pode configurar o tempo para outros usuários.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

1. Siga um destes procedimentos, dependendo do seu objetivo e do seu nível de acesso no sistema:

   * **O usuário do planejador configura o registro de tempo para você mesmo:** Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, clique no nome do usuário ao lado da imagem do perfil. Em seguida, clique no botão **Mais** ícone ao lado do seu nome e selecione **Editar**.

   * **Administrador do sistema configurando o registro de tempo para outros:** Comece a editar uma ou mais contas de usuário, conforme descrito em [Editar o perfil de um usuário](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. Na caixa de diálogo resultante, no **Planejamento de recursos** localize a **Tempo de logon** opção.

   ![](assets/new-timesheet-log-hours-350x249.png)

1. (Condicional) Se você for um administrador do sistema editando vários usuários simultaneamente, selecione **Tempo de logon**.
1. Selecione uma das seguintes opções para tempo de registro:

   | Opção | Descrição |
   |---|---|
   | **Horas** | Os usuários especificam horas ao registrar o tempo no Workfront. |
   | **Dias** | Os usuários especificam os dias ao registrar a hora no Workfront. |

1. (Condicional) Se você selecionou registrar o tempo em dias, na variável **Horas equivalentes para Workday completo** digite o número de horas que equivale a um dia inteiro. Um dia na folha de ponto de um usuário é o equivalente ao número de horas que você digita aqui.

   Leve em consideração o seguinte ao definir essa configuração:

   * Essa opção não está disponível ao configurar para registrar o tempo em horas.
   * Essa opção é usada somente para a finalidade de tempo de registro. Essa opção não está relacionada ao **Agendar** que também está disponível ao editar um usuário. O **Agendar** é usada para calcular linhas do tempo e em outras áreas do Workfront. (Para obter mais informações sobre como usar o **Agendar** consulte [Criar um agendamento](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).) 

1. Clique em **Salvar alterações**.
