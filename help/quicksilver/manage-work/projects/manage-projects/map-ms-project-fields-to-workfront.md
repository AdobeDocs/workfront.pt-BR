---
product-area: projects
navigation-topic: manage-projects
title: Mapear campos de projeto do Microsoft para projetos do Adobe Workfront
description: Os projetos no Adobe Workfront e no Microsoft Project são em sua maioria compatíveis. Este artigo descreve como os campos de projeto mais comuns dos dois aplicativos são mapeados entre si.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: c566eb094e96abca6073554433434822c567bc34
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 3%

---

# Mapear campos de projeto do Microsoft para projetos do Adobe Workfront

Os projetos no Adobe Workfront e no Microsoft Project são em sua maioria compatíveis. Usando os dois aplicativos, você pode fazer o seguinte:

* Exportar projetos do Microsoft Project e importá-los para o Workfront
* Exportar projetos do Workfront e importá-los para o Microsoft Project. 

Para obter mais informações sobre como importar projetos do Microsoft Project para o Workfront, consulte [Importar um projeto do Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Para obter mais informações sobre como exportar um projeto do Workfront para importá-lo para o Microsoft Project, consulte [Exportar um projeto para o Projeto Microsoft](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Ao executar essas importações de dados, é importante entender como as informações são traduzidas de um aplicativo para outro. Na maioria das vezes, você terá que fazer algumas modificações manuais no projeto depois de concluir a importação. 

## Visão geral do mapeamento de campo

>[!NOTE]
>
>As datas previstas nem sempre correspondem a ambos os sistemas. As discrepâncias podem ser contabilizadas por meio de programação e diferenças nas preferências do sistema entre o Workfront e o Microsoft Project. Essas discrepâncias de datas também podem resultar em diferenças no esforço, duração e porcentagem concluída.

| **Campo de projeto do Microsoft** | **Campo Workfront** |
|---|---|
| Título do projeto | Nome do Projeto |
| Datas de início e término | Datas de Início e Conclusão Planejadas |
| Nome da tarefa | Nome da tarefa |
| Duração da tarefa | Duração planejada da tarefa |
| Trabalho da Tarefa | Horas Planejadas da Tarefa |
| % de Tarefa Concluída | % de Tarefa Concluída (com base na Duração da tarefa) |
| % de Trabalho da Tarefa Concluída | % de Tarefa Concluída (com base nas Horas Planejadas da tarefa) |
| Início e término agendados | Datas de Início e Conclusão Planejadas |
| Início e término reais | Datas de início e conclusão reais |
| Nome do recurso | Atribuição de tarefa |
| Unidades de Atribuição | Porcentagem de Alocação |
| Nota de Tarefa | Descrição da tarefa |
| Predecessor | Predecessor |

## Visão geral dos dados não incluídos

Há vários campos de projeto que não são importados ou exportados do Workfront.

Esses campos incluem, entre outros, os seguintes:

* Anexos do documento
* Campos personalizados (nos níveis de projeto ou tarefa)
* Notas da Workfront
* Problemas
* Atraso negativo em tarefas com uma relação de antecessor Start/Finish (as tarefas são importadas sem o atraso)
* Atribuições
* Restrições de tarefa

   >[!NOTE]
   Como as Restrições não mapeiam entre o Microsoft Project e o Workfront, verifique se há relações entre os antecessores das tarefas. Caso contrário, as Datas de início e conclusão planejada das tarefas podem não ser precisas no projeto importado. 
