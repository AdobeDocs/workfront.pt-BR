---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Criar um relatório de KPI em um painel da tela
description: Um relatório de KPI que exibe de forma destacada um único KPI agregado pode ser adicionado a um Painel da tela.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: e1c68ac3-112e-4f9e-b644-f44bb0778b92
source-git-commit: d7caaa0871263fb8ef4224a9c298778f3ee2454a
workflow-type: tm+mt
source-wordcount: '1260'
ht-degree: 1%

---

# Criar um relatório de KPI em um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Contate o Suporte ao Cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

É possível criar e adicionar um relatório de KPI a um Painel da tela que representa visualmente seus dados principais do indicador de desempenho como um número, que você pode usar para ver como seus projetos e equipes estão se saindo.

![Exemplo de relatório de KPI](assets/kpi-example-main.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
<p>Padrão</p> 
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

Você deve criar um painel antes de criar um relatório de KPI.

## Criar um relatório de KPI em um painel da tela

Há muitas opções de configuração disponíveis para criar um relatório de KPI. Nesta seção, guiaremos você pelo processo geral de criação de um.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **KPI**.

1. No canto superior direito, clique em **Criar relatório**.

1. Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Insira um relatório **Nome**.
   1. Insira uma **Descrição** do relatório.

      >[!NOTE]
      >
      >A descrição será usada como uma legenda abaixo do valor do KPI. Se você não inserir uma descrição, uma legenda será gerada para você com base no agregador e no tipo de agregação selecionados nas etapas a seguir.

1. Siga as etapas abaixo para configurar a seção **Criar KPI**:

   1. No painel esquerdo, clique no ícone **Criar KPI** ![Criar KPI](assets/build-kpi-icon.png).

   1. Clique em **Selecionar campo** e especifique o campo que deseja adicionar ao relatório.

   1. No menu suspenso **Tipo de agregação**, selecione como os dados são acumulados para produzir a saída de KPI. As opções nesse campo variam de acordo com o tipo de campo selecionado na etapa anterior.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selecione **Editar filtro**.

   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender.

   1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

      Para obter mais informações sobre filtros, consulte [Editar filtros de relatório em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/edit-report-filters.md).

1. Siga as etapas abaixo para configurar a seção **Configurações de Coluna de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Colunas de Detalhamento** ![Colunas de Detalhamento](assets/drilldown-column.png). Os campos do gráfico aparecem automaticamente como colunas na seção de visualização à direita.

   1. (Opcional) Para atualizar qualquer uma das configurações de coluna existentes, selecione a coluna que deseja atualizar na seção **Colunas atuais** e atualize as informações desejadas (por exemplo, rótulo, status vinculado e regras de formatação).

   1. Clique em **Adicionar coluna** e selecione o campo que deseja exibir como uma coluna na tabela. Repita esse processo para cada coluna que deseja adicionar.

1. Siga as etapas abaixo para configurar a seção **Configurações do Grupo de Detalhamento**:

   1. No painel esquerdo, clique no ícone do **Grupo de configurações** ![Grupo de detalhamento](assets/drilldown-group-icon.png).

   1. Clique no botão **Adicionar agrupamento** e selecione o campo que deseja criar como agrupamento.

1. Clique em **Salvar** para criar o relatório e adicioná-lo ao painel.

## Criar um exemplo de relatório de KPI

Nesta seção, veremos as etapas para criar um relatório de KPI que exibe aprovações pendentes de documentos.

Para obter mais informações sobre exemplos de relatório de KPI, consulte [Criar um painel de relatório para revisão e aprovações](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-review-and-approval-dashboard.md).

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Clique em **Novo Painel** no canto superior direito.

1. Na caixa **Criar painel**, digite o **Nome** e a **Descrição** do painel.

1. Clique em **Criar**.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **KPI**.

1. No canto superior direito, clique em **Criar relatório**.

1. Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Digite *Pendente* no campo **Nome**.
   1. Digite *Aprovações pendentes* no campo **Descrição**. É exibido como uma legenda abaixo do valor do KPI.

1. Siga as etapas abaixo para configurar a seção **Criar KPI**:

   1. No painel esquerdo, clique no **ícone Criar KPI** ![Criar KPI](assets/build-kpi-icon.png).

   1. Clique em **Selecionar campo**.

   1. Localize e selecione a pasta **Aprovação de documentos**.

   1. Selecione **Status**.

   1. No menu suspenso **Tipo de agregação**, selecione **Contagem**.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selecione **Editar filtro**.

   1. Clique em **Adicionar condição**.

   1. Clique no filtro de condição vazio, clique em **Escolher um Campo** e escolha **Status**.
   1. Deixe o operador como **Igual** e digite _revisão pendente_ na caixa de texto.
      ![Exemplo de filtro de kpi pendente](assets/pending-kpi-filter.png)
1. Clique em **Salvar** no canto superior direito da tela.

## Considerações ao criar um relatório de KPI

### Relatórios com dados financeiros

Os usuários com acesso de Visualização ou Edição a Dados financeiros em seu nível de acesso ainda verão os dados financeiros nas visualizações do Painel do Canvas, mesmo se a permissão de Visualização de finanças for removida no nível de tarefa ou projeto.

* Os usuários sem direitos de dados financeiros no nível de acesso não verão dados financeiros nos relatórios.
* Os usuários que veem dados financeiros estão limitados a registros para os quais já têm permissão para visualizar (projetos, tarefas, problemas, etc.). Eles não verão valores financeiros para registros que não podem acessar.
* Os criadores de relatórios devem ter cuidado ao incluir dados financeiros nos painéis e estar cientes de com quem compartilham painéis para evitar acesso não intencional.

Esse é um limite conhecido e pretendemos resolvê-lo o mais rápido possível.

### Utilização do seletor de campos

O menu suspenso **Seções** da seção **Criar KPI** foi projetado para restringir as opções em um seletor de campos para facilitar a localização de um objeto ao criar um relatório de tabela. Para iniciar, você selecionaria um objeto de entidade base.

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


