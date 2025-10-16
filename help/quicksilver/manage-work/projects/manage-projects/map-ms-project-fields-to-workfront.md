---
product-area: projects
navigation-topic: manage-projects
title: Mapear campos de projeto do Microsoft para projetos do Adobe Workfront
description: Os projetos do Adobe Workfront e do Microsoft Project são em sua maioria compatíveis. Este artigo descreve como os campos de projeto mais comuns dos dois aplicativos são mapeados entre si.
author: Alina
feature: Work Management
exl-id: 381eb6ad-8084-406b-90f9-44460b58a04c
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 4%

---

# Mapear campos de projeto do Microsoft para projetos do Adobe Workfront

Os projetos do Adobe Workfront e do Microsoft Project são em sua maioria compatíveis. Usando os dois aplicativos, você pode fazer o seguinte:

* Exportar projetos do Microsoft Project e importá-los para o Workfront
* Exportar projetos do Workfront e importá-los para o Microsoft Project. 

Para obter mais informações sobre como importar projetos do Microsoft Project no Workfront, consulte [Importar um projeto do Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md).

Para obter mais informações sobre como exportar um projeto do Workfront para importá-lo para o Microsoft Project, consulte [Exportar um projeto para o Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md).

Ao executar essas importações de dados, é importante entender como as informações são traduzidas de um aplicativo para outro. Na maioria das vezes, será necessário fazer algumas modificações manuais no projeto após concluir a importação. 

## Visão geral do mapeamento de campos

>[!NOTE]
>
>As datas planejadas nem sempre correspondem entre os dois sistemas. As discrepâncias podem ser contabilizadas por meio do agendamento e de diferenças nas preferências do sistema entre o Workfront e o Microsoft Project. Essas discrepâncias de datas também podem resultar em diferenças no esforço, na duração e no percentual concluído.

| **Campo de projeto do Microsoft** | **Campo do Workfront** |
|---|---|
| Título do projeto | Nome do Projeto |
| Datas de início e término | Datas de Início e Término Planejadas |
| Nome da tarefa | Nome da tarefa |
| Duração da tarefa | Duração planejada da tarefa |
| Trabalho da tarefa | Horas planejadas da tarefa |
| % Concluída da Tarefa | % Concluída da Tarefa (com base na Duração da tarefa) |
| % Concluída do Trabalho da Tarefa | % Concluída da Tarefa (com base nas Horas Planejadas da tarefa) |
| Início e Término Agendados | Datas de Início e Término Planejadas |
| Início e Término Reais | Datas de Início Efetivo e Término |
| Nome do recurso | Atribuição de tarefa |
| Unidades de atribuição | Porcentagem de Alocação de Atribuição |
| Nota de Tarefa | Descrição da tarefa |
| Predecessor | Predecessor |

## Visão geral dos dados que não estão incluídos

Há vários campos de projeto que não são importados para ou exportados do Workfront.

Esses campos incluem, mas não estão limitados ao seguinte:

* Anexos de documento
* Campos personalizados (nos níveis de projeto ou tarefa)
* Observações do Workfront
* Problemas
* Atraso negativo nas tarefas com um relacionamento de predecessor de Início/ Término (as tarefas são importadas sem o atraso)
* Atribuições
* Restrições de Tarefa

  >[!NOTE]
  >
  >Como as Restrições não são mapeadas entre o Microsoft Project e o Workfront, verifique se há relações predecessoras entre as tarefas. Caso contrário, as Datas de início planejadas e de conclusão planejada das tarefas podem não ser precisas no projeto importado. 
