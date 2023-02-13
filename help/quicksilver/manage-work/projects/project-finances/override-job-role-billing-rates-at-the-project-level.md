---
product-area: projects
navigation-topic: financials
title: Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto
description: Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de cargo em um projeto específico. Essa taxa de faturamento no nível do projeto substitui a taxa de faturamento no nível do sistema para essa função de trabalho. O Workfront usa a taxa de faturamento no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de faturamento no nível do sistema.
author: Alina
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 0%

---

# Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto

Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de cargo em um projeto específico. Essa taxa de faturamento no nível do projeto substitui a taxa de faturamento no nível do sistema para essa função de trabalho. O Workfront usa a taxa de faturamento no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de faturamento no nível do sistema.

Este artigo descreve como você pode substituir as taxas de faturamento da função de trabalho do sistema para um projeto.

Para obter informações gerais sobre a sobreposição das taxas de faturamento da função de cargo para projetos e calcular a Receita do projeto, consulte [Visão Geral das Taxas de Faturamento da Função do Trabalho e cálculo da Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Para obter mais informações sobre qual função de cargo é usada para calcular a receita no projeto, consulte a seção &quot;Como entender cálculos de receita para tarefas com base em atribuições de usuário e função&quot; no artigo [Visão Geral da Faturamento e Receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>No caso da Receita Real, as taxas de faturamento aplicadas às horas adicionadas a um Registro de Faturamento que está marcado como Faturado não devem ser afetadas pelas substituições da taxa de faturamento que ocorrem após o Registro de Faturamento ter sido faturado.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Acesso administrativo para funções de Tarefa</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerencie permissões do projeto que inclui Editar dados financeiros </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Substituir as Taxas de Faturamento da Função de Trabalho no nível do projeto

Você pode substituir a taxa de faturamento de uma função de cargo em um projeto das seguintes maneiras:

* Uma vez, selecionando uma nova taxa para a função de trabalho.\
   A nova taxa é usada para calcular a receita por toda a duração do projeto.

* Várias vezes, selecionando várias novas taxas para intervalos de datas específicos.\
   Uma taxa diferente pode ser usada durante cada intervalo de datas especificado.

>[!TIP]
>
>Não é possível substituir as taxas de faturamento do usuário de um projeto.

Para substituir uma taxa de faturamento de um projeto:

1. Vá para o projeto para o qual deseja substituir as taxas de faturamento.
1. Clique em **Taxas de Faturamento** no painel esquerdo. Talvez seja necessário clicar primeiro **Mostrar mais**.
1. Clique em **Adicionar Taxa de Faturamento** > **Nova Taxa de Faturamento**.

   A caixa Nova Taxa de Faturamento é aberta.

1. No **Função da Tarefa** selecione a função de cargo para a qual deseja alterar a taxa de faturamento.

   ![](assets/override-billing-rate-on-project-nwe-350x310.png)

   O **Taxa de Faturamento Padrão** exibe a taxa de nível do sistema para essa função de trabalho.

1. No **Taxas de Faturamento 1** , insira a substituição de taxa de faturamento única e clique em **Salvar** para substituir a taxa de faturamento uma vez

   Ou

   Clique em **Taxa de adição** para adicionar mais substituições da taxa de faturamento.

1. (Condicional) Se estiver adicionando mais de uma substituição de taxa de faturamento, especifique as seguintes informações:

   * **Taxas de Faturamento 1**: o valor da Taxa de Faturamento desde o início do projeto até a primeira data da primeira substituição. Normalmente, é a mesma quantidade da variável **Taxa padrão**.
   * **Data inicial**: essa é a data em que a Taxa padrão termina.
   * **Data final**: a data em que a nova substituição da taxa de faturamento termina.

   ![new_billing_rate_with_adapt_dates.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. O fuso horário das datas selecionadas é exibido na parte inferior da caixa Nova Taxa de Faturamento . Esse é o fuso horário associado à sua instância do Workfront, como mostrado na área Informações do cliente da Configuração. Para obter mais informações, consulte [Configurar informações básicas para seu sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. O Workfront aplica a taxa de função de tarefa de substituição às horas que ocorrem durante os períodos especificados ao calcular a receita no projeto.
1. Não deve haver intervalos entre os intervalos de tempo de duas taxas de sobreposição. O **Data inicial** de uma taxa de sobreposição deve ser o dia imediatamente seguinte ao **Data final** da data de substituição anterior.

1. Não é possível especificar uma Data Inicial para a primeira taxa de sobreposição, nem uma Data Final para a última taxa de sobreposição.\
   Recomendamos que você use a Taxa padrão para a primeira taxa de substituição.\
   A Workfront parte do princípio que a primeira taxa de substituição é aplicada para todas as horas com uma data anterior à Data final da primeira substituição e que a última taxa de substituição é aplicada para todas as horas com uma data posterior à Data inicial da última substituição.\
   Se uma hora for registrada antes da Data de início planejada do projeto, a primeira taxa de faturamento será usada.\
   Se uma hora for registrada após a Data de conclusão planejada do projeto, a última taxa de faturamento será usada.

1. Clique em **Salvar**.
