---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 15
description: O Adobe Workfront lançou a API versão 14 em 14 de junho de 2022. A API versão 15 apresenta as seguintes alterações da versão 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: 1cfdc136-f3b4-4beb-b58b-f546a5510e6d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '2349'
ht-degree: 3%

---

# Novidades da API versão 15

O Adobe Workfront lançou a API versão 15 em 14 de junho de 2022. A API versão 15 apresenta as seguintes alterações da versão 14.

## Recursos adicionados

* [Iniciativa INITIV](#Initiati)

* [IssueDef (ISSDEF)](#IssueDef)

* [ObjectIntegration (OBJINT)](#ObjectIn)

* [RichTextGroupParameterValue (GRCVAL)](#RichText)

* [TaskDef (TSKDEF)](#TaskDef)

* [Aprovação do usuário (USRAPV)](#UserAppr)

### Iniciativa INITIV

O objeto Iniciativa cria estimativas no Planejador de cenários da Workfront para o tipo e o número de funções de trabalho, os Custos fixos e o Benefício planejado.

Para obter mais informações sobre iniciativas, consulte [Visão geral das iniciativas no Planejador de cenários](../../scenario-planner/initiatives-overview.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Este é um objeto interno.</p>
          </li>
          <li>
            <p><b>duração</b>
            </p>
            <p>A quantidade de tempo entre endDate e startDate.</p>
          </li>
          <li>
            <p><b>endDate</b>
            </p>
            <p>A data de conclusão planejada da iniciativa.</p>
          </li>
          <li>
            <p><b>enteredByID</b>
            </p>
            <p>A ID associada ao usuário que enviou a solicitação.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>A ID associada à ação</p>
          </li>
          <li>
            <p><b>ID da iniciativa</b>
            </p>
            <p>A ID associada à iniciativa.</p>
          </li>
          <li>
            <p><b>lastPublishedDate</b>
            </p>
            <p>A data em que a Iniciativa foi publicada pela última vez no Planejador de cenários do Workfront.</p>
          </li>
          <li>
            <p><b>name</b>
            </p>
            <p>O nome da Iniciativa</p>
          </li>
          <li>
            <p><b>planID</b>
            </p>
            <p>A ID do plano associado à iniciativa.</p>
          </li>
          <li>
            <p><b>planName</b>
            </p>
            <p>O nome do Plano associado à Iniciativa.</p>
          </li>
          <li>
            <p><b>projectID</b>
            </p>
            <p>A ID do projeto associado à iniciativa.</p>
          </li>
          <li>
            <p><b>scenarioID</b>
            </p>
            <p>A ID do cenário no Planejador de cenários do Workfront associado à iniciativa.</p>
          </li>
          <li>
            <p><b>startDate</b>
            </p>
            <p>A data de início planejada da iniciativa.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td >
        <ul>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>enteredBy</b>
            </p>
          </li>
          <li>
            <p><b>projeto</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>name</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operações</td>
      <td>
        <ul>
          <li>
            <p><b>CONTAGEM</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RELATÓRIO </b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### IssueDef (ISSDEF)

O objeto IssueDef representa um conjunto de dados relativos ao formato dos problemas. Este objeto pode ser anexado a Projetos ou Modelos e afeta os problemas adicionados a esse Projeto ou Modelo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>isInlineAddEnabled</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ObjectIntegration (OBJINT)

Em alguns casos, é possível vincular itens de trabalho do Workfront diretamente a objetos em um produto de software externo. O objeto ObjectIntegration representa esse link.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>customerID</b>
            </p>
            <p>Este é um objeto interno.</p>
          </li>
          <li>
            <p><b>entryDate</b>
            </p>
            <p>A data e a hora em que a Integração de objetos foi inserida no Sistema Workfront.</p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
            <p>A ID exclusiva do Workfront do objeto ObjectIntegration específico.</p>
          </li>
          <li>
            <p><b>integrationType</b>
            </p>
            <p>O software externo com o qual o objeto ObjectIntegration cria um link. Os valores possíveis são:</p>
            <ul>
              <li>
                <p>JIRA</p>
              </li>
              <li>
                <p>SALESFORCE</p>
              </li>
              <li>
                <p>ANAPLAN</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>linkedObjectID</b>
            </p>
          </li>
          <li>
            <p><b>objID</b>
            </p>
            <p>O objeto no Workfront ao qual a ObjectIntegration está associada.</p>
          </li>
          <li>
            <p><b>objObjCode</b>
            </p>
            <p>O código do objeto no Workfront ao qual a ObjectIntegration está associada.</p>
          </li>
          <li>
            <p><b>param1</b>
            </p>
          </li>
          <li>
            <p><b>param2</b>
            </p>
          </li>
          <li>
            <p style="font-weight: bold;">param3</p>
          </li>
          <li>
            <p><b>URL</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td >
        <ul>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### TaskDef (TSKDEF)

O objeto TaskDef representa um conjunto de dados relativos ao formato de tarefas. Este objeto pode ser anexado a Projetos ou Modelos e afeta as tarefas adicionadas a esse Projeto ou Modelo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>autoCalcPlannedHours </b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td >
        <ul>
          <li>
            <p><b>defaultApprovalProcess </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories
</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aprovação do usuário (USRAPV)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos </td>
      <td>
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>customerID</b>
            </p>
          </li>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>requestedDate</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td >
        <ul>
          <li>
            <p><b>aprovador</b>
            </p>
          </li>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>solicitante</b>
            </p>
          </li>
          <li>
            <p><b>usuário</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>ID</b>
            </p>
          </li>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos padrão</td>
      <td >
        <ul>
          <li>
            <p><b>approverID</b>
            </p>
          </li>
          <li>
            <p><b>requestorID</b>
            </p>
          </li>
          <li>
            <p><b>status</b>
            </p>
          </li>
          <li>
            <p><b>userID</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>aprovar</b>
            </p>
          </li>
          <li>
            <p><b>Rejeitar</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operações</td>
      <td>
        <ul>
          <li>
            <p><b>ADICIONAR</b>
            </p>
          </li>
          <li>
            <p><b>CONTAGEM</b>
            </p>
          </li>
          <li>
            <p><b>DELETE</b>
            </p>
          </li>
          <li>
            <p><b>GET</b>
            </p>
          </li>
          <li>
            <p><b>RELATÓRIO</b>
            </p>
          </li>
          <li>
            <p><b>SEARCH</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

## Recursos removidos

Nenhum recurso foi removido para a API versão 15.

## Recursos modificados

* [AccessLevel (ACSLVL)](#AccessLe)

* [Permissões de Nível de Acesso (ALVPER)](#AccessLe2)

* [Solicitação de acesso (ACSREQ)](#AccessRe)

* [Regra de acesso (ACSRUL)](#AccessRu)

* [Aprovação (APPROVAL)](#Approval)

* [Categoria (CTGY)](#Category)

* [Parâmetro da categoria (CTGYPA)](#Category2)

* [Preferências do cliente (CUSTPR)](#Customer)

* [DocumentFolder (DOCFDR)](#Document)

* [Versão do documento (DOCV)](#Document2)

* [Grupo (GRUPO)](#Group)

* [JournalEntry (JRNLE)](#JournalE)

* [LinkedFolder (LNKFDR)](#LinkedFo)

* [OpTask/Problema (OPTASK)](#OpTask)

* [Parâmetro (PARAM)](#Paramete)

* [Portfolio (PORTA)](#Portfoli)

* [Programa (PRGM)](#Program)

* [Projeto (PROJ)](#Project)

* [QueueDef (QUED)](#QueueDef)

* [ScoreCardQuestion (SCOREQ)](#ScoreCar)

* [Tarefa (TASK)](#Task)

* [Modelo (TMPL)](#Template)

* [Planilha de horas (TSHET)](#Timeshee)

* [Visualização (UIVIEW)](#View)

* [Atualizar (UPDATE)](#Update)

* [Usuário (USER)](#User)

* [Nota de Usuário (USRNOT)](#UserNote)

* [Trabalho (WORK)](#Work)

### AccessLevel (ACSLVL)

Um objeto AccessLevel está associado a usuários e descreve o conjunto de AccessLevelPermissions que determinam o que o usuário pode acessar.

Para obter mais informações sobre níveis de acesso, consulte [Níveis de acesso](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>fieldAccessPrivileges</b> (string[])</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>VTMAWMG (Exibir equipes associadas aos meus grupos)</p>
              </li>
              <li>
                <p>VALLTM (Exibir todas as equipes)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b>coreAction</b> (string[])</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
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
            <p><b>ação</b> (sequência de caracteres)</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>autoShareAction</b> (sequência de caracteres)</p>
            <p>Adição do seguinte valor possível:</p>
            <ul>
              <li>
                <p>WDL</p>
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
            <p><b>coreAction</b> (string[])</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>forbiddenActions</b> (string[])</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>secondaryActions</b> (string[])</p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
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
            <p><b>resourcePlannerBudgetedHours </b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td >
        <ul>
          <li>
            <p><b>iniciativa</b>
            </p>
            <p>Adicionado.</p>
            <p>O objeto Iniciativa cria estimativas no Planejador de cenários da Workfront para o tipo e o número de funções de trabalho, os Custos fixos e o Benefício planejado. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
            <p>Adicionado.</p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
            <p>Adicionado.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p style="font-weight: bold;"><b>objectIntegations
</b>
            </p>
            <p style="font-weight: normal;">Adicionado.</p>
            <p>Em alguns casos, é possível vincular itens de trabalho do Workfront diretamente a objetos em um produto de software externo. O objeto ObjectIntegration representa esse link.</p>
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
            <p><b>catObjCode</b> (sequência de caracteres)</p>
            <p>Adição do seguinte valor possível:</p>
            <ul>
              <li>
                <p>GROUP (Grupo)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Adicionado.</p>
            <p style="font-weight: normal;">Esse parâmetro é uma matriz de objetos possíveis aos quais o formulário personalizado pode ser anexado. Ele foi adicionado para oferecer suporte à capacidade de anexar um formulário personalizado a vários tipos de objetos.</p>
            <p>Valores possíveis: </p>
            <p>COMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objTypes</b> (string[])</p>
            <p>Adicionado.</p>
            <p style="font-weight: normal;">Esse parâmetro é uma matriz de objetos possíveis aos quais o formulário personalizado pode ser anexado. Ele foi adicionado para oferecer suporte à capacidade de anexar um formulário personalizado a vários tipos de objetos.</p>
            <p>Valores possíveis: </p>
            <p>COMPY, PORT, PRGM, PROJ, TASK, OPTASK, USER, DOCU, EXPNS, ITRN, BILL, GROUP</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b>ocultarFórmulaDaDescrição</b>
            </p>
            <p>Adicionado.</p>
          </li>
          <li>
            <p><b>journaledObjCodes</b>
            </p>
            <p>Adicionado.</p>
          </li>
          <li>
            <p><b>rawCustomExpression</b>
            </p>
            <p>Adicionado.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

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
            <p><b>name</b>
            </p>
            <p>Os seguintes valores foram adicionados:</p>
            <ul>
              <li>
                <p><code>password:sharePointV2IntegrationEnabled</code> (Integração do SharePoint (Graph API) habilitada)</p>
                <p>Este valor oferece suporte à integração atualizada com o Sharepoint.</p>
              </li>
              <li>
                <p><code>project.mgmt:default.project.allowcreatewithouttemplate</code> (Permitir que os usuários criem projetos sem usar um modelo)</p>
              </li>
              <li>
                <p><code>project.mgmt:taskissue.delegate</code> (config.taskissue.delegate)</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### DocumentFolder (DOCFDR)

Os documentos podem ser organizados em pastas. Você pode criar pastas pessoais na área Documentos pessoal. O objeto DocumentFolder representa uma dessas pastas.

O objeto DocumentFolder adicionou o sinalizador `SHARABLE`.

### Versão do documento (DOCV)

Um objeto DocumentVersion representa uma versão específica de um arquivo (como material escrito, imagens ou outras formas de informação).

Para obter mais informações sobre versões de documentos, consulte [Fazer upload de uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Adição do seguinte valor: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>Este valor oferece suporte à integração atualizada com o Sharepoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grupo (GRUPO)

Um objeto Grupo representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

Para obter mais informações sobre grupos, consulte Grupos versus equipes.

O objeto Group adicionou o sinalizador `DATA_EXTENDIBLE`

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <p>Os seguintes campos foram adicionados:</p>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Uma categoria é um formulário personalizado. Esse parâmetro foi adicionado para oferecer suporte à capacidade de adicionar Forms personalizado a objetos de Grupo. </p>
          </li>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Este é um parâmetro booleano cujo valor é verdadeiro se um objeto estiver Ativo e falso se não estiver. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td >
        <p>Os seguintes campos foram adicionados:</p>
        <ul>
          <li>
            <p><b>aprovador</b>
            </p>
          </li>
          <li>
            <p><b>cliente</b>
            </p>
          </li>
          <li>
            <p><b>solicitante</b>
            </p>
          </li>
          <li>
            <p><b>usuário</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <p>Os seguintes campos foram adicionados:</p>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
          </li>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>Em alguns casos, é possível vincular itens de trabalho do Workfront diretamente a objetos em um produto de software externo. O objeto ObjectIntegration representa esse link.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos padrão</td>
      <td >
        <p>O seguinte campo foi adicionado:</p>
        <ul>
          <li>
            <p><b>isActive</b>
            </p>
            <p>Este é um parâmetro booleano cujo valor é verdadeiro se um objeto estiver Ativo e falso se não estiver. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <p>Os seguintes campos foram adicionados:</p>
        <ul>
          <li>
            <p><b>calculateDataExtension</b>
            </p>
            <p>Esta ação recalcula as expressões em campos de formulário personalizados.</p>
          </li>
          <li>
            <p><b>completeGroupInfo</b>
            </p>
          </li>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
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
        <p><b>changeType</b>
        </p>
        <p>Adição do seguinte valor: </p>
        <ul>
          <li>
            <p>DW (Download)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### LinkedFolder (LNKFDR)

Um objeto LinkedFolder representa uma pasta vinculada de um provedor de documentos externo, como Google Drive ou Dropbox.

Para obter mais informações sobre Pastas vinculadas, consulte Vincular documentos de aplicativos externos.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>externalIntegrationType</b>
            </p>
            <p>Adição do seguinte valor: </p>
            <ul>
              <li>
                <p><code>SHAREPOINT_V2</code> (SharePoint (Graph API))</p>
                <p>Este valor oferece suporte à integração atualizada com o Sharepoint.</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OpTask/Problema (OPTASK)

Um objeto OpTask é comumente conhecido como um Problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de Help Desk. Pedidos de alteração, solicitações e bugs também são problemas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <p>As seguintes ações foram adicionadas:</p>
        <ul>
          <li>
            <p><b>bulkMoveWithOptions</b>
            </p>
          </li>
          <li>
            <p><b>getRequestPath</b>
            </p>
          </li>
        </ul>
        <p>A seguinte ação foi modificada:</p>
        <ul>
          <li>
            <p><b>copyIssue</b>
            </p>
            <p>Campo adicionado <code>parentID</code></p>
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
        <p>O seguinte campo foi adicionado:</p>
        <ul>
          <li>
            <p><b>fieldDefinition</b>
            </p>
          </li>
        </ul>
        <p>Os seguintes campos foram modificados:</p>
        <ul>
          <li>
            <p><b>dataType</b>
            </p>
            <p>Adição do valor possível <code>WIDGET </code>(Widget) </p>
            <p>Este valor suporta o uso de imagens em formulários personalizados.</p>
          </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Adição do valor possível <code>WIDGET </code>(Widget)</p>
            <p>Este valor suporta o uso de imagens em formulários personalizados.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Portfolio (PORTA)

Um objeto Portfolio é uma coleção de projetos que competem pelos mesmos recursos, normalmente dinheiro ou pessoas para concluí-los.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Programa (PRGM)

Um objeto Programa é um subconjunto de projetos em um portfólio, em que projetos semelhantes podem ser agrupados.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>linkExternalObject</b>
            </p>
          </li>
          <li>
            <p><b>unlinkExternalObject</b>
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
            <p><b>resourcePlannerBudgetedHours</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td >
        <ul>
          <li>
            <p><b>iniciativa</b>
            </p>
            <p>O objeto Iniciativa cria estimativas no Planejador de cenários da Workfront para o tipo e o número de funções de trabalho, os Custos fixos e o Benefício planejado. </p>
          </li>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>Em alguns casos, é possível vincular itens de trabalho do Workfront diretamente a objetos em um produto de software externo. O objeto ObjectIntegration representa esse link.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Um objeto QueueDef representa uma Fila, que é um projeto publicado na área Help Desk para permitir que os usuários enviem problemas a ele.

Para obter mais informações sobre Filas de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>requestorCoreAction</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>requestorForbiddenActions</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p>EDIT_TEAMS_I_AM_ON (Editar equipes em que estou)</p>
              </li>
              <li>
                <p>EDIT_TEAMS_I_GROUP_ADMIN (Editar equipes nos grupos que eu gerencio (somente Administradores de grupo))</p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Um objeto ScoreCardQuestion representa uma pergunta que foi adicionada a um Scorecard. Essas perguntas geralmente são determinadas pelo gerente de Portfolio, e suas respostas permitem que o gerente entenda como um projeto se alinha com as metas do portfólio.

Para obter mais informações sobre perguntas do Scorecard, consulte [Criar um cartão de pontuação](../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md).

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
            <p>Adição do valor possível <code>WIDGET </code>(Widget)</p>
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
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>Em alguns casos, é possível vincular itens de trabalho do Workfront diretamente a objetos em um produto de software externo. O objeto ObjectIntegration representa esse link.</p>
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
      <td role="rowheader">Campos de referência</td>
      <td>
        <ul>
          <li>
            <p><b>issueDef</b>
            </p>
          </li>
          <li>
            <p><b>taskDef</b>
            </p>
          </li>
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
        <p>O seguinte campo foi removido:</p>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Visualização (UIVIEW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>uiviewType</b>
            </p>
            <p>Os seguintes valores possíveis foram removidos:</p>
            <ul>
              <li>
                <p><code>FOUR_COL</code> (Layout de quatro colunas)</p>
              </li>
              <li>
                <p><code>UPDATES</code> (Atualizações)</p>
              </li>
              <li>
                <p><code>UPDATESTOOLBAR_FEED</code> (Atualizações)</p>
              </li>
              <li>
                <p><code>WORKINGON</code> (Trabalhando Em)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA</code> (Dados personalizados)</p>
              </li>
              <li>
                <p><code>CUSTOMDATA_UPDATE</code> (Atualizar dados personalizados)</p>
              </li>
              <li>
                <p><code>STATUS_UPDATE</code> (Atualização de Status)</p>
              </li>
              <li>
                <p><code>OPTASK_STATUS_UPDATE</code> (Atualização de Status)</p>
              </li>
              <li>
                <p><code>PROJ_STATUS_UPDATE</code> (Atualização de Status)</p>
              </li>
              <li>
                <p><code>PROJECT_TIMEENTRY</code> (Atualização de Status)</p>
              </li>
              <li>
                <p><code>DLIST</code> (Lista Detalhada)</p>
              </li>
              <li>
                <p><code>DLIST_SECTION</code> (Lista Detalhada)</p>
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
            <p>Adição do valor possível <code>documentVersionDownload </code>(enum.updatetypeenum.documentversiondownload)</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Usuário (USER)

Um objeto Usuário representa uma pessoa com uma conta no Workfront que pode fazer logon e interagir com o sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>
        <ul>
          <li>
            <p><b>userApproval</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>getUsersAvailableTime</b>
            </p>
          </li>
          <li>
            <p><b>resetRopgPassword</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Nota de Usuário (USRNOT)

Um objeto UserNote é uma notificação.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>eventType</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>DUP </code>(Solicitou que você revise um documento)</p>
              </li>
              <li>
                <p><code>DUV </code>(Permite que você exiba um documento)</p>
              </li>
            </ul>
          </li>
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
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objectIntegations</b>
            </p>
            <p>Em alguns casos, é possível vincular itens de trabalho do Workfront diretamente a objetos em um produto de software externo. O objeto ObjectIntegration representa esse link.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>
