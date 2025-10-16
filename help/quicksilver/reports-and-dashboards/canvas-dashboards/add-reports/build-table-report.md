---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Criar um relatório de tabela em um painel da tela
description: É possível adicionar um relatório de tabela a um Painel da tela para visualizar seus dados em formato de tabela.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: a7aa8614-6e80-4fc1-88ff-d952d87ddcbc
source-git-commit: 1059950dd3b20e0959c626e580f958bed5076541
workflow-type: tm+mt
source-wordcount: '1074'
ht-degree: 1%

---

# Criar um relatório de tabela em um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>&#x200B;>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Contate o Suporte ao Cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>&#x200B;>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

É possível adicionar um relatório de tabela a um Painel da tela para visualizar seus dados em formato de tabela.

![Exemplo de relatório de tabela](assets/table-example-main.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> 
<p>Standard </p> 
<p>Plano</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurações de nível de acesso</p></td> 
   <td><p>Editar acesso a relatórios, painéis e calendários</p>
  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

Você deve criar um painel antes de criar um relatório de tabela.


## Criar um relatório de tabela em um painel da tela

Há muitas opções de configuração disponíveis para criar um relatório de tabela. Nesta seção, guiaremos você pelo processo geral de criação de um.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **Tabela**.

1. No canto superior direito, clique em **Criar relatório**.

1. (Opcional) Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Insira um relatório **Nome**.

   1. Insira uma **Descrição** do relatório.

1. Siga as etapas abaixo para configurar a seção **Tabela de compilação**:

   1. No painel esquerdo, clique no ícone **Colunas da tabela** ![Criar tabela](assets/drilldown-column.png).

   1. Clique em **Adicionar coluna** e selecione o campo que deseja exibir como uma coluna na tabela. A coluna é exibida na seção de visualização à direita.



   1. Repita a etapa acima para cada coluna que deseja adicionar.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selecione **Editar filtro**.

   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender. A coluna é exibida na seção de visualização à direita.

1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Configurações de grupo** ![Configurações de grupo](assets/drilldown-group-icon.png).

   1. Clique no botão **Adicionar agrupamento** e selecione o campo que deseja criar como agrupamento. A coluna de agrupamento aparece na seção de visualização à direita.

1. Clique em **Salvar** para criar o relatório e adicioná-lo ao painel.

## Criar um exemplo de relatório de tabela

Nesta seção, vamos percorrer as etapas para criar um relatório de tabela que exibe aprovações de documentos pendentes.

Para obter mais informações sobre exemplos de relatório de tabela, consulte [Criar um painel de relatório para revisão e aprovações](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **Tabela**.

1. No canto superior direito, clique em **Criar relatório**.

1. Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Digite _Aprovações pendentes_ no campo **Nome**.
   1. Digite uma descrição no campo **Descrição**. Esse texto é exibido como uma dica de ferramenta ao lado do nome do gráfico.

1. Siga as etapas abaixo para configurar a seção **Tabela de compilação**:

   1. No painel esquerdo, clique no ícone **Colunas da tabela** ![Colunas da tabela](assets/drilldown-column.png).
   1. Clique em **Adicionar coluna**.
   1. Role para baixo e selecione **Aprovações de documentos** > **Status**.
   1. Adicione as seguintes colunas:

   <table>
    <tr>
    <td><strong>Nome do projeto</strong></td>
    <td>Versão do documento &gt; Documento &gt; Projeto &gt; Nome</td>
    </tr>
    <tr>
    <td><strong>Nome do documento</strong></td>
    <td>Versão do documento &gt; Documento &gt; digite <em>Nome</em> na caixa de pesquisa.</td>
    </tr>
    <tr>
    <td><strong>Versão do documento</strong></td>
    <td>Versão do documento &gt; Documento &gt; Versão</td>
    </tr>
    <tr>
    <td><strong>Prazo</strong></td>
    <td>Aprovação de documento &gt; Estágio de aprovação &gt; Prazo</td>
    </tr>
    <tr>
    <td><strong>Requisitado por</strong></td>
    <td>Aprovação de documento &gt; Estágio de aprovação &gt; Participantes do estágio de aprovação* &gt; Solicitante &gt; digite <em>Name</em> na caixa de pesquisa.</td>
    </tr>
    <tr>
    <td><strong>Data de solicitação</strong></td>
    <td>Aprovação de documento &gt; Estágio de aprovação &gt; Participantes do estágio de aprovação* &gt; Criado em</td>
    </tr>
    <tr>
    <td><strong>Aprovador</strong></td>
    <td>Aprovação de documento &gt; Estágio de aprovação &gt; Participantes do estágio de aprovação* &gt; Usuário participante &gt; tipo <em>Nome</em> na caixa de pesquisa.</td>
    </tr>
    </table>


   *Os Participantes do Estágio de Aprovação estão truncados para _Pasta do Estágio de Aprovação.._


1. Siga as etapas abaixo para configurar a seção **Filtro**:
   1. No painel esquerdo, clique no ícone da **guia Filtro** ![filtro](assets/filter-tab.png).
   1. Clique em **Editar Filtro** e depois em **Adicionar condição**.
   1. Clique no filtro de condição vazio e em **Escolher um Campo**.
   1. Selecione **Status**.
   1. Altere o operador para **Igual** e digite _aprovação pendente_ na caixa de texto.
      ![exemplo de filtro de tabela de aprovação pendente](assets/pending-approval-table-filter.png)
   1. (Opcional) Adicione mais filtros conforme descrito na seção **Filtros opcionais** abaixo.
1. Clique em **Salvar** no canto superior direito da tela.

## Considerações ao criar um relatório de tabela

### Utilização do seletor de campos

O menu suspenso **Seções** na seção **Tabela de compilação** foi criado para restringir as opções em um seletor de campos para facilitar a localização de um objeto ao criar um relatório de tabela. Para iniciar, você selecionaria um objeto de entidade base.

* **Todas as Seções**: todos os tipos de objetos no Workfront Workflow e no Workfront Planning.
* **Objetos Workfront**: objetos de Fluxo de Trabalho Workfront nativos.
* **Tipos de Registro do Planning**: tipos de registro personalizados definidos no Workfront Planning.

![Menu suspenso de seções](assets/sections-dropdown.png)

Depois que o objeto de entidade base for selecionado, o menu suspenso **Seções** será atualizado com as opções de tipo de campo aplicáveis.

* **Todas as Seções**: campos nativos, campos personalizados e objetos relacionados.
* **Todos os campos**: campos nativos e personalizados (exclui relações).
* **Campos Personalizados**: campos definidos pelo cliente em um formulário personalizado ou em um registro do Planning.
* **Campos do Workfront**: somente campos nativos.
* **Relações**: registros conectados.

![Seleção de objetos relatáveis](assets/reportable-objects-selection.png)

### Fazendo referência a objetos filho

Os relacionamentos disponíveis para colunas adicionais, opções de filtro e atributos de agrupamento geralmente são limitados a objetos superiores na hierarquia de objetos do Workfront ou têm uma única seleção no objeto de entidade base do relatório. Há algumas exceções a isso, que incluem:

* Projeto > Tarefas
* Aprovação de documento > Estágios de aprovação de documento
* Estágios de aprovação de documento > Participantes do estágio de aprovação de documento

Ao utilizar qualquer uma das relações pai-filho listadas acima, você verá uma linha na tabela para cada registro filho conectado ao objeto pai.
