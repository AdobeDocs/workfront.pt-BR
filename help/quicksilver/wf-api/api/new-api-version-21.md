---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 21
description: O Adobe Workfront lançou a API versão 21 em 23 de outubro de 2025. A API versão 21 apresenta as seguintes alterações da versão 20.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: d72c5b4337ea04dbfef4622908824a0bd138b551
workflow-type: tm+mt
source-wordcount: '858'
ht-degree: 4%

---

# Novidades da API versão 20

O Adobe Workfront lançou a API versão 21 em 23 de outubro de 2025. A API versão 21 apresenta as seguintes alterações da versão 20.

## Recursos adicionados

### StaffingPlanTemplate (SPTMPL)

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

### AtribuiçãoFunçãoDeFaturamento (ASBLRL)

O objeto AssignmentBillingRole e todos os seus campos foram removidos.

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
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>açõesProibidas</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>açõesSecundárias</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
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
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
         </li>
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
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>açõesProibidas</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
          </li>
          <li>
            <p><b>açõesSecundárias</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
            </ul>
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
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
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
            <p><b>TrabalhoRequeridoDuplo</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>atribuiçõesDeEquipe</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Atribuição (ASSGN)

Um objeto Atribuição representa a conexão entre um item de trabalho e o usuário, equipe ou grupo atribuído para trabalhar nele.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>assignmentBillingRoles</b>
            </p>
            <p>Removido</p>
              </li>
            </ul>
         </li>
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
            <p><b>catObjCode</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> (Equipe)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>objTypes</b>
            </p>
            <p>Foram adicionados os seguintes valores possíveis:</p>
             <ul>
              <li>
                <p><code>SPTMPL</code> (enum.categorytypeenum.staffingplantemplate)</p>
              </li>
              <li>
                <p><code>TEAMOB</code> (Equipe)</p>
              </li>
            </ul>
          </li>
           </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Cliente (CUST)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><code>APDISAB</code> (Desativar o uso de um miniaplicativo Java para cálculos de cronograma)
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### Documento (DOCU)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>getTemporaryCloudURL</b>
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### PastaDocumento

O objeto DocumentFolder adicionou o sinalizador `RESTORABLE`.

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
            <p><b>getTerejectionCommentporaryCloudURL</b>
            </p>
            <p>Adição do validador <code>MAX_LENGTH</code></p>
              </li>
            </ul>
         </li>
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
          <li>
            <p><b>TrabalhoRequeridoDuplo</b>
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
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
            <p><b>dataType</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>RICHLX</code> (Rich Text Lexical)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Rollup de Linha Única)</p>
              </li></ul>
         <li>
            <p><b>estáAtivo</b>
            </p>
            <p>Adicionado</p>
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
            <p><b>estáAtivo</b>
            </p>
            <p>Adicionado</p>
           </li>
           </ul>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>overrideCurrency</b>
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
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
      <td>
        <ul>
          <li>
            <p><b>moeda</b>
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
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
            <p><b>TrabalhoRequeridoDuplo</b>
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
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
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
              </li>
            </ul>
         </li>
          <li>
            <p><b>solicitanteForbiddenActions</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>EDIT_CONTACTINFO</code> (Editar informações de contato)</p>
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
            <p><b>projetosHelpDesk</b>
            </p>
            <p>Adicionado</p>
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
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>localBillingPerHour</b>
            </p>
            <p>Removido</p>
              </li>
          <li>
            <p><b>localCostPerHour</b>
            </p>
            <p>Removido</p>
              </li>
         </li>
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
              <li><p><code>AI</code></p></li>
              <li><p><code>PSD</code></p></li>
              <li><p><code>ASE</code></p></li>
              <li><p><code>INDD</code></p></li>
              <li><p><code>PUB</code></p></li>
              <li><p><code>BMP</code></p></li>
              <li><p><code>DNG</code></p></li>
              <li><p><code>HEIC</code></p></li>
              <li><p><code>HEIF</code></p></li>
              <li><p><code>JP2</code></p></li>
              <li><p><code>PJPEG</code></p></li>
              <li><p><code>RAW</code></p></li>
              <li><p><code>SVG</code></p></li>
              <li><p><code>WEBP</code></p></li>
              <li><p><code>EPS</code></p></li>
              <li><p><code>MP4</code></p></li>
              <li><p><code>FLV</code></p></li>
              <li><p><code>M4V</code></p></li>
              <li><p><code>MPEG</code></p></li>
              <li><p><code>WMV</code></p></li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Um objeto ScoreCardQuestion representa uma pergunta que foi adicionada a um Scorecard. Essas perguntas geralmente são determinadas pelo gerente da Portfolio e suas respostas permitem que o gerente entenda como um projeto se alinha às metas do portfólio.<table>
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
            <p>Adição do seguinte valor possível:</p>
             <ul>
              <li>
                <p><code>SNGLROLLUP</code> (Rollup de Linha Única)</p>
              </li></ul>
         </ul>
      </td>
    </tr>
 </tbody>
</table>

### Plano de Equipe

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>custoEstimadoTotal</b>
            </p>
            <p>Adicionado</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Adicionado</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
      </td>
    </tr>
  </tbody>
</table>

### RecursosDePlanoDePessoal

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>custoEstimadoTotal</b>
            </p>
            <p>Adicionado</p>
              </li>
         <li>
            <p><b>totalEstimatedHours</b>
            </p>
            <p>Adicionado</p>
              </li>
         <li>
            <p><b>totalEstimatedRevenue</b>
            </p>
            <p>Adicionado</p>
              </li>
            </ul>
         </li>
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
            <p><b>TrabalhoRequeridoDuplo</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>atribuiçõesDeEquipe</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>

### Equipe

O objeto Equipe adicionou os sinalizadores `DATA_EXTENDIBLE` e `SHARABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>categoryID</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>
        <ul>
          <li>
            <p><b>categoria</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>objectCategories</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


### AtribuiçãoModelo

O objeto TemplateAssignment adicionou o sinalizador `ATTRIBUTE_ATTACHABLE`.

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
            <p><b>TrabalhoRequeridoDuplo</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>atribuiçõesDeEquipe</b>
            </p>
            <p>Adicionado</p>
          </li>
      </td>
    </tr>
  </tbody>
</table>


