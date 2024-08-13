---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gerenciar Tipos de Hora
description: Você pode associar tipos de horas a suas entradas de horas. Os tipos de horas são rótulos usados para definir suas entradas de horas.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 1%

---

# Gerenciar tipos de horas

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Você pode associar tipos de horas a suas entradas de horas. Os tipos de horas são rótulos usados para definir suas entradas de horas.

Há dois conjuntos de tipos de horas:

* **Tipos de Horas Específicas do Projeto**: Este é o tempo gasto em projetos, tarefas e problemas. Tipos de hora específicos do projeto podem ser associados a entradas de hora em qualquer lugar no [!DNL Adobe Workfront], onde você pode registrar horas para projetos, tarefas e problemas.

  Ao registrar horas em [!DNL Workfront], os tipos de horas específicos do projeto que estão disponíveis dependem das opções de configuração definidas nos níveis de sistema, projeto e usuário.

  Os seguintes tipos de horas específicos do projeto padrão estão sempre disponíveis:

   * Tempo em Projeto
   * Tempo de tarefa
   * Tempo do problema

  O administrador [!DNL Workfront] determina quais tipos de horas específicas do projeto são disponibilizadas, conforme descrito em [Definir tipos de horas e disponibilidade](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Se você habilitar qualquer tipo de hora específico de projeto no sistema [!DNL Workfront], pelo menos um tipo de hora específico de projeto deve ser habilitado em cada projeto no sistema. Você não pode ativar um tipo de hora específico do projeto no nível do sistema e não tem tipos de hora específicos do projeto disponíveis no nível do projeto.

* **Tipos de Horas Gerais**: as horas gerais não podem ser associadas a um projeto, tarefa ou problema, e estão registradas diretamente em uma folha de horas.

Para obter informações sobre como registrar horas e associá-las a tipos de horas, consulte [Registrar tempo](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano do [!UICONTROL Adobe Workfront]</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>Novo: [!UICONTROL Padrão]</p>
   <p>Atual: [!UICONTROL Plano]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront].</p> <p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de horas incorporadas

O Workfront vem com um conjunto de tipos de horas incorporados. Esses tipos de horas não podem ser editados e não podem ser ocultos.

Os tipos de horas que vêm com [!DNL Workfront] são:

* **[!UICONTROL Período de licença]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. As horas de licença por doença não podem ser contadas como receita.
* **[!UICONTROL Férias]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. O período de férias não pode ser contado como receita.
* **[!UICONTROL Sobrecarga Geral]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. No entanto, pode contar como receita no processo de planejamento do projeto.
* **[!UICONTROL Hora do Projeto]**: um tipo de hora geral que pode ser associado apenas a entradas de hora em um projeto.
* **[!UICONTROL Horário da Tarefa]**: um tipo de hora geral que pode ser associado apenas a entradas de hora em uma tarefa.
* **[!UICONTROL Hora do Problema]**:Um tipo de hora geral que pode ser associado apenas a entradas de hora em um problema.

## Criar tipos de horas

Como administrador do [!DNL Workfront], você pode criar novos tipos de horas para sua organização nos níveis do sistema e do projeto. Depois de criar tipos de horas nos níveis de sistema e projeto, os usuários podem definir quais tipos de horas estão disponíveis para projetos e usuários específicos. Para obter mais informações, consulte [Definir tipos de hora e disponibilidade](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para criar novos tipos de horas:

{{step-1-to-setup}}

1. Clique em **[!UICONTROL Planilha de horas e horas]** > **[!UICONTROL Tipos de horas]**.

1. Clique em **[!UICONTROL Novo Tipo de Hora].**
1. Especifique as seguintes informações no formulário **[!UICONTROL Novo Tipo de Hora]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Dê ao novo tipo de hora um nome que seja facilmente reconhecível no sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Adicione uma descrição para o tipo de hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Escopo]</td> 
      <td> <p>Defina se o tipo de hora é geral ou específico do projeto selecionando o escopo correto no menu suspenso.</p> <p>As horas do tipo geral são visíveis apenas em planilhas de horas e não podem ser associadas a projetos, tarefas ou problemas.</p> <p><b>IMPORTANTE</b>: se você tiver um Tipo de Hora personalizado [!UICONTROL Específico do Projeto], altere-o para [!UICONTROL Geral], todas as horas existentes de Tarefa, Problemas e Projeto serão definidas para seus tipos padrão do sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contar como Receita]</td> 
      <td><p>Selecione esta opção se quiser que a entrada de horas associada a este tipo de hora afete seus cálculos de receita.</p>
      <p>O período de licença por doença e o período de férias não podem ser contados como receita.</p>
      <p><b>Nota</b></p>
      <p>Quando os tipos de hora gerais são contados como receita, a Taxa de custo associada ao perfil do usuário que registra o tempo é associada ao custo por hora.  
      </td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Contar como Receita]**: selecione essa opção se desejar que a entrada de hora associada a esse tipo de hora afete seus cálculos de receita.

1. Clique em **[!UICONTROL Criar Tipo de Hora].**

## Desativar tipos de horas

Se os tipos de horas se tornarem obsoletos e você não quiser mais que os usuários associem suas entradas de horas a eles, será possível desativar os tipos de horas.

A desativação de tipos de horas oculta os tipos de horas de qualquer lugar no [!DNL Workfront] em que os tipos de horas estejam visíveis.

Para desativar um tipo de hora:

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Preferências de Horas e Planilha de Horas]** e clique em **[!UICONTROL Tipos de Horas]**.

1. Selecione o tipo de hora que deseja desativar.

1. Clique em **[!UICONTROL Desativar]**.
