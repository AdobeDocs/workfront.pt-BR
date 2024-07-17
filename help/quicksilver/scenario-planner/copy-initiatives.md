---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Copiar iniciativas no Planejador de cenários
description: É possível criar iniciativas copiando as existentes. Você pode copiar iniciativas em um plano que criar ou em um plano que alguém compartilhar com você.
author: Alina
feature: Workfront Scenario Planner
exl-id: 0aadb074-69c3-4229-a01a-7cabdb87e7cb
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 0%

---

# Copiar iniciativas no [!DNL Scenario Planner]

É possível criar iniciativas copiando as existentes. Você pode copiar iniciativas em um plano que criar ou em um plano que alguém compartilhar com você.

## Requisitos de acesso

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plano*</b> </p> </td> 
   <td>[!UICONTROL Business] ou superior</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licença</b>*</p> </td> 
   <td> <p>[!UICONTROL Review] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produto</b> </td> 
   <td> <p>Você deve comprar uma licença adicional para o [!DNL Adobe Workfront Scenario Planner] acessar a funcionalidade descrita neste artigo.</p> <p>Para obter informações sobre como obter o [!DNL Workfront Scenario Planner], consulte <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Acesso necessário para usar o [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Configurações de nível de acesso*</strong> </td> 
   <td> <p>[!UICONTROL Editar] acesso ou superior à [!DNL Scenario Planner]</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode alterar seu nível de acesso, consulte <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Permissões de objeto</strong> </p> </td> 
   <td> <p>[!UICONTROL Gerenciar] permissões para um plano</p> <p>Para obter informações sobre como solicitar acesso adicional a um plano, consulte <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Solicitar acesso a um plano no [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Copiar iniciativas

Considere o seguinte ao copiar iniciativas:

* Copiar uma iniciativa coloca a cópia no mesmo plano da iniciativa original.
* Copiar uma iniciativa copia e adiciona as seguintes informações da iniciativa original à nova iniciativa:

   * [!UICONTROL Duração]
   * [!UICONTROL Funções de trabalho]
   * [!UICONTROL Pessoas] e [!UICONTROL Custos Fixos]
   * [!UICONTROL Benefício Planejado]

* Copiar uma iniciativa pode modificar as seguintes informações do plano, se as informações existirem na iniciativa original:

   * Quantidade necessária de funções de trabalho
   * [!UICONTROL Custos]
   * [!UICONTROL Utilização do Plano]
   * Utilização da função de trabalho
   * [!UICONTROL Valor Líquido]

* Copiar uma iniciativa que foi criada ao importar um projeto ou que foi publicada em um projeto pelo menos uma vez tem as seguintes implicações:

   * Não duplica o projeto associado à iniciativa.
   * Ela não conecta a iniciativa copiada ao projeto.
   * Ela não modifica a seção [!DNL Scenario Planner] no projeto para projetos que foram publicados pelo menos uma vez.

  Para obter informações sobre como publicar iniciativas em projetos, consulte [Atualizar ou criar projetos publicando iniciativas em [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

  Para obter informações sobre como criar iniciativas importando projetos, consulte [Importar projetos para planos na [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

## Copiar iniciativas

1. Clique no ícone ![](assets/main-menu-icon.png) do **[!UICONTROL Menu principal]** e em [!UICONTROL Cenários].

   Uma lista de planos é exibida.

1. Clique no nome de um plano para abri-lo e localize as iniciativas que deseja copiar.
1. Selecione a caixa à esquerda da iniciativa ou iniciativas que deseja copiar e clique em **[!UICONTROL Copiar]** no menu exibido na parte inferior do plano.

   ![](assets/bottom-manage-initiative-menu-350x45.png)

   [!DNL Workfront] copia as iniciativas imediatamente e as coloca abaixo da última iniciativa selecionada.

   O nome da iniciativa copiada é *[!UICONTROL Cópia de]`<Name of original initiative>`*.

   >[!NOTE]
   >
   >Dependendo de onde você inserir as novas iniciativas, os números de iniciativas existentes podem mudar.

1. Atualize o nome da iniciativa copiada.

   >[!TIP]
   >
   >Recomendamos que você sempre atualize o nome da iniciativa para evitar confusão caso deseje copiá-las novamente.

1. (Opcional) Atualize a prioridade de suas iniciativas recém-criadas.

   Para obter informações sobre como priorizar iniciativas, consulte [Atualizar prioridades de iniciativa no [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Clique em **[!UICONTROL Salvar Plano]** para salvar suas alterações.
