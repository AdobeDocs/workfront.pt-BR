---
content-type: api
navigation-topic: api-navigation-topic
title: Novidades da API versão 14
description: O Adobe Workfront lançou a API versão 14 em 9 de setembro de 2021. A API versão 14 apresenta as seguintes alterações da versão 14.
author: Becky
feature: Workfront API
role: Developer
exl-id: eca5d1cc-6348-445c-be84-c0a29f15980d
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '891'
ht-degree: 0%

---

# Novidades da API versão 14

O Adobe Workfront lançou a API versão 14 em 9 de setembro de 2021. A API versão 14 apresenta as seguintes alterações da versão 14.

## Recursos adicionados

Nenhum recurso foi adicionado para a API versão 14.

## Recursos removidos

Nenhum recurso foi removido para a API versão 14.

## Recursos modificados

Os recursos a seguir foram modificados para a API versão 14.

* [RegistroDeCobrança (BILL)](#billingrecord-bill)
* [Categoria (CTGY)](#category-ctgy)
* [CustomEnum (CSTEM)](#customenum-cstem)
* [Cliente (CUST)](#customer-cust)
* [PreferênciasDoCliente (CUSTPR)](#customerpreferences-custpr)
* [VersãoDocumento (DOCV)](#documentversion-docv)
* [Grupo (GRUPO)](#group-group)
* [NoteTag (NTAG)](#notetag-ntag)
* [Projeto (PROJ)](#project-proj)
* [QueueDef (QUED)](#queuedef-qued)
* [Alocação de recursos (RSALLO)](#resource-allocation-rsallo)
* [Função (ROLE)](#role-role)
* [Modelo (TMPL)](#template-tmpl)
* [Planilha de horas (TSHET)](#timesheet-tshet)

### Registro de Cobrança (BILL) {#billingrecord-bill}

Um objeto BillingRecord registra a receita, as horas ou as despesas que podem ser faturadas. Essas informações podem ser usadas para criar faturas em um sistema de contabilidade externo.

Para obter mais informações sobre registros de cobrança, consulte [Criar registros de cobrança](../../manage-work/projects/project-finances/create-billing-records.md).

O objeto BillingRecord adicionou o sinalizador **DATA_EXTENDIBLE**.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">Campos diretos</p> </td> 
   <td> 
    <ul> 
     <li> <p><b>categoryID</b> </p> <p>Adição de. Uma categoria é um formulário personalizado. Esse parâmetro foi adicionado para oferecer suporte à capacidade de adicionar Forms personalizado a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referência</td> 
   <td> 
    <ul> 
     <li> <p><b>categoria</b> </p> <p>Adição de. Categoria é um formulário personalizado. Esse parâmetro foi adicionado para oferecer suporte à capacidade de adicionar formulários personalizados a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de coleção</td> 
   <td> 
    <ul> 
     <li> <p><b>objectCategories</b> </p> <p>Adição de. Representa uma coleção de Categorias (formulários personalizados) associada ao objeto BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>calculateDataExtension</b> </p> <p>Adição de. Esta ação recalcula as expressões em campos de formulário personalizados.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Categoria (CTGY) {#category-ctgy}

Um objeto de Categoria é um formulário personalizado.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>catObjCode</b> </p> <p>Valor adicionado possível:</p> 
      <ul> 
       <li> <p> BILL (Registro de Cobrança)</p> </li> 
      </ul> <p>Esse valor foi adicionado para oferecer suporte à capacidade de adicionar formulários personalizados a objetos BillingRecord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>isObjectFrozenInPendingApprovalStatus</b> </p> <p>Essa ação pega os parâmetros objID e objCode e retorna um valor booleano.</p> </li> 
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
   <td role="rowheader">Consultas</td> 
   <td> 
    <ul> 
     <li> <p><b>getGroupStatuses</b> </p> <p>Adição de. Este query suporta a capacidade de criar e gerenciar status para grupos e subgrupos. </p> <p>Para obter mais informações, consulte <a href="../../administration-and-setup/manage-groups/manage-group-statuses/manage-group-statuses.md" class="MCXref xref">Gerenciar status do grupo</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Cliente (CUST) {#customer-cust}

Um objeto Customer representa uma organização que usa uma instância do Workfront.

Este é um objeto interno.

### Preferências do cliente (CUSTPR) {#customerpreferences-custpr}

Um objeto CustomerPreferences representa o conjunto de preferências que um cliente definiu para sua instância do Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>nome</b> </p> <p>Valor adicionado possível:</p> 
      <ul> 
       <li> <p>Permitir que os usuários adicionem imagens em atualizações (updates:images.toggle)</p> </li> 
      </ul> <p>Este parâmetro oferece suporte à capacidade de adicionar imagens em atualizações de item de trabalho. </p> <p>Para obter mais informações, consulte <a href="../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md" class="MCXref xref">Atualizar trabalho</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Versão do documento (DOCV) {#documentversion-docv}

Um objeto DocumentVersion representa uma versão específica de um arquivo (como material escrito, imagens ou outras formas de informação).

Para obter mais informações sobre versões de documentos, consulte [Carregar uma nova versão de um documento](../../documents/managing-documents/upload-new-document-version.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li> <p><b>lastCallbackDate</b> </p> <p>Adição de. Esse campo registra a data e a hora do último retorno de chamada do Workfront Proof, se a versão estiver associada a uma prova.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Grupo (GRUPO) {#group-group}

Um objeto Grupo representa um conjunto de usuários e equipes. Os grupos geralmente representam a estrutura departamental.

Para obter mais informações sobre grupos, consulte [Grupos versus equipes no Adobe Workfront](../../people-teams-and-groups/work-with-groups-and-teams/understanding-differences-and-similarities-between-groups-and-teams.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>adicionarSubgrupos</b> </p> <p>Adição de. Essa ação pega uma matriz de groupIDs e adiciona esses grupos como subgrupos ao grupo especificado.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### NoteTag (NTAG) {#notetag-ntag}

Um objeto NoteTag representa o ato de marcar um usuário ou equipe em uma atualização de um item de trabalho.

Para obter mais informações sobre marcação em atualizações, consulte [Marcar outros em atualizações](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Operações</td> 
   <td> <p>As seguintes operações foram adicionadas ao objeto NoteTag:</p> 
    <ul> 
     <li> <p><b>CONTAGEM</b> </p> </li> 
     <li> <p><b>GET</b> </p> </li> 
     <li> <p><b>RELATÓRIO</b> </p> </li> 
     <li> <p><b>PESQUISAR</b> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Projeto (PROJ) {#project-proj}

Os projetos são itens de trabalho no Workfront e um elemento principal da maneira como o Workfront ajuda as pessoas a trabalhar. Um objeto Projeto representa um grupo de tarefas com uma meta comum e específica.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>updateBusinessCaseSource</b> </p> <p>Adição de.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### QueueDef (QUED) {#queuedef-qued}

Um objeto QueueDef representa uma Fila, que é um projeto publicado na área Help Desk para permitir que os usuários enviem problemas a ele.

Para obter mais informações sobre Filas de solicitações, consulte [Criar uma fila de solicitações](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ações</td> 
   <td> 
    <ul> 
     <li> <p><b>pesquisarPorCaminho</b> </p> <p>Adição de. Essa ação oferece suporte à capacidade de localizar solicitações usando o caminho por meio da fila de solicitações e dos grupos de tópicos.</p> <p>Para obter mais informações sobre como pesquisar filas de solicitações por caminho, consulte <a href="../../manage-work/requests/create-requests/create-submit-requests.md#create-requests-in-the-web-app" class="MCXref xref">Criar solicitações e gerar rascunhos no aplicativo Web do Workfront</a> em <a href="../../manage-work/requests/create-requests/create-submit-requests.md" class="MCXref xref">Criar e enviar solicitações do Adobe Workfront</a>.</p> </li> 
    </ul> <p> </p> </td> 
  </tr> 
 </tbody> 
</table>

### Alocação de Recursos (RSALLO) {#resource-allocation-rsallo}

Um objeto de Alocação de Recursos representa a estimativa de recursos necessários para um determinado projeto. Este objeto é usado somente no Planejador de recursos herdado. Para o campo correspondente no novo Planejador de recursos, use Hora orçada (BGHR).

O objeto de Alocação de Recursos removeu o sinalizador **REPORTABLE**.

### Função (ROLE) {#role-role}

Um objeto Função (função de trabalho) representa uma capacidade funcional ou um conjunto de habilidades que um usuário pode preencher, como Designer ou Gerente de produto.

Para obter informações sobre funções de trabalho, consulte [Visão geral da função de trabalho](../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>isActive</p> <p style="font-weight: normal;">Adição de. Este é um parâmetro booleano cujo valor é verdadeiro se um objeto estiver Ativo e falso se não estiver. Os objetos definidos como Ativos aparecem em menus suspensos e campos de digitação antecipada e podem ser anexados a outros objetos.</p> </li> 
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
   <td role="rowheader">Campos diretos</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>groupID</p> <p style="font-weight: normal;">Adição de. Este campo foi adicionado para oferecer suporte à capacidade de associar grupos a modelos.</p> <p style="font-weight: normal;">Para obter mais informações, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar modelos de projeto</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Campos de referência</td> 
   <td> 
    <ul> 
     <li style="font-weight: bold;"> <p>grupo</p> <p style="font-weight: normal;">Adição de. Este campo foi adicionado para oferecer suporte à capacidade de associar grupos a modelos.</p> <p style="font-weight: normal;">Para obter mais informações, consulte <a href="../../manage-work/projects/create-and-manage-templates/edit-templates.md" class="MCXref xref">Editar modelos de projeto</a>.</p> </li> 
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
