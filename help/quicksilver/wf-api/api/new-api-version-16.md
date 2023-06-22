---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 16
description: O Adobe Workfront lançou a API versão 16 em 6 de abril de 2022. A API versão 16 apresenta as seguintes alterações da versão 15.
author: Becky
feature: Workfront API
exl-id: a3d8534b-fe6e-4782-baab-7c94555ea40c
source-git-commit: 3e6f4b8c8bfb9cb6106dbb9522d77f5133a886e3
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Novidades da API versão 16

O Adobe Workfront lançou a API versão 16 em 6 de abril de 2022. A API versão 16 apresenta as seguintes alterações da versão 15.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 16.

## Recursos removidos

Nenhum recurso foi removido para a API versão 16

## Recursos modificados

<!--* [AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Aprovação (APPROVAL)](#approval-approval)
* [Preferências do cliente (CUSTPR)](#customerpreferences-custpr)
* [ExternalSection (EXTSEC)](#externalsection-extsec)
* [Hora (HORA)](#hour-hour)
* [Modelo de layout (UITMPL)](#layouttemplate-uitmpl)
* [Nota (NOTA)](#note-note)
* [OpTask/Problema (OPTASK)](#note-note)
* [Projeto (PROJ)](#project-proj)
* [Taxa (RATE)](#rate-rate)
* [RichTextNote (Nota)](#richtextnote-rhnote)
* [Função/Função (ROLE)](#role--job-role-role)
* [Tarefa (TASK)](#task-task)
* [Planilha de horas (TSHET)](#timesheet-tshet)
* [UIFilter / Filtro (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Agrupamento (UIGB)](#uigroupby--grouping-uigb)
* [UIView / Visualização (UIVW)](#uiview--view-uivw)
* [Usuário (USER)](#user-user)
* [Nota de Usuário (USRNOT)](#usernote-usrnot)

<!--

### AccessLevel (ACSLVL)

An AccessLevel object is associated with users, and describes the set of AccessLevelPermissions that determine what the user can access.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

-->

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
            <p><b>workPerDate</b>
            </p>
            <p>Este campo foi adicionado e mostra quantos minutos de trabalho por dia são necessários. Tem o formato <code>YYYY-MM-DD: (number of minutes)</code>, e considera o fuso horário.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Atribuição (ASSGN)

Um objeto de atribuição representa a conexão entre um item de trabalho e o usuário, equipe ou grupo atribuído para trabalhar nele.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Este campo foi adicionado e mostra quantos minutos de trabalho por dia são necessários. Tem o formato <code>YYYY-MM-DD: (number of minutes)</code>, e considera o fuso horário.</p>
          </li>
          <li>
            <p><b>isContoured</b>
            </p>
            <p>Este campo foi adicionado, e é um booleano que reflete se a atribuição está com contorno. Se os minutos por dia da atribuição tiverem sido editados no Balanceador de carga de trabalho, a atribuição terá sido contornada.</p>
          </li>
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
      <td>
        <ul>
          <li>
            <p><b>getDefaultProjectStatusEnumForGroup
</b>
            </p>
            <p></p>
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
            <p>Foram adicionados os seguintes valores possíveis:</p>
            <ul>
              <li>
                <p><code>customer:config.general.autoupgradedisabled</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ações</td>
      <td>
        <ul>
          <li>
            <p><b>getIsAutoUpgradeDisabled</b>
            </p>
            <p>Esta ação retorna um valor booleano que descreve se o cliente desativou a opção de atualizar automaticamente os titulares da licença do Colaborador.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### ExternalSection (EXTSEC)

Um objeto ExternalSection é uma página externa da Web incorporada em um relatório do Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">ações</td>
      <td>
        <ul>
           <li>
            <p><b>calculateIframeURL</b>
            </p>
            <p>Ele foi adicionado e calcula o URL de um iFrame incorporado em um relatório.</p>
         </li>
          <li>
            <p><b>calculateIframeURLS</b>
            </p>
            <p>Isso foi adicionado e calcula os URLs de iFrames incorporados em um relatório.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>timesheetHourIdentifier</b>
            </p>
            <p>Adicionado. Este parâmetro é usado para identificar as horas criadas com <code>batchSave</code>. </p>
           </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

<!--

### LayoutTemplate (UITMPL)

Adobe Workfront administrators or group administrators can create templates to customize the layout elements in Adobe Workfront. A LayoutTemplate object represents one of these templates.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>licenseType</b>
            </p>
            <p>Added the following possible values:</p>
            <ul>
              <li>
                <p><code>x</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
-->

### Nota (NOTA)

Um objeto Note é um comentário ou uma atualização feita em um objeto Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>anexadosDocumentos</b>
            </p>
            <p>Este campo foi adicionado e representa uma lista de documentos anexados ao comentário.</p>
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
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>workPerDate</b>
            </p>
            <p>Este campo foi adicionado e mostra quantos minutos de trabalho por dia são necessários. Tem o formato <code>YYYY-MM-DD: (number of minutes)</code>, e considera o fuso horário.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ações</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Essa ação adicionou o campo <code>teamIDs</code> para oferecer suporte à funcionalidade de atribuir várias equipes a uma tarefa ou problema.</p>
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
            <p>Este campo foi adicionado e representa a soma de todas as horas orçadas no projeto.</p>
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
             <p><b>costPerHour</b></p>
            <p><b>LocalBillingPerHour</b></p>
            <p><b>localCostPerHour</b></p>
            <p><b>localCurrency</b></p>
           <p>Esses parâmetros foram movidos do objeto Função para o objeto Taxa, de modo que os objetos Função e Usuário possam ter vários valores (para intervalos de datas separados).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Esses parâmetros representam a ID e o código do objeto ao qual a Taxa está anexada.
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Ações</td>
      <td>
        <ul>
          <li>
             <p><b>setRateForObject</b></p>
           <p>Esta ação foi adicionada e anexa objetos Taxa ao objeto fornecido. Esse endpoint funciona para todos os objetos de Taxa Anexável.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (Nota)

Um objeto RichTextNote é um comentário ou uma atualização feita em um objeto do Workfront, que inclui rich text, como negrito ou itálico.

O objeto RichTextNote removeu o sinalizador `REPORTABLE`.

### Função/Função (ROLE)

Um objeto Função (função de trabalho) representa uma capacidade funcional ou um conjunto de habilidades que um usuário pode preencher, como Designer ou Gerente de produto.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
           <li>
            <p><b>taxas</b>
            </p>
            <p>Foi adicionado e representa os objetos de Taxa anexados a esta função.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>Este campo foi adicionado e mostra quantos minutos de trabalho por dia são necessários. Tem o formato <code>YYYY-MM-DD: (number of minutes)</code>, e considera o fuso horário.</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ações</td>
      <td>
        <ul>
           <li>
            <p><b>assignMultiple</b>
            </p>
            <p>Essa ação adicionou o campo <code>teamIDs</code> para oferecer suporte à funcionalidade de atribuir várias equipes a uma tarefa ou problema.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>availableActions</b>
            </p>
            <p>Esse parâmetro removeu o sinalizador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Esse parâmetro removeu o sinalizador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Esse parâmetro foi adicionado e armazena a duração da folha de horas em dias, independentemente das alterações em "Horas equivalentes para Full Workday".  Por exemplo, se Equivalent Hours (Horas equivalentes) estiver definido como 6 e um dia for registrado, então Equivalent Hours (Horas equivalentes) será alterado para 8 hours (8 horas), <code>totalDays</code> ainda tem um valor de 1.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIFilter / Filtro (UIFT)



<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">ações</td>
      <td>
        <ul>
          <li>
            <p><b>addJoinForNullableFields</b>
            </p>
            <p>Esta ação foi adicionada, pega um mapa de consulta de filtro e adiciona o <code>allowingnull</code> junte-se para campos anuláveis.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Essas ações oferecem suporte à capacidade de compartilhar filtros, visualizações e agrupamentos em todo o sistema.</p><p>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Disponibilizar filtros, visualizações ou agrupamentos a todos os usuários</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Agrupamento (UIGB)


<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">ações</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Essas ações oferecem suporte à capacidade de compartilhar filtros, visualizações e agrupamentos em todo o sistema.</p><p>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Disponibilizar filtros, visualizações ou agrupamentos a todos os usuários</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / Visualização (UIVW)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos diretos</td>
      <td>
        <ul>
          <li>
            <p><b>layoutType</b>
            </p>
            <p>Adição do seguinte valor possível:</p>
            <ul>
              <li>
                <p><code>WLIST</code></p>
              </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">ações</td>
      <td>
        <ul>
          <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Essas ações oferecem suporte à capacidade de compartilhar filtros, visualizações e agrupamentos em todo o sistema.</p><p>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Disponibilizar filtros, visualizações ou agrupamentos a todos os usuários</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Usuário (USER)

Um objeto Usuário representa uma pessoa com uma conta no Workfront que pode fazer logon e interagir com o sistema.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
           <li>
            <p><b>taxas</b>
            </p>
            <p>Ele foi adicionado e representa os objetos de Taxa anexados a esse usuário.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Nota de Usuário (USRNOT)

Um objeto UserNote é uma notificação.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Consultas</td>
      <td>
        <ul>
          <li>
            <p><b>myAllObjectTypesUnreadNotifications</b>
            </p>
            <p>Adição do seguinte valor possível:
            <ul>
            <li>
            includeAll
            </li>
            </ul>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
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
            <p><b>workPerDate</b>
            </p>
            <p>Este campo foi adicionado e mostra quantos minutos de trabalho por dia são necessários. Tem o formato <code>YYYY-MM-DD: (number of minutes)</code>, e considera o fuso horário.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
