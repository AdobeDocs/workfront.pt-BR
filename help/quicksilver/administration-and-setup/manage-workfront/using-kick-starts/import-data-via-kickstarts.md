---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Importar dados para o Adobe Workfront usando um modelo do Kickstart
description: Kickstarts são pastas de trabalho do Excel especialmente formatadas que você pode preencher com dados que deseja importar para o Workfront. O Adobe Workfront fornece um modelo de Início que você pode usar para fazer isso, conforme explicado no importador de dados de Início.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: 3aad2a3d9ad32313cb14670965bc3ad05ab215d3
workflow-type: tm+mt
source-wordcount: '2421'
ht-degree: 8%

---

# Importar dados para o Adobe Workfront usando um modelo do Kickstart

Kickstarts são pastas de trabalho do Excel especialmente formatadas que você pode preencher com dados que deseja importar para o Workfront. O Adobe Workfront fornece um modelo de Início que você pode usar para fazer isso, conforme explicado em [Importador de dados Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Esse processo é dividido em três tarefas principais:

* Primeiro, você exporta um modelo do Kickstart como um arquivo de planilha
* Em segundo lugar, você preenche a planilha com seus dados
* Por fim, importe a planilha preenchida para o Workfront

Cada um desses procedimentos é descrito na ordem correta neste artigo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limitação

Você pode importar um grande número de objetos para o Workfront usando um template do Kickstart. No entanto, considere as seguintes limitações:

* Importar dados dessa maneira não atualiza as informações nos registros que já existem no Workfront
* Você pode importar somente novos registros e suas informações
* Importe não mais do que 2.000 registros de cada vez para garantir que a importação não expire

## Exportar um modelo do Kickstart como um arquivo de planilha

Ao exportar um modelo de Início, você recebe uma pasta de trabalho em branco da planilha do Excel. Nos procedimentos subsequentes deste artigo, você preencherá a pasta de trabalho com suas informações e a importará de volta para o Workfront.

Para exportar um modelo do Kickstart:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Exportar dados (Kick-Starts)**.

1. Clique em **Mais opções**, em seguida, selecione os tipos de informações que deseja incluir.

   Cada opção selecionada representa uma coleção de várias guias na planilha exportada. Por exemplo, se você selecionar a opção Relatório, todos os objetos necessários para criar um relatório serão incluídos na planilha (exibições, filtros, agrupamentos, relatórios).

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
      <th> <p><strong>Planilhas na planilha exportada</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Painel de Controle</p> <p>Todos os painéis no sistema estão disponíveis para exportação. Você pode selecionar até 100 painéis específicos em uma única exportação.</p> </td> 
      <td scope="col">Exporta como arquivo ZIP</td> 
      <td scope="col"> <p>Parâmetro</p> <p>Opção de parâmetro</p> <p>Grupo de Parâmetros</p> <p>Parâmetro da Categoria</p> <p>Categoria</p> <p>Relatório</p> <p>Seção de Guias do Portal</p> <p>Painel de Controle</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Relatório</p> <p>Todos os relatórios do sistema estão disponíveis para exportação. É possível selecionar até 100 relatórios específicos em uma única exportação.</p> </td> 
      <td scope="col">Exporta como arquivo ZIP </td> 
      <td scope="col"> <p scope="col">Parâmetro</p> <p scope="col">Opção de parâmetro</p> <p scope="col">Grupo de Parâmetros</p> <p scope="col">Parâmetro da Categoria</p> <p scope="col">Categoria</p> <p scope="col">Relatório</p> <p scope="col">Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Aprovação</p> </td> 
      <td scope="col"> <p>Exporta como arquivo do Excel</p> </td> 
      <td scope="col"> <p>Aprovador da etapa</p> <p>Etapa de aprovação</p> <p>Aprovação</p> <p>Processo de aprovação</p> <p>Preferências</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Dados personalizados</p> </td> 
      <td scope="col"> <p>Exporta como arquivo do Excel</p> </td> 
      <td scope="col"> <p>Parâmetro</p> <p>Opção de parâmetro</p> <p>Grupo de Parâmetros</p> <p>Parâmetro da Categoria</p> <p>Categoria</p> <p>Preferências</p> </td> 
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
      <td> <p>Exporta como arquivo do Excel. Para ver a lista completa de opções, clique em <strong>Mais opções</strong>.</p> </td> 
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
      <td>Função de trabalho</td> 
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
      <td>Conjunto de Recursos</td> 
      <td>Exporta como arquivo do Excel</td> 
      <td> <p> Conjunto de Recursos</p> <p>Preferências </p> </td> 
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
      <td> <p>Questões do Scorecard</p> <p>Opção de scorecard</p> <p>Scorecard</p> <p>Preferências </p> </td> 
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
1. Continuar com [Preencha o modelo de planilha com seus dados](#populate-the-spreadsheet-template-with-your-data) para preencher o template com suas informações.

## Preencha o modelo de planilha com seus dados {#populate-the-spreadsheet-template-with-your-data}

* [Sobre as guias (folhas de dados) incluídas na planilha](#about-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importar um registro](#import-a-record)
* [Incluir datas](#include-dates)
* [Usar curingas](#use-wildcards)
* [Substituição de nome de atributo para IDs](#attribute-name-substitution-for-ids)

### Sobre as guias (folhas de dados) incluídas na planilha {#about-the-tabs-data-sheets-included-in-the-spreadsheet}

>[!TIP]
>
>Para entender melhor como você precisará formatar as informações em cada coluna ao preencher o modelo de Início, considere fazer uma prática executada exportando um Início com dados existentes do Workfront nos objetos que você está tentando importar. Para obter instruções, consulte [Exportar dados do Adobe Workfront via Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Quando você abre um modelo de Kick-Starts em branco, várias guias (folhas de dados) estão disponíveis. Eles dependem dos objetos selecionados para download. Cada um representa um objeto no aplicativo, como projeto, tarefas, horas, painel e usuários:

Quando você abre uma dessas guias, a linha 2 exibe os campos para cada objeto que pode ser definido durante uma importação. Em um cabeçalho de coluna, depois da palavra &quot;set&quot;, o nome do campo é exibido como aparece no banco de dados. Esses campos atuam como cabeçalhos de coluna.

>[!IMPORTANT]
>
>Para evitar erros, verifique o seguinte:
>
>* Não exclua nem modifique esses campos de forma alguma. Por exemplo, não altere a ordem ou os nomes deles.
>* Preencha cada campo com um cabeçalho de coluna exibido em negrito. Eles representam campos obrigatórios.
>
>  No entanto, se um campo obrigatório contiver um valor padrão definido nas preferências do sistema, não será necessário preenchê-lo.
>
>  Por exemplo, no campo **Projeto PROJ** , a guia **setCondition** e **setConditionType** os campos podem ficar vazios, mas a variável **setGroupID** e **setName** colunas não podem.
>

### Importar um registro  {#import-a-record}

Cada linha da planilha corresponde a um objeto exclusivo.

1. Preencha a célula na **isNew** coluna:

   * Se o objeto que você está importando for novo, digite **TRUE** para importar os dados na linha.
   * Se o objeto já estiver na Workfront, digite **FALSO** para ignorar a linha.

1. Preencha a célula na **ID** de uma das seguintes formas:

   * Se o objeto que você está importando for novo (e você digitou **TRUE** no **isNew** ), especifique qualquer número para a ID. Esse número deve ser exclusivo na planilha.

   * Se o objeto que você está importando já existir no sistema Workfront (e você digitou **FALSO** no **isNew** ), a ID deve ser o GUID alfanumérico que existe no Workfront para esse objeto.

     **Exemplo:** Para um projeto, o valor exibido na variável **setGroupID** deve ser uma das seguintes:

      * O GUID para um Grupo existente na sua instância do Workfront
      * O valor (número) na coluna ID no **Grupo do GRUPO** se você estiver criando um novo Grupo durante a importação

        ![ID de exemplo para um grupo](assets/kick-start-group-example.png)

1. Insira valores para os campos obrigatórios e quaisquer outros campos que você deseja preencher durante a importação.
1. (Opcional) Para adicionar dados personalizados:

   * Crie uma nova coluna para cada campo personalizado que deseja incluir no processo de importação.
   * Nomeie cada nova coluna para seu campo personalizado correspondente da seguinte maneira: **DE:[O nome do campo personalizado conforme exibido no Workfront]**.
   * Na coluna **setCategoryID**, digite a GUID do formulário personalizado existente no qual este campo personalizado reside. Esse campo é necessário ao importar dados personalizados.
   * Se precisar adicionar vários valores de dados no campo personalizado (como botões de opção, caixas de seleção ou listas), use o delimitador de dados personalizado da barra vertical &quot;|&quot; listado na guia Preferências para separar os valores.

     **Exemplo:** Digite A|D na coluna DE:Departamentos para preencher o departamento A e o departamento D no formulário personalizado.

### Incluir datas  {#include-dates}

O Workfront pode processar a maioria dos formatos de data. No entanto, você deve garantir que a coluna de data na planilha seja formatada como uma data. A importação falhará se a coluna estiver formatada como geral, um número ou texto.

>[!TIP]
>
>A maioria das pessoas acha mais fácil usar o formato MM/DD/AAAA (por exemplo: 07/10/2022).

O Workfront também aceita valores de hora como parte da data (por exemplo: 07/10/2022 13h30 ou 07/10/2022 13h).

Se você omitir uma hora na data, a Workfront executará um dos seguintes procedimentos:

* Pressupõe 12h. Para ver o resultado de data esperado, o fuso horário do sistema deve corresponder ao seu fuso horário.
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
   <th> <p><strong>Caractere curinga</strong> </p> </th> 
   <th> <p><strong>Comportamento</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Quando usado em um <strong>setDate</strong> , esse curinga definirá a data como meia-noite no dia em que você importar o Kick-Start.</p> <p>Você pode modificar o curinga usando a sintaxe padrão permitida com o curinga em um filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se quiser que um projeto seja iniciado na segunda-feira da semana em que é importado, independentemente do dia em que você realmente executa a importação, você poderá usar <strong>$$TODAYbw</strong>. Isso define a data de início planejada do seu projeto como 12h de domingo. Como o cronograma do projeto provavelmente não permite o trabalho nesse momento, ele começará às 9:00 da manhã de segunda-feira.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Quando usado em um <strong>setDate</strong> , esse curinga definirá a data de acordo com o momento em que você criar o registro durante a importação do Kick-Start.</p> <p>Você pode modificar o curinga usando a sintaxe padrão permitida com o curinga em um filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exemplo: </b></span></span>Se quiser que um projeto seja iniciado 3 horas após sua importação, use <strong>$$AGORA+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Quando usado em um <strong>setAssignedToID</strong> ou outro campo baseado em ID de usuário, esse curinga atribui o trabalho ou associa o registro ao indivíduo que executa a importação.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Este curinga foi adicionado especificamente para importações de usuário do Kickstart. Quando uma conta do Workfront é criada, um usuário com nível de acesso de Administrador do sistema é criado. O nome de usuário atribuído ao administrador padrão pode ser usado como um prefixo ao criar outros usuários na conta.</p> <p>Como os nomes de usuários devem ser exclusivos em todos os clientes, isso é útil quando você tem vários indivíduos com nomes de usuários muito comuns, como John Smith, que podem ter um nome de usuário "jsmith". Ao anexar a atribuição do nome de usuário ao nome de usuário do administrador padrão, você garante que cada nome de usuário seja exclusivo (por exemplo: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Dica: uma maneira mais elegante de garantir que os nomes de usuários sejam exclusivos em todo o sistema é inserir o endereço de email do indivíduo na <strong>setUsername</strong> campo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Substituição de nome de atributo para IDs  {#attribute-name-substitution-for-ids}

Embora seja uma prática recomendada usar IDs sempre que possível, às vezes é inconveniente usar IDs de referência cruzada de uma planilha para outra ao definir uma **setAttributeID** valor. Você pode fazer referência a valores por nome simplesmente alterando o cabeçalho da coluna.

**Exemplos:**

* **(importação do projeto)**

  Ao importar projetos, defina as **setGroupID** dos projetos, acessando a página **Grupo do GRUPO** planilha, anotando as respectivas IDs de Grupo e colando-as nas células corretas (**setGroupID** coluna) no **Projeto PROJ** planilha.

  Isso é viável ao trabalhar com apenas alguns grupos e projetos, mas se você estiver trabalhando com vários de cada um, não é prático.

  Para fazer a Substituição de Nome de Atributo para o exemplo descrito acima, altere a variável **setGroupID** cabeçalho da coluna para **#setGroupID GROUP****nome**. Em seguida, você pode fazer referência a cada grupo do projeto por nome.

  >[!NOTE]
  >
  >A opção para usar a Substituição de Nome de Atributo está limitada a referências somente para registros existentes. Não é possível usar a substituição de nome para objetos que você está criando na mesma importação.

* **(importação de usuários)**

  Ao importar usuários, preencha o **setRoleID** de uma lista de funções no **Função Função** guia.

  Algumas IDs de função são para registros que já existem na conta, e outras estão sendo criadas durante a importação.

  Para os novos registros de usuário atribuídos às funções existentes, é possível usar a substituição de nome. Para os novos registros de usuário atribuídos às funções importadas recentemente, não é possível.

  Veja como usar ambos os métodos no mesmo arquivo de importação:

   * Adicione uma coluna na planilha à esquerda do **setRoleID** coluna.
   * Nomeie a nova coluna **#setRoleID ROLE name**.
   * Para atribuições de funções a registros existentes, insira os nomes das funções no **#setRoleID ROLE name** coluna.

     Para atribuições de funções a novos registros de funções, insira a ID que você atribuiu na planilha Função Função do setRoleID.

     ![ID de função para usuários](assets/set-role-id.png)

## Importar os dados da planilha para o Workfront

Depois de preencher o modelo do Excel com seus dados, você pode carregá-los no Workfront.

A importação do Kickstart suporta os seguintes tipos de arquivos:

* Excel baseado em XML (&#42;.xlsx)
* Excel herdado (&#42;.xls)
* Compactado (&#42;ZIP) arquivo xlsx ou xls

  >[!NOTE]
  >
  >Você deve usar um arquivo ZIP ao importar planilhas do Excel que fazem referência a relatórios, documentos e avatares, ou visualizar, filtrar ou agrupar arquivos de propriedades. Ao usar um arquivo de importação compactado, a variável &#42;O arquivo ZIP deve ter o mesmo nome que &#42;.xlsx ou &#42;O arquivo .xls e todo o conteúdo devem estar no mesmo nível de estrutura de arquivo (sem pastas).


Para importar os dados da planilha do modelo para o Workfront:

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** >**Importar dados (Kick-Starts)**.

1. No **Carregar dados com a planilha do Kickstart** clique em **Escolher arquivo**, em seguida, navegue até a planilha preenchida e selecione-a.

1. Clique em **Carregar.**

   Se o arquivo do Excel levar mais de 5 minutos para ser carregado no Workfront, o aplicativo expirará e o arquivo não poderá ser carregado.

   Tente importar seus dados em lotes menores de objetos.

1. (Condicional) Se estiver usando o Workfront Fusion, agora você pode ativar os FLOs ou cenários.
