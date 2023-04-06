---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 16
description: A Adobe Workfront lançou a API versão 16 em 6 de abril de 2022. A API versão 16 apresenta as seguintes alterações da versão 15.
author: Becky
feature: Workfront API
source-git-commit: 19978aaa2886008afc3c0faa9cfd18bd7c4b2555
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Novidades da API versão 16

A Adobe Workfront lançou a API versão 16 em 6 de abril de 2022. A API versão 16 apresenta as seguintes alterações da versão 15.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 16.

## Recursos removidos

Nenhum recurso foi removido para a API versão 16

## Recursos modificados

* <!--[AccessLevel (ACSLVL)](#accesslevel-acslvl)-->
* [Homologação (APROVAÇÃO)](#approval-approval)
* [Preferências do cliente (CUSTPR)](#customerpreferences-custpr)
* [Seção Externa (EXTSEC)](#externalsection-extsec)
* [Hora (HORA)](#hour-hour)
* [Modelo de layout (UITMPL)](#layouttemplate-uitmpl)
* [Nota (OBSERVAÇÃO)](#note-note)
* [OpTask / Problema (OPTASK)](#note-note)
* [Projeto (PROJ)](#project-proj)
* [Taxa (TAXA)](#rate-rate)
* [RichTextNote (NOTA)](#richtextnote-rhnote)
* [Função / Função de trabalho (FUNÇÃO)](#role--job-role-role)
* [Tarefa (TAREFA)](#task-task)
* [Folha de Horas (TSHET)](#timesheet-tshet)
* [UIFilter / Filtro (UIFT)](#uifilter--filter-uift)
* [UIGroupBy / Grouping (UIGB)](#uigroupby--grouping-uigb)
* [UIView / View (UIVW)](#uiview--view-uivw)
* [Usuário (USUÁRIO)](#user-user)
* [UserNote (USRNOT)](#usernote-usrnot)

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

### Homologação (APROVAÇÃO)

Um determinado item de trabalho, como uma tarefa, documento ou folha de ponto, pode exigir que um supervisor ou outro usuário faça logoff no item de trabalho. Um objeto Approval representa a ação de desconectar-se em um item de trabalho.

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
            <p>Este campo foi adicionado e mostra o número de minutos de trabalho por dia que você precisa fazer. Ele tem o formato <code>YYYY-MM-DD: (number of minutes)</code>e considera o fuso horário.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Atribuição (ASSGN)

Um objeto de atribuição representa a conexão entre um item de trabalho e o usuário, a equipe ou o grupo atribuído para trabalhar nele.

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
            <p>Este campo foi adicionado e mostra o número de minutos de trabalho por dia que você precisa fazer. Ele tem o formato <code>YYYY-MM-DD: (number of minutes)</code>e considera o fuso horário.</p>
          </li>
          <li>
            <p><b>isContered</b>
            </p>
            <p>Este campo foi adicionado e é um booleano que reflete se a atribuição está contida. Se os minutos da atribuição por dia tiverem sido editados no Balanceador de Carga de Trabalho, a atribuição terá sido contornada.</p>
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
            <p>Os seguintes valores possíveis foram adicionados:</p>
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
            <p>Essa ação retorna um booleano que descreve se o cliente desabilitou a opção de atualizar automaticamente os titulares de licenças do Contribuidor.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Seção Externa (EXTSEC)

Um objeto ExternalSection é uma página da Web externa incorporada em um relatório do Workfront.

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
            <p>Isso foi adicionado e calcula o URL de um iFrame incorporado em um relatório.</p>
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

Um objeto Hora representa uma hora registrada por um usuário em uma folha de ponto.

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
            <p>Adicionado. Esse parâmetro é usado para identificar as horas criadas com <code>batchSave</code>. </p>
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

### Nota (OBSERVAÇÃO)

Um objeto Nota é um comentário ou atualização feito em um objeto Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos de coleção</td>
      <td>
        <ul>
          <li>
            <p><b>AttachedDocuments</b>
            </p>
            <p>Este campo foi adicionado e representa uma lista de documentos anexados ao comentário.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### OpTask / Problema (OPTASK)

Um objeto OpTask é normalmente conhecido como um problema. Um problema é um item de trabalho que geralmente indica que há um problema que impede a conclusão de uma tarefa ou projeto. Um problema também pode ser uma solicitação de suporte técnico. Pedidos de alteração, solicitações e bugs também são problemas.

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
            <p>Este campo foi adicionado e mostra o número de minutos de trabalho por dia que você precisa fazer. Ele tem o formato <code>YYYY-MM-DD: (number of minutes)</code>e considera o fuso horário.</p>
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
            <p>Esta ação adicionou o campo <code>teamIDs</code> para dar suporte à funcionalidade de atribuir várias equipes a uma tarefa ou problema.</p>
         </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Projeto (PROJ)

Os projetos são itens de trabalho no Workfront e são um elemento essencial na maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Project representa um grupo de tarefas com um objetivo comum e específico.

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
            <p>Este campo foi adicionado e representa a soma de todas as Horas Orçadas no projeto.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### Taxa (TAXA)

Um objeto Rate representa uma taxa de faturamento no Workfront.

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
           <p>Esses parâmetros foram movidos para o objeto Rate a partir do objeto Role , de modo que os objetos Role e User possam ter vários valores (para intervalos de datas separados).</p>
          </li>
          <li><p><b>objID</b></p><p><b>objObjCode</b></p>
          <p>Esses parâmetros representam a ID e o código do objeto ao qual a Taxa é anexada.
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
           <p>Essa ação foi adicionada e anexa os objetos Rate ao Objeto especificado. Esse ponto de extremidade funciona para todos os objetos de Taxa anexável.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>

### RichTextNote (NOTA)

Um objeto RichTextNote é um comentário ou atualização feito em um objeto Workfront, que inclui rich text, como negrito ou itálico.

O objeto RichTextNote removeu o sinalizador `REPORTABLE`.

### Função / Função de trabalho (FUNÇÃO)

Um objeto de Função (função de trabalho) representa uma capacidade funcional ou um conjunto de habilidades que um usuário pode preencher, como o Designer ou o Gerenciador de Produtos.

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
            <p>Isso foi adicionado e representa os objetos Rate anexados a essa função.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Tarefa (TAREFA)

Um objeto Task representa um item de trabalho que deve ser executado como uma etapa para atingir uma meta final (conclusão de um projeto).

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
            <p>Este campo foi adicionado e mostra o número de minutos de trabalho por dia que você precisa fazer. Ele tem o formato <code>YYYY-MM-DD: (number of minutes)</code>e considera o fuso horário.</p>
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
            <p>Esta ação adicionou o campo <code>teamIDs</code> para dar suporte à funcionalidade de atribuir várias equipes a uma tarefa ou problema.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### Folha de Horas (TSHET)

Um objeto de Folha de Horas representa um cartão de ponto virtual que permite que os usuários insiram horas reais trabalhadas para Tarefas, Projetos e Tipos de Horário de Custo.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Campos Diretos</td>
      <td>
        <ul>
           <li>
            <p><b>availableActions</b>
            </p>
            <p>Este parâmetro removeu o sinalizador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>isEditable</b>
            </p>
            <p>Este parâmetro removeu o sinalizador <code>READ_ONLY</code>.</p>
         </li>
           <li>
            <p><b>totalDays</b>
            </p>
            <p>Esse parâmetro foi adicionado e armazena a duração das folhas de horas em dias, independentemente das alterações em "Horas equivalentes para Workday completo".  Por exemplo, se Horas Equivalentes for definido como 6 e um dia for registrado, Horas Equivalentes será alterado para 8 horas, <code>totalDays</code> O ainda tem um valor de 1.</p>
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
            <p><b>addJoinForNullabelFields</b>
            </p>
            <p>Essa ação foi adicionada e obtém um mapa de consulta de filtro e adiciona a variável <code>allowingnull</code> unir para campos que podem ser nulos.</p>
         </li>
         <li>
            <p><b>disableSystemWideVisibility
</b>
            </p>
            <p><b>enableSystemWideVisibility </b>
            </p>
            <p>Essas ações oferecem suporte à capacidade de compartilhar filtros, visualizações e agrupamentos em todo o sistema.</p><p>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Disponibilizar filtros, visualizações ou agrupamentos para todos os usuários</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UIGroupBy / Grouping (UIGB)


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
            <p>Essas ações oferecem suporte à capacidade de compartilhar filtros, visualizações e agrupamentos em todo o sistema.</p><p>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Disponibilizar filtros, visualizações ou agrupamentos para todos os usuários</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>


### UIView / View (UIVW)

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
            <p>Essas ações oferecem suporte à capacidade de compartilhar filtros, visualizações e agrupamentos em todo o sistema.</p><p>Para obter mais informações, consulte <a href="https://experienceleague.adobe.com/docs/workfront/using/administration-and-setup/set-up-wf/configure-system-defaults/create-and-share-default-fvgs.html?lang=en#make-filters-views-or-groupings-available-to-users">Disponibilizar filtros, visualizações ou agrupamentos para todos os usuários</a>.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### Usuário (USUÁRIO)

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
            <p>Isso foi adicionado e representa os objetos Rate anexados a esse usuário.</p>
         </li>
        </ul>
      </td>
    </tr>  </tbody>
</table>

### UserNote (USRNOT)

Um objeto UserNote é uma notificação.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Queries</td>
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

### Trabalho (TRABALHO)

Um objeto de trabalho é uma interface comum que Tarefa e OpTask herdam e compartilha um código comum entre os dois.

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
            <p>Este campo foi adicionado e mostra o número de minutos de trabalho por dia que você precisa fazer. Ele tem o formato <code>YYYY-MM-DD: (number of minutes)</code>e considera o fuso horário.</p>
          </li>
        </ul>
      </td>
    </tr>
 </tbody>
</table>
