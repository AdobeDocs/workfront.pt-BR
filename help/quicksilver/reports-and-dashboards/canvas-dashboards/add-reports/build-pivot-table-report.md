---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Criar um relatório de tabela dinâmica em um painel da tela de desenho
description: É possível adicionar um relatório de tabela dinâmica a um Painel da tela para ver os totais agregados dos dados em um formato de tabela.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 79d9eb9d3066cc83c1190d9732c64712917798aa
workflow-type: tm+mt
source-wordcount: '1556'
ht-degree: 8%

---

# Criar um relatório de tabela dinâmica em um painel da tela de desenho

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Falar com o suporte ao cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

É possível adicionar um relatório de tabela dinâmica a um Painel da Tela para ver os totais agregados dos seus dados — como somas, contagens e médias — em um formato de tabela. As tabelas dinâmicas são úteis ao comparar vários valores agregados ou contagens com várias dimensões.

![Exemplo de relatório de tabela dinâmica](assets/pivot-table-example.png)

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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

Você deve criar um painel antes de criar um relatório de tabela dinâmica. Para obter mais informações, consulte [Criar um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Criar um relatório de tabela dinâmica em um painel da tela de desenho

Há muitas opções de configuração disponíveis para criar um relatório de tabela dinâmica. Nesta seção, guiaremos você pelo processo geral de criação de um.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis da Tela de Pintura** e, em seguida, clique no nome do painel ao qual deseja adicionar o relatório.

1. Clique em **Adicionar relatório** no canto superior direito da página.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **Tabela Dinâmica**.

1. No canto superior direito, clique em **Criar relatório**.

1. (Opcional) Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Escolha a **Entidade Raiz** para o relatório.

      >[!NOTE]
      >
      > A Entidade raiz define de qual objeto seus campos vêm. Uma vez selecionado, cada seletor de campo usado posteriormente neste relatório começa a partir desse objeto, para que você possa ir diretamente para o campo desejado.


   1. Insira um relatório **Nome**.

   1. Insira uma **Descrição** do relatório.

   1. (Opcional) No campo **Executar este relatório com os direitos de acesso de**, comece digitando o nome do usuário cujas permissões você deseja que o relatório use e, em seguida, selecione o usuário quando ele aparecer na lista. Ao configurar um relatório para ser executado como outro usuário, todos os visualizadores do painel visualizam os mesmos dados, independentemente do seu próprio nível de acesso. Se você não selecionar um usuário, cada visualizador verá os dados com base em suas próprias permissões.

      >[!IMPORTANT]
      >
      >Se o usuário selecionado estiver desativado ou perder acesso aos espaços de trabalho ou tipos de registro relevantes, o relatório poderá exibir dados incompletos ou não ser renderizado.

1. Siga as etapas abaixo para configurar a seção **Métricas**:

   1. No painel esquerdo, clique no ícone **Mostrar métricas** ![Criar KPI](assets/build-kpi-icon.png).

   1. Clique em **Adicionar métrica** e selecione o campo desejado. O campo aparece como uma coluna na seção de visualização à direita.

      >[!NOTE]
      >
      > Uma métrica (também chamada de medida) é um campo numérico que você deseja adicionar ao total. Por exemplo, você pode somar todos os custos ou contar quantas tarefas há.


   1. Insira um **rótulo de coluna**.

   1. No menu suspenso **Tipo de agregação**, selecione o acúmulo de dados desse campo. As opções nesse campo variam dependendo do tipo de campo selecionado.

   1. Repita as duas etapas acima para cada métrica que deseja adicionar.

1. Siga as etapas abaixo para configurar a seção **Segmentos**:

   1. No painel esquerdo, clique no ícone do **Segmentos** ![Grupo de detalhamento](assets/drilldown-group-icon.png).

   1. Clique em **Adicionar segmento** e selecione o segmento desejado. O campo aparece como uma coluna na seção de visualização à direita.

      >[!NOTE]
      >
      >Um segmento é a categoria usada para agrupar seus dados, como tarefas de agrupamento por status ou por proprietário. É assim que suas métricas são classificadas e totalizadas.


   1. Repita as duas etapas acima para adicionar até 2 segmentos.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro** ![Filtro](assets/filter-icon.png).

   1. Selecione **Editar filtro**.

   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender.

   1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Siga as etapas abaixo para configurar a seção **Configurações de Coluna de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Colunas de Detalhamento** ![Colunas de Detalhamento](assets/drilldown-column.png).

   1. Clique em **Adicionar coluna** e selecione o campo que deseja exibir como uma coluna na tabela de detalhamento. Repita esse processo para cada coluna que deseja adicionar.

1. Clique em **Salvar** para criar o relatório e adicioná-lo ao painel.

## Criar um exemplo de relatório de tabela dinâmica

Nesta seção, veremos as etapas para criar um relatório de tabela dinâmica que resume os dados de conclusão da tarefa.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis da Tela de Pintura** e, em seguida, clique no nome do painel ao qual deseja adicionar o relatório.

1. Clique em **Adicionar relatório** no canto superior direito da página.

1. Na caixa **Adicionar relatório**, selecione **Criar relatório**.

1. No lado esquerdo, selecione **Tabela Dinâmica**.

1. No canto superior direito, clique em **Criar relatório**.

1. Siga as etapas abaixo para configurar a seção **Detalhes**:

   1. Escolha **Tarefa** como **Entidade Raiz**.
   1. Digite *Horas planejadas da tarefa vs. horas efetivas por portfólio e projeto* no campo **Nome**.
   1. Digite uma descrição no campo **Descrição**.

1. Siga as etapas abaixo para configurar a seção **Métricas**:

   1. No painel esquerdo, clique no ícone **Mostrar métricas** ![Criar KPI](assets/build-kpi-icon.png).
   1. Clique em **Adicionar métrica** e selecione **Nome**. Digite *Contagem de tarefas* no campo **Rótulo da coluna**. No menu suspenso **Tipo de agregação**, selecione **Contagem**.
   1. Clique em **Adicionar métrica** e selecione **Horas efetivas**. Digite *Horas efetivas* no campo **Rótulo da coluna**. No menu suspenso **Tipo de agregação**, selecione **Soma**.
   1. Clique em **Adicionar métrica** e selecione **Horas planejadas**. Digite *Total de horas planejadas* no campo **Rótulo da coluna**. No menu suspenso **Tipo de agregação**, selecione **Soma**.

1. Siga as etapas abaixo para configurar a seção **Segmentos**:

   1. No painel esquerdo, clique no ícone do **Segmentos** ![Grupo de detalhamento](assets/drilldown-group-icon.png).
   1. Clique em **Adicionar segmento** e selecione **Projeto** > **Portfolio** > **Nome**.
   1. Clique em **Adicionar segmento** e selecione **Projeto** > **Nome**.

1. Siga as etapas abaixo para configurar a seção **Filtro**:

   1. No painel esquerdo, clique no ícone **Filtro** ![Filtro](assets/filter-icon.png).
   1. Selecione **Editar filtro** e **Adicionar condição**.
   1. Clique no filtro de condição vazio e em **Escolher um Campo**.
   1. Selecione **Status**.
   1. Altere o operador para **Igual** e escolha *em andamento*.

1. Siga as etapas abaixo para configurar a seção **Configurações de Coluna de Detalhamento**:

   1. No painel esquerdo, clique no ícone **Colunas de Detalhamento** ![Colunas de Detalhamento](assets/drilldown-column.png).
   1. Clique em **Adicionar coluna** e selecione **Nome**.
   1. Clique em **Adicionar coluna** e selecione **Atribuído a** > **Nome**.
   1. Clique em **Adicionar coluna** e selecione **Data de conclusão planejada**.

1. Clique em **Salvar** no canto superior direito da tela.

## Considerações ao criar um relatório de tabela dinâmica

### Relatórios com dados financeiros

Os usuários com acesso de Visualização ou Edição a Dados financeiros em seu nível de acesso ainda verão os dados financeiros nas visualizações do Painel do Canvas, mesmo se a permissão de Visualização de finanças for removida no nível de tarefa ou projeto.

* Os usuários sem direitos referentes a dados financeiros no nível de acesso não verão dados financeiros nos relatórios.
* Os usuários que veem dados financeiros estão limitados a registros para os quais já têm permissão de visualização (projetos, tarefas, problemas, etc.). Eles não verão valores financeiros correspondentes a registros que não podem acessar.
* Os criadores de relatórios devem ter cuidado ao incluir dados financeiros nos painéis e estar cientes de com quem compartilham painéis para evitar acessos não intencionais.

Este é um limite conhecido, e planejamos solucioná-lo no futuro.

### Utilização do seletor de campos

O menu suspenso **Seções** na seção **Criar tabela dinâmica** foi criado para restringir as opções em um seletor de campos para facilitar a localização de um objeto ao criar um relatório de tabela dinâmica. Para iniciar, você selecionaria um objeto de entidade base.

* **Todas as Seções**: todos os tipos de objetos no Workfront e no Workfront Planning.
* **Objetos Workfront**: objetos Workfront nativos.
* **Tipos de Registro do Planning**: tipos de registro personalizados definidos no Workfront Planning.

![Menu suspenso de seções](assets/sections-dropdown.png)

Depois que o objeto de entidade base for selecionado, o menu suspenso **Seções** será atualizado com as opções de tipo de campo aplicáveis.

* **Todas as Seções**: campos nativos, campos personalizados e objetos relacionados.
* **Todos os campos**: campos nativos e personalizados (exclui relações).
* **Campos Personalizados**: campos definidos pelo cliente em um formulário personalizado ou em um registro do Planning.
* **Campos do Workfront**: somente campos nativos.
* **Relações**: registros conectados.

![Seleção de objetos relatáveis](assets/reportable-objects-selection.png)

### Fazendo referência a objetos relacionados

Limitamos o acesso para escolher objetos secundários como segmentos de uma tabela dinâmica. As opções de segmento podem ser atributos do próprio registro ou outros registros relacionados que não representam uma relação de 1:many ou muitos:many.

Também limitamos o acesso à referência a qualquer atributo pai ou filho como uma métrica para reduzir o potencial de contagem dupla ou resumir valores, resultando em uma representação incorreta dos dados reais.
