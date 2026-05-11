---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 22
description: O Adobe Workfront lançou a API versão 22 em 11 de maio de 2026. A API versão 22 apresenta as seguintes alterações da versão 21.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 682cf24c4c7932afeb66a2e5434fe3cec887e889
workflow-type: tm+mt
source-wordcount: '1326'
ht-degree: 3%

---

# Novidades da API versão 22

O Adobe Workfront lançou a API versão 22 em 8 de maio de 2026. A API versão 22 apresenta as seguintes alterações da versão 21.

## Recursos adicionados

Os recursos a seguir foram adicionados para a API versão 22.

### ReportShareableFolder (RPSHFD)

Você pode usar pastas de relatórios compartilháveis para organizar relatórios e compartilhá-las com outros usuários. Esse recurso foi projetado para equipes que gerenciam grandes volumes de relatórios e precisam de controle de acesso escalável e consistente.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>ID</li>
          <li>name</li>
          <li>objCode</li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campos padrão</td>
      <td>
        <ul>
          <li>name</li>
        </ul>
      </td>
    </tr>
   <tr>
      <td role="rowheader">Operações</td>
      <td>
        <ul>
          <li>ADICIONAR</li>
          <li>CONTAGEM</li>
          <li>EXCLUIR</li>
          <li>EDITAR</li>
          <li>GET</li>
          <li>RELATÓRIO</li>
          <li>SEARCH</li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

## Recursos removidos

Os recursos a seguir foram removidos da API versão 22.

### UserLocation (USRLOC)

Este objeto foi removido.

## Recursos modificados

Os recursos a seguir foram modificados para a API versão 22.

### AccessLevel (ACSLVL)

Um objeto AccessLevel está associado a usuários e descreve o conjunto de AccessLevelPermissions que determinam o que o usuário pode acessar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>O campo a seguir foi modificado com alterações em valores possíveis. Para obter detalhes, consulte a documentação do desenvolvedor.
        <ul>
          <li><b>fieldAccessPrivileges</b></li>
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
      <td>Os campos a seguir foram modificados com alterações em valores possíveis. Para obter detalhes, consulte a documentação do desenvolvedor.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
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
      <td>O campo a seguir foi modificado com alterações em valores possíveis. Para obter detalhes, consulte a documentação do desenvolvedor.
        <ul>
          <li><b>ação</b></li>
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
      <td>Os campos a seguir foram modificados com alterações em valores possíveis. Para obter detalhes, consulte a documentação do desenvolvedor.
        <ul>
          <li><b>coreAction</b></li>
          <li><b>forbiddenActions</b></li>
          <li><b>secondaryActions</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aprovação (APPROVAL)

Um determinado item de trabalho, como uma tarefa, documento ou folha de horas, pode exigir que um supervisor ou outro usuário aprove o item de trabalho. Um objeto de Aprovação representa a ação de desconectar em um item de trabalho.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>O campo a seguir foi adicionado.
        <ul>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### Empresa (CMPY)

Um objeto Company representa uma organização que consiste em uma coleção de pessoas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmProjectID</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### CustomEnum (CSTEM)

O objeto CustomEnum auxilia na conversão de códigos de status em texto legível.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>Adicionado
        <ul>
          <li><p><b>getDefaultAssignmentStatusEnum</b></p></li>
          <li><p><b>getDefaultBookingStatusEnum</b></p></li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Consultas</td>
      <td>Adicionado
        <ul>
          <li><p><b>assignmentStatus</b></p></li>
          <li><p><b>bookingStatus</b></p></li>
        </ul>
      </td>
    </tr>
</tbody>
</table>

### Cliente (CUST)

Um objeto Customer representa uma organização que usa uma instância do Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>O campo a seguir foi modificado.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis.</p>
             <ul>
              <li>
                <p><code>STATUS_BOOKING</code> (Status de Reserva)</p>
              </li>
              <li>
                <p><code>STATUS_ASSIGNMENT</code> (Status das Atribuições)</p>
              </li>
            </ul>
         </li>
         </ul>
         <p>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
         <ul>
         <li><b>isLegacyCustomerEsmStorageEnabled</b></li>
         <li><b>isLegacyCustomerSystemFileMigrationEnabled</b></li>
         <li><b>legacyCustomerEsmStorageMigrationDate</b></li>
         <li><b>legacyCustomerSystemFileMigrationDate</b></li>
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
      <td>O campo a seguir foi modificado.
        <ul>
          <li>
            <p><b>customEnumTypes</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis para oferecer suporte ao gerenciamento de armazenamento corporativo:</p>
             <ul>
              <li>
                <p><code>customer:config.defaultStorageModeAllowOverride</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageMode</code></p>
              </li>
              <li>
                <p><code>customer:config.defaultStorageGroupRollout</code> </p>
              </li>
               <li>
                <p><code>customer:config.defaultStorageGroupOptions</code> </p>
              </li>
             </ul>
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
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmAsset</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>A ação a seguir foi modificada.
        <ul>
          <li><p><b>createLargeDocument
          </b></p><p>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
         <ul>
         <li><b>docObjCode</b></li>
         <li><b>objID</b></li>
         </ul>
         </li>
        </ul>
      </td>
    </tr>  
 </tbody>
</table>

### DocumentFolder (DOCFDR)

Os documentos podem ser organizados em pastas. Você pode criar pastas pessoais na área Documentos pessoal. O objeto DocumentFolder representa uma dessas pastas.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isEsmFolder</b></li>
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
      <td>O campo a seguir foi adicionado para oferecer suporte ao Enterprise Storage Management.
        <ul>
          <li><b>esmVersionID</b></li>
        </ul>
      O campo a seguir foi modificado.
        <ul>
          <li><b>version</b><p>O validador "OBRIGATÓRIO" foi removido.</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>A ação a seguir foi adicionada.
        <ul>
          <li><p><b>sendToAEMDetails</b></p>
         </li>
        </ul>
      </td>
    </tr>  
    <tr>
      <td role="rowheader">Operações</td>
      <td>A operação a seguir foi adicionada.
        <ul>
          <li><p><b>EDITAR</b></p>
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
      <td>Os campos a seguir foram adicionados.
        <ul>
          <li><b>portfolioID</b></li>
          <li><b>programID
          </b></li>
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
      <td>Os campos a seguir foram modificados.
        <ul>
          <li>
            <p><b>changeType</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Mover pasta)</p>
              </li>
              </ul>
         </li>
          <li>
            <p><b>sinalizadores</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis.</p>
             <ul>
              <li>
                <p><code>CI</code>(enum.journalentryflagenum.iscontactinfoentry)</p>
              </li>
              </ul>
         </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalField (JRNLF)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram modificados.
        <ul>
          <li>
            <p><b>ação</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis.</p>
             <ul>
              <li>
                <p><code>PFM</code>(Mover pasta)</p>
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
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li><b>atualWorkRequired</b><p>Adição dos seguintes sinalizadores:
           <ul>
           <li><code>AUTO_LOAD</code></li>
           <li><code>DYNAMIC</code></li>
           </ul>
           </p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Pesquisar campos</td>
      <td>
        <ul>
          <li><b>atualWork</b><p>Tipo alterado de <code>null</code> para <code>double</code>.</p></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### OriginalRequest(ORGREQ)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Operações</td>
      <td>As operações a seguir foram adicionadas.
        <ul>
          <li><p><b>CONTAGEM</b></p>
          <li><p><b>GET</b></p>
          <li><p><b>RELATÓRIO</b></p>
          <li><p><b>SEARCH</b></p>
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
      <td>Os campos a seguir foram adicionados.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>


### ParameterGroup (PGRP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados.
        <ul>
          <li><b>enteredByID</b></li>
          <li><b>entryDate</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### PortalSection (PTLSEC)

Um objeto PortalSection é um Relatório.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>O campo a seguir foi adicionado.
        <ul>
          <li><b>reportShareableFolderID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>O campo a seguir foi adicionado.
        <ul>
          <li><b>reportShareableFolder</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Portfolio (PORTA)

Um objeto do Portfolio é uma coleção de projetos que competem pelos mesmos recursos, normalmente dinheiro ou pessoas para concluí-los.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
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
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      O campo a seguir foi modificado.
        <ul>
          <li><b>portfolioID</b><p>Adição do validador "OBRIGATÓRIO".</li>
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
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
          <li><b>isEsmDocStorageEnabled</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### QueueDef (QUED)

Um objeto QueueDef representa uma definição de fila de solicitações no Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram modificados com alterações em valores possíveis. Para obter detalhes, consulte a documentação do desenvolvedor.
        <ul>
          <li><b>requestorCoreAction</b></li>
          <li><b>requestorForbiddenActions</b></li>
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
      <td>O campo a seguir foi modificado com extensas alterações em valores possíveis. Para obter detalhes, consulte a documentação do desenvolvedor.
        <ul>
          <li><b>formato</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Tarefa (TASK)

Um objeto Tarefa representa um item de trabalho que deve ser concluído como parte de alcançar uma meta final (concluir um projeto).

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li><p><b>convertedOpTaskID</b><p>
              <p>Adicionado</p></li>
          <li><p><b>atualWorkRequired</b></p><p>Sinalizadores <code>AUTO_LOAD</code> e <code>DYNAMIC</code> adicionados.</p></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>
        <ul>
          <li>
            <p><b>TarefaOpconvertida</b>
            </p>
            <p>Adicionado</p>
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
      <td>Os campos a seguir foram adicionados para oferecer suporte ao gerenciamento de armazenamento corporativo.
        <ul>
          <li><b>esmID</b></li>
          <li><b>isCscProject</b></li>
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
      <td>O campo a seguir foi modificado.
        <ul>
          <li>
            <p><b>ação</b>
            </p>
            <p>Adição do seguinte valor possível.</p>
             <ul>
              <li>
                <p><code>primaryFolderMoved</code></p>
              </li>
              </ul>
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
      <td role="rowheader">Campos diretos</td>
      <td>O campo a seguir foi adicionado.
        <ul>
          <li><b>eauthUserID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>O campo a seguir foi removido.
        <ul>
          <li><b>userLocations</b></li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>





