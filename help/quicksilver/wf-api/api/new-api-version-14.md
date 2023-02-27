---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 14
description: A Adobe Workfront lançou a API versão 14 em 9 de setembro de 2021. A API versão 14 apresenta as seguintes alterações da versão 14.
author: Becky
feature: Workfront API
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 2%

---

# Novidades da API versão 14

A Adobe Workfront lançou a API versão 14 em 9 de setembro de 2021. A API versão 14 apresenta as seguintes alterações da versão 14.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 14.

## Recursos removidos

Nenhum recurso foi removido para a API versão 14.

## Recursos modificados

Os recursos a seguir foram modificados para a API versão 14.

* [Registro de Faturamento (BILL)](#billingrecord-bill)
* [Categoria (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Cliente (CUST)](#customer-cust)
* [Preferências do cliente (CUSTPR)](#customerpreferences-custpr)
* [DocumentVersion (DOCV)](#documentversion-docv)
* [Grupo (GRUPO)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Projeto (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Alocação de Recursos (RSALLO)](#resource-allocation-rsallo)
* [Função (FUNÇÃO)](#role-role)
* [Modelo (TMPL)](#template-tmpl)
* [Folha de Horas (TSHET)](#timesheet-tshet)

### Registro de Faturamento (BILL) {#billingrecord-bill}

Um objeto BillingRecord registra a receita, as horas ou as despesas que podem ser faturadas. Essas informações podem ser usadas para criar faturas em um sistema de contabilidade externo.

Para obter mais informações sobre registros de faturamento, consulte [Criar registros de faturamento](../../manage-work/projects/project-finances/create-billing-records.md).

O objeto BillingRecord adicionou o sinalizador **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Campos Diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Adicionado. Uma Categoria é um Formulário personalizado. Esse parâmetro foi adicionado para oferecer suporte à capacidade de adicionar Forms personalizado a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referência</td> 
   <td> 
    <ul> 
     <li> <p><b>categoria</b> </p> <p>Adicionado. Uma Categoria é um formulário personalizado. Esse parâmetro foi adicionado para oferecer suporte à capacidade de adicionar formulários personalizados a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de coleção</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Adicionado. Representa uma coleção de Categorias (formulários personalizados) associadas ao objeto BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Adicionado. Essa ação recalcula as expressões em campos de formulário personalizados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoria (CTGY) {#category-ctgy}

Um objeto Category é um formulário personalizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos Diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Valor possível adicionado:</p> 
      <ul> 
       <li> <p> BILL (Registro de Faturamento)</p> </li> 
      </ul> <p>Esse valor foi adicionado para oferecer suporte à capacidade de adicionar formulários personalizados a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Essa ação obtém os parâmetros objID e objCode, e retorna um booleano.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### CustomEnum (CSTEM) {#customenum-cstem}

O objeto CustomEnum auxilia na conversão de códigos de status em texto legível.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Queries</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatus</b> </p> <p>Adicionado. Esta consulta oferece suporte à capacidade de criar e gerenciar status para grupos e subgrupos. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Gerenciar status de grupo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente (CUST) {#customer-cust}

Um objeto Cliente representa uma organização que usa uma instância do Workfront.

Este é um objeto interno.

### Preferências do cliente (CUSTPR) {#customerpreferences-custpr}

Um objeto CustomerPreferences representa o conjunto de preferências que um cliente definiu para sua instância do Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos Diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>name</b> </p> <p>Valor possível adicionado:</p> 
      <ul> 
       <li> <p>Permitir que usuários adicionem imagens em atualizações (atualizações:imagens.toggle)</p> </li> 
      </ul> <p>Esse parâmetro suporta a capacidade de adicionar imagens em atualizações de itens de trabalho. </p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### DocumentVersion (DOCV) {#documentversion-docv}

Um objeto DocumentVersion representa uma versão específica de um arquivo (como material gravado, imagens ou outras formas de informações).

Para obter mais informações sobre versões de documentos, consulte [Fazer upload de uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos Diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Adicionado. Este campo registra a data e a hora do último retorno de chamada da Workfront Proof, se a versão estiver associada a uma prova.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo (GRUPO) {#group-group}

Um objeto Group representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

Para obter mais informações sobre grupos, consulte [Grupos versus equipes no Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>addSubgroups</b> </p> <p>Adicionado. Essa ação obtém uma matriz de groupIDs e adiciona esses grupos como subgrupos ao grupo especificado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

Um objeto NoteTag representa o ato de marcar um usuário ou equipe em uma atualização de um item de trabalho.

Para obter mais informações sobre marcação em atualizações, consulte [Marcar outras pessoas em atualizações](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Operações</td> 
   <td> <p>As seguintes operações foram adicionadas ao objeto NoteTag :</p> 
    <ul> 
     <li> <p><b>CONTAGEM</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>RELATÓRIO</b> </p> </li> 
     <li> <p><b>SEARCH</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projeto (PROJ) {#project-proj}

Os projetos são itens de trabalho no Workfront e são um elemento essencial na maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Project representa um grupo de tarefas com um objetivo comum e específico.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Adicionado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Um objeto QueueDef representa uma Fila, que é um projeto que foi publicado na área Help Desk para permitir que os usuários enviem problemas para ela.

Para obter mais informações sobre as filas de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>searchByPath</b> </p> <p>Adicionado. Essa ação oferece suporte à capacidade de localizar solicitações usando o caminho pela fila de solicitações e grupos de tópicos.</p> <p>Para obter mais informações sobre como pesquisar filas de solicitações por caminho, consulte <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Criar solicitações e gerar rascunhos no aplicativo Web do Workfront</a> em <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Criar e enviar solicitações do Adobe Workfront</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Alocação de Recursos (RSALLO) {#resource-allocation-rsallo}

Um objeto Alocação de Recursos representa a estimativa de recursos necessários para um determinado projeto. Esse objeto é usado somente no Planejador de Recursos herdado. Para o campo correspondente no novo Planejador de Recursos, use Hora Orçada (BGHR).

O objeto Alocação de Recursos removeu o sinalizador **REPORTABLE**.

### Função (FUNÇÃO) {#role-role}

Um objeto de Função (função de trabalho) representa uma capacidade funcional ou um conjunto de habilidades que um usuário pode preencher, como o Designer ou o Gerenciador de Produtos.

Para obter informações sobre funções de job, consulte [Visão geral da função de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos Diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado. Este é um parâmetro booleano que tem um valor true se um objeto for Ative e false caso contrário. Os objetos definidos como Ativo são exibidos nos menus suspensos e nos campos do tipo avançar e podem ser anexados a outros objetos.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos padrão</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adicionado</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Modelo (TMPL) {#template-tmpl}

Um objeto Modelo representa um padrão para um projeto. Os projetos podem ser criados a partir de modelos para economizar tempo. Um modelo contém uma equipe e tarefas, que serão copiadas para qualquer projeto criado a partir do modelo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos Diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Adicionado. Este campo foi adicionado para oferecer suporte à capacidade de associar grupos a modelos.</p> <p style="font-weight: normal;">Para obter mais informações, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar modelos de projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">Adicionado. Este campo foi adicionado para oferecer suporte à capacidade de associar grupos a modelos.</p> <p style="font-weight: normal;">Para obter mais informações, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar modelos de projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><strong>Timesheet (TSHET)</strong></p>
<p>A&nbsp;Timesheet object represents a virtual timecard that allows users to enter actual hours worked for tasks, projects, and overhead hour types.</p>
<p>For more information, see <a href="../../timesheets/timesheets/timesheets-overview.md" class="MCXref xref">Timesheets overview</a>.</p>
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">Core Fields</td>
<td>
<ul>
<li> <p><b>objCode</b> </p> <p>Removed.</p> </li>
</ul> </td>
</tr>
</tbody>
</table>
</div>
-->
