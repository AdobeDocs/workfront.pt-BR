---
content-type: overview
product-area: projects
navigation-topic: financials
title: Sobrepor Taxas de Cobrança do Usuário no Nível do Projeto
description: Este artigo descreve como você pode sobrepor as taxas de faturamento do usuário do sistema para um projeto.
author: Lisa
feature: Work Management
source-git-commit: 8f6f14d4b36a9eee499111b1a37912f641c9f2ba
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 4%

---

# Substituir taxas de cobrança do usuário no nível do projeto

{{highlighted-preview-article-level}}

Como um gerente de projeto, você pode especificar a taxa de faturamento de um usuário em um projeto específico. Essa taxa de cobrança no nível do projeto substitui a taxa de cobrança no nível do sistema para esse usuário. O Workfront usa a taxa de cobrança no nível do projeto do usuário para calcular a receita, em vez de usar a taxa de cobrança no nível do sistema.

Este artigo descreve como você pode sobrepor as taxas de faturamento do usuário do sistema para um projeto.

Para obter informações gerais sobre substituição de taxas de cobrança para projetos e cálculo de receita do projeto, consulte [Visão geral da substituição de taxas de cobrança e cálculo de receita em um projeto](/help/quicksilver/manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

Para obter mais informações sobre como calcular a receita no projeto, consulte a [Visão geral da hierarquia de receita e custo](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md) e a [seção Cálculos de receita para tarefas baseadas em atribuições de usuário e função](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md#revenue-calculations-for-tasks-based-on-user-and-role-assignments) no artigo [Visão geral de faturamento e receita](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

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
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td>Padrão</td> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a Projetos e Dados Financeiros</p>
       <p><p>Você também deve ter um dos seguintes:</p> 
        <ul> 
          <li> <p>O nível de acesso Administrador do sistema. </li> 
          <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se <b>Administrador de Usuários (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul></td> 
  </tr> 
  <tr> 
   <td>Permissões de objeto</td> 
   <td>Gerenciar permissões para o projeto que inclui Editar Dados Financeiros </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Sobrepor Taxas de Cobrança do Usuário no nível do projeto

Quando você sobrepõe a taxa de faturamento de um usuário em um projeto, é possível atribuir datas de efetivação e cada faixa de datas tem uma taxa diferente. Se você não atribuir datas de efetivação, a sobreposição da taxa de faturamento informada será usada por toda a duração do projeto para calcular a receita.

Para sobrepor uma taxa de faturamento do usuário para um projeto:

1. Vá para o projeto para o qual você deseja substituir as taxas de faturamento.
1. Clique em **Taxas** no painel esquerdo. Talvez seja necessário clicar primeiro em **Mostrar mais**.
1. Clique na guia **Faturamento** se ela ainda não estiver selecionada.
1. Clique em **Adicionar taxa de cobrança** > **Nova taxa de cobrança de usuário**.

   A caixa Nova taxa de faturamento do usuário é aberta.

1. No campo **Usuário**, selecione o usuário para o qual deseja alterar a taxa de cobrança.
1. Selecione a **Moeda** para a substituição da taxa de cobrança.
1. No campo **Taxa de Cobrança**, insira a primeira substituição de taxa de cobrança.
1. (Opcional) Clique em **Adicionar taxa efetiva de data** para adicionar mais substituições de taxa de cobrança.
1. (Condicional) Se você estiver adicionando várias sobreposições de taxa de faturamento, especifique as seguintes informações para cada linha:

   * **Taxa de Cobrança**: o valor da taxa de cobrança durante o período especificado.
   * **Data de Início**: a data em que a substituição da taxa de cobrança começa.
   * **Data Final**: a data em que termina a substituição da taxa de cobrança.

   ![Caixa Nova taxa de cobrança de usuário mostrando as datas de efetivação](assets/new-user-billing-rate-on-project2.png)

   O Workfront aplica a taxa de substituição de usuário às horas que ocorrem durante esses períodos ao calcular a receita do projeto.

   O Workfront permite que você deixe intervalos entre os períodos de substituição, mas você receberá um aviso para confirmar que isso é intencional.

   Você não precisa especificar uma Data Inicial para a primeira taxa de sobreposição, nem uma Data Final para a última taxa de sobreposição.

   Se você informar apenas uma sobreposição de taxa de faturamento, essa taxa será aplicada para toda a duração do projeto. Se você adicionar várias sobreposições de data de efetivação, o Workfront presume que a primeira sobreposição se aplica a todas as horas antes de sua Data Final e a última sobreposição se aplica a todas as horas após sua Data Inicial.

   O Workfront presume que a primeira taxa de sobreposição seja aplicada para todas as horas com uma data anterior à Data Final da primeira sobreposição e que a última taxa de sobreposição seja aplicada para todas as horas com uma data mais recente que a Data Inicial da última sobreposição.

   Se uma hora for registrada antes da Data de início planejada do projeto, a primeira taxa de cobrança será usada.

   Se uma hora for registrada depois da Data de conclusão planejada do projeto, a última taxa de cobrança será usada.

1. Clique em **Salvar**.
