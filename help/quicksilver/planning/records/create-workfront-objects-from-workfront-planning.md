---
title: Criar Objetos Workfront a partir do Workfront Planning
description: Você pode criar tipos de objetos do Workfront à medida que os conecta a outros registros no Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7c3db950-4cd9-424c-a7a7-4fa7dfa995f6
source-git-commit: 928ea5da9955b8c1c98782df81698c49987d4c18
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Criar objetos Workfront a partir do Workfront Planning


<!-- remove preview and production at release time-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode criar os seguintes tipos de objetos do Workfront no Workfront Planning:

* Projetos
* Portfólios

Você pode criar projetos e portfólios do Workfront no Workfront Planning ao conectar um registro do Workfront Planning a um projeto ou portfólio.

>[!IMPORTANT]
>
>* Você pode criar somente projetos e portfólios no Workfront ao conectá-los a partir de um registro.
>
>* Não é possível criar programas, grupos ou empresas ao conectá-los a partir de um registro no Workfront Planning.
>
<!--* You cannot create a project from a template when when you create projects by connecting them from a record. You must manually add tasks and project information or a template to the new project after you add it to the record.-->

Para obter informações sobre como conectar registros do Planning a objetos do Workfront, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso do Workfront Planning.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Produtos</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Planejamento do Adobe Workfront<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer um dos seguintes planos da Workfront:</p> 
<ul><li>Selecionar</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>O Workfront Planning não está disponível para planos herdados do Workfront</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Pacote de planejamento do Adobe Workfront*</p></td> 
   <td> 
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada do Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td> Padrão
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p> 
   <p>Edite o acesso no Workfront para os tipos de objeto que deseja criar (projetos e portfólios) à medida que os registros são conectados a eles. </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Gerencie permissões no espaço de trabalho ao qual deseja adicionar registros. </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   <p>Gerencie permissões para objetos do Workfront (portfólios) para adicionar objetos secundários (projetos).</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos para criar objetos do Workfront ao conectá-los a registros do Workfront Planning

Você deve ter o seguinte antes de adicionar novos projetos ou portfólios, conectando-os a partir de registros existentes:

* Tipos de registros conectados a projetos ou portfólios do Workfront. Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
* Registros. Para obter informações, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).
* O acesso e as permissões corretos no Workfront Planning e no Workfront, conforme descrito na seção [Requisitos de acesso](#access-requirements) deste artigo.

## Criar projetos ao conectá-los a registros do Workfront Planning

Para criar projetos ao conectá-los a partir de outros registros:

1. Vá para a página de detalhes de um registro ou para a tabela do tipo de registro e comece a conectar os registros do Workfront Planning aos projetos do Workfront, conforme descrito no artigo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   Você pode conectar projetos a partir de um campo de conexão nas seguintes áreas do Workfront Planning:

   * A exibição de tabela de um tipo de registro
   * A página de detalhes ou a caixa de visualização de um registro

1. (Condicional) Se não conseguir encontrar um projeto ao tentar adicioná-lo do campo de registro conectado de outro registro, adicione um nome e clique em **+ Adicionar**. O botão Adicionar é seguido pelo nome do projeto digitado.

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction above out and say "Click +Add to add a new project"; take this out too: "The Add button is followed by the project name you typed."-->

   ![](assets/add-project-when-connecting-it-from-connection-field.png)

   <span class="preview">A caixa **Criar projeto** é aberta.</span>

1. <span class="preview">(Opcional) Atualize o **Nome do projeto**. Por padrão, o projeto é nomeado de acordo com o que você adicionou como item de pesquisa ao conectá-lo do registro. </span>
1. <span class="preview">(Opcional) Selecione um **Modelo de projeto**. Se você não selecionar um modelo, o Workfront criará um projeto em branco, sem tarefas. </span>
1. <span class="preview">Clique em **Criar**. </span>
1. <span class="preview">(Condicional) Se você optou por criar um projeto a partir de um modelo, siga as etapas do artigo [Criar um projeto usando um modelo](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md) para concluir a adição do projeto.</span>

   O novo projeto é criado e adicionado ao campo conectado do registro selecionado.

1. (Opcional) Clique no nome do novo projeto no Workfront Planning para abrir a página do projeto no Workfront e fazer atualizações adicionais no projeto.

## Criar portfólios ao conectá-los a registros do Workfront Planning

Para criar portfólios à medida que você os conecta a partir de outros registros:

1. Vá para a página de detalhes de um registro ou para a tabela do tipo de registro e comece a conectar os registros do Workfront Planning aos portfólios do Workfront, conforme descrito no artigo [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   Você pode conectar portfólios de um campo de conexão nas seguintes áreas do Workfront Planning:

   * A exibição de tabela de um tipo de registro
   * A página de detalhes ou a caixa de visualização de um registro

   <!--at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new portfolio"; take this out too: "The Add button is followed by the portfolio name you typed."-->

1. (Condicional) Se não conseguir encontrar um portfólio ao tentar adicioná-lo do campo de registro conectado de outro registro, adicione um nome e clique em **+ Adicionar portfólio**. O botão Add também é seguido pelo nome do portfólio digitado.

   ![](assets/add-portfolio-when-connecting-it-from-connection-field.png)

   O portfólio é criado e adicionado ao campo de conexão do registro selecionado.

1. (Opcional) Clique no nome do novo portfólio no Workfront Planning para abrir a página do portfólio no Workfront e fazer atualizações adicionais no portfólio.

<!--

<div class="preview">

## Create programs when connecting them with records from Workfront Planning

To create programs as you are connecting them from other records: 

1. Go to a record's details page or to the record type's table and start connecting Workfront Planning records with Workfront portfolios, as described in the article [Connect records](/help/quicksilver/planning/records/connect-records.md). 

    You can connect programs from a connection field in following areas of Workfront Planning:

    * The table view of a record type
    * The details page or preview box of a record

    ********at production or when the permanent Add button is released to preview, take the first part of the direction below out and say "Click +Add to add a new program"; take this out too: "The Add button is followed by the program name you typed."***********
    
1. (Conditional) If you cannot find a program when trying to add it from the connected record field of another record, add a name, then click **+ Add**. The Add button is followed by the program name you typed. 

    ![](assets/add-wf-program-when-connecting-it-from-connection-field.png)

    The **Create program** box opens.

1. Update the **Program name**. This is a required field.
1. Choose a **Portfolio** from the drop-down, or start typing the name of a portfolio, then select it when it displays in the list. This is a required field. 
1. Click **Create**.

    The program is created and added to the connection field of the record you selected. 

1. (Optional) Click the name of the new program from Workfront Planning to open the program's page in Workfront and make additional updates to it. 

</div>

-->