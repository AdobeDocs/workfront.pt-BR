---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 20
description: O Adobe Workfront lançou a API versão 20 em 6 de abril de 2022. A API versão 20 apresenta as seguintes alterações da versão 19.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# Novidades da API versão 20

O Adobe Workfront lançou a API versão 20 em 4 de maio de 2025. A API versão 20 apresenta as seguintes alterações da versão 19.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 20.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## Recursos removidos

Nenhum recurso foi removido para a API versão 20

## Recursos modificados

### Permissões de Nível de Acesso (ALVPER)

Um objeto AccessLevelPermissions representa uma permissão específica para acessar, criar ou modificar um objeto Workfront. Essas permissões podem ser associadas a um Nível de acesso.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>açõesProibidas</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>açõesSecundárias</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Solicitação de acesso (ACSREQ)

Se um usuário não tiver acesso a um objeto no Workfront necessário, ele poderá solicitar acesso a esse objeto. O objeto AccessRequest representa essa solicitação.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>ação</b>
            </p>
             <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Regra de acesso (ACSRUL)

Um objeto AccessRule representa um conjunto de regras em níveis de acesso personalizados que determina como os usuários podem compartilhar projetos criados por eles.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>açõesProibidas</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>açõesSecundárias</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Anexo da notificação (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
             <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aprovação (APPROVAL)

Um determinado item de trabalho, como uma tarefa, um documento ou uma folha de horas, pode exigir que um supervisor ou outro usuário faça logoff no item de trabalho. Um objeto de Aprovação representa a ação de desconectar em um item de trabalho.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualBenefit</li>
              <li>atualBillableExpenseCost</li>
              <li>atualCost</li>
              <li>atualExpenseCost</li>
              <li>atualLaborCost</li>
              <li>atualNonBillableExpenseCost</li>
              <li>atualRevenue</li>
              <li>atualRiskCost</li>
              <li>atualValue</li>
              <li>billingRevenue</li>
              <li>orçamento</li>
              <li>budgetCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>atualCost</li>
          <li>atualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>Adicionados os sinalizadores <code>DYNAMIC</code>, <code>LAZY_READ</code> e <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Adição do sinalizador <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Adicionado o valor possível <code>URH</code> (Usuário e Função por hora) </li>
          <li><p><b>revenueType</b></p> <p>Adicionados os valores possíveis <code>URH</code> (Usuário e Função por hora), <code>URC</code> (Usuário e Função por hora com Cap) e <code>URF</code> (Usuário e Função por hora mais Fixo)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
          <p>Os seguintes campos foram adicionados:</p>
             <ul>
              <li><b>taxasDeCobrança</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Atribuição (ASSGN)

Um objeto Atribuição representa a conexão entre um item de trabalho e o usuário, equipe ou grupo atribuído para trabalhar nele.

O objeto Assignment adicionou os sinalizadores `ATTRIBUTE_ATTACHABLE` e `DOMAIN_EXTENDABLE`.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### Avatar

Um objeto Avatar é uma foto do usuário.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>códigoObjetoAnexado</b>
            </p>
             <p>Adicionado</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>códigoObjetoAnexado</b>
            </p>
             <p>Adicionado</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operações</td>
      <td>
        <ul>
          <li>
            <p><b>CÓPIA</b>
            </p>
             <p>Adicionado</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

### Linha de base (BLIN)

Linhas de Base são instantâneos de como era o desempenho de um projeto em um determinado momento. Eles armazenam informações importantes sobre o projeto, como datas importantes, progresso, valores de custo e receita.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualBillableExpenseCost</li>
              <li>atualCost</li>
              <li>atualNonBillableExpenseCost</li>
              <li>orçamento</li>
              <li>eac</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>atualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Adição do sinalizador <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarefa da linha de base (BSTSK)

Linhas de Base são instantâneos de como era o desempenho de um projeto em um determinado momento. Eles armazenam informações importantes sobre o projeto, como datas importantes, progresso, valores de custo e receita. Quando você cria uma linha de base, as informações sobre a tarefa também são capturadas nas tarefas dessa linha de base.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualBillableExpenseCost</li>
              <li>atualCost</li>
              <li>atualNonBillableExpenseCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedNonBillableExpenseCost</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>atualCost</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Adição do sinalizador <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Registro de Cobrança (BILL)

Um objeto BillingRecord registra a receita, as horas ou as despesas que podem ser faturadas. Essas informações podem ser usadas para criar faturas em um sistema de contabilidade externo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>quantidade</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Adicionado</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

### Parâmetro da categoria (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>configurações</b>
            </p>
             <p>Adicionado</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Empresa (CMPY)

Um objeto Company representa uma organização que consiste em uma coleção de pessoas.

O objeto Company adicionou o sinalizador `SHARABLE`.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

### Preferências do cliente (CUSTPR)

Um objeto CustomerPreferences representa o conjunto de preferências que um cliente definiu para sua instância do Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>nome</b>
            </p>
             <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (singleassignmentschedule)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskissuemove)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Taxa de Câmbio (EXRATE)

Um objeto ExchangeRate representa uma taxa de câmbio de moeda configurada no Workfront. Os objetos ExchangeRate não são dinâmicos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
           <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>taxa</li>
      </td>
    </tr>
  </tbody>
</table>


### Dados financeiros (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualBillableExpenseCost</li>
              <li>atualExpenseCost</li>
              <li>atualFixedRevenue</li>
              <li>atualLaborCost</li>
              <li>atualLaborCostHours</li>
              <li>atualLaborRevenue</li>
              <li>atualNonBillableExpenseCost</li>
              <li>fixedCost</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedFixedRevenue</li>
              <li>plannedLaborCost</li>
              <li>plannedLaborCostHours</li>
              <li>plannedLaborRevenue</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>totalAtualCost</li>
              <li>totalAtualRevenue</li>
              <li>totalPlannedCost</li>
              <li>totalPlannedRevenue</li>
              <li>totalCustoVariação</li>
              <li>totalVarianceRevenue</li>
              <li>varianceExpenseCost</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Grupo (GRUPO)

Um objeto Grupo representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>moeda</b>
            </p>
             <p>Adicionado</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### Hora (HORA)

Um objeto Hour representa uma hora registrada por um usuário em uma folha de horas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
              <li>atualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Adicionado</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

Um objeto OpTask é comumente conhecido como um Problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de Help Desk. Pedidos de alteração, solicitações e bugs também são problemas.

O objeto OpTask adicionou o sinalizador DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualCost</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
              <li>atualCost</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Parâmetro (PARAM)

Um objeto Parameter é um campo personalizado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (Pesquisa interna)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Pesquisa Interna de Seleção Múltipla)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio (PORTA)

Um objeto do Portfolio é uma coleção de projetos que competem pelos mesmos recursos, normalmente dinheiro ou pessoas para concluí-los.

O objeto Portfolio adicionou o sinalizador `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>alinhado</li>
              <li>orçamento</li>
              <li>moeda</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Programa (PRGM)

Um objeto Programa é um subconjunto de projetos em um portfólio, em que projetos semelhantes podem ser agrupados.

O objeto Program adicionou o sinalizador `DOMAIN_EXTENDABLE`.

### Projeto (PROJ)

Os projetos são itens de trabalho no Workfront e um elemento principal da maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Projeto representa um grupo de tarefas com uma meta comum e específica.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualBenefit</li>
              <li>atualBillableExpenseCost</li>
              <li>atualCost</li>
              <li>atualExpenseCost</li>
              <li>atualLaborCost</li>
              <li>atualNonBillableExpenseCost</li>
              <li>atualRevenue</li>
              <li>atualRiskCost</li>
              <li>atualValue</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>billingRevenue</li>
              <li>orçamento</li>
              <li>budgetCost</li>
              <li>budgetedHours</li>
              <li>budgetedLaborCost</li>
              <li>eac</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>plannedValue</li>
              <li>remainingCost</li>
              <li>remainingRevenue</li>
              <li>remainingRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>atualCost</li>
          <li>atualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Adição do sinalizador <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Um objeto QueueDef representa uma Fila, que é um projeto publicado na área Help Desk para permitir que os usuários enviem problemas a ele.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>solicitanteCoreAction</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>solicitanteForbiddenActions</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Remover dos dados personalizados)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Adicionar subprojetos)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Taxa (RATE)

Um objeto de Taxa representa uma taxa de cobrança no Workfront.

O objeto Rate adicionou o sinalizador `ATTRIBUTE_ATTACHABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>Os seguintes campos foram adicionados:
          <ul>
          <li>moeda</li>
          <li>bloqueado</li>
          <li>tipo</li>
          <li>value</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Função (ROLE)

Um objeto Função (função de trabalho) representa uma capacidade funcional ou um conjunto de habilidades que um usuário pode preencher, como Designer ou Gerente de produto.

O objeto de Função adicionou o sinalizador `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
          <p>Os seguintes campos foram adicionados:
          <ul>
          <li>taxasDeCobrança</li>
          <li>costRates</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Relatório agendado (SCHREP)

Um objeto ScheduledReport representa um relatório que foi configurado para ser agendado para entrega.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>formato</b>
            </p>
             <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Um objeto ScoreCardQuestion representa uma pergunta que foi adicionada a um Scorecard. Essas perguntas geralmente são determinadas pelo gerente da Portfolio e suas respostas permitem que o gerente entenda como um projeto se alinha às metas do portfólio.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
             <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li><p><code>INTRNL</code> (Pesquisa interna)</p></li>
              <li><p><code>MULTINTRNL</code> (Pesquisa Interna de Seleção Múltipla)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarefa (TASK)

Um objeto Tarefa representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (concluir um Projeto).

O objeto Task adicionou o sinalizador `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualBillableExpenseCost</li>
              <li>atualCost</li>
              <li>atualExpenseCost</li>
              <li>atualLaborCost</li>
              <li>atualNonBillableExpenseCost</li>
              <li>atualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>atualCost</li>
          <li>atualRevenue</li>
          <li>plannedCost</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Foram adicionados os seguintes valores possíveis:<ul><li><code>URH</code> (Usuário e Função por Hora)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Foram adicionados os seguintes valores possíveis:<ul><li><code>URH</code> (Usuário e Função por Hora)</li><li><code>URC</code> (Horas por dia do usuário e função com limite)</li><li><code>URF</code> (Horas por Valor da Hora do Usuário e Função mais Taxa Fixa)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Modelo (TMPL)

Um objeto Modelo representa um padrão para um projeto. Os projetos podem ser criados a partir de modelos para economizar tempo. Um modelo contém uma equipe e tarefas, que serão copiadas para qualquer projeto criado a partir do modelo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>orçamento</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>plannedBenefit</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>plannedRiskCost</li>
              <li>workRequired</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
          <p>Os seguintes campos foram adicionados:</p>
             <ul>
              <li><b>taxasDeCobrança</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tarefa de modelo (TTSK)

Um objeto TemplateTask representa uma Tarefa que faz parte de um Template. Modelos de Tarefa se tornam Tarefas no Projeto onde o Modelo é usado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingAmount</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost/li&gt;
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
              <li>revenueType</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Foram adicionados os seguintes valores possíveis:<ul><li><code>URH</code> (Usuário e Função por Hora)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Foram adicionados os seguintes valores possíveis:<ul><li><code>URH</code> (Usuário e Função por Hora)</li><li><code>URC</code> (Horas por dia do usuário e função com limite)</li><li><code>URF</code> (Horas por Valor da Hora do Usuário e Função mais Taxa Fixa)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Planilha de horas (TSHET)

Um objeto de Planilha de Horas representa um cartão de ponto virtual que permite aos Usuários inserir as horas reais trabalhadas para Tarefas, Projetos e Tipos de Horas Gerais.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>Removido</p>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Atualizar (UPDATE)

Os itens de trabalho no Workfront podem ser atualizados para manter os usuários informados sobre o status atual. Um objeto Update representa uma dessas atualizações. As atualizações podem ser inseridas por usuários ou criadas pelo sistema do Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
             <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Usuário (USER)

Um objeto Usuário representa uma pessoa com uma conta no Workfront que pode fazer logon e interagir com o sistema.

O objeto de usuário adicionou os campos `ATTRIBUTE_ATTACHABLE` e `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>billingPerHour</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
          <p>Os seguintes campos foram adicionados:</p>
             <ul>
              <li><b>taxasDeCobrança</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Trabalho (WORK)

Um objeto Trabalho é uma interface comum que tanto Tarefa quanto OpTask herdam e compartilha código comum entre os dois.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Os seguintes campos adicionaram o sinalizador <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>atualBillableExpenseCost</li>
              <li>atualCost</li>
              <li>atualExpenseCost</li>
              <li>atualLaborCost</li>
              <li>atualNonBillableExpenseCost</li>
              <li>atualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>plannedBillableExpenseCost</li>
              <li>plannedCost</li>
              <li>plannedExpenseCost</li>
              <li>plannedLaborCost</li>
              <li>plannedNonBillableExpenseCost</li>
              <li>plannedRevenue</li>
            </ul>
          </li>
          <li>
          <p>Os seguintes campos alteraram seu tipo de <code>double</code> para <code>class java.math.BigDecimal</code>:
          <ul>
          <li>atualCost</li>
          <li>atualRevenue</li>
          <li>plannedCost</li>
          <li>plannedRevenue</li>
          </ul>
          </li>
          <li><p><b>plannedDuration</b></p> <p>Adicionados os sinalizadores <code>DYNAMIC</code>, <code>LAZY_READ</code> e <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Adição do sinalizador <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Adicionado o valor possível <code>URH</code> (Usuário e Função por hora) </li>
          <li><p><b>revenueType</b></p> <p>Adicionados os valores possíveis <code>URH</code> (Usuário e Função por hora), <code>URC</code> (Usuário e Função por hora com Cap) e <code>URF</code> (Usuário e Função por hora mais Fixo)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



