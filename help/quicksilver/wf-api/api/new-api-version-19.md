---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 19
description: O Adobe Workfront lançou a API versão 19 em 6 de abril de 2022. A API versão 19 apresenta as seguintes alterações da versão 18.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 13910328903744aa9bf619e8b4c376520c21b89e
workflow-type: tm+mt
source-wordcount: '970'
ht-degree: 0%

---

# Novidades da API versão 19

A Adobe Workfront lançou a API versão 19 em 8 de abril de 2024. A API versão 19 apresenta as seguintes alterações da versão 18.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 19.

## Recursos removidos

Nenhum recurso foi removido para a API versão 19

## Recursos modificados

### AccessLevel (ACSLVL)

Um objeto AccessLevel está associado a usuários e descreve o conjunto de AccessLevelPermissions que determinam o que o usuário pode acessar.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>accessRestrictions</b><p>Foram adicionados os seguintes valores possíveis:
            </p>
            <ul>
              <li>
                <p>Desative o Workfront AI Assistant (AIOFF)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Atribuição (ASSGN)

Um objeto Atribuição representa a conexão entre um item de trabalho e o usuário, equipe ou grupo atribuído para trabalhar nele.

O objeto Assignment adicionou o sinalizador **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Foram adicionados os seguintes campos diretos:
        <ul>
          <li>
            <p><b>categoryID</b><p>Uma categoria é um formulário personalizado. Este campo oferece suporte à capacidade de adicionar um formulário personalizado a uma atribuição.
            </p>
          </li>
          <li>
            <p><b>prioridade</b><p>Esse campo permite os seguintes valores:
            <ul>
              <li>0 (Nenhum)</li>
              <li>1 (Baixo)</li>
              <li>2 (Normal)</li>
              <li>3 (Alto)</li>
              <li>4 (Urgente)</li>
             </ul>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>Foram adicionados os seguintes campos de referência:
        <ul>
          <li>
            <p><b>categoria</b><p>Uma categoria é um formulário personalizado. Este campo oferece suporte à capacidade de adicionar um formulário personalizado a uma atribuição.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>Foram adicionados os seguintes campos de coleção:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Uma categoria é um formulário personalizado. Este campo oferece suporte à capacidade de adicionar um formulário personalizado a uma atribuição.
            </p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



### Categoria (CTGY)

Um objeto de Categoria é um formulário personalizado.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Os campos a seguir foram adicionados para oferecer suporte à capacidade de adicionar um formulário personalizado a uma atribuição.
        <ul>
          <li>
            <p><b>catObjCode</b><p>Foram adicionados os seguintes valores possíveis:
            </p>
            <ul>
              <li>
                <p>Atribuição (ASSGN)
                </p>
              </li>
             </ul>
          </li>
          <li>
            <p><b>objTypes</b><p>Foram adicionados os seguintes valores possíveis:
            </p>
            <ul>
              <li>
                <p>Atribuição (ASSGN)
                </p>
              </li>
             </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Classificador (CLSF)

Um classificador é um local.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>Foram adicionadas as seguintes ações:
        <ul>
          <li>
            <b>ativateClassifiers</b>
          </li>
          <li>
            <b>deactivateClassifiers</b>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Cliente

Um objeto Customer representa uma organização que usa uma instância do Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>customEnumTypes</b><p>Foram adicionados os seguintes valores possíveis:
            </p>
            <ul>
              <li>
                <p>Prioridades de Atribuição (PRIORITY_ASSIGNMENT)
                </p>
              </li>
             </ul>
          </li>
              <p>O objeto CustomEnum auxilia na conversão de códigos de status em texto legível.</p>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Preferências do cliente (CUSTPR)

Um objeto CustomerPreferences representa o conjunto de preferências que um cliente definiu para sua instância do Workfront.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>name</b><p>Os seguintes valores possíveis foram removidos:
            </p>
            <ul>
              <li>
                <p>Habilitar a integração do Zoom no fluxo de atualizações (password:zoomIntegrationEnabled)
                </p>
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
  <tbody>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
            <p><b>createLargeDocument</b><p>Adição do campo <code>folderID</code>.</p>
          </li>
          <li>
            <p><b>sendDocumentsToExternalProvider</b><p>Adição de.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


### Taxa de Câmbio (EXRATE)

Um objeto ExchangeRate representa uma taxa de câmbio de moeda configurada no Workfront. Os objetos ExchangeRate não são dinâmicos.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
      <ul>
      <li>Os seguintes campos adicionaram o validador <code>REQUIRED</code>:
        <ul>
          <li><p><b>moeda</b></li>
          <li><p><b>taxa</b></li></ul>
      <li>Os seguintes campos foram adicionados:
        <ul>
          <li><p><b>enteredByID</b></li>
          <li><p><b>entryDate</b></li>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>
      <ul>
        <li>Os seguintes campos foram adicionados:
        <ul>
          <li><p><b>enteredBy</b></li>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Grupo (GRUPO)

Um objeto Grupo representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

O objeto Group adicionou o sinalizador **SHARABLE**.

### Hora (HORA)

Um objeto Hour representa uma hora registrada por um usuário em uma folha de horas.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
      Os seguintes campos foram adicionados:
        <ul>
          <li><p><b>assignedApproverID</b></li>
          <li><p><b>isBillable</b></li>
          <li><p><b>isBilled</b></li>
          <li><p><b>rejectedByID</b></li>
          <li><p><b>rejectedOnDate</b></li>
          <li><p><b>rejectionComment</b></li>
          <li><p><b>submitByID</b></li>
          </ul>
          <p>As alterações a seguir foram feitas no campo <b>horas</b>.</p>
          <ul> 
          <li> Validador <b>GREATER_THAN</b> removido</li>
          <li> Validador adicionado <b>NOT_EQUAL</b></li>
          </ul>
     </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
      As seguintes ações foram adicionadas:
        <ul>
          <li><p><b>aprovar</b></li>
          <li><p><b>cancelar aprovação</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### JournalEntry (JRNLE)

O objeto JournalEntry pode ser configurado para registrar informações sobre campos de objeto específicos sempre que esses campos forem modificados. Quando um campo é configurado para ser registrado como parte do objeto de Entrada de diário, uma Entrada de diário correspondente será criada toda vez que o campo for modificado.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>sinalizadores</b><p>Foram adicionados os seguintes valores possíveis:
            </p>
            <ul>
              <li>
                <p>É taxa de custo (CR)
                </p>
              </li>
              <li>
                <p>É taxa de cobrança (BR)
                </p>
              </li>
              <li>
                <p>É financiamento geral (GF)
                </p>
              </li>
              <li>
                <p>É financiamento combinado (FC)
                </p>
              </li>
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
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>dataType</b></p><p>Adição do seguinte valor possível:
            <ul>
            <li>Duração (DRTN)</li>
            </ul>
          </li>
          <li>
            <p><b>displayType</b></p><p>Para criar um sistema mais simples e flexível, o tipo de campo <b>Widget (WIDGET)</b> foi descontinuado e dividido nos seguintes tipos de campos:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Imagem (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Vídeo (VÍDEO)</li>
            <li>Pesquisa externa (EXTRNL)</li>
            <li>Pesquisa Externa de Seleção Múltipla (MULTEXTRNL)</li>
            <li>Campo nativo (WFNATIVE)</li>
            <li>Campo de Planejamento (WFPLANNING)</li>
            <li>KPI distribuído no tempo (TIMEPHASED)</li>
            <li>Acúmulo (ROLLUP)</li>
            <li>Documentos (DOCUMENTO)</li>
           </ul>
          </li>
          <li>
            <p><b>configurações</b><p>Adição de.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>

### Função (ROLE)

Um objeto Função (função de trabalho) representa uma capacidade funcional ou um conjunto de habilidades que um usuário pode preencher, como Designer ou Gerente de produto.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
    Os seguintes campos foram adicionados:
        <ul>
          <li><p><b>lastUpdateDate</b></li>
          <li><p><b>lastUpdatedByID</b></li>
          </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>
        Os seguintes campos foram adicionados:
        <ul>
          <li><p><b>lastUpdatedBy</b></li>
          </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion {#scorecardquestion}

Um objeto ScoreCardQuestion representa uma pergunta que foi adicionada a um Scorecard. Essas perguntas geralmente são determinadas pelo gerente de Portfolio, e suas respostas permitem que o gerente entenda como um projeto se alinha com as metas do portfólio.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
            <p><b>displayType</b></p><p>Para criar um sistema mais simples e flexível, o tipo de campo <b>Widget (WIDGET)</b> foi descontinuado e dividido nos seguintes tipos de campos:
            <ul>
            <li>Adobe XD (ADOBEXD)</li>
            <li>Imagem (IMAGE)</li>
            <li>PDF (PDF)</li>
            <li>Vídeo (VÍDEO)</li>
            <li>Pesquisa externa (EXTRNL)</li>
            <li>Pesquisa Externa de Seleção Múltipla (MULTEXTRNL)</li>
            <li>Campo nativo (WFNATIVE)</li>
            <li>Campo de Planejamento (WFPLANNING)</li>
            <li>KPI distribuído no tempo (TIMEPHASED)</li>
            <li>Acúmulo (ROLLUP)</li>
            <li>Documentos (DOCUMENTO)</li>
           </ul>
      </td>
  </tbody>
</table>

### Atribuição de modelo (TASGN)

Um objeto TemplateAssignment representa a conexão entre uma tarefa de modelo e o usuário, a equipe ou o grupo atribuído para trabalhar nela. Quando o modelo é usado para um projeto, esse usuário, equipe ou grupo é atribuído à tarefa.

O objeto TemplateAssignment adicionou o sinalizador **DATA_EXTENDIBLE**.

<table>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>Foram adicionados os seguintes campos diretos:
        <ul>
          <li>
            <p><b>categoryID</b><p>Uma categoria é um formulário personalizado. Este campo oferece suporte à capacidade de adicionar um formulário personalizado a uma atribuição.
            </p>
          </li>
        </ul>
      </td>
    <tr>
      <td role="rowheader">Campos de referência</td>
      <td>Foram adicionados os seguintes campos de referência:
        <ul>
          <li>
            <p><b>categoria</b><p>Uma categoria é um formulário personalizado. Este campo oferece suporte à capacidade de adicionar um formulário personalizado a uma atribuição.
            </p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>Foram adicionados os seguintes campos de coleção:
        <ul>
          <li>
            <p><b>objectCategories</b><p>Uma categoria é um formulário personalizado. Este campo oferece suporte à capacidade de adicionar um formulário personalizado a uma atribuição.
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
  <tbody>
    <tr>
      <td role="rowheader">Campos principais</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b></p><p>Removido.</p>
          </li>
        </ul>
      </td>
  </tbody>
</table>


