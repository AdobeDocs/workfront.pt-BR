---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Referência de filtro de relatório para Painéis do Canvas
description: Referência para os campos, operadores, curingas e regras especiais que você pode usar ao filtrar um relatório em um Painel da tela.
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 34%
---
# Referência de filtro de relatório para Painéis do Canvas

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Partes do recurso podem não estar completas ou não funcionar conforme o esperado durante essa etapa. Envie seus comentários sobre a experiência seguindo as instruções na seção [Fornecer feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) do artigo de visão geral sobre a versão beta dos Painéis da Tela.<br>
>Se você tiver feedback sobre um possível erro ou problema técnico, envie um tíquete ao Suporte da Workfront. Para obter mais informações, consulte [Falar com o suporte ao cliente](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observe que esse beta não está disponível nos seguintes provedores de nuvem:
>
>* Traga sua própria chave para o Amazon Web Services
>* Azure
>* Google Cloud Platform

Este artigo descreve os campos, operadores, curingas e regras especiais disponíveis ao filtrar um relatório. Para obter as etapas para criar ou editar um filtro, consulte [Filtrar um relatório em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-a-report.md).

## Operadores de campo por tipo de campo

+++ Expanda para exibir a lista de operadores de campo por tipo de campo. 

<table>
    <tr>
        <td><b>Tipo de campo</b></td>
        <td><b>Exemplo</b></td>
       <td><b>Operadores</b></td>
        <td><b>Caractereeeeeeeees curinga</b></td>
    </tr>
    <tr>
        <td>Nome do objeto/referência</td>
        <td>Qualquer atributo de nome nativo ou pesquisa personalizada</td>
              <td><ul>
        <li>Igual</li>
        <li>Não igual</li>
        <li>Contém</li>
          <li>Não contém</li>
            <li>É nulo</li>
              <li>Não é nulo</li>
        </ul></td>
        <td>Usuário: Nome
        <ul>
        <li>Eu (usuário conectado)</li>
        </ul>
        Grupo: Nome
        <ul>
          <li>Meu grupo doméstico (grupo de usuários conectados)</li>
            <li>Meus outros grupos (grupos de usuários conectados)</li>
          </ul>
          Equipe: Nome
                  <ul>
          <li>Minha equipe padrão (equipe de usuários conectados)</li>
            <li>Minhas outras equipes (equipes de usuários conectados)</li>
          </ul>
        </td>
    </tr>
    <tr>
        <td>Entrada de string/texto </td>
                <td>Projeto: Descrição</td>
                      <td><ul>
             <li>Igual</li>
        <li>Não igual</li>
        <li>Contém</li>
          <li>Não contém</li>
            <li>É nulo</li>
              <li>Não é nulo</li>
        </ul></td>
        <td></td>
    </tr>
    <tr>
        <td>Inteiro / Duplo</td>
             <td>Projeto: Trabalho de Horas Planejado
        <br>Tarefa: porcentagem concluída</td>
              <td><ul>
        <li>Igual</li>
        <li>Não igual</li>
        <li>Maior que</li>
          <li>Maior ou igual a</li>
          <li>Menor que</li>
          <li>Menor ou igual a</li>
            <li>É nulo</li>
              <li>Não é nulo</li>
        </ul></td>
        <td></td>
    </tr>
       <tr>
        <td> Data / Data e hora </td>
                    <td>Projeto: Data de Início Planejada
        <br>Hora: Data de Entrada</td>
              <td><ul>
        <li>Igual</li>
        <li>Não igual</li>
        </ul></td>
        <td>Ao alternar a opção <b>Definir data relativa</b>, é possível aplicar curingas de data relativos para tornar o relatório mais dinâmico e autoajustado com base em períodos de data comuns. 
         <ul><li>$$TODAY</li>
         <li>$$NOW</li>
         </ul>
        </td>
    </tr>
       <tr>
        <td>Booleano </td>
                  <td>Projeto: tem documentos
        <br>Tarefa: É Crítica
        <br> Usuário: Está Ativo</td>
        <td><ul>
        <li>Igual</li>
        <li>Não igual</li>
        </ul></td>
        <td> </td>
    </tr>
   </table>

+++

## Variáveis de filtro de curinga baseado em data

As opções de curinga baseado em data podem ser usadas em combinação com qualquer atributo de filtro de data. Para obter informações sobre como adicionar um curinga baseado em data a um relatório, consulte [Usar curingas baseados em data para generalizar relatórios](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>Se você criar um cálculo de data e hora que não inclua uma parte de hora ou que use os curingas de data $$TODAY ou $$NOW, o sistema usará a data de acordo com o fuso horário do Tempo Universal Coordenado (UTC), e não de acordo com o seu fuso horário local. Isso pode causar um resultado inesperado na data.

Você pode escolher entre os seguintes curingas baseados em data:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>Recomendamos que você crie filtros sensíveis à data usando esse curinga para evitar ter que criar o filtro novamente amanhã, na próxima semana ou no próximo mês.</p> <p>Por exemplo, se você quiser exibir todas as tarefas que vencem antes de hoje, use a seguinte regra em um filtro de tarefas: <em>Data de início planejada anterior a $$TODAY</em>.</p> <p>$$TODAY é sempre igual à meia-noite do dia atual.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>Semelhante ao curinga $$TODAY, mas inclui a data e a hora atuais. $$NOW é igual à data e hora atuais.</p> <p>Por exemplo, se você quiser exibir todas as entradas de horas fornecidas até a hora atual, pode fazer isso usando a seguinte regra em um filtro de horas: <em>Data de início planejada anterior a $$NOW</em>.</p> <p>Nota: esse curinga não é compatível com o planejador de recursos.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para indicar vários períodos e vários pontos no tempo (futuros ou passados), você pode combinar os curingas acima com o seguinte:

| Atributos |   |
|---|---|
| **q** | trimestre do calendário |
| **h** | hora |
| **d** | dia |
| **w** | semana |
| **m** | mês |
| **y** | ano |

{style="table-layout:auto"}

| **Qualificadores** |   |
|---|---|
| **b** | início do período (sem um atributo especificado, o padrão é início da semana: domingo) |
| **e** | fim do período (sem um atributo especificado, o padrão é fim da semana: sábado) |

{style="table-layout:auto"}

| **Operadores** |   |
|---|---|
| **+** | adicionar valor ao curinga |
| **-** | subtrair valor do curinga |

{style="table-layout:auto"}

Por exemplo, o curinga `$$TODAYb+2w` se refere a “2 semanas a partir do início desta semana”. O curinga `$$NOW+2h` se refere a &quot;daqui a 2 horas&quot;.

## Variáveis de filtro curinga do usuário conectado

* Ao filtrar no atributo do usuário `name`, você visualizará a opção **Eu (usuário conectado)**.

  ![Atributo de nome de usuário](assets/user-name-attribute.png)

* Ao filtrar em um atributo de grupo `name`, você visualizará as opções **Meu grupo inicial (grupo de usuários conectado)** e **Meus outros grupos (grupos de usuários conectados)** para usar em uma condição de filtro.

  ![Atributo de nome do grupo](assets/group-name-attribute.png)

* Ao filtrar por um atributo de equipe `name`, você visualizará as opções **Minha equipe padrão (Equipe de usuários conectada)** e **Minhas outras equipes (Equipes de usuários conectadas)** para escolher na condição de filtro.

  ![Atributo de nome da equipe](assets/team-name-attribute.png)

## Fazendo referência a objetos filho

Os relacionamentos disponíveis para colunas adicionais, opções de filtro e atributos de agrupamento geralmente são limitados a objetos superiores na hierarquia de objetos do Workfront ou têm uma única seleção no objeto de entidade base do relatório. Há algumas exceções a isso, que incluem:

* Projeto > Tarefas
* Aprovação de documento > Estágios de aprovação de documento
* Estágios de aprovação de documento > Participantes do estágio de aprovação de documento

Ao utilizar qualquer uma das relações pai-filho listadas acima, você verá uma linha na tabela para cada registro filho conectado ao objeto pai.

<div class="preview">

## Filtrar os relacionamentos da coleção na visualização

Uma coleção é um campo vinculado a um grupo de registros relacionados, em vez de a um único registro. Por exemplo, os participantes dos estágios de aprovação de um projeto são uma coleção. Ao criar um filtro, você pode filtrar coleções diretamente, sem alternar para o modo de texto.

Para filtrar em uma coleção, abra o painel Selecionar um campo e selecione Coleções. Esta seção lista somente relações de coleção. Os relacionamentos com registro único ficam em Relacionamentos.

![relações de coleção](assets/collections.png)

Depois de selecionar uma coleção, você pode fazer duas coisas:

* Filtre nos próprios campos da coleção. Por exemplo, a partir dos projetos de um portfólio, você pode filtrar o status de um projeto.
* Siga um relacionamento de registro único fora da coleção. Por exemplo, nos projetos de um portfólio, é possível entrar em contato com o proprietário do projeto.

As coleções não são compatíveis com navegação mais profunda. Não é possível abrir uma coleção aninhada dentro de outra coleção, seguir mais de uma relação ou selecionar a relação que leva de volta ao local em que você começou.

A seção Coleções é exibida somente quando você cria um filtro. Ele não é exibido em outros seletores de campo, como aqueles para colunas de tabela, agrupamentos ou campos de gráfico.

</div>

## Excluir projetos pessoais, tarefas e usuários de bot

>[!NOTE]
>
>Se um relatório de Painéis do Canvas retornar mais resultados do que você espera em comparação a um relatório clássico semelhante, projetos pessoais, tarefas pessoais ou usuários de bot podem ser incluídos por padrão. Adicione uma condição de filtro para excluí-los.

Nos relatórios de Projeto e Tarefa de Painéis de Tela, o filtro `isPersonal` não é aplicado automaticamente, portanto, projetos pessoais e tarefas pessoais são incluídos nos resultados por padrão. Para excluí-los, adicione uma condição de filtro como `isPersonal=false`.

Da mesma forma, os relatórios de usuário dos painéis do Canvas incluem todos os usuários por padrão, incluindo os colaboradores de IA (usuários de bot). Para excluir usuários de bot, adicione uma condição de filtro como `isBot=false`.

Os relatórios de Projeto e Tarefa clássicos excluem automaticamente projetos pessoais e tarefas pessoais, enquanto os relatórios de Usuário clássicos excluem automaticamente os usuários de bot. Para incluí-los em um relatório clássico, adicione uma condição de filtro como `isPersonal=true` (somente itens pessoais) ou `isPersonal_Mod=notnull` (itens pessoais e não pessoais).
