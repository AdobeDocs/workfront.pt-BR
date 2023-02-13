---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral do Tipo de atualização do projeto
description: O Tipo de atualização de um projeto indica como o Adobe Workfront calcula a linha do tempo de um projeto. As alterações no plano do projeto podem desencadear alterações na linha do tempo do projeto. A linha do tempo do projeto deve ser recalculada automática ou manualmente para garantir que esteja atualizada com essas alterações.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# Visão geral do Tipo de atualização do projeto

O Tipo de atualização de um projeto indica como o Adobe Workfront calcula a linha do tempo de um projeto. As alterações no plano do projeto podem desencadear alterações na linha do tempo do projeto. A linha do tempo do projeto deve ser recalculada automática ou manualmente para garantir que esteja atualizada com essas alterações.

Para obter informações sobre como recalcular a linha do tempo do projeto, consulte [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Tipos de atualização do projeto

Existem quatro tipos de atualização para um projeto, dependendo de quando você deseja que o Workfront recalcule a linha do tempo do projeto. Escolha um Tipo de atualização na lista abaixo.

Para obter informações sobre como atualizar o Tipo de atualização do projeto, consulte [Selecione o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Se a linha do tempo de um projeto for superior a 15 anos, a Workfront não calculará a linha do tempo automaticamente ou após a alteração. O Tipo de atualização de um projeto com mais de 15 anos é sempre Manual.

* **Automático e On Change:** Esta é a configuração padrão. A linha do tempo do projeto é atualizada sempre que uma alteração ocorre no projeto ou em outro projeto do qual a linha do tempo depende. A linha do tempo do projeto também é atualizada todas as noites. \
   Essa é a configuração recomendada, pois garante que a linha do tempo do projeto esteja sempre atualizada.

   Quando você atualiza uma tarefa ou o projeto e aciona um recálculo de linha do tempo, todas as datas disponíveis são exibidas imediatamente, permitindo que você continue trabalhando. Em projetos com mais de 100 tarefas, as datas que exigem cálculos mais longos são esmaecidas.

   ![](assets/dates-dimmed-when-insline-editing-350x146.png)

   Isso indica que o recálculo ainda não foi concluído e que as datas estão sujeitas a alterações.

* **Somente alteração:** A linha do tempo do projeto é atualizada sempre que ocorre uma alteração no projeto ou em outro projeto dependente da linha do tempo; atualizações programadas não ocorrem.\
   Você pode selecionar essa opção se estiver preocupado com o desempenho do sistema e se ocorrerem alterações raramente no projeto ou em outros projetos dependentes da linha do tempo.

* **Somente Automático:** O calendário do projeto é atualizado todas as noites; ela não é atualizada imediatamente após a realização de alterações.\
   Você pode selecionar essa opção se estiver preocupado com o desempenho do sistema e se muitas alterações ocorrerem todos os dias no projeto ou em outros projetos dependentes da linha do tempo.

   >[!NOTE]
   >
   >Um projeto não recalcula automaticamente a cada noite se estiver no status de Planejamento. Ele só recalcula quando alterado.

* **Somente Manual:** A linha do tempo do projeto é atualizada somente quando você seleciona a opção para **Recalcular Linhas do Tempo**, conforme descrito na seção &quot;Recálculo manual&quot; do artigo [Recalcular linhas do tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
   Talvez você queira selecionar essa opção se estiver fazendo muitas alterações no projeto de uma vez e desejar que o recálculo da linha do tempo ocorra após todas as alterações terem sido feitas (em vez de após cada alteração individual).
