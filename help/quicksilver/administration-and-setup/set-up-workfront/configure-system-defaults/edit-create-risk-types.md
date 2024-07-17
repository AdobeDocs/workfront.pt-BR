---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Editar e criar tipos de risco
description: Você pode adicionar riscos a um projeto na fase de planejamento para identificar possíveis obstáculos antes da aprovação de qualquer trabalho. Os riscos são eventos possíveis que podem impedir a conclusão do projeto no prazo ou dentro do orçamento.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f929806f-9087-4b64-be4b-70bbceaaeab0
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# Editar e criar tipos de risco

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Você pode adicionar riscos a um projeto na fase de planejamento para identificar possíveis obstáculos antes da aprovação de qualquer trabalho. Os riscos são eventos possíveis que podem impedir a conclusão do projeto no prazo ou dentro do orçamento.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>[!UICONTROL Plano]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront].</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de riscos

Os tipos de risco são rótulos que você pode usar para seus riscos a fim de categorizá-los para fins de relatório. Eles foram criados na área **[!UICONTROL Configuração]** pelo administrador [!DNL Adobe Workfront]. Depois que os tipos de risco forem estabelecidos na área **[!UICONTROL Configuração]**, eles se tornarão universais para o sistema. Todos os proprietários de projetos podem usar os mesmos tipos de risco para seus projetos.

## Editar e criar tipos de risco

Alguns tipos de risco já estão em [!DNL Workfront], por padrão. Para refletir as necessidades de sua organização, você pode editar os tipos de risco existentes ou criar novos tipos de risco.

* [Editar tipos de risco existentes](#edit-existing-risk-types)
* [Criar novos tipos de risco](#create-new-risk-types)

### Editar tipos de risco existentes {#edit-existing-risk-types}

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Tipos de Riscos]**.
1. Selecione o tipo de risco que deseja editar.
1. Clique em **[!UICONTROL Editar]**.
1. (Opcional) Altere o nome e a descrição do tipo de risco.

   Há um limite de 50 caracteres para os campos **[!UICONTROL Nome]** e **[!UICONTROL Descrição]**.

1. Clique em **[!UICONTROL Salvar alterações].**

### Criar novos tipos de risco {#create-new-risk-types}

Você pode criar novos tipos de risco, além dos tipos padrão, para refletir as necessidades da sua organização.

Para criar um novo tipo de risco:

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu Principal]** no canto superior direito de [!DNL Adobe Workfront] e em **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clique em **[!UICONTROL Tipos de Riscos]**.
1. Clique em **[!UICONTROL Novo Tipo de Risco]**.
1. Digite um **[!UICONTROL Nome]** (obrigatório) e uma **[!UICONTROL Descrição]** (opcional) para o tipo de risco.

   Há um limite de 50 caracteres para os campos **[!UICONTROL Nome]** e **[!UICONTROL Descrição]**.

1. Clique em **[!UICONTROL Criar Tipo de Risco]**. Se você usou edição em linha para adicionar seu tipo de risco, clique em **[!UICONTROL Inserir]** quando terminar.

   >[!NOTE]
   >
   >Se você precisar editar um tipo de risco personalizado, consulte a seção [[!UICONTROL Editar tipos de risco] existentes](#edit-existing-risk-types) neste artigo.

## Associar riscos com tipos de risco em projetos

Os tipos de riscos podem ser usados para rotular riscos que são adicionados aos seus projetos. Para obter mais informações sobre como adicionar riscos a projetos, consulte [Criar e editar riscos em projetos](../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md).
