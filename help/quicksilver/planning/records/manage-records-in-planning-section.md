---
title: Gerenciar Registros na Seção de Planejamento de Objetos do Adobe Workfront
description: Você pode exibir os registros do Workfront Planning conectados a objetos do Adobe Workfront na seção Planning de um objeto do Workfront, no painel esquerdo.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: d86cf3f9-cacc-4457-acb3-a5122ae91be8
source-git-commit: bddd0dcd2263bd65420a17e4b9cc74336877719f
workflow-type: tm+mt
source-wordcount: '1567'
ht-degree: 1%

---


<!--add also Group and Company when they are available-->

# Gerenciar conexões de registro de objetos do Workfront

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>-->

{{planning-important-intro}}

Você pode exibir registros do Workfront Planning no Workfront nas seguintes áreas dos objetos conectados a eles:

* A seção Planejamento de um objeto do Workfront: exibe todos os tipos de registros conectados a um objeto e seus respectivos registros conectados.
* Um campo personalizado de conexão do Planning: exibe um tipo de registro e seus respectivos registros conectados.

<!--replace the last sentence above with this: 

Displays one record type, its respective connected records, <span class="preview">and up to 7 lookup fields of the connected records.</span>

-->

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
<p>Qualquer</p>
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p>
   </td>

<tr>
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td>
   <td>
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p>
<p>Para obter mais informações, consulte <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Experiência unificada da Adobe para Workfront</a>. </p>
   </td>

</tr>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Padrão</p>
   <p>O Workfront Planning não está disponível para licenças herdadas do Workfront</p>
  </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Configuração do nível de acesso</p></td>
   <td> <p>Visualize ou tenha mais acesso a projetos, programas e portfólios</p>  
   <p>Não há configuração de nível de acesso para o Workfront Planning. </p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões de objeto</p></td>
   <td>
   <p>No Workfront, visualize ou aumente as permissões para um projeto, portfólio ou programa</a> </p> 
   <p>No Workfront Planning, visualize permissões em um espaço de trabalho para visualizar registros conectados ou o Contribute ou permissões mais altas em um espaço de trabalho para conectar ou desconectar registros</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho do Workfront Planning, incluindo aqueles que eles não criaram</p> 
  </td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>Para exibir a área Planejamento ou a seção Planejamento de um objeto do Workfront, todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu Principal e a área Planejamento para projetos, portfólios e programas. </p> Para obter mais informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral sobre acesso ao Adobe Planning</a>. </p>  </p>  
</td>
  </tr>
 </tbody>
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Gerenciar registros na seção Planejamento

Você pode usar a seção Planejamento de um objeto do Workfront para exibir todos os tipos de registros e seus respectivos registros conectados ao objeto do Workfront.
A seção Planejamento está disponível para os seguintes objetos do Workfront:

* Projeto
* Portfólio
* Programa
<!--* Group
* Company-->

### Considerações sobre a seção Planejamento de objetos do Workfront

Considere o seguinte ao exibir registros do Workfront Planning na seção Planning de um objeto Workfront:

* Os tipos de registro do Workfront Planning devem primeiro ser conectados aos tipos de objeto do Workfront.

  Para obter informações, consulte os seguintes artigos:

   * [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md)
   * [Conectar registros](/help/quicksilver/planning/records/connect-records.md)
* Você pode exibir a seção Planejamento de um objeto do Workfront, mesmo quando não há registros associados ao objeto do Workfront.

### Gerenciar conexões de registro na seção Planejamento

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique no cartão de um tipo de registro conectado a um projeto, portfólio ou programa do Workfront.
1. Vá para um campo de registro conectado que tenha uma conexão com um objeto do Workfront, na exibição de tabela ou na página de detalhes de um registro. Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Clique no nome de um objeto Workfront no campo de registro conectado.
A página do objeto é aberta no Workfront.

   >[!NOTE]
   >
   >  Se você souber de um objeto do Workfront já conectado a um registro do Planning, poderá navegar até a seção do Planning a partir do objeto do Workfront.

1. Clique em **Planejamento** no painel esquerdo.

   >[!NOTE]
   >
   >   O administrador do Workfront ou do grupo deve adicionar a seção Planejamento ao modelo de layout antes que seja exibida para um projeto, portfólio ou programa do Workfront.

   A seção Planejamento é exibida com as seguintes informações:

   * Os registros conectados são exibidos em cartões individuais que contêm as seguintes informações:
      * Nome do registro
      * A miniatura do registro
      * O nome do campo de registro conectado conforme exibido no Workfront Planning.
   * Os registros são exibidos em seu respectivo espaço de trabalho e tipo de registro.

   ![](assets/planning-section-on-project.png)

1. (Opcional) Clique em **Mostrar todas as conexões** para mostrar todos os tipos de registros conectados, incluindo aqueles sem registros conectados. Por padrão, os tipos de registro sem registros conectados não são exibidos.
1. Clique em um cartão de registro para exibir mais informações sobre o registro. A caixa de visualização do registro é exibida.
1. (Opcional) Inicie a modificação de campos na caixa de visualização do registro. Suas alterações são salvas automaticamente.
1. (Opcional) Clique no ícone ![](assets/open-details-in-a-new-tab-icon.png) de **Abrir em uma nova guia** no canto superior direito da caixa de visualização para abrir a página de detalhes do registro. A página de detalhes do registro é aberta no Workfront Planning.
1. (Opcional) Passe o mouse sobre um cartão de registro, em seguida, clique no ícone de desconectar registro **-** e clique em **Desconectar**.
As seguintes situações ocorrem:
   * O registro não está mais conectado ao objeto Workfront.
   * O objeto Workfront também é removido do campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning também são excluídos.
1. Clique em **Conectar** para conectar mais registros aos tipos de registro conectados.

   Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. (Opcional) Se você não encontrar um registro para conexão e quiser adicioná-lo, clique em **+ Adicionar** para adicionar um novo registro. Para obter mais informações, consulte a seção &quot;Criar registros ao conectá-los a partir de outros registros&quot; no artigo [Criar registros](/help/quicksilver/planning/records/create-records.md).

   As seguintes situações ocorrem:

   * Os registros são conectados imediatamente ao objeto Workfront e são exibidos na seção Planejamento.
   * O objeto Workfront é adicionado ao campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning são preenchidos no Workfront Planning.

## Gerenciar registros no tipo de campo de conexão do Planning

Você pode usar um campo personalizado de conexão do Planning em um objeto do Workfront para exibir um tipo de registro e seus respectivos registros conectados ao objeto do Workfront.

Você pode controlar quais tipos de registro do Planning são exibidos para o objeto do Workfront quando você cria campos personalizados de conexão do Planning.

* O campo de conexão do Planning exibe registros do Planning depois que uma conexão é estabelecida e quando o campo é anexado a formulários para os seguintes objetos do Workfront:

   * Projeto
   * Portfólio
   * Programa
   * Grupo
   * Empresa

Para obter mais informações, consulte [Criar um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Considerações sobre o tipo de campo de conexão do Planning

Considere o seguinte ao exibir registros do Workfront Planning de um campo de conexão do Planning de um objeto do Workfront:

<!--
* A Planning connection field displays in the following ways on a Workfront object's custom form, after Planning records are connected to the Workfront object:

   * If only the primary field of the connected record is selected, as a field with multiple values, if the connection allows for multiple records to be linked. For information, see [Connect record types overview](/help/quicksilver/planning/architecture/connect-record-types-overview.md).
   * <span class="preview">If any additional lookup fields from the connected record are selected, the Planning connection field displays as a table. Up to 7 fields can be selected for the Planning connection field. The table view is read-only.  </span>
-->
* Você pode associar apenas um tipo de registro a um campo de conexão do Planning. Não há limite para quantos campos de conexão do Planning você tem em um formulário.
* Você deve ter o acesso e as permissões corretas para o objeto, o registro e o Workfront Planning para anexar um formulário personalizado com um campo personalizado de conexão do Planning a um objeto do Workfront.
* Você deve ter permissões do Contribute para um espaço de trabalho no Workfront Planning para poder conectar ou desconectar registros do campo de conexão do Planning de um objeto do Workfront.
* Os tipos de registro do Workfront Planning devem primeiro ser conectados aos tipos de objeto do Workfront. Para obter informações, consulte [Tipos de registro do Connect](/help/quicksilver/planning/architecture/connect-record-types.md). Isso torna os registros do Workfront Planning acessíveis no Workfront.
* Você pode conectar ou desconectar registros do campo de conexão do Planning de um objeto do Workfront somente para objetos que podem ter conexões do Workfront Planning.

  Por exemplo, talvez seja possível anexar um formulário personalizado com um campo de conexão do Planning a tarefas, mas não é possível conectar objetos do Workfront Planning a tarefas.
* Não é possível editar um campo de conexão do Planning ao editar objetos do Workfront em massa.

### Gerenciar conexões de registro do tipo de campo de conexão do Planning

1. Vá para um dos seguintes tipos de objeto que foi conectado a um tipo de registro do Workfront Planning:

   * Projeto
   * Portfólio
   * Programa
   * Empresa
   * Grupo

1. Clique em **&lt; Objeto > Detalhes** no painel esquerdo.
1. (Condicional) Adicione um formulário personalizado com pelo menos um campo de conexão do Planning para o objeto selecionado, se não houver um presente.

   >[!NOTE]
   >
   >O administrador do Workfront ou do grupo deve primeiro criar o formulário e adicionar um campo de conexão do Planning a ele antes que você possa adicioná-lo a um objeto.


1. Clique dentro do campo para adicionar registros conectados e, em seguida, clique na seta para baixo dentro do campo para selecionar registros da lista.

   ![](assets/planning-connection-field-on-project-with-record-list-open.png)

   >[!TIP]
   >
   >Não é possível adicionar registros aos campos de conexão do Planning associados a objetos Workfront diferentes do objeto selecionado quando o campo foi configurado.
   >
   >Por exemplo, não é possível adicionar registros a um campo de conexão do Planning criado para uma conexão do Portfolio a partir de um formulário personalizado do Project.
   >
   >Há uma indicação de que o objeto do campo e o objeto selecionado não correspondem.
   >
   >![](assets/warning-unsupported-object-planning-connection-field-on-form.png)

1. Clique fora da lista para fechá-la.

   As seguintes situações ocorrem:

   * Os registros são conectados imediatamente ao objeto Workfront e são exibidos no campo de conexão Planning, bem como na seção Planning do objeto Workfront.
   * O objeto Workfront é adicionado ao campo conectado do registro do Workfront Planning.
   * Os valores dos campos de pesquisa do Workfront conectados ao registro do Planning são preenchidos no Workfront Planning.
   <!--* <span class="preview">If any record lookup fields were added when the custom form was set up, the record's lookup fields populate automatically in a table view. The table view in the Planning connection field is read-only</span>
   
      ![](assets/planning-connection-field-with-table-on-project-details-custom-form.png)-->

1. (Opcional) Clique no nome de um registro <!--<span class="preview">or hover the name of the record in the table, then click the **Open record** icon ![Open record icon on Planning connection custom form](assets/open-record-icon-on-planning-connection-custom-form.png)</span>--> no campo de conexão do Planning para abri-lo no Workfront Planning.
A caixa de visualização de detalhes do registro do Workfront Planning é aberta.
Você pode revisar ou editar informações sobre o registro ou clicar no ícone **Abrir em uma nova guia** ![Abrir registro em nova guia](assets/open-details-in-a-new-tab-icon.png) para abrir a página de detalhes do registro.

1. (Opcional) No formulário personalizado no Workfront, clique no ícone ![](assets/remove-icon.png) de **Remover** em um registro para removê-lo do campo de conexão do Planning e desconectá-lo do objeto do Workfront.
O objeto do Workfront é desconectado do registro do Planning e qualquer informação de pesquisa do Workfront é removida do registro.

1. Clique em **Salvar alterações** para salvar o formulário personalizado e quaisquer outras alterações feitas no objeto do Workfront.