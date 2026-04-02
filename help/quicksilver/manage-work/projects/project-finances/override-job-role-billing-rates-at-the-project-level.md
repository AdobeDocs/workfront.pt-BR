---
product-area: projects
navigation-topic: financials
title: Substituir Taxas de Cobrança de Função de Trabalho no Nível do Projeto
description: Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de trabalho em um projeto específico. Essa taxa de cobrança no nível do projeto substitui a taxa de cobrança no nível do sistema para essa função de trabalho. O Workfront usa a taxa de cobrança no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de cobrança no nível do sistema.
author: Lisa
feature: Work Management
exl-id: b7a33459-6929-4611-8546-06ca979e5dbe
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: b9e0747a58618353caf3ce1c7e8521d22d2b412d
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 6%

---

# Substituir as taxas de faturamento das funções de trabalho no nível do projeto

{{highlighted-preview}}

Como gerente de projeto, você pode especificar a taxa de faturamento de uma função de trabalho em um projeto específico. Essa taxa de cobrança no nível do projeto substitui a taxa de cobrança no nível do sistema para essa função de trabalho. O Workfront usa a taxa de cobrança no nível do projeto da função de trabalho para calcular a receita, em vez de usar a taxa de cobrança no nível do sistema.

Este artigo descreve como você pode substituir as taxas de faturamento de função de trabalho do sistema para um projeto.

Para obter informações gerais sobre substituição de taxas de cobrança de função de trabalho para projetos e cálculo de Receita do projeto, consulte [Visão geral da substituição de taxas de cobrança e cálculo de receita em um projeto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Para obter mais informações sobre qual função de trabalho é usada para calcular a receita do projeto, consulte a [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e a [seção Cálculos de receita para tarefas baseadas em atribuições de usuário e função](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) no artigo [Visão geral de faturamento e receita](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

>[!NOTE]
>
>No caso da receita real, as taxas de cobrança aplicadas a horas que são adicionadas a um registro de cobrança que está marcado como faturado não devem ser afetadas por sobreposições de taxa de cobrança que ocorrem após o registro de cobrança ter sido faturado.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td> <p>Para sobrepor uma taxa de faturamento de função de cargo para um projeto: Qualquer pacote do Workfront ou do Workflow</p>
        <p>Para aplicar atributos à função de trabalho: Ultimate do Workflow</p> </td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>
   <p>Padrão</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p> <p>Acesso administrativo para funções de trabalho</p></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto que inclui Editar Dados Financeiros </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Substituir as taxas de faturamento das funções de trabalho no nível do projeto

Quando você sobrepõe a taxa de faturamento de uma ordem de produção em um projeto, é possível atribuir datas de efetivação e cada faixa de datas tem uma taxa diferente. Se você não atribuir datas de efetivação, a sobreposição da taxa de faturamento informada será usada por toda a duração do projeto para calcular a receita.

Você pode adicionar novas taxas de faturamento a um modelo de projeto e elas se tornarão taxas de faturamento do projeto ao criar o projeto a partir desse modelo. Para obter informações sobre como editar modelos, consulte [Editar modelos de projeto](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md).

>[!TIP]
>
>Não é possível substituir taxas de faturamento do usuário para um projeto, a menos que você tenha o pacote Workflow Ultimate.

Para sobrepor uma taxa de faturamento para um projeto:

1. Vá para o projeto para o qual você deseja substituir as taxas de faturamento.
1. Clique em **Taxas de cobrança** no painel esquerdo.

   Ou

   <span class="preview">Clique em **Taxas** no painel esquerdo e clique na guia **Faturamento** se ela ainda não estiver selecionada.</span>

1. Clique em **Adicionar Taxa de Cobrança** > **Nova Taxa de Cobrança**.

   Ou

   <span class="preview">Clique em **Adicionar taxa de cobrança > Nova taxa de cobrança de função de trabalho**.</span>

   A caixa Nova taxa de cobrança é aberta.

1. No campo **Função de trabalho**, selecione a função de trabalho para a qual deseja alterar a taxa de cobrança.

1. <span class="preview">(Opcional) Selecione atributos para a taxa de cobrança, como agência ou local.</span>

   <span class="preview">O administrador do sistema define atributos de taxa na área Instalação.</span>

1. Selecione a **Moeda** para a substituição da taxa de cobrança.
1. No campo **Taxa de Cobrança**, insira a substituição de taxa de cobrança e clique em **Salvar** para substituir a taxa de cobrança uma vez

   Ou

   Clique em **Adicionar taxa** para adicionar mais substituições de taxa de cobrança.

1. (Condicional) Para sobreposições de taxa de faturamento de data de efetivação, especifique as seguintes informações para cada linha:

   * **Taxa de Cobrança**: o valor da Taxa de Cobrança desde o início do projeto até a primeira data da primeira substituição.
   * **Data de Início**: a data em que a substituição da taxa de cobrança começa.
   * **Data de Término**: a data em que termina a substituição da taxa de cobrança.

   ![Taxas de cobrança com datas de substituição](assets/new-job-role-billing-rate-on-project2.png)

   O Workfront aplica a taxa de substituição de função de trabalho às horas que ocorrem durante esses períodos ao calcular a receita do projeto.

   O Workfront permite que você deixe intervalos entre os períodos de substituição, mas você receberá um aviso para confirmar que isso é intencional.

   Você não precisa especificar uma Data Inicial para a primeira taxa de sobreposição, nem uma Data Final para a última taxa de sobreposição.

   Se você informar apenas uma sobreposição de taxa de faturamento, essa taxa será aplicada para toda a duração do projeto. Se você adicionar várias sobreposições de data de efetivação, o Workfront presume que a primeira sobreposição se aplica a todas as horas antes de sua Data Final e a última sobreposição se aplica a todas as horas após sua Data Inicial.

   O Workfront presume que a primeira taxa de sobreposição seja aplicada para todas as horas com uma data anterior à Data Final da primeira sobreposição e que a última taxa de sobreposição seja aplicada para todas as horas com uma data mais recente que a Data Inicial da última sobreposição.

   Se uma hora for registrada antes da Data de início planejada do projeto, a primeira taxa de cobrança será usada.

   Se uma hora for registrada depois da Data de conclusão planejada do projeto, a última taxa de cobrança será usada.

1. Clique em **Salvar**.
