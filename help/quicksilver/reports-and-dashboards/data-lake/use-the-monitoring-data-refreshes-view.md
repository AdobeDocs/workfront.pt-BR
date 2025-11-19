---
product-area: reports and dashboards
navigation-topic: data-connect
title: Usar a exibição Monitoramento de atualizações de dados na Conexão de dados
description: Com o Data Connect, os administradores do Workfront podem acessar registros detalhados das atualizações recentes feitas na data do data lake durante a atualização mais recente.
author: Jenny
feature: Reports and Dashboards
source-git-commit: 1bcb64fbcdf2cb8b40cb50e5a7d4f5768f3a712f
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 2%

---

# Usar a exibição Monitoramento de atualizações de dados na Conexão de dados

A visualização Monitoramento de atualizações de dados exibe as atualizações recentes feitas na data do data lake durante a atualização mais recente. Os dados dessa visualização são atualizados após cada conclusão bem-sucedida de um carregamento de dados.

Devido ao alto volume de dados e à complexidade das agregações, a visualização Atualizações de dados de monitoramento exibe somente as visualizações de objeto que foram atualizadas nas últimas duas semanas. Se um tipo de registro específico estiver ausente nessa exibição, é provável que seja devido a uma falta de atividade nesse período.

>[!NOTE]
>
>Essa exibição mostra uma coleta detalhada dos dados fornecidos pelo aplicativo e as atividades de atualização em vez de uma exibição de evento ou histórico diário que mostra o histórico de atividades de atualização. Para obter detalhes históricos da atividade de atualização, você pode utilizar o <code>DL_LOAD_TIMESTAMP</code> objeto de data.

## Monitorando colunas de view de Atualizações de Dados

As colunas de view Atualizações de Dados de Monitoramento contêm as seguintes informações:

<table>
    <tr>
        <td><b>Nome da coluna</b></td>
        <td><b>Tipo</b></td>
        <td><b>Descrição</b></td>
    </tr>
    <tr>
        <td>OBJ_TYPE</td>
        <td>Varchar
        </td>
        <td> 
      O tipo de objeto associado aos registros do Workfront enviados para o data lake. 
        </ul></td>
    </tr>
    <tr>
        <td>DATA_CALENDÁRIO </td>
        <td>Data</td>
        <td>
   A data da última atualização de dados bem-sucedida para o tipo de objeto exibido na coluna OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>RECORD_LOAD_TIMESTAMP </td>
        <td>Carimbo de data/hora_NTZ</td>
        <td>
 A data e o horário da atualização de dados mais recente para o tipo de objeto exibido na coluna OBJ_TYPE.  </td>
    </tr>
        <tr>
        <td>PREVIOUS_RECORD_LOAD_TIMESTAMP </td>
        <td>Carimbo de data/hora_NTZ </td>
        <td>
       A data e o horário da segunda atualização de dados mais recente para o tipo de objeto exibido na coluna OBJ_TYPE. </td>
    </tr>
        <tr>
        <td>MINUTES_SINCE_PREVIOUS_LOAD </td>
        <td>Número</td>
        <td>
     O tempo em minutos decorrido desde a última atualização de dados para o tipo de objeto. </td>
    </tr>
            <tr>
        <td>CRIADO </td>
        <td>Número </td>
        <td>Uma contagem dos eventos CREATE record capturados entre as atualizações de dados anteriores e mais recentes para o tipo de objeto.  </td>
    </tr>
                <tr>
        <td>ATUALIZADO</td>
        <td>Número </td>
        <td>Uma contagem dos eventos de registro UPDATE capturados entre as atualizações de dados anteriores e mais recentes para o tipo de objeto.</td>
    </tr>
                <tr>
        <td>EXCLUÍDO</td>
        <td>Número </td>
        <td>Uma contagem dos eventos de registro do DELETE capturados entre as atualizações de dados anteriores e mais recentes para o tipo de objeto. </td>
    </tr>
                <tr>
        <td>Total</td>
        <td>Número </td>
        <td>Uma contagem do número total de eventos entre as atualizações de dados anteriores e mais recentes para o tipo de objeto. 
        <br> 
        <br><b>Observação</b>: não é o mesmo que o número total de registros afetados pelos eventos CREATE, UPDATE ou DELETE, pois o mesmo registro pôde ser CREATED e UPDATED várias vezes no intervalo entre as atualizações.  </td>
    </tr>
   </table>

