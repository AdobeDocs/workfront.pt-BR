---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Importar dados para o Adobe Workfront usando um modelo do Kickstart
description: Kickstarts são pastas de trabalho do Excel especialmente formatadas que você pode preencher com dados que deseja importar para o Workfront. O Adobe Workfront fornece um modelo de Início que você pode usar para fazer isso, conforme explicado no importador de dados de Início.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 8e076e9c89ad208aa94ddefead4b8c6105992542
workflow-type: tm+mt
source-wordcount: '2755'
ht-degree: 6%

---

# Importar dados para o Adobe Workfront usando um modelo do Kickstart

<!--Audited: 12/2023-->

Kickstarts são pastas de trabalho do Excel especialmente formatadas que você pode preencher com dados que deseja importar para o Workfront. A Adobe Workfront fornece um modelo de Início que você pode usar para fazer isso, conforme explicado em [Importador de dados de Início](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Esse processo é dividido em três tarefas principais:

* Primeiro, você exporta um modelo do Kickstart como um arquivo de planilha
* Em segundo lugar, você preenche a planilha com seus dados
* Por fim, importe a planilha preenchida para o Workfront

Cada um desses procedimentos é descrito na ordem correta neste artigo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p> Novo: Padrão</p>
   ou
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador do Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitação

Você pode importar um grande número de objetos para o Workfront usando um template do Kickstart. No entanto, considere as seguintes limitações:

* Importar dados dessa maneira não atualiza as informações nos registros que já existem no Workfront.
* Você pode importar somente novos registros e suas informações.
* Importe não mais do que 2.000 registros de cada vez para garantir que a importação não expire

## Exportar um modelo do Kickstart como um arquivo de planilha

Ao exportar um modelo de Início, você recebe uma pasta de trabalho em branco da planilha do Excel. Depois que a planilha for baixada no computador, você poderá usá-la para preenchê-la com suas informações e importá-la de volta para o Workfront.

Para exportar um modelo do Kickstart:

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  -->

1. Clique em **Sistema** > **Importar Dados (Kick-Starts)**.

1. Selecione os tipos de informações que deseja incluir.

   Cada opção selecionada representa uma coleção de várias guias na planilha exportada. Por exemplo, se você selecionar a opção **Relatório**, todos os objetos necessários para criar um relatório serão incluídos na planilha (exibições, filtros, agrupamentos, relatórios).

   Você pode usar todos os tipos de objetos listados abaixo para importar dados para o Workfront. (A única exceção é a opção Níveis de Acesso. A data sheet Níveis de acesso em uma exportação é fornecida para fins de referência; ela permite que você atribua um nível de acesso a uma nova conta de usuário por ID.)

   O modelo para cada tipo de objeto pode ser exportado nos formatos de arquivo a seguir e contém as seguintes planilhas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objeto</strong> </p> </th> 
      <th> <p><strong>Exporta como</strong> </p> </th> 
      <th> <p><strong>Planilha exportada</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Painel</p> <p>Todos os painéis no sistema estão disponíveis para exportação. Você pode selecionar até 100 painéis específicos em uma única exportação.</p> </td> 
      <td scope="col">Exporta como arquivo ZIP</td> 
      <td scope="col"> <p>Parâmetro</p> <p>Texto descritivo</p><p>Opção de parâmetro</p> <p>Grupo de Parâmetros</p> <p>Parâmetro da Categoria</p> <p>Categoria</p> <p>Relatório</p> <p>Seção de Guias do Portal</p> <p>Painel</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Relatório</p> <p>Todos os relatórios do sistema estão disponíveis para exportação. É possível selecionar até 100 relatórios específicos em uma única exportação.</p> <p>O Kick-Starts não é compatível com filtros do modo de texto. Para uma exportação bem-sucedida, os filtros de relatórios devem ser alternados para o Modo Padrão.</p> </td> 
      <td scope="col">Exporta como arquivo ZIP </td> 
      <td scope="col"> <p scope="col">Parâmetro</p> <p scope="col">Texto descritivo</p> <p scope="col">Opção de parâmetro</p> <p scope="col">Grupo de Parâmetros</p> <p scope="col">Parâmetro da Categoria</p> <p scope="col">Categoria</p> <p scope="col">Relatório</p> <p scope="col">Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Aprovação</p> </td> 
      <td scope="col"> <p>Exporta como arquivo do Excel</p> </td> 
      <td scope="col"> <p>Aprovador de estágio</p> <p>Estágio de aprovação</p> <p>Aprovação</p> <p>Processo de aprovação</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Dados personalizados</p> </td> 
      <td scope="col"> <p>Exporta como arquivo do Excel</p> </td> 
      <td scope="col"> <p>Parâmetro</p> <p>Texto descritivo</p>  <p>Opção de parâmetro</p> <p>Grupo de Parâmetros</p> <p>Parâmetro da Categoria</p> <p>Categoria</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Tipo de Despesa</p> </td> 
      <td scope="col"> <p>Exporta como arquivo do Excel</p> </td> 
      <td> <p>Tipo de Despesa</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Tipo de hora</p> </td> 
      <td scope="col"> <p>Exporta como arquivo do Excel</p> </td> 
      <td> <p>Tipo de hora</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Equipe</p> </td> 
      <td scope="col"> <p>Exporta como arquivo do Excel</p> </td> 
      <td> <p> Integrante da Equipe</p> <p>Equipe</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Usuário</p> </td> 
      <td> <p>Exporta como arquivo do Excel. Para ver a lista completa de opções, clique em <strong>Mais Opções</strong>.</p> </td> 
      <td> <p>Usuário</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Nível de acesso</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p>Nível de acesso</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Atribuição</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p>Atribuição</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Empresa</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Empresa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Modelo de email</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p>Modelo de email</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Despesa</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Despesa'</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Página Externa</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Página Externa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Filtro</td> 
      <td>Exporta como um arquivo ZIP</td> 
      <td> <p> Filtro</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Grupo</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Grupo</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Agrupamento</td> 
      <td>Exporta como um arquivo ZIP</td> 
      <td> <p> Agrupamento</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Hora</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Hora</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Problema</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Problema</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Função no trabalho</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Função de trabalho</p> <p>Preferências </p> </td> 
     </tr>

   <tr> 
      <td>Caminho de Etapas</td> 
      <td> Exporta como arquivo do Excel</td> 
      <td> <p> Etapa</p> <p>Caminho de Etapas</p> <p>Preferências </p> </td> 
     </tr>

   <tr> 
      <td>Nota</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Nota</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Portfólio</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Portfólio</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Projeto</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Fila</p> <p>Projeto</p> <p>Regra de Encaminhamento</p> <p>Enfileirar tópico</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Estimativa de Recursos</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Estimativa de Recursos</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Risco</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Risco</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Tipo de Risco</td> 
      <td> Exporta como arquivo do Excel</td> 
      <td> <p> Tipo de Risco</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Scorecard</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p>Pergunta do Scorecard</p> <p>Opção de scorecard</p> <p>Scorecard</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Tarefa</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Tarefa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Modelo</td> 
      <td> Exporta como arquivo do Excel</td> 
      <td> <p> Fila</p> <p>Modelo</p> <p>Regra de Encaminhamento</p> <p>Enfileirar tópico</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Atribuição de Modelo</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Atribuição de Modelo</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Modelo de Tarefa</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Modelo de Tarefa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Planilha de horas</td> 
      <td> Exporta como arquivo do Excel</td> 
      <td> <p> Perfil da Planilha de Horas</p> <p>Planilha de horas</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Exibir </td> 
      <td> <p>Exporta como arquivo ZIP</p> </td> 
      <td> <p> Exibir</p> <p>Preferências </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Baixar**.
1. Continue com [Preencha o modelo de planilha com seus dados](#populate-the-spreadsheet-template-with-your-data) para preencher a planilha de modelo em branco com suas informações.

## Preencha o modelo de planilha com seus dados {#populate-the-spreadsheet-template-with-your-data}

* [Visão geral das guias (folhas de dados) incluídas na planilha](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importar um registro](#import-a-record)
* [Incluir datas](#include-dates)
* [Usar curingas](#use-wildcards)
* [Substituição de nome de atributo para IDs](#attribute-name-substitution-for-ids)

### Visão geral das guias (folhas de dados) incluídas na planilha

>[!TIP]
>
>Para entender melhor como você precisará formatar as informações em cada coluna ao preencher o modelo de Início, considere fazer uma prática executada exportando um Início com dados existentes do Workfront nos objetos que você está tentando importar. Para obter instruções, consulte [Exportar dados do Adobe Workfront via Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Quando você abre um modelo de Kick-Starts em branco, várias guias (folhas de dados) estão disponíveis. Eles dependem dos objetos selecionados para download. Cada um representa um objeto no aplicativo, como projeto, tarefas, horas, painel e usuários:

Quando você abre uma dessas guias, a linha 2 exibe os campos para cada objeto que pode ser definido durante uma importação. Em um cabeçalho de coluna, depois da palavra &quot;set&quot;, o nome do campo é exibido como aparece no banco de dados. Esses campos atuam como cabeçalhos de coluna.

>[!IMPORTANT]
>
>Para evitar erros, verifique o seguinte:
>
>* Não exclua a primeira linha vazia de uma planilha de início rápido.
>* Não exclua, modifique ou reorganize esses campos (cabeçalhos de coluna) de forma alguma. Por exemplo, não altere a ordem ou os nomes deles.
>* Adicione valores a cada campo exibido em negrito no cabeçalho da coluna. Eles representam campos obrigatórios.
>
>     No entanto, se um campo obrigatório contiver um valor padrão definido nas preferências do sistema, não será necessário preenchê-lo.
>
>     Por exemplo, na guia **Projeto PROJ**, os campos **setCondition** e **setConditionType** podem ficar vazios, mas as colunas **setGroupID** e **setName** não podem.
>
>* Determinados campos, incluindo **setResourceRevenue** e **setEnteredByID**, são gerados automaticamente pelo sistema. Se você inserir dados para esses campos na planilha, o processo de início os substituirá quando você fizer upload da planilha.

### Importar um registro  {#import-a-record}

Cada linha da planilha corresponde a um objeto exclusivo.

1. Adicionar informações na coluna **isNew**:

   * Se o objeto que você está importando for novo, digite **TRUE** para importar os dados na linha. Esse valor diferencia maiúsculas de minúsculas e sempre deve estar em letras maiúsculas
   * Se o objeto já estiver na Workfront, digite **FALSE** na coluna **isNew** para ignorar a linha. Esse valor diferencia maiúsculas de minúsculas e sempre deve estar em letras maiúsculas

      * Os registros que já existem no Workfront não são atualizados.
      * Se você baixou um modelo com dados do Workfront, os objetos existentes já estão marcados com **FALSE**.
      * Se você baixou um modelo em branco, não é necessário adicionar novas linhas para objetos existentes.

1. Adicione informações na coluna **ID** de uma das seguintes maneiras:

   * Se o objeto que você está importando for novo (e você digitou **TRUE** na coluna **isNew**), digite qualquer número para a ID. Esse número deve ser exclusivo na planilha. Por exemplo, se você importar três objetos, poderá fornecer a eles a ID 1, 2, 3, respectivamente.

   * Se o objeto já existir no Workfront (e **FALSE** estiver na coluna **isNew**) e você estiver importando novas informações sobre objetos existentes, a ID deverá ser o GUID alfanumérico que existe no Workfront para esse objeto.

   >[!TIP]
   >
   > Para descobrir o GUID exclusivo de um objeto no Workfront, você pode criar um relatório para esse objeto e adicionar a coluna ID ao relatório. O valor de cada objeto nessa coluna é o GUID do objeto.

   * Os registros que já existem no Workfront não são atualizados.
   * Se você baixou um modelo com dados, os objetos existentes já contêm o GUID como a ID.
   * Você pode importar um novo objeto com base em um objeto existente alterando **FALSE** para **TRUE** na coluna **isNew**, alterando a ID e fazendo os ajustes de dados necessários antes da importação.

   ![ID de exemplo para um Grupo](assets/kick-start-group-example.png)

   * Ao importar um projeto, você deve indicar uma ID de grupo.

      * Se o grupo já existir no Workfront, você deverá adicionar sua ID exclusiva ao campo **setGroupID** para o projeto.
      * Se o grupo não existir no Workfront, você poderá adicionar a planilha **Grupo** ao arquivo de importação, definir o campo **isNew** como **TRUE** na planilha Grupo e indicar uma ID numérica para o novo grupo na coluna **ID**. O campo **setGroupID** do novo projeto deve corresponder à **ID** numérica do novo grupo.

     **Exemplo:** Para um projeto, o valor exibido na coluna **setGroupID** deve ser um dos seguintes:

      * O GUID para um Grupo existente na sua instância do Workfront
      * O valor (número) na coluna ID da planilha **Grupo** se você estiver criando um novo Grupo durante a importação

1. Insira valores para os campos obrigatórios e quaisquer outros campos que você deseja preencher durante a importação.
1. (Opcional) Para adicionar dados personalizados:

   * Crie uma nova coluna para cada campo personalizado que deseja incluir no processo de importação.
   * Nomeie cada nova coluna para seu campo personalizado correspondente da seguinte maneira: **DE:[Nome do campo personalizado como ele aparece no Workfront]**. Por exemplo, você pode criar o seguinte campo personalizado: &quot;DE: Departamentos&quot;.
   * Na coluna **setCategoryID**, digite o GUID do formulário personalizado existente no qual este campo personalizado reside. Esse campo é necessário ao importar dados personalizados.
   * Se precisar adicionar vários valores de dados no campo personalizado (como botões de opção, caixas de seleção ou listas), use o delimitador de dados personalizado da barra vertical &quot;|&quot; listado na guia Preferências para separar os valores.

     **Exemplo:** Digite A|D na coluna DE:Departamentos para preencher os departamentos A e D no formulário personalizado.

### Incluir datas  {#include-dates}

O Workfront pode processar a maioria dos formatos de data. No entanto, você deve garantir que a coluna de data na planilha seja formatada como uma data. A importação falhará se a coluna estiver formatada como geral, um número ou texto.

>[!TIP]
>
>O formato mais popular é o formato MM/DD/AAAA.
>
>Por exemplo: 10/07/2023.

A Workfront também aceita valores de tempo como parte da data.

Por exemplo: 10/07/2022 13h30 ou 10h/2022 13h.

Se você omitir uma hora na data, a Workfront executará um dos seguintes procedimentos:

* O horário assume que é 12h. Para ver o resultado de data esperado, o fuso horário do sistema deve corresponder ao seu fuso horário.
* Se estiver em um objeto associado a um agendamento, o horário diferirá para o horário mais antigo permitido pelo agendamento.

>[!NOTE]
>
>Ao usar um carimbo de data e hora UNIX, você deve incluir três zeros adicionais no final do valor.
>
>Por exemplo, se o carimbo de data e hora for 7336899000, você deve inserir 7336899000000 na célula.

### Usar curingas {#use-wildcards}

Você pode usar os seguintes curingas ao preencher sua planilha de modelo do Kickstart:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Curinga</strong> </p> </th> 
   <th> <p><strong>Comportamento</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Quando usado em um campo <strong>setDate</strong>, este curinga define a data como meia-noite do dia em que você importa o Kick-Start.</p> <p>Você pode modificar o curinga usando a sintaxe padrão permitida com o curinga em um filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se quiser que um projeto inicie na segunda-feira da semana em que é importado, independentemente do dia em que você realmente realizar a importação, você poderá usar <strong>$$TODAYbw</strong>. Isso define a data de início planejada do seu projeto como 12h de domingo. Como o cronograma do projeto provavelmente não permite o trabalho nesse momento, ele começará às 9:00 da manhã de segunda-feira.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Quando usado em um campo <strong>setDate</strong>, este curinga define a data de acordo com o momento em que você cria o registro durante a importação do Kick-Start.</p> <p>Você pode modificar o curinga usando a sintaxe padrão permitida com o curinga em um filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se quiser que um projeto seja iniciado 3 horas após ser importado, você poderá usar <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Quando usado em um <strong>setAssignedToID</strong> ou outro campo baseado em userID, esse curinga atribui o trabalho ou associa o registro ao indivíduo que está executando a importação.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Este curinga foi adicionado especificamente para importações de usuário do Kickstart. Quando uma conta do Workfront é criada, um usuário com nível de acesso de Administrador do sistema é criado. O nome de usuário atribuído ao administrador padrão pode ser usado como um prefixo ao criar outros usuários na conta.</p> <p>Como os nomes de usuários devem ser exclusivos em todos os clientes, isso é útil quando você tem vários indivíduos com nomes de usuários muito comuns, como John Smith, que podem ter um nome de usuário "jsmith". Ao anexar a atribuição do nome de usuário ao nome de usuário do administrador padrão, você garante que cada nome de usuário seja exclusivo (por exemplo: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Dica: uma maneira mais elegante de garantir que os nomes de usuários sejam exclusivos em todo o sistema é inserir o endereço de email do indivíduo no campo <strong>setUsername</strong>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Substituição de nome de atributo para IDs  {#attribute-name-substitution-for-ids}

Embora seja uma prática recomendada usar IDs sempre que possível, às vezes é inconveniente usar IDs de referência cruzada de uma planilha para outra ao definir um valor de **setAttributeID**. Você pode fazer referência a valores por nome simplesmente alterando o cabeçalho da coluna.

**Exemplos:**

* **Importação do projeto**

  Ao importar projetos, defina a **setGroupID** dos projetos, acessando a planilha **Grupo de Grupos**, anotando as respectivas IDs de Grupos e colando-as nas células corretas (**setGroupID** coluna) na planilha **Projeto PROJ**.

  Isso é viável ao trabalhar com apenas alguns grupos e projetos, mas se você estiver trabalhando com vários de cada um, não é prático.

  Para fazer a Substituição de Nome de Atributo para o exemplo descrito acima, altere o cabeçalho da coluna **setGroupID** para **#setGroupID GROUP name**. Em seguida, você pode fazer referência a cada grupo do projeto por nome.

  >[!NOTE]
  >
  >A opção para usar a Substituição de Nome de Atributo está limitada a referências somente para registros existentes. Não é possível usar a substituição de nome para objetos que você está criando na mesma importação.

* **Importação de usuário**

  Ao importar usuários, preencha o **setRoleID** de uma lista de funções na guia **Função**.

  Algumas IDs de função são para registros que já existem na conta, e outras estão sendo criadas durante a importação.

  Para os novos registros de usuário atribuídos às funções existentes, é possível usar a substituição de nome. Para os novos registros de usuário atribuídos às funções importadas recentemente, não é possível.

  Veja como usar ambos os métodos no mesmo arquivo de importação:

   * Adicione uma coluna na planilha à esquerda da coluna **setRoleID**.
   * Nomeie a nova coluna **#setRoleID ROLE name**.
   * Para atribuições de função a registros existentes, insira os nomes de função na coluna **#setRoleID ROLE name**.

     Para atribuições de funções a novos registros de funções, insira a ID que você atribuiu na planilha Função Função do setRoleID.

     ![ID de Função para usuários](assets/set-role-id.png)

## Importar os dados da planilha para o Workfront

Depois de preencher o modelo do Excel com seus dados, você pode fazer upload dos dados no Workfront.

A importação do Kickstart suporta os seguintes tipos de arquivos:

* Excel (.xls ou .xlsx)
* Arquivo compactado (.ZIP) (que contém apenas arquivos .xlsx ou .xls)

  >[!NOTE]
  >
  >Você deve usar um arquivo .ZIP ao importar planilhas do Excel que fazem referência aos seguintes objetos:
  >
  >* Relatórios
  >* Documentos
  >* Avatares
  >* Visualizar, filtrar ou agrupar arquivos de propriedade
  >
  >Ao usar um arquivo de importação compactado, o arquivo .ZIP deve ter o mesmo nome do arquivo .xlsx ou .xls e todos os arquivos devem estar no mesmo nível de estrutura (sem pastas).

Para importar os dados da planilha do modelo para o Workfront:

<!--1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Clique em **Sistema** > **Importar Dados (Kick-Starts)**.

1. Na seção **Carregar dados com planilha do Kickstart**, clique em **Escolher Arquivo**, procure e selecione a planilha preenchida.

1. Clique em **Carregar.**

   Se o arquivo do Excel levar mais de 5 minutos para ser carregado para o Workfront, o aplicativo expirará e o Workfront não poderá carregar o arquivo.

   Tente importar seus dados em lotes menores de objetos.

1. (Condicional) Se estiver usando o Workfront Fusion, agora você pode ativar os FLOs ou cenários.
