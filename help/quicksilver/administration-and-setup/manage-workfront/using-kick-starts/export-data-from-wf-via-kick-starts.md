---
user-type: administrator
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Exportar dados do Adobe Workfront via Kick-Starts
description: Como administrador do Adobe Workfront, você pode usar o exportador de dados Kick-Starts para exportar dados do Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7f56b63e-a674-43e4-bef6-d276898e2074
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '1101'
ht-degree: 9%

---

# Exportar dados do Adobe Workfront via Kick-Starts

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Como administrador do Adobe Workfront, você pode usar o exportador de dados Kick-Starts para exportar dados do Workfront. Você pode usá-lo em outros aplicativos depois de exportá-lo.

A exportação de dados por meio de Kick-Starts também é útil para entender quais campos estão associados a cada objeto, como esses campos são codificados e como os valores desses campos são formatados no banco de dados.

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

## Vantagens e desvantagens de usar o início para exportar dados

Há duas maneiras de exportar dados no Workfront:

* Exportação de dados de um relatório ou lista

   Para obter mais informações sobre como exportar dados de um relatório ou lista, consulte [Exportar dados](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* Exportação de dados por início

A tabela a seguir mostra as vantagens e desvantagens de cada método:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>  </th> 
   <th> <p>Os dados exportados incluem valores de objeto e campo</p> </th> 
   <th> <p>Capacidade de exportar dados em torno de vários tipos de objetos simultaneamente</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Exportar dados de uma exibição de lista</strong> </p> <p>Para obter mais informações sobre como exportar dados de uma lista, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md" class="MCXref xref">Exportar dados</a></p> </td> 
   <td> <p>Sim</p> <p>Os campos nativos do Workfront e os campos personalizados associados aos objetos são exportados.</p> </td> 
   <td> <p>não</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Exportação de dados por meio de Kick-Starts</strong> </p> </td> 
   <td> <p>Sim (limitado)</p> <p>A maioria dos campos nativos do Workfront associados aos objetos são exportados, mas alguns não são. Por exemplo, não é possível exportar os campos Programação, Proprietário do projeto ou Patrocinador do projeto por meio de uma exportação de início de projeto.</p> <p>Em um projeto que tem um formulário personalizado anexado, os dados inseridos nos campos do formulário não são exportados.</p> <p>Mas é possível exportar um formulário personalizado. O arquivo resultante lista os campos configurados no formulário, como caixas de texto e botões de opção.</p> </td> 
   <td> <p>Sim</p> <p>Usar o Kick-Starts para exportar dados do Workfront permite exportar dados relacionados a vários tipos de objetos em uma única exportação. Por exemplo, é possível incluir tarefas, problemas e projetos em uma única exportação.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Limites de exportação

As seguintes limitações existem ao exportar dados por início (os dados são exportados em um formato de arquivo Excel):

* **50.000 linhas:** O número de linhas permitidas no arquivo.
* **65.530 hiperlinks:** Esse é um limite imposto pelo Excel para documentos que contêm mais de 65.530 hiperlinks. Esses documentos não podem ser abertos após serem exportados. Observe que um documento do Excel pode ter apenas 200 linhas de dados, mas se houver mais de 65.530 links dentro do documento, ele não abrirá.

## Exportar dados via início

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Primeiros Passos,** em seguida, clique em **Exportar dados.**

1. Selecione o objeto que deseja exportar.
1. Clique em **Mais opções** para ver a lista completa de objetos.

   Todos os objetos listados aqui também podem ser usados para importar dados para o Workfront.

   A única exceção é a **Níveis de acesso** objeto. A folha de dados Níveis de Acesso incluída em uma exportação é fornecida somente para fins de referência. Ela permite atribuir um nível de acesso a uma nova conta de usuário por ID.

   Para obter mais informações sobre a importação de dados para o Workfront por meio de inicializações, consulte [Importar dados para o Adobe Workfront usando um modelo de Início rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md). Esta é uma lista de todos os objetos que podem ser exportados por meio de início:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p>Objeto</p> </th> 
      <th> <p>Planilhas exportadas do arquivo Excel</p> </th> 
      <th> <p>Formato de exportação</p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top">Nível de acesso</td> 
      <td scope="col" valign="top">Nível de acesso<br>Preferências</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Atribuição</td> 
      <td scope="col" valign="top">Atribuição<br>Preferências</td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Empresa</td> 
      <td scope="col" valign="top"> Empresa<br>Preferências </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Modelo de email</td> 
      <td scope="col" valign="top"> Modelo de email<br>Preferências </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top">Despesa</td> 
      <td valign="top"> Despesa<br>Preferências </td> 
      <td scope="col" valign="top"> Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Página Externa</td> 
      <td valign="top"> Página Externa<br>Preferências </td> 
      <td scope="col" valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Filtro</td> 
      <td valign="top"> Filtro<br>Preferências </td> 
      <td valign="top">ZIP </td> 
     </tr> 
     <tr> 
      <td valign="top">Grupo</td> 
      <td valign="top"> Grupo<br>Preferências  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Agrupamento</td> 
      <td valign="top"> Agrupamento<br>Preferências </td> 
      <td valign="top">ZIP</td> 
     </tr> 
     <tr> 
      <td valign="top">Hora</td> 
      <td valign="top"> Hora<br>Preferências </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Problema</td> 
      <td valign="top"> Problema<br>Preferências </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Função de trabalho</td> 
      <td valign="top"> Função<br>Preferências </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Caminho de Etapas</td> 
      <td valign="top"> Marco<br>Caminho do marco<br>Preferências </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Nota</td> 
      <td valign="top"> Observação<br>Preferências </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Portfólio</td> 
      <td valign="top"> Portfolio<br>Preferências  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Projeto</td> 
      <td valign="top"> Fila<br>Projeto<br>Regra de Roteamento<br>Tópico da fila<br>Preferências </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Estimativa de Recursos</td> 
      <td valign="top"> Estimativa de recursos<br>Preferências </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Conjunto de Recursos</td> 
      <td valign="top"> Pool de Recursos<br>Preferências </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Risco</td> 
      <td valign="top"> Risco<br>Preferências  </td> 
      <td valign="top">Excel</td> 
     </tr> 
     <tr> 
      <td valign="top">Tipo de Risco</td> 
      <td valign="top"> Tipo de risco<br>Preferências  </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Scorecard</td> 
      <td valign="top">Perguntas sobre Scorecard<br>Opção de Scorecard<br>Scorecard<br>Preferências </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Tarefa</td> 
      <td valign="top"> Tarefa<br>Preferências </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Modelo</td> 
      <td valign="top"> Fila<br>Modelo<br>Regra de Roteamento<br>Tópico da fila<br>Preferências </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top">Atribuição de Modelo</td> 
      <td valign="top"> Atribuição de Modelo<br>Preferências </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Modelo de Tarefa</td> 
      <td valign="top"> Tarefa de Modelo<br>Preferências </td> 
      <td valign="top">Excel </td> 
     </tr> 
     <tr> 
      <td valign="top">Planilha de horas</td> 
      <td valign="top"> Perfil da folha de horas<br>Folha de Horas<br>Preferências </td> 
      <td valign="top">Excel  </td> 
     </tr> 
     <tr> 
      <td valign="top"> Exibir </td> 
      <td valign="top"> Exibir<br>Preferências  </td> 
      <td valign="top">ZIP</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Download.**

   O arquivo de início de lançamento exportado é baixado para o computador como um arquivo do Excel ou um . arquivo zip contendo vários arquivos Excel e propriedades. Cada arquivo do Excel é uma coleção de folhas, em que cada folha representa um campo associado ao objeto selecionado. Existe um **Propriedades** planilha associada a cada exportação.

   O **Painel** e **Relatório** permitem selecionar painéis e relatórios específicos para incluir no download. Você pode exportar somente Painéis que são compartilhados em todo o sistema.

   Não é possível exportar relatórios de matriz. Para obter mais informações sobre relatórios de matriz, consulte [Criar um relatório de matriz](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-matrix-report.md).

   É possível selecionar até 100 Painéis e 100 Relatórios em uma única exportação.

   ![](assets/kickstart-export-350x381.png)

   É possível exportar vários objetos de uma vez.

   Por padrão, os seguintes objetos são exibidos na variável **O que incluir** rótulo (antes de clicar em **Mais opções**):

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objeto</strong> </p> </th> 
      <th> <p><strong>Planilhas exportadas do arquivo Excel</strong> </p> </th> 
      <th> <p> <strong>Formato de exportação</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Painel de Controle</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parâmetro<br>Opção de parâmetro<br>Grupo de parâmetros<br>Parâmetro de categoria<br>Categoria<br>Relatório<br>Seção Guia Portal<br>Painel<br>Preferências</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Relatório</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parâmetro<br>Opção de parâmetro<br>Grupo de parâmetros<br>Parâmetro de categoria<br>Categoria<br>Relatório<br>Preferências</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Aprovação</p> </td> 
      <td scope="col" valign="top"> <p>Aprovador de etapa<br>Etapa de aprovação<br>Aprovação<br>Processo de aprovação<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Dados personalizados</p> </td> 
      <td scope="col" valign="top"> <p>Parâmetro<br>Opção de parâmetro<br>Grupo de parâmetros<br>Parâmetro de categoria<br>Categoria<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Tipo de Despesa</p> </td> 
      <td valign="top"> <p>Tipo de Despesa<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Tipo de hora</p> </td> 
      <td valign="top"> <p>Tipo de hora<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Equipe</p> </td> 
      <td valign="top"> Membro da Equipe<br>Equipe<br>Preferências </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Usuário</p> </td> 
      <td valign="top"> <p>Usuário<br>Preferências</p> </td> 
      <td valign="top"> <p> Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong></strong> </p> </th> 
      <th> <p><strong>Planilhas exportadas do arquivo Excel</strong> </p> </th> 
      <th> <p> <strong>Formato de exportação</strong></p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col" valign="top"> <p>Painel de Controle</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top"> <p>Parâmetro<br>Opção de parâmetro<br>Grupo de parâmetros<br>Parâmetro de categoria<br>Categoria<br>Relatório<br>Seção Guia Portal<br>Painel<br>Preferências</p> </td> 
      <td scope="col" valign="top"> ZIP</td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Relatório</p> <p> </p> <p> </p> </td> 
      <td scope="col" valign="top">Parâmetro<br>Opção de parâmetro<br>Grupo de parâmetros<br>Parâmetro de categoria<br>Categoria<br>Relatório<br>Preferências</td> 
      <td scope="col" valign="top"> ZIP </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Aprovação</p> </td> 
      <td scope="col" valign="top"> <p>Aprovador de etapa<br>Etapa de aprovação<br>Aprovação<br>Processo de aprovação<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Dados personalizados</p> </td> 
      <td scope="col" valign="top"> <p>Parâmetro<br>Opção de parâmetro<br>Grupo de parâmetros<br>Parâmetro de categoria<br>Categoria<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td scope="col" valign="top"> <p>Tipo de Despesa</p> </td> 
      <td valign="top"> <p>Tipo de Despesa<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Tipo de hora</p> </td> 
      <td valign="top"> <p>Tipo de hora<br>Preferências</p> </td> 
      <td scope="col" valign="top"> <p>Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Equipe</p> </td> 
      <td valign="top"> Membro da Equipe<br>Equipe<br>Preferências </td> 
      <td scope="col" valign="top"> <p> Excel</p> </td> 
     </tr> 
     <tr> 
      <td valign="top"> <p>Usuário</p> </td> 
      <td valign="top"> <p>Usuário<br>Preferências</p> </td> 
      <td valign="top"> <p>Excel</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Recomendado) Analise os dados exportados para garantir que todas as informações que você espera ver foram exportadas.

   Para exportações grandes, o Workfront funciona em segundo plano para produzir o arquivo Excel e fornece uma mensagem de aviso sobre o atraso. O arquivo de início é enviado por email para você quando o download termina.

   ![](assets/large-kick-start-file-warning-350x65.png)
