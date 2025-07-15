---
title: Exportar Registros da Exibição de Tabela
description: É possível exportar registros e suas informações da exibição de tabela para um arquivo CSV ou do Excel.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 8f4c1be156094d18df4bc3628d4f1fca90372119
workflow-type: tm+mt
source-wordcount: '498'
ht-degree: 2%

---


# Exportar registros da exibição de tabela

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Você pode exportar registros e suas informações da exibição de tabela para um arquivo Excel ou CSV no Adobe Workfront Planning.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

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
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar o Workfront Planning.</p> 
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td> 
   <td><p> Padrão </p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configuração do nível de acesso</p></td> 
   <td> <p>Não há controles de nível de acesso para o Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para uma exibição</p>  
   <p>Permissões de exibição para uma exibição para alterar temporariamente as configurações de exibição, duplicá-las ou exportá-las.</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exportar registros da exibição de tabela

Considere o seguinte ao exportar a exibição de tabela:

* As informações exportadas para um arquivo do Excel preservam os filtros, agrupamentos e classificações aplicados à exibição de tabela no Workfront Planning. Os agrupamentos não estão visíveis no arquivo CSV.

* Miniaturas e cores de linha personalizadas não são suportadas em arquivos exportados.

* Somente os campos tornados visíveis na interface do Workfront são exportados. Campos ocultos não são exportados.

Para exportar informações da exibição de tabela ou de um tipo de registro:

1. Vá para uma página de tipo de registro e clique em uma guia de exibição de tabela.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o nome da guia de exibição de tabela, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome da exibição e clique em **Exportar**.

   ![Mais menus em um modo de exibição](assets/view-more-menu-with-duplicate-option.png)

   * Clique em **Compartilhar** > **Exportar a exibição atual**. Essa opção está disponível somente quando você exibe a exibição de tabela.

   ![Botão Compartilhar com tipo de registro e opções de compartilhamento de exibição](assets/share-button-with-record-type-and-view-sharing-options.png)

1. Selecione um dos seguintes formatos:

   * **Excel**
   * **CSV**

   >[!IMPORTANT]
   >
   >Não é possível exportar informações da exibição de tabela quando você exibe uma exibição diferente na tela. Você deve exibir a exibição de tabela que deseja exportar para acessar a opção Exportar no menu Mais.

   O arquivo é baixado no computador.

1. (Opcional) Vá para a pasta de downloads no seu computador e localize o arquivo baixado.

   O nome do arquivo exportado segue o seguinte formato:

   `Name of the view - name of the record type`

   Por exemplo, uma exibição de tabela para o tipo de registro Campanhas gera um arquivo chamado `Table view - Campaigns`.

   O arquivo exibe as seguintes informações:

   * Os cabeçalhos de coluna são realçados em preto no arquivo do Excel
   * Todos os campos visíveis na interface do Workfront, classificados e filtrados pelos mesmos critérios
   * Os agrupamentos são preservados no arquivo do Excel

   Agora é possível compartilhar os arquivos exportados com outras pessoas ou anexá-los a qualquer comunicação.

</div>
