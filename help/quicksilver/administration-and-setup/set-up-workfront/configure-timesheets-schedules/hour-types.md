---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Gerenciar Tipos de Hora
description: Você pode associar tipos de horas a suas entradas de horas. Os tipos de horas são rótulos usados para definir suas entradas de horas. Os tipos de horas podem ser para tempo geral ou para tempo específico do projeto.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '1127'
ht-degree: 1%

---

# Gerenciar tipos de horas

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>-->

Os tipos de horas são rótulos usados para definir suas entradas de horas. Você pode associar tipos de horas a suas entradas de horas.

Há duas categorias de tipos de horas:

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
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
       <p>[!UICONTROL Plano]</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de horas incorporadas

O Workfront vem com um conjunto de tipos de horas incorporados. Esses tipos de horas não podem ser editados ou ocultos.

Os tipos de horas que vêm com [!DNL Workfront] são:

* **[!UICONTROL Período de licença por doença]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. O período de licença por doença não pode ser contado como receita.
* **[!UICONTROL Férias]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. O período de férias não pode ser contado como receita.
* **[!UICONTROL Horas Gerais Gerais]**: um tipo de hora geral que não pode ser associado a entradas de hora em um projeto, tarefa ou problema. Pode contar como receita no processo de planejamento do projeto.
* **[!UICONTROL Hora do Projeto]**: um tipo de hora geral que só pode ser associado a entradas de hora em um projeto.
* **[!UICONTROL Horário da Tarefa]**: um tipo de hora geral que só pode ser associado a entradas de hora em uma tarefa.
* **[!UICONTROL Hora do Problema]**: um tipo de hora geral que só pode ser associado a entradas de hora em um problema.

## Criar tipos de horas

Como administrador do [!DNL Workfront], você pode criar tipos de horas para sua organização no nível do sistema e do projeto.

Após definir os tipos de horas no nível do sistema, os usuários podem definir quais tipos de horas estão disponíveis para projetos específicos ou para usuários específicos.

Para obter mais informações, consulte [Definir tipos de hora e disponibilidade](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para criar tipos de horas:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Folhas de horas e Horas** e em **Tipos de horas**.

1. Na seção **Tipos de Hora**, clique em **Novo Tipo de Hora**.
1. Na caixa de diálogo **Novos Tipos de Hora**, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Insira um nome de tipo de hora que seja facilmente reconhecível no sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Adicione uma descrição para o tipo de hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Escopo]</td> 
      <td> <p>Selecione se o tipo de hora é geral ou específico do projeto no menu suspenso <strong>Escopo</strong>.</p> <p>Os tipos de horas gerais são visíveis apenas em folhas de horas e não podem ser associados a projetos, tarefas ou problemas.</p> <p><b>IMPORTANTE</b></p><p> Se você tiver um Tipo de Hora personalizado que seja [!UICONTROL Específico do Projeto] e alterá-lo para [!UICONTROL Geral], todas as horas de Tarefa, Problemas e Projeto existentes serão definidas para seus tipos padrão do sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contar como Receita]</td> 
      <td><p>Selecione esta opção se quiser que a entrada de horas associada a este tipo de hora afete seus cálculos de receita.</p>
      <p>O Período de Doença e o Período de Férias não podem ser contados como receita.</p>
      <p><b>Nota</b></p>
      <p>Quando os tipos de hora gerais são contados como receita, a Taxa de custo associada ao perfil do usuário que registra o tempo é associada ao custo por hora.  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

   O tipo de hora é adicionado ao sistema do Workfront e é ativado por padrão.

## Editar tipos de horas

Como administrador do [!DNL Workfront], você pode editar os tipos de horas da sua organização no nível do sistema e do projeto.

>[!NOTE]
>
>* Não é possível editar tipos de horas predefinidos.
>* Não é possível editar tipos de horas em massa.

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Folhas de horas e Horas** e em **Tipos de horas**.

1. Clique no nome de um tipo de hora ou selecione o tipo de hora e clique no **ícone Editar** ![ícone Editar](assets/edit-icon.png) na parte superior da lista.
1. Na caixa de diálogo **Editar Tipos de Hora**, especifique as seguintes informações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome]</td> 
      <td>Insira um nome de tipo de hora que seja facilmente reconhecível no sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descrição]</td> 
      <td>Adicione uma descrição para o tipo de hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Escopo]</td> 
      <td> <p>Selecione se o tipo de hora é geral ou específico do projeto no menu suspenso <strong>Escopo</strong>.</p> <p>Os tipos de horas gerais são visíveis apenas em folhas de horas e não podem ser associados a projetos, tarefas ou problemas.</p> <p><b>IMPORTANTE</b></p> <p>Se você tiver um Tipo de Hora personalizado que seja [!UICONTROL Específico do Projeto] e alterá-lo para [!UICONTROL Geral], todas as horas de Tarefa, Problemas e Projeto existentes serão definidas para seus tipos padrão do sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contar como Receita]</td> 
      <td><p>Selecione esta opção se quiser que a entrada de horas associada a este tipo de hora afete seus cálculos de receita.</p>
      <p>O Período de Doença e o Período de Férias não podem ser contados como receita.</p>
      <p><b>Nota</b></p>
      <p>Quando os tipos de hora gerais são contados como receita, a Taxa de custo associada ao perfil do usuário que registra o tempo é associada ao custo por hora.  
      </td> 
     </tr> 
    </tbody> 
   </table>


1. Clique em **Salvar**.

   Suas alterações são salvas e o tipo de hora é editado.

## Desativar tipos de horas

Você pode desativar os tipos de horas se não quiser mais que os usuários associem suas horas a eles. A desativação de tipos de horas os oculta de qualquer lugar em [!DNL Workfront] onde os tipos de horas estejam visíveis.

>[!NOTE]
>
>* Não é possível desativar os tipos de horas predefinidos.
>* Você pode desativar tipos de horas em massa.
>* Quando você desativa um Tipo de Hora específico do projeto, todo o tempo registrado para esse tipo automaticamente usa como padrão um tipo de hora específico do projeto interno. Por exemplo, o tempo registrado para um projeto assume como padrão o tipo de hora Tempo do Projeto; o tempo registrado para uma tarefa assume como padrão o tipo de hora Tempo da Tarefa.
>* Quando você desativa um tipo de hora geral, o tempo registrado permanece na folha de horas, mas os usuários não podem mais registrar tempo para esse tipo de hora no futuro.



Para desativar um tipo de hora:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **[!UICONTROL Folhas de horas e Horas]** e em **[!UICONTROL Tipos de horas]**.

1. Selecione o tipo de hora que deseja desativar. Você pode selecionar vários tipos de horas.

1. Clique em **Mais** e depois em **Desativar**.

   ![Ativar e desativar links de tipo de hora](assets/activate-and-deactivate-hour-type-links.png)

   O tipo de hora é desativado e os usuários não podem mais encontrá-lo ao registrar horas.

1. (Opcional) Para reativar um tipo de hora, selecione-o na lista **Tipos de Hora** e clique em **Mais** > **Ativar**.

