---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 18
description: O Adobe Workfront lançou a API versão 18 em 6 de abril de 2022. A API versão 18 apresenta as seguintes alterações da versão 15.
author: Becky
feature: Workfront API
role: Developer
exl-id: d0675dc1-b2d9-4d80-8c12-f26284cfb4cf
source-git-commit: c2ce6776ceebe3c1d3915e3791fc84eb0245ba4d
workflow-type: tm+mt
source-wordcount: '1141'
ht-degree: 0%

---

# Novidades da API versão 18

A Adobe Workfront lançou a API versão 18 em 8 de abril de 2024. A API versão 18 apresenta as seguintes alterações da versão 15.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 18.

## Recursos removidos

Nenhum recurso foi removido para a API versão 18

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
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>açõesProibidas</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>açõesSecundárias</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
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
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
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
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>açõesProibidas</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>açõesSecundárias</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
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
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aguardando Aprovação (AWAPVL)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Operações</td>
      <td>
        <ul>
          <li>
            <p>Foram adicionadas as seguintes operações:
            </p>
            <ul>
              <li>
                <p><b>ADICIONAR</b>
                </p>
              </li>
              <li>
                <p><b>DELETE</b>
                </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
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
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
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
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Categoria (CTGY)

Um objeto de Categoria é um formulário personalizado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>:
            </p>
            <p>Foram adicionados os seguintes valores possíveis:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoria de Recursos Não Mão-de-Obra)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Hora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Cartão de tarifa)
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>objTypes</b>:
            </p>
            <p>Foram adicionados os seguintes valores possíveis:
            <ul>
              <li>
                <p><code>NLBRCY</code> (Categoria de Recursos Não Mão-de-Obra)
                </p>
              </li>
              <li>
                <p><code>HOUR</code> (Hora)
                </p>
              </li>
              <li>
                <p><code>RTCRD</code> (Cartão de tarifa)
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Documento (DOCU)

Um objeto Documento representa um arquivo (como material escrito, imagens ou outras formas de informação).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b>:
            </p>
            <p>Adição do seguinte parâmetro:
            <ul>
              <li>
                <p><code>documentID</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>moveToFolder</b>:
            </p>
            <p>Adição de. Essa nova ação usa os seguintes parâmetros:
            <ul>
              <li>
                <p><code>documentIDs</code>
                </p>
              </li>
              <li>
                <p><code>folderID</code> 
                </p>
              </li>
              <li>
                <p><code>moveToFolder</code> 
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
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
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos padrão</td>
      <td>
        <ul>
          <li>
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

O objeto JournalEntry pode ser configurado para registrar informações sobre campos de objeto específicos sempre que esses campos forem modificados. Quando um campo é configurado para ser registrado como parte do objeto de Entrada de diário, uma Entrada de diário correspondente será criada toda vez que o campo for modificado.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>AAO</code> (enum.actiontypeenum.assetapproval.opened)</p>
              </li>
              <li>
                <p><code>ADM</code> (enum.actiontypeenum.assetapproval.locked.all.decision.made)</p>
              </li>
              <li>
                <p><code>AUL</code> (enum.actiontypeenum.assetapproval.unlocked.manual)</p>
              </li>
              <li>
                <p><code>ALM</code> (enum.actiontypeenum.assetapproval.locked.manual)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask (OPTASK)

Um objeto OpTask é comumente conhecido como um Problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de Help Desk. Pedidos de alteração, solicitações e bugs também são problemas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>:
            </p>
            <p>Adição dos seguintes campos:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
          <li>
            <p><b>convertToTask</b>:
            </p>
            <p>Adição dos seguintes campos:
            <ul>
              <li>
                <code>copyCategories</code></li><li><code>copyNativeFields</code>
                </p>
              </li>
             </ul>
             </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>createProjectWithOverride</b>
            </p>
             <p>Adição de.
            </p>
           </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### FunçãoUsuárioProjeto (PTEAM)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Adição do seguinte campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p>Adição do seguinte campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
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
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>solicitanteForbiddenActions</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>VIEW_COST_RATES</code> (Exibir Taxas de Custo)</p>
              </li>
              <li>
                <p><code>VIEW_BILLING_RATES</code> (Ver Taxas de Cobrança)</p>
              </li>
              <li>
                <p><code>VIEW_GENERAL_FINANCE</code> (Exibir finanças gerais)</p>
              </li>
              <li>
                <p><code>EDIT_COST_RATES</code> (Editar taxas de custo)</p>
              </li>
              <li>
                <p><code>EDIT_BILLING_RATES</code> (Editar taxas de cobrança)</p>
              </li>
              <li>
                <p><code>EDIT_GENERAL_FINANCE</code> (Editar Finanças Gerais)</p>
              </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Taxa (RATE)

Um objeto de Taxa representa uma taxa de cobrança no Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>companyID</b></p><p>Adição dos seguintes sinalizadores:
            </p>
            <ul>
              <li>
                <p>AUTO_LOAD
                </p>
              </li>
              <li>
                <p>DINÂMICO
                </p>
              </li>
             </ul>
          </li>
          <li>
          <p><b>displayName</b></p><p>Adição de.</p>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>displayName</b>
            </p><p>Adição de.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Tarefa (TASK)

Um objeto Tarefa representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (concluir um Projeto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>convertToProject</b>
            </p>
             <p>Adição do seguinte campo:
             <ul><li><code>copyCategories</code></li></ul>
            </p>
           </li>
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
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Tarefa de modelo (TTSK)

Um objeto TemplateTask representa uma Tarefa que faz parte de um Template. Modelos de Tarefa se tornam Tarefas no Projeto onde o Modelo é usado.<table>
<col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateUserRole (EQUIPE)

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p>Adição do seguinte campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p>Adição do seguinte campo:
            </p>
            <ul>
              <li>
                <p><b>ID</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Planilha de horas (TSHET)

Um objeto de Planilha de Horas representa um cartão de ponto virtual que permite aos Usuários inserir as horas reais trabalhadas para Tarefas, Projetos e Tipos de Horas Gerais.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p>O seguinte campo foi removido:
            </p>
            <ul>
              <li>
                <p><b>objCode</b>
                </p>
              </li>
             </ul>
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
                <p><code>assetapprovalsLockedAllDecisionsMade</code></p>
              </li>
              <li>
                <p><code>assetapprovalsUnlockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalsLockedManual</code></p>
              </li>
              <li>
                <p><code>assetapprovalOpened</code> </p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>recentUpdatesObjIDs</b>
            </p>
            <p>Adição de.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### UserPrefValue (USERPF)

Um objeto UserPrefValue representa uma preferência do usuário.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>valor</b>
            </p>
            <p>Adição do validador <code>MAX_LENGTH</code></p>
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
            <p>Adição dos seguintes campos:
            </p>
            <ul>
              <li>
                <p><b>realBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>atualNonBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedBillableExpenseCost</b>
                </p>
              </li>
              <li>
                <p><b>plannedNonBillableExpenseCost</b>
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

