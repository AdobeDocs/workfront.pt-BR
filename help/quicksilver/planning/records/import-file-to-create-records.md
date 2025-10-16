---
title: Criar registros importando informações de um arquivo CSV ou do Excel
description: Os registros são instâncias individuais de tipos de registro, que são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível criar registros importando informações de um arquivo CSV ou do Excel.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 940945df-391c-4672-9d9d-180d5028509b
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---


# Criar registros importando informações de um arquivo CSV ou do Excel

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Os registros são instâncias individuais de tipos de registro, que são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível criar registros importando informações de um arquivo CSV ou do Excel.

Para obter mais informações sobre como criar registros, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).

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
<p>Qualquer Workfront e qualquer pacote do Planning</p> <p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td> <p>Contribute ou tenha permissões mais altas para o espaço de trabalho e tipo de registro em que você importa registros. </p>
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
   </td> 
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
   <td> Standard
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p> 
   <p>Edit access in Workfront for the object types that you want to create (projects, programs, and portfolios) as you connect them from new records  </p>  
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td> <p>Contribute or higher permissions to the workspace and record type where you want to add records. </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Manage permissions to Workfront objects (portfolios) to add children objects (projects).</p>
   </td> 
  </tr> 
</tbody> 
</table> -->


## Considerações sobre a importação de registros usando um arquivo Excel ou CSV

* Os cabeçalhos de colunas em cada planilha se tornam os campos associados aos registros.
* Cada linha em cada planilha se torna um registro exclusivo associado.
* Se o arquivo do Excel contiver mais de uma planilha, somente as informações de uma planilha selecionadas durante o processo de importação serão importadas.
* O arquivo não deve exceder o seguinte:
   * 25.000 linhas
   * 500 colunas
* O arquivo não deve ter mais de 5 MB.
* Planilhas vazias não são suportadas.
* Os campos dos seguintes tipos não são suportados e não podem ser mapeados para campos na planilha de importação:

   * Campos de conexão para tipos de objeto Workfront e AEM Assets. Você pode mapear apenas campos de conexão para tipos de registro do Planning.
   * Campos de pesquisa de registros conectados do Planning ou objetos do Workfront e AEM Assets
   * Campos de fórmula
   * Data de criação, Criado por
   * Última data de modificação, Última modificação por
   * Data de Aprovação, Aprovado por
   * People
   * Se um campo de seleção única ou múltipla for importado e tiver mais opções do que um campo semelhante no Planning, as opções adicionais serão criadas durante a importação. Somente usuários com permissões para Gerenciar o espaço de trabalho podem importar novas opções.

## Criar registros importando um arquivo CSV ou do Excel

{{step1-to-planning}}

1. Clique no espaço de trabalho onde deseja criar registros,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.
1. Clique no cartão do tipo de registro para o qual deseja importar os registros.
1. Clique em **Novo registro** no canto superior direito da tela.

   ![Escolha a maneira de adicionar registros à caixa de três botões](assets/choose-way-to-add-records-three-button-box.png)
1. Clique em **Carregar do arquivo** e depois em **Continuar**. <!--add screen shot when all three buttons are added - with the Submit a request button-->
1. Arraste e solte um arquivo Excel ou CSV salvo anteriormente no computador ou clique em **Selecionar um arquivo CSV ou Excel** para procurar um.
1. Clique em **Visualizar e editar**.
1. (Condicional) Se o arquivo importado tiver mais de uma planilha, selecione o botão de opção da planilha que deseja importar na caixa **Selecione uma planilha a ser importada** e clique em **Avançar**. Caso contrário, continue para a próxima etapa.

   ![Selecione uma planilha para importar registros](assets/select-a-sheet-to-import-box.png)
1. Em **Mapear os campos do Planning para os cabeçalhos de coluna**, selecione o **campo do Planning** que melhor corresponda às informações em cada uma das colunas da planilha.

   ![Mapear campos do Planning para colunas ao importar registros](assets/map-planning-fields-to-columns-when-importing-records.png)

   Cada linha representa um novo registro. Somente os primeiros 10 registros são exibidos na caixa Preview and edit.

   >[!TIP]
   >
   >Nem todos os tipos de campo são suportados. Para obter mais informações, consulte a seção [Considerações sobre a importação de registros usando um arquivo Excel ou CSV](#considerations-about-importing-records-using-an-excel-or-csv-file) neste artigo.


1. (Opcional e condicional) Se você tiver permissões de Gerenciamento para o espaço de trabalho, selecione a opção **Criar opções ausentes** no canto inferior esquerdo da tela. Quando ativado, as opções ausentes de campos de seleção única e múltipla são adicionadas.

   >[!NOTE]
   >
   >Por exemplo, se o tipo de registro selecionado tiver um campo Status de seleção única com as opções Novo, Em Andamento e Fechado e um campo Status importado de um arquivo também tiver uma opção Status de Suspensão, a opção Status de Suspensão também será adicionada.
   >
   >Se você não tiver permissões Gerenciar para o espaço de trabalho, poderá importar registros, mas as opções adicionais não serão criadas. Em vez disso, você receberá a seguinte mensagem no canto superior direito da caixa Mapear os campos do Planning para seus cabeçalhos de coluna: **As opções que não existem nos campos de conexão, de seleção única ou de seleção múltipla não serão adicionadas**.

1. Clique em **Importar**.

   As seguintes informações são importadas para o Workfront Planning:

   * Novos registros exibidos na parte inferior da exibição de tabela do tipo de registro selecionado.
   * Novos valores de campo para campos existentes associados a cada registro.
   * Novas opções de um campo de seleção única ou múltipla que não existia no Planning.  <!--when we add connected records - add those here too-->

   Você pode começar a gerenciar campos e registros na página de tipos de registro.

   Todos os usuários com acesso ao Workfront Planning e ao espaço de trabalho agora podem exibir e editar os registros importados e suas informações.

   <!--when we add connected records and the info icon in the tool changes, also add those items to the Import step and to the NOTE above it-->
