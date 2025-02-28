---
product-area: projects
navigation-topic: financials
title: Substituir Taxas de Cobrança de Função de Trabalho no Nível do Projeto
description: Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de trabalho em um projeto específico. Essa taxa de cobrança no nível do projeto substitui a taxa de cobrança no nível do sistema para essa função de trabalho. O Workfront usa a taxa de cobrança no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de cobrança no nível do sistema.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 0%

---

# Substituir Taxas de Cobrança de Função de Trabalho no nível do projeto

Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de trabalho em um projeto específico. Essa taxa de cobrança no nível do projeto substitui a taxa de cobrança no nível do sistema para essa função de trabalho. O Workfront usa a taxa de cobrança no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de cobrança no nível do sistema.

Este artigo descreve como você pode substituir as taxas de faturamento de função de trabalho do sistema para um projeto.

Para obter informações gerais sobre substituição de taxas de cobrança de função de trabalho para projetos e cálculo de Receita do projeto, consulte [Visão geral da substituição de Taxas de cobrança de função de trabalho e cálculo de Receita em um projeto](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Para obter mais informações sobre qual função de trabalho é usada para calcular a receita do projeto, consulte a seção &quot;Understanding Revenue Calculations for Tasks Based on User and Role Assignments&quot; no artigo [Overview of Billing and Revenue](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>No caso da receita real, as taxas de cobrança aplicadas a horas que são adicionadas a um registro de cobrança que está marcado como faturado não devem ser afetadas por sobreposições de taxa de cobrança que ocorrem após o registro de cobrança ter sido faturado.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Acesso administrativo para funções de trabalho</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto que inclui Editar Dados Financeiros </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Substituir Taxas de Cobrança de Função de Trabalho no nível do projeto

Você pode sobrepor a taxa de faturamento de uma função de trabalho em um projeto das seguintes maneiras:

* Uma vez, selecionando uma nova taxa para a função de trabalho.\
  A nova taxa é usada para toda a duração do projeto, para calcular a receita.

* Várias vezes, selecionando várias novas taxas para intervalos de datas específicos.\
  Uma taxa diferente pode ser usada durante cada intervalo de datas especificado.

>[!TIP]
>
>Não é possível substituir as taxas de faturamento do usuário em um projeto.

Para sobrepor uma taxa de faturamento para um projeto:

1. Vá para o projeto para o qual você deseja substituir as taxas de faturamento.
1. Clique em **Taxas de cobrança** no painel esquerdo. Talvez seja necessário clicar primeiro em **Mostrar mais**.
1. Clique em **Adicionar Taxa de Cobrança** > **Nova Taxa de Cobrança**.

   A caixa Nova taxa de cobrança é aberta.

1. No campo **Função de trabalho**, selecione a função de trabalho para a qual deseja alterar a taxa de cobrança.

   ![Substituir taxa de cobrança no projeto](assets/override-billing-rate-on-project-nwe-350x310.png)

   O campo **Taxa de Cobrança Padrão** exibe a taxa no nível do sistema para esta função de trabalho.

1. No campo **Taxas de Cobrança 1**, insira a substituição de taxa de cobrança ocasional e clique em **Salvar** para substituir a taxa de cobrança uma vez

   Ou

   Clique em **Adicionar taxa** para adicionar mais substituições de taxa de cobrança.

1. (Condicional) Se você estiver adicionando mais de uma sobreposição de taxa de faturamento, especifique as seguintes informações:

   * **Taxas de Cobrança 1**: o valor da Taxa de Cobrança desde o início do projeto até a primeira data da primeira substituição. Normalmente, esse valor é igual ao **Taxa Padrão**.
   * **Data de Início**: esta é a data em que a Taxa Padrão termina.
   * **Data Final**: a data em que termina a nova substituição de taxa de cobrança.

   ![nova_taxa_de_cobrança_com_datas_de_ajuste.png](assets/new-billing-rate-with-adjustment-dates-350x266.png)

1. O fuso horário para as datas selecionadas é exibido na parte inferior da caixa Nova taxa de cobrança. Esse é o fuso horário associado à sua instância do Workfront, como mostrado na área Informações do cliente da Configuração. Para obter informações, consulte [Configurar informações básicas do sistema](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).
1. O Workfront aplica a taxa de substituição de função de trabalho às horas que ocorrem durante os períodos especificados ao calcular a receita do projeto.
1. Não deve haver lacunas entre os intervalos de tempo de duas taxas de substituição. A **Data de Início** de uma taxa de substituição deve ser o dia imediatamente após a **Data de Término** da data de substituição anterior.

1. Você não pode especificar uma Data Inicial para a primeira taxa de sobreposição, nem uma Data Final para a última taxa de sobreposição.\
   Recomendamos que você use a Taxa padrão para a primeira taxa de substituição.\
   O Workfront presume que a primeira taxa de sobreposição seja aplicada para todas as horas com uma data anterior à Data Final da primeira sobreposição e que a última taxa de sobreposição seja aplicada para todas as horas com uma data mais recente que a Data Inicial da última sobreposição.\
   Se uma hora for registrada antes da Data de início planejada do projeto, a primeira taxa de cobrança será usada.\
   Se uma hora for registrada depois da Data de conclusão planejada do projeto, a última taxa de cobrança será usada.

1. Clique em **Salvar**.
