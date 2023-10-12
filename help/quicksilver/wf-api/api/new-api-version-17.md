---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 17
description: O Adobe Workfront lançou a API versão 17 em 6 de abril de 2022. A API versão 17 apresenta as seguintes alterações da versão 15.
author: Becky
feature: Workfront API
source-git-commit: e0b040b062796a1d1b1e0c029ca0ef71b77ed54a
workflow-type: tm+mt
source-wordcount: '1351'
ht-degree: 4%

---

# Novidades da API versão 17

O Adobe Workfront lançou a API versão 17 em 12 de outubro de 2023. A API versão 17 apresenta as seguintes alterações da versão 16.

## Recursos adicionados

<!--

### Booking (BOOKNG)

-->

### Documento externo (EXTDOC)

Um objeto ExternalDocument é um documento ou outro ativo digital localizado em um provedor de armazenamento de documentos externo ao Workfront. Esses ativos podem ser vinculados ao Workfront e vice-versa.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>descrição</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>caminho</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>tamanho</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li><p><b>dateModified</b></p></li>
          <li><p><b>descrição</b></p></li>
          <li><p><b>documentProviderID</b></p></li>
          <li><p><b>ext</b></p></li>
          <li><p><b>fileType</b></p></li>
          <li><p><b>iconURL</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isGoogleRootItem</b></p></li>
          <li><p><b>isTeamDriveItem</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
          <li><p><b>caminho</b></p></li>
          <li><p><b>providerType</b></p></li>
          <li><p><b>readOnly</b></p></li>
          <li><p><b>tamanho</b></p></li>
          <li><p><b>thumbnailURL</b></p></li>
          <li><p><b>value</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos padrão</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>name</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li><p><b>browseListWithLinkAction</b></p></li>
          <li><p><b>getDocumentDownloadUrl</b></p></li>
          <li><p><b>getRootFolderID</b></p></li>
          <li><p><b>getRootFolderIDFromDB</b></p></li>
          <li><p><b>linkExternalDocumentObjects</b></p></li>
          <li><p><b>setLinkedFolderMetadata</b></p></li>
        </ul>
      </td>
    </tr>
    </tr>
    <tr>
      <td role="rowheader">Consultas</td>
      <td>
        <ul>
          <li><p><b>browseList</b></p></li>
          <li><p><b>getFolderMetaData</b></p></li>
          <li><p><b>searchExternalDocuments</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operações</td>
      <td>
        <ul>
          <li><p><b>SEARCH</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### NlbrGroups (NLBRGP)

### NonLaborResource (NLBR)

### NonLaborResourceParameterValue (NLBRPV)

### RichTextNonLaborResourceParameterValue (NLRRPV)

-->

### UserLocation (USRLOC)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li><p><b>classifierID</b></p></li>
          <li><p><b>customerID</b></p></li>
          <li><p><b>endDate</b></p></li>
          <li><p><b>ID</b></p></li>
          <li><p><b>isCurrent</b></p></li>
          <li><p><b>startDate</b></p></li>
          <li><p><b>userID</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>
        <ul>
          <li><p><b>cliente</b></p></li>
          <li><p><b>usuário</b></p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li><p><b>ID</b></p></li>
          <li><p><b>objCode</b></p></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

## Recursos removidos

Nenhum recurso foi removido para a API versão 17

## Recursos modificados

Os recursos a seguir foram modificados para a API versão 17.

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

### AccessRequest (ACSREQ)

If a User does not have access to an object in Workfront that they need, they can request access to that object. The AccessRequest object represents this request.

### AccessRule (ACSRUL)

An AccessRule object represents a rule set in custom access levels that determines how users can share projects they create.

-->

### Linha de base (BLIN)

Linhas de Base são instantâneos de como era o desempenho de um projeto em um determinado momento. Eles armazenam informações importantes sobre o projeto, como datas importantes, progresso, valores de custo e receita.

O objeto de Linha de Base removeu o sinalizador **INLINE_EDITABLE**.

### Registro de Cobrança (BILL)

Um objeto BillingRecord registra a receita, as horas ou as despesas que podem ser faturadas. Essas informações podem ser usadas para criar faturas em um sistema de contabilidade externo.

O objeto BillingRecord removeu o sinalizador **INLINE_EDITABLE**.

<!--

### Category (CTGY)

A Category object is a custom form.

-->

### Empresa (CMPY)

Um objeto Company representa uma organização que consiste em uma coleção de pessoas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Removido</p>
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
            <p>Adição do valor possível "config.defaultToNewHomeDescription" (customer:config.defaultToNewHome)&gt;/p?<p>Isso permite que uma organização torne a nova experiência da Página inicial a padrão para seus usuários.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Versão do documento (DOCV)

Um objeto DocumentVersion representa uma versão específica de um arquivo (como material escrito, imagens ou outras formas de informação).

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
            <p>Adição do possível valor "Frame.io" (FRAMEIO)</p>
          </li>
          <li>
            <p><b>fileType</b>
            </p>
            <p>Adição do possível valor "enum.filetype.site" (site)</p>
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
      <td>Os seguintes campos foram adicionados:
        <ul>
          <li><p><b>endDate</b></p></li>
          <li><p><b>startDate</b></p></li>
       </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li><p><b>getCustomerCurrencies</b></p></li>
          <p>Adicionado.</p>
       </ul>
      </td>
    </tr>
 </tbody>
</table>

### Despesa (EXPNS)

As despesas representam os custos não mão de obra que podem ser incorridos durante a vida útil de um projeto.

O objeto Despesa removeu o sinalizador **INLINE_EDITABLE**.

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
            <p><b>defaultInterface</b>
            </p>
            <p>Removido</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Hora (HORA)

Um objeto Hour representa uma hora registrada por um usuário em uma folha de horas.

O objeto Hora removeu o sinalizador **INLINE_EDITABLE**.

### Iteração (ITRN)

Um objeto de Iteração representa uma única Iteração Agile. Iterações são períodos discretos usados para planejar e concluir histórias Agile.

O objeto de Iteração removeu o sinalizador **INLINE_EDITABLE**.


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
              <li>Aprovador adicionado (AAA)</li>
              <li>Revisor adicionado (AAR)</li>
              <li>Revisor removido (ARR)</li>
              <li>Aprovador removido (ARA)</li>
              <li>Decisão aprovada (ADA)</li>
              <li>Decisão aprovada com alterações (ADC)</li>
              <li>A decisão precisa de trabalho (ADN)</li>
              <li>Decisão revogada (RAL)</li>
              <li>Aprovador alterado (AAC)</li>
              <li>Revisor alterado (ARC)</li>
              <li>Revisão concluída (RDC)</li>
              <li>Revisão revogada (RDR)</li>
              <li>Publicar (PUB)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Quadro Kanban (KNBNBD)

Um quadro Kanban é usado para rastrear tarefas em um ambiente Agile.

O objeto do Quadro Kanban removeu o sinalizador **INLINE_EDITABLE**.


### LinkedFolder (LNKFDR)

Um objeto LinkedFolder representa uma pasta vinculada de um provedor de documentos externo, como Google Drive ou Dropbox.

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
            <p>Valor possível adicionado "Frame.io (FRAMEIO)</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask/Problema (OPTASK)

Um objeto OpTask é comumente conhecido como um Problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de Help Desk. Pedidos de alteração, solicitações e bugs também são problemas.

O objeto Problema removeu o sinalizador **INLINE_EDITABLE**.

### Projeto (PROJ)

Os projetos são itens de trabalho no Workfront e um elemento principal da maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Projeto representa um grupo de tarefas com uma meta comum e específica.

O objeto Project removeu o sinalizador **INLINE_EDITABLE**.

### Usuário de Projeto (PRTU)

Um objeto ProjectUser representa um usuário associado a um projeto específico.

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
            <p>Adicionado.</p>
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
            <p>Adicionado.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### QueueDef (QUED)

A QueueDef object represents a Queue, which is a project that has been published to the Help Desk area to allow users to submit issues to it.

-->

### Taxa (RATE)

Um objeto de Taxa representa uma taxa de cobrança no Workfront.

O objeto Rate removeu o sinalizador **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>As seguintes ações foram adicionadas para oferecer suporte à funcionalidade Cartão de taxa:
        <ul>
          <li><p><b>deleteRateForRole</b></p></li>
          <li><p><b>editRatesForRole</b></p></li>
          <li><p><b>getUsedClassifierIds</b></p></li>
          <li><p><b>setRatesFromRateCard</b></p></li>
        </ul>
        <p>A variável <b>setRatesForRole</b> A ação foi modificada para adicionar os seguintes campos:
        <ul>
        <li>classifierID</li>
        <li>currencyCode</li>
        <li>sourceRateCardID</li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Risco (RISK)

Um objeto de Risco representa um evento possível que pode impedir que um projeto seja concluído no prazo ou dentro do orçamento. Os riscos são adicionados aos projetos na fase de planejamento para identificar possíveis obstáculos antes da aprovação de qualquer trabalho.

O objeto de Risco removeu o sinalizador **INLINE_EDITABLE**.

### Função/Função (ROLE)

Um objeto Função (função de trabalho) representa uma capacidade funcional ou um conjunto de habilidades que um usuário pode preencher, como Designer ou Gerente de produto.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Removido</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tarefa (TASK)

Um objeto Tarefa representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (concluir um Projeto).

O objeto Tarefa removeu o sinalizador **INLINE_EDITABLE**.

### Equipe (TEAMOB)

Um objeto Equipe é uma coleção de Usuários que pode ser atribuída a um item de trabalho.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>defaultInterface</b>
            </p>
            <p>Removido</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Integrante da equipe (TEAMMB)

Um objeto TeamMember é um usuário associado a uma equipe específica.

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
            <p>Adicionado.</p>
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
            <p>Adicionado.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### TemplateUser (TMTU)

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
            <p>Adicionado.</p>
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
            <p>Adicionado.</p>
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
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
            <p>Removido</p>
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
            <p><b>changeType</b>
            </p>
            <p>Os seguintes valores foram adicionados:</p>
            <ul>
              <li>Aprovador adicionado (assetapprovalAddApprover)</li>
              <li>Revisor adicionado (assetapprovalAddReviewer)</li>
              <li>Aprovador removido (assetapprovalRemoveApprover)</li>
              <li>Revisor removido (assetapprovalRemoveReviewer)</li>
              <li>Decisão aprovada (assetapprovalDecisionApproved)</li>
              <li>A decisão precisa de trabalho (assetapprovalDecisionNeedsWork)</li>
              <li>Decisão aprovada com alterações (assetapprovalDecisionApprovedChanges)</li>
              <li>Decisão revogada (assetapprovalDecisionRevoked)</li>
              <li>Aprovador alterado (assetapprovalApproverChanged)</li>
              <li>Revisor alterado (assetapprovalReviewerChanged)</li>
              <li>Revisão concluída (assetapprovalReviewerDecisionComplete)</li>
              <li>Revisão revogada (assetapprovalReviewerDecisionRevoked)</li>
              <li>Erro de envio de documento externo (externalDocumentSendError)</li>
              <li>Versão do documento publicada (documentVersionPublish)</li>
              <li>Fluxo de trabalho de pasta vinculado (linkedFolderWorkflow)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
 </table>

### Usuário (USER)

Um objeto Usuário representa uma pessoa com uma conta no Workfront que pode fazer logon e interagir com o sistema.

O objeto Usuário removeu o sinalizador **INLINE_EDITABLE**.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>workTime</b>
            </p>
            <p>Este campo foi adicionado e é um número entre 0 e 1 que representa a porcentagem de tempo que um usuário pode gastar no trabalho do projeto (trabalho não administrativo) a cada dia. Um valor de 1 significa que o usuário pode gastar 100% de seu tempo no trabalho do projeto.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>userLocations</b>
            </p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Grupos de usuários (USRGPS)

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
            <p>Adicionado.</p>
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
            <p>Adicionado.</p>
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
            <p><b>changeType</b>
            </p>
            <p>Os seguintes valores foram adicionados:</p>
            <ul>
              <li>O documento precisa de sua aprovação (AAA)</li>
              <li>O documento precisa de sua revisão (AAR)</li>
              <li>O documento não precisa mais de sua aprovação (ARA)</li>
              <li>O documento não precisa mais de sua revisão (ARR)</li>
              <li>Necessidades de documento (usuário) para aprovação (ATA)</li>
              <li>Revisão (ATR) das necessidades do documento (usuário)</li>
              <li>O documento não precisa mais da aprovação (RTA) do (usuário)</li>
              <li>O documento não precisa mais da revisão (RTR) do (usuário)</li>
              <li>Documento aprovado (ADA)</li>
              <li>Documento aprovado com alterações (ADC)</li>
              <li>O documento precisa de trabalho (ADN)</li>
              <li>(Usuário) marcou (documento) como aprovado. Sua aprovação não é mais necessária. AAN)</li>
              <li>(Usuário) marcou (documento) como aprovado com alterações. Sua aprovação não é mais necessária. (ACN)</li>
              <li>(Usuário) marcou (documento) como precisa do trabalho. Sua aprovação não é mais necessária. (AWN)</li>
              <li>O documento precisa de sua revisão agora em vez de aprovação (AAC)</li>
              <li>O documento precisa de sua aprovação agora em vez de uma revisão (ADN)</li>
              <li>Documento revisado (RDC)</li>
              <li>Documento revisado (TRC)</li>
              <li>(Usuário) revisou (documento) como concluído. Sua revisão não é mais necessária. TRN)</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Função do usuário (USRROL)

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
            <p>Adicionado.</p>
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
            <p>Adicionado.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
