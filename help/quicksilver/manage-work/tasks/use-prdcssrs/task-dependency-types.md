---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Visão geral dos tipos de dependência de tarefa
description: Os Tipos de dependência se referem às relações do antecessor entre tarefas. Eles definem quando a tarefa dependente pode iniciar ou terminar com base no início ou no término de seu antecessor.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '283'
ht-degree: 0%

---

# Visão geral dos tipos de dependência de tarefa

Os Tipos de dependência se referem às relações do antecessor entre tarefas. Eles definem quando a tarefa dependente pode iniciar ou terminar com base no início ou no término de seu antecessor.

>[!IMPORTANT]
>
>O Adobe Workfront não restringe o início ou a conclusão das tarefas dependentes com base nos tipos de dependência, a menos que os relacionamentos do antecessor sejam aplicados. Para obter informações sobre como impor predecessores, consulte [Impor predecessores](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Você deve especificar o Tipo de Dependência de uma relação antecessora ao estabelecer essa relação entre suas tarefas.

Para obter mais informações sobre predecessores, consulte [Visão geral dos antecessores de tarefas](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Estes são os Tipos de dependência do Workfront:

* **Finish-Start (fs)**: A tarefa predecessora deve ser concluída antes que a tarefa dependente possa ser iniciada. Esse é o tipo de dependência padrão, usado quando nenhum outro tipo de dependência é especificado.
* **Finish-Finish (ff)**: A tarefa predecessora deve ser concluída antes que a tarefa dependente possa ser concluída.
* **Início (ss)**: A tarefa predecessora deve ser iniciada antes que a tarefa dependente possa ser iniciada. Não é possível iniciar a tarefa dependente, a menos que o antecessor tenha pelo menos iniciado.
* **Início - Conclusão (sf)**: A tarefa predecessora deve ser iniciada antes que a tarefa dependente possa ser concluída. Você pode iniciar a tarefa dependente antes que o antecessor inicie, mas não poderá concluí-la a menos que o antecessor tenha iniciado.
* **Início agendado (sd)**: Isso agendará uma tarefa como Finish-Start, mas o tipo de imposição real é Finish-Finish. Ao usá-lo, a tarefa dependente é agendada para iniciar após a conclusão da tarefa antecessora. No entanto, a aplicação faz com que a tarefa dependente possa ser iniciada a qualquer momento, mas não possa ser concluída até que a tarefa antecessora seja concluída.
