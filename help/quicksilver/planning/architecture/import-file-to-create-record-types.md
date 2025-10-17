---
title: Criar tipos de registro importando informações de um arquivo CSV ou do Excel
description: Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível criar tipos de registro personalizados que ilustrem os itens de trabalho necessários no ciclo de vida da organização importando informações de um arquivo CSV ou do Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2afd6d57-d658-4065-86f5-2324d3818d1f
source-git-commit: df0686038adb1278339e872e122a311884cb6d29
workflow-type: tm+mt
source-wordcount: '796'
ht-degree: 0%

---

# Criar tipos de registro importando informações de um arquivo CSV ou do Excel

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível criar tipos de registro personalizados que ilustrem os itens de trabalho necessários no ciclo de vida da organização importando informações de um arquivo CSV ou do Excel.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront e qualquer pacote do Planning</p>
<p>Ou</p>
<p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões em um espaço de trabalho</p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
 
</tbody> 
</table>-->


## Considerações sobre a importação de tipos de registro usando um arquivo Excel ou CSV

* Cada folha do arquivo do Excel se torna um tipo de registro. O nome da planilha se tornará o nome do tipo de registro.
* Se houver apenas uma planilha ou se você importar um arquivo CSV, o nome do arquivo se tornará o nome do tipo de registro.
* Os cabeçalhos de colunas em cada planilha se tornam os campos associados a cada tipo de registro.
* Os campos são exclusivos para seus respectivos tipos de registro.
* Cada linha em cada planilha se torna um registro exclusivo associado ao respectivo tipo de registro.
* Cada folha do arquivo Excel não deve exceder o seguinte:
   * 25.000 linhas
   * 500 colunas
* O arquivo não deve ter mais de 5 MB.
* Planilhas vazias não são suportadas.
* Os campos dos seguintes tipos não são suportados e não podem ser mapeados para campos na planilha de importação:

   * Campos de conexão para tipos de objeto Workfront e AEM Assets.
   * Campos de pesquisa de registros conectados do Planning ou objetos do Workfront e AEM Assets
   * Campos de fórmula
   * Data de criação, Criado por
   * Última data de modificação, Última modificação por
   * Data de Aprovação, Aprovado por
   * People

Para importar tipos de registro usando um arquivo Excel ou CSV:

{{step1-to-planning}}

1. Clique no espaço de trabalho onde deseja criar tipos de registro,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.
1. Clique em **Adicionar tipo de registro**.
1. Clique em **Carregar do arquivo**.
1. Arraste e solte um arquivo Excel ou CSV salvo anteriormente no computador ou clique em **Selecionar um arquivo CSV ou Excel** para procurar um arquivo e selecione-o.
1. Clique em **Visualizar e editar**.

   A caixa **Visualizar e editar** é exibida com as seguintes informações:

   * Os nomes das planilhas ou dos futuros tipos de registros são exibidos no painel esquerdo. Por padrão, o Workfront Planning seleciona um ícone e uma cor para cada novo tipo de registro.
   * A primeira folha ou tipo de registro é selecionado e os nomes dos campos associados a ela são exibidos como cabeçalhos de coluna. O tipo de cada campo é selecionado por padrão.
   * Cada linha representa um novo registro. Somente os primeiros 10 registros são exibidos na caixa Preview and edit.

   ![Visualizar e editar caixa](assets/preview-and-edit-box.png)

1. (Opcional) Clique no nome de cada planilha no painel esquerdo para revisar as informações que ela contém.

   >[!NOTE]
   >
   >Planilhas vazias não são suportadas e estão esmaecidas.

1. (Opcional) Desmarque as planilhas que você não deseja importar do painel esquerdo.

   ![Selecione as planilhas a serem importadas com o menu suspenso não selecionado](assets/select-sheets-to-import-drop-down-with-unselected.png)

   As planilhas desmarcadas são exibidas com um plano de fundo cinza.

1. (Opcional) Clique na seta para baixo à direita do cabeçalho de uma coluna para executar um dos procedimentos a seguir, na guia **Campo**:

   ![Guia Campo na caixa de importação de mapeamento de tipo de registro](assets/field-tab-on-record-type-import-mapping-box.png)

   * Renomear um dos campos
   * Alterar o **Tipo de campo**
   * Atualizar o campo **Descrição**

1. (Opcional) Clique na guia **Conexão** para mapear as informações da coluna para um campo conectado de outros tipos de registro.

   ![Guia Conexão na caixa de mapeamento de importação do tipo de registro](assets/connection-tab-on-record-type-import-mapping-box.png)

   >[!TIP]
   >
   >Você só pode mapear para campos a partir de registros conectados do Workfront Planning. Não é possível mapear para campos de conexões Workfront ou AEM Assets. Para obter mais informações, consulte a seção [Considerações sobre a importação de tipos de registros usando um arquivo Excel ou CSV](#considerations-about-importing-record-types-using-an-excel-or-csv-file) neste artigo.

1. (Condicional) Depois de atualizar as informações sobre o campo, clique em **Salvar**.

1. Clique em **Importar** quando estiver pronto para importar o arquivo.

   As seguintes informações são importadas para o Workfront Planning:

   * Novos tipos de registro
   * Novos campos associados a cada tipo de registro
   * Novos registros associados a cada tipo de registro

   Você pode começar a gerenciar campos e registros nas páginas de tipos de registro.

   Todos os usuários com acesso ao Workfront Planning e ao espaço de trabalho agora podem exibir e editar os tipos de registros importados e suas informações.
