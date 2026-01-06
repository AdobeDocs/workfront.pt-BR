---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Visão geral do tipo de atualização de projeto
description: O Tipo de atualização de um projeto indica como o Adobe Workfront calcula a linha do tempo de um projeto. As alterações no plano de projeto podem acionar alterações na linha do tempo do projeto. A linha do tempo do projeto deve ser recalculada automática ou manualmente para garantir que esteja atualizada com essas alterações.
author: Alina
feature: Work Management
exl-id: a6394961-2ac8-4b95-aa1b-dba8108c612f
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '515'
ht-degree: 0%

---

# Visão geral do Tipo de atualização de projeto

O Tipo de atualização de um projeto indica como o Adobe Workfront calcula a linha do tempo de um projeto. As alterações no plano de projeto podem acionar alterações na linha do tempo do projeto. A linha do tempo do projeto deve ser recalculada automática ou manualmente para garantir que esteja atualizada com essas alterações.

Para obter informações sobre como recalcular a linha de tempo do projeto, consulte [Recalcular linhas de tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

## Tipos de atualização de projeto

Há quatro Tipos de atualização para um projeto, dependendo de quando você deseja que o Workfront recalcule a linha do tempo do projeto. Escolha um Tipo de Atualização na lista abaixo.

Para obter informações sobre como atualizar o Tipo de Atualização do projeto, consulte [Selecionar o Tipo de Atualização do projeto](../../../manage-work/projects/manage-projects/select-project-update-type.md).

>[!IMPORTANT]
>
>Se a linha do tempo de um projeto tiver mais de 15 anos, a Workfront não calculará a linha do tempo automaticamente ou quando houver alteração. O tipo de atualização de um projeto com mais de 15 anos é sempre manual.

* **Automático e Mediante alteração:** Esta é a configuração padrão. A linha do tempo do projeto é atualizada sempre que ocorre uma alteração no projeto ou em outro projeto do qual a linha do tempo depende. A linha do tempo do projeto também é atualizada todas as noites.\
  Essa é a configuração recomendada, pois garante que a linha do tempo do projeto esteja sempre atualizada.

  Quando você atualiza uma tarefa ou o projeto e aciona um novo cálculo de linha do tempo, todas as datas disponíveis são exibidas imediatamente, permitindo que você continue trabalhando. Em projetos com mais de 100 tarefas, as datas que exigem cálculos mais longos ficam esmaecidas.

  ![](assets/dates-dimmed-when-insline-editing-350x146.png)

  Isso indica que o recálculo ainda não foi concluído e as datas estão sujeitas a alterações.

* **Alterar Somente:** A linha de tempo do projeto é atualizada sempre que ocorre uma alteração no projeto ou em outro projeto do qual a linha de tempo depende; não ocorrem atualizações agendadas.\
  Você pode selecionar essa opção se estiver preocupado com o desempenho do sistema e se alterações raramente ocorrerem no projeto ou em outros projetos dos quais a linha do tempo dependa.

* **Somente Automático:** A linha do tempo do projeto é atualizada todas as noites; ela não é atualizada imediatamente após as alterações serem feitas.\
  Você pode querer selecionar esta opção se estiver preocupado com o desempenho do sistema e se muitas alterações ocorrem a cada dia no projeto ou em outros projetos dos quais a linha do tempo depende.

  >[!NOTE]
  >
  >Um projeto não recalcula automaticamente todas as noites se estiver no status Planejamento. Ele só é recalculado quando há alteração.

* **Somente Manual:** A linha de tempo do projeto é atualizada somente quando você seleciona a opção **Recalcular Linhas de Tempo**, conforme descrito na seção &quot;Recálculo Manual&quot; do artigo [Recalcular linhas de tempo do projeto](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).\
  Você pode selecionar essa opção se estiver fazendo muitas alterações ao projeto de uma vez e quiser que o recálculo da linha do tempo ocorra após todas as alterações terem sido feitas (em vez de após cada alteração individual).
