---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gerenciar tipos de horas
description: Você pode associar tipos de horas a suas entradas de horas. Os tipos de horas são rótulos usados para definir suas entradas de horas.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: e881aa57b5175ce5b559180a2713de0c607b3b1d
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Gerenciar tipos de horas

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Você pode associar tipos de horas a suas entradas de horas. Os tipos de horas são rótulos usados para definir suas entradas de horas.

Há dois conjuntos de tipos de horas:

* **Tipos de Horas Específicas do Projeto**: Este é o tempo gasto em projetos, tarefas e problemas. Tipos de hora específicos do projeto podem ser associados a entradas de hora em qualquer lugar no [!DNL Adobe Workfront] onde você pode registrar horas para projetos, tarefas e problemas.

  Ao fazer logon no [!DNL Workfront], os tipos de horas específicos do projeto que estão disponíveis dependem das opções de configuração definidas nos níveis do sistema, do projeto e do usuário.

  Os seguintes tipos de horas específicos do projeto padrão estão sempre disponíveis:

   * Tempo em Projeto
   * Tempo de tarefa
   * Tempo do problema

  A variável [!DNL Workfront] O administrador determina quais tipos de horas específicas do projeto são disponibilizadas, conforme descrito em [Definir tipos de horas e disponibilidade para folhas de horas](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Se você habilitar quaisquer tipos de horas específicos do projeto em seu [!DNL Workfront] sistema, pelo menos um tipo de hora específico do projeto deve estar ativado em cada projeto em seu sistema. Você não pode ativar um tipo de hora específico do projeto no nível do sistema e não tem tipos de hora específicos do projeto disponíveis no nível do projeto.

* **Tipos de Hora Geral**: horas gerais não podem ser associadas a um projeto, tarefa ou problema, e estão conectadas diretamente em uma folha de horas. Para obter mais informações sobre o tempo de registro, consulte [Registrar tempo](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano do [!UICONTROL Adobe Workfront]</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de horas incorporadas

O Workfront vem com um conjunto de tipos de horas incorporados. Esses tipos de horas não podem ser editados e não podem ser ocultos.

Os tipos de hora que vêm com [!DNL Workfront] são:

* **[!UICONTROL Período de Doença]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. As horas de licença por doença não podem ser contadas como receita.
* **[!UICONTROL Férias]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. O período de férias não pode ser contado como receita.
* **[!UICONTROL Despesas Gerais]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. No entanto, pode contar como receita no processo de planejamento do projeto.
* **[!UICONTROL Tempo do Projeto]**: um tipo de hora geral que pode ser associado apenas a entradas de hora em um projeto.
* **[!UICONTROL Tempo em Tarefa]**: um tipo de hora geral que pode ser associado apenas a entradas de hora em uma tarefa.
* **[!UICONTROL Hora do Problema]**: um tipo de hora geral que pode ser associado apenas a entradas de hora em uma ocorrência.

## Criar tipos de horas

Como um [!DNL Workfront] administrador, você pode criar novos tipos de horas para sua organização nos níveis do sistema e do projeto. Depois de criar tipos de horas nos níveis de sistema e projeto, os usuários podem definir quais tipos de horas estão disponíveis para projetos e usuários específicos. Para obter mais informações, consulte [Definir tipos de horas e disponibilidade para folhas de horas](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para criar novos tipos de horas:

1. Clique em **[!UICONTROL Menu principal]** ícone ![](assets/main-menu-icon.png) no canto superior direito de [!DNL Adobe] Workfront e clique em **[!UICONTROL Configuração]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Horas e Planilha de Horas]** > **[!UICONTROL Tipos de Hora]**.

1. Clique em **[!UICONTROL Novo Tipo de Hora].**
1. Especifique as seguintes informações sobre o **[!UICONTROL Novo Tipo de Hora]** formulário:

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
      <td> <p>Defina se o tipo de hora é geral ou específico do projeto selecionando o escopo correto no menu suspenso.</p> <p>As horas do tipo geral são visíveis apenas em planilhas de horas e não podem ser associadas a projetos, tarefas ou problemas.</p> <p><b>IMPORTANTE</b>: Se você tiver um Tipo de Hora personalizado que seja [!UICONTROL Específico do Projeto], altere-o para [!UICONTROL Geral], todas as Horas de Tarefa, Problemas e Projeto existentes serão definidas para seus tipos padrão do sistema.</p> </td> 
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

   **[!UICONTROL Contar como Receita]**: selecione esta opção se quiser que a entrada de horas associada a este tipo de hora afete seus cálculos de receita.

1. Clique em **[!UICONTROL Criar Tipo de Hora].**

## Desativar tipos de horas

Se os tipos de horas se tornarem obsoletos e você não quiser mais que os usuários associem suas entradas de horas a eles, será possível desativar os tipos de horas.

A desativação de tipos de horas oculta os tipos de horas de qualquer lugar no [!DNL Workfront] onde os tipos de hora estão visíveis.

Para desativar um tipo de hora:

1. Clique em **[!UICONTROL Configuração]** próximo ao canto superior direito de [!DNL Adobe Workfront] na Barra de navegação global.

1. Expandir **[!UICONTROL Preferências de Horas e Planilha de Horas]** e, em seguida, clique em **[!UICONTROL Tipos de Hora]**.

1. Selecione o tipo de hora que deseja desativar.

1. Clique em **[!UICONTROL Desativar]**.
