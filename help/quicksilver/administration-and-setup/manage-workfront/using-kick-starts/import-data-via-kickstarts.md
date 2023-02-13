---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Importar dados para o Adobe Workfront usando um modelo de Início rápido
description: Os Primeiros passos são pastas de trabalho do Excel especialmente formatadas que podem ser preenchidas com os dados que você deseja importar para o Workfront. O Adobe Workfront fornece um modelo de Início rápido que você pode usar para fazer isso, conforme explicado no importador de dados de Início rápido .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 4912349cbbc74a6f7587312e83297169ecd52f51
workflow-type: tm+mt
source-wordcount: '2412'
ht-degree: 8%

---

# Importar dados para o Adobe Workfront usando um modelo de Início rápido

Os Primeiros passos são pastas de trabalho do Excel especialmente formatadas que podem ser preenchidas com os dados que você deseja importar para o Workfront. O Adobe Workfront fornece um modelo de Início Rápido que você pode usar para fazer isso, como explicado em [Importador de dados do Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Esse processo é dividido em 3 tarefas principais:

* Primeiro, você exporta um modelo de Início Rápido como um arquivo de planilha
* Segundo, você preenche a planilha com seus dados
* Por fim, você importa a planilha preenchida para o Workfront

Cada um desses procedimentos é descrito na ordem correta neste artigo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limitações

É possível importar grandes números de objetos para o Workfront usando um modelo de Início rápido. No entanto, considere as seguintes limitações:

* Importar dados dessa forma não atualiza informações em registros que já existem no Workfront
* É possível importar apenas novos registros e suas informações
* Não importe mais de 2.000 registros de cada vez para garantir que a importação não atinja o tempo limite

## Exportar um modelo de Início Rápido como um arquivo de planilha

Ao exportar um modelo de Início rápido, você recebe uma pasta de trabalho em branco da planilha do Excel. Em procedimentos subsequentes neste artigo, você preencherá a pasta de trabalho com suas informações e a importará novamente para o Workfront.

Para exportar um modelo de Início Rápido:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Exportar dados (início rápido)**.

1. Clique em **Mais opções** e selecione os tipos de informações que deseja incluir.

   Cada opção selecionada representa uma coleção de várias guias na planilha exportada. Por exemplo, se você selecionar a opção Relatório , todos os objetos necessários para criar um relatório serão incluídos na planilha (exibições, filtros, agrupamentos, relatórios).

   Você pode usar todos os tipos de objetos listados abaixo para importar dados para o Workfront. (A única exceção é a opção Níveis de Acesso. A folha de dados Níveis de Acesso em uma exportação é fornecida para fins de referência. Ela permite atribuir um nível de acesso a uma nova conta de usuário por ID.)

   O modelo para cada um dos tipos de objetos pode ser exportado nos seguintes formatos de arquivo e contém as seguintes planilhas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objeto</strong> </p> </th> 
      <th> <p><strong>Exportações como</strong> </p> </th> 
      <th> <p><strong>Planilhas na planilha exportada</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Painel de Controle</p> <p>Todos os painéis no sistema estão disponíveis para exportação. Você pode selecionar até 100 painéis específicos em uma única exportação.</p> </td> 
      <td scope="col">Exportar como arquivo ZIP</td> 
      <td scope="col"> <p>Parâmetro</p> <p>Opção de parâmetro</p> <p>Grupo de Parâmetros</p> <p>Parâmetro da Categoria</p> <p>Categoria</p> <p>Relatório</p> <p>Seção de Guias do Portal</p> <p>Painel de Controle</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Relatório</p> <p>Todos os relatórios no sistema estão disponíveis para exportação. É possível selecionar até 100 relatórios específicos em uma única exportação.</p> </td> 
      <td scope="col">Exportar como arquivo ZIP </td> 
      <td scope="col"> <p scope="col">Parâmetro</p> <p scope="col">Opção de parâmetro</p> <p scope="col">Grupo de Parâmetros</p> <p scope="col">Parâmetro da Categoria</p> <p scope="col">Categoria</p> <p scope="col">Relatório</p> <p scope="col">Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Aprovação</p> </td> 
      <td scope="col"> <p>Exportar como arquivo Excel</p> </td> 
      <td scope="col"> <p>Aprovador de etapa</p> <p>Etapa de aprovação</p> <p>Aprovação</p> <p>Processo de aprovação</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Dados personalizados</p> </td> 
      <td scope="col"> <p>Exportar como arquivo Excel</p> </td> 
      <td scope="col"> <p>Parâmetro</p> <p>Opção de parâmetro</p> <p>Grupo de Parâmetros</p> <p>Parâmetro da Categoria</p> <p>Categoria</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Tipo de Despesa</p> </td> 
      <td scope="col"> <p>Exportar como arquivo Excel</p> </td> 
      <td> <p>Tipo de Despesa</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Tipo de hora</p> </td> 
      <td scope="col"> <p>Exportar como arquivo Excel</p> </td> 
      <td> <p>Tipo de hora</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Equipe</p> </td> 
      <td scope="col"> <p>Exportar como arquivo Excel</p> </td> 
      <td> <p> Integrante da Equipe</p> <p>Equipe</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Usuário</p> </td> 
      <td> <p>Exporta como arquivo Excel. Para ver a lista completa de opções, clique em <strong>Mais opções</strong>.</p> </td> 
      <td> <p>Usuário</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Nível de acesso</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p>Nível de acesso</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Atribuição</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p>Atribuição</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Empresa</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Empresa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Modelo de email</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p>Modelo de email</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Despesa</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Despesa'</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Página Externa</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Página Externa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Filtro</td> 
      <td>Exportações como arquivo ZIP</td> 
      <td> <p> Filtro</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Grupo</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Grupo</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Agrupamento</td> 
      <td>Exportações como arquivo ZIP</td> 
      <td> <p> Agrupamento</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Hora</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Hora</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Problema</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Problema</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Função de trabalho</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Função</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Caminho de Etapas</td> 
      <td> Exportar como arquivo Excel</td> 
      <td> <p> Etapa</p> <p>Caminho de Etapas</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Nota</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Nota</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Portfólio</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Portfólio</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Projeto</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Fila</p> <p>Projeto</p> <p>Regra de Encaminhamento</p> <p>Enfileirar tópico</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Estimativa de Recursos</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Estimativa de Recursos</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Conjunto de Recursos</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Conjunto de Recursos</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Risco</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Risco</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Tipo de Risco</td> 
      <td> Exportar como arquivo Excel</td> 
      <td> <p> Tipo de Risco</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td>Scorecard</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p>Questões do Scorecard</p> <p>Opção de scorecard</p> <p>Scorecard</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Tarefa</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Tarefa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Modelo</td> 
      <td> Exportar como arquivo Excel</td> 
      <td> <p> Fila</p> <p>Modelo</p> <p>Regra de Encaminhamento</p> <p>Enfileirar tópico</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Atribuição de Modelo</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Atribuição de Modelo</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Modelo de Tarefa</td> 
      <td>Exportar como arquivo Excel</td> 
      <td> <p> Modelo de Tarefa</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Planilha de horas</td> 
      <td> Exportar como arquivo Excel</td> 
      <td> <p> Perfil da Planilha de Horas</p> <p>Planilha de horas</p> <p>Preferências </p> </td> 
     </tr> 
     <tr> 
      <td>Exibir </td> 
      <td> <p>Exportar como arquivo ZIP</p> </td> 
      <td> <p> Exibir</p> <p>Preferências </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Baixar**.
1. Continue com [Preencha o modelo de planilha com seus dados](#populate-the-spreadsheet-template-with-your-data) para preencher o modelo com suas informações.

## Preencha o modelo de planilha com seus dados {#populate-the-spreadsheet-template-with-your-data}

* [Sobre as guias (folhas de dados) incluídas na planilha](#about-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importar um registro](#import-a-record)
* [Incluir datas](#include-dates)
* [Usar curingas](#use-wildcards)
* [Substituição de nome de atributo para IDs](#attribute-name-substitution-for-ids)

### Sobre as guias (folhas de dados) incluídas na planilha {#about-the-tabs-data-sheets-included-in-the-spreadsheet}

>[!TIP]
>
>Para entender melhor como você precisará formatar as informações em cada coluna ao preencher o modelo de Início rápido, considere fazer uma prática executada exportando um Início rápido com dados existentes do Workfront nos objetos que você está tentando importar. Para obter instruções, consulte [Exportar dados do Adobe Workfront via Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Quando você abre um modelo Kick-Starts em branco, várias guias (folhas de dados) ficam disponíveis. Eles dependem dos objetos selecionados para download. Cada um representa um objeto no aplicativo, como projeto, tarefas, horas, painel e usuários:

Ao abrir uma dessas guias, a linha 2 exibe os campos para cada objeto que pode ser definido durante uma importação. Em um cabeçalho de coluna, após a palavra &quot;conjunto&quot;, o nome do campo é exibido como aparece no banco de dados. Esses campos atuam como cabeçalhos de coluna.

>[!IMPORTANT]
>
>Para evitar erros, verifique o seguinte:
>
>* Não exclua nem modifique esses campos de forma alguma. Por exemplo, não altere sua ordem ou seus nomes.
>* Preencha todos os campos com um cabeçalho de coluna exibido em negrito. Elas representam campos obrigatórios.
>
>  No entanto, se um campo obrigatório contiver um valor padrão definido nas preferências do sistema, você não precisará preenchê-lo.
>
>  Por exemplo, no **Projeto PROJ** , a variável **setCondition** e **setConditionType** os campos podem ficar vazios, mas a variável **setGroupID** e **setName** não é possível.

### Importar um registro  {#import-a-record}

Cada linha da folha corresponde a um objeto exclusivo.

1. Complete a célula na **isNew** coluna:

   * Se o objeto que você está importando for novo, digite **TRUE** para importar os dados na linha.
   * Se o objeto já estiver no Workfront, digite **FALSE** para ignorar a linha.

1. Complete a célula na **ID** em uma das seguintes maneiras:

   * Se o objeto que você está importando for novo (e você digitou **TRUE** no **isNew** ), especifique qualquer número para a ID. Esse número deve ser exclusivo na planilha.

   * Se o objeto que você está importando já existir no sistema Workfront (e você digitou **FALSE** no **isNew** ), a ID deve ser o GUID alfanumérico existente no Workfront para esse objeto.

      **Exemplo:** Para um projeto, o valor exibido na variável **setGroupID** deve ser uma das seguintes opções:

      * O GUID de um grupo existente na sua instância do Workfront
      * O valor (número) na coluna ID do **Grupo GRUPO** planilha se estiver criando um novo Grupo durante a importação

         ![](assets/verysimplekickstartprojectimport-350x31.png)

1. Insira valores para os campos obrigatórios e quaisquer outros campos que você deseja preencher durante a importação.
1. (Opcional) Para adicionar dados personalizados:

   * Crie uma nova coluna para cada campo personalizado que deseja incluir no processo de importação.
   * Nomeie cada nova coluna para seu campo personalizado correspondente da seguinte maneira: **DE:[Nome do campo personalizado como aparece no Workfront]**.
   * Na coluna **setCategoryID**, digite o GUID do formulário personalizado existente no qual esse campo personalizado reside. Esse campo é necessário ao importar dados personalizados.
   * Se você precisar adicionar vários valores de dados no campo personalizado (como botões de opção, caixas de seleção ou listas), use o delimitador de dados personalizado da barra vertical &quot;|&quot; listado na guia Preferências para separar os valores.

      **Exemplo:** Digite A|D na coluna DE:Departamentos para preencher o departamento A e o departamento D em seu formulário personalizado.

### Incluir datas  {#include-dates}

O Workfront pode processar a maioria dos formatos de data. No entanto, é necessário garantir que a coluna de data na planilha seja formatada como uma data. A importação falhará se a coluna for formatada como geral, número ou texto.

>[!TIP]
>
>A maioria das pessoas acha mais fácil usar o formato MM/DD/AAAA (por exemplo: 10/07/2022).

A Workfront também aceita valores de hora como parte da data (por exemplo: 07/10/2022 01:30 ou 07/10/2022 1:00 PM).

Se você omitir uma hora na data, o Workfront executará um dos seguintes procedimentos:

* Pressupõe 12:00 Para ver o resultado da data que você espera, o fuso horário do sistema deve corresponder ao seu fuso horário.
* Se estiver em um objeto associado a uma programação, a hora será adiada para a hora mais antiga que a programação permitir.

>[!NOTE]
>
>Ao usar um carimbo de data e hora UNIX, você deve incluir três zeros adicionais no final do valor.
>
>Por exemplo, se o carimbo de data e hora é 7336899000, você inseriria 733689900000 na célula.

### Usar curingas {#use-wildcards}

Você pode usar os seguintes curingas ao preencher a planilha do modelo de Início Rápido:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Caractere curinga</strong> </p> </th> 
   <th> <p><strong>Comportamento</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Quando usado em um <strong>setDate</strong> , esse curinga define a data como meia-noite no dia em que você importar o Início.</p> <p>Você pode modificar o curinga usando a sintaxe padrão permitida com o curinga em um filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se você quiser que um projeto tenha início na segunda-feira da semana em que ele for importado, independentemente do dia em que você realmente realizar a importação, poderá usar <strong>$$TODAYbw</strong>. Isso define a data de início planejada do seu projeto como 12h no domingo. Como o cronograma do projeto provavelmente não permite trabalho naquela hora, ele começará às 9h na segunda-feira de manhã.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Quando usado em um <strong>setDate</strong> , esse curinga define a data de acordo com o momento em que você cria o registro durante a importação de Início.</p> <p>Você pode modificar o curinga usando a sintaxe padrão permitida com o curinga em um filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se quiser que um projeto seja iniciado 3 horas após a importação, use <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Quando usado em um <strong>setAssignedToID</strong> Para outro campo baseado em userID , esse curinga atribui o trabalho ou associa o registro ao indivíduo que está executando a importação.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Esse curinga foi adicionado especificamente para importações de usuários do Kick-Start. Quando uma conta Workfront é criada, um usuário com o nível de acesso Administrador do sistema é criado. O nome de usuário atribuído ao administrador padrão pode ser usado como um prefixo ao criar outros usuários na conta.</p> <p>Como os nomes de usuário devem ser exclusivos em todos os clientes, isso é útil quando você tem vários indivíduos com nomes de usuário muito comuns, como John Smith, que podem ter um nome de usuário "jsmith". Ao anexar a atribuição de nome de usuário ao nome de usuário padrão do administrador, você garante que cada nome de usuário seja exclusivo (por exemplo: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Dica: Uma maneira mais elegante de garantir que os nomes de usuário sejam exclusivos em todo o sistema é inserir o endereço de email do indivíduo no <strong>setUsername</strong> campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Substituição de nome de atributo para IDs  {#attribute-name-substitution-for-ids}

Embora seja uma prática recomendada usar IDs sempre que possível, às vezes é inconveniente cruzar as IDs de referência de uma planilha para outra ao definir uma **setAttributeID** valor. Você pode fazer referência a valores por nome simplesmente alterando o cabeçalho da coluna.

**Exemplos:**

* **(importação de projeto)**

   Ao importar projetos, defina a variável **setGroupID** dos projetos, indo para a **Grupo GRUPO** , anotando as respectivas IDs de grupo e colando nas células corretas (**setGroupID** na coluna **Projeto PROJ** folha.

   Isso é viável ao trabalhar com apenas alguns grupos e projetos, mas se você estiver trabalhando com vários de cada um, não é prático.

   Para fazer a Substituição de Nome de Atributo do exemplo descrito acima, altere a **setGroupID** cabeçalho da coluna para **#setGroupID GROUP***name**. Você pode fazer referência ao grupo de cada projeto por nome.

   >[!NOTE]
   >
   >A opção para usar a Substituição de Nome de Atributo é limitada apenas a referências para registros existentes. Não é possível usar substituição de nome para objetos que você está criando na mesma importação.

* **(importação de usuário)**

   Ao importar usuários, preencha o **setRoleID** de uma lista de funções na **Função** guia .

   Algumas das IDs de função são para registros que já existem na conta e outras estão sendo criadas durante a importação.

   Para os novos registros de usuário atribuídos às funções existentes, você pode usar a substituição de nome. Para os novos registros de usuário atribuídos a funções recém-importadas, não é possível.

   Veja como usar ambos os métodos no mesmo arquivo de importação:

   * Adicionar uma coluna na planilha à esquerda da **setRoleID** coluna.
   * Nomeie a nova coluna **#setRoleID nome da FUNLE**.
   * Para atribuições de função para registros existentes, insira os nomes da função no **#setRoleID nome da FUNLE** coluna.

      Para atribuições de função para novos registros de função, insira a ID atribuída na folha Função de FUNÇÃO em setRoleID.

      ![](assets/setroleid-350x66.png)

## Importar os dados da planilha para o Workfront

Depois de preencher o modelo do Excel com seus dados, você pode fazer upload dos dados no Workfront.

A importação de Início Rápido é compatível com os seguintes tipos de arquivo:

* Excel baseado em XML (&#42;.xlsx)
* Excel herdado (&#42;.xls)
* Zipado (&#42;ZIP) arquivo xlsx ou xls

   >[!NOTE]
   >
   >Você deve usar um arquivo ZIP ao importar planilhas do Excel que fazem referência a relatórios, documentos e avatares, ou visualizar, filtrar ou agrupar arquivos de propriedades. Ao usar um arquivo de importação compactado, a variável &#42;O arquivo ZIP deve ter o mesmo nome do arquivo &#42;.xlsx ou &#42;Arquivo .xls e todo o conteúdo deve estar no mesmo nível de estrutura de arquivo (sem pastas).


Para importar os dados da planilha de modelos para o Workfront:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** >**Importar dados (Início)**.

1. No **Fazer upload de dados com a planilha de início rápido** seção , clique em **Escolher arquivo**, em seguida, navegue até a planilha preenchida e selecione-a.

1. Clique em **Faça upload.**

   Se o arquivo Excel levar mais de 5 minutos para ser carregado no Workfront, o aplicativo expirará e o arquivo não poderá ser carregado.

   Tente importar seus dados em lotes menores de objetos.

1. (Condicional) Se você estiver usando o Workfront Fusion, agora poderá ativar os FLOs ou cenários.
