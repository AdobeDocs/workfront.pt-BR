---
title: Editar registros
description: É possível editar informações de registro no Adobe Workfront Planning. Você deve criar tipos de registro antes de começar a criar e editar registros.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 82633fcb858273dee360fc44b031fec5a5cdff54
workflow-type: tm+mt
source-wordcount: '1948'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# Editar registros

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

É possível editar informações de registro no Adobe Workfront Planning editando os valores dos campos associados aos registros.

Você deve criar tipos de registro antes de começar a criar e editar registros.

Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

Para obter informações sobre como criar registros, consulte [Criar registros](/help/quicksilver/planning/records/create-records.md).

&lt;!— mencione aqui que os campos na exibição Detalhes são os mesmos da exibição de tabela — este artigo é vinculado da opção Gerenciar exibições de registro para fazer referência a essas informações—>

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
   <td role="rowheader"><p>Plano de planejamento do Adobe Workfront*</p></td> 
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
   <td> <p>Padrão</p> 
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
   <td>  <p>Contribute ou permissões superiores para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   Or
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configurations</p></td>
   <td> <p>There are no access controls for Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Contribute or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## Considerações sobre a edição de registros

* É possível editar registros criados ou registros criados por outras pessoas, se você tiver recebido permissões para o espaço de trabalho.
* É possível editar campos de registro nas seguintes áreas:

   * A visualização do registro em uma exibição de registro
   * A página do registro
   * Em linha, em uma exibição de tabela.

* Quando um usuário edita um registro em uma exibição, as alterações são visíveis imediatamente em todas as exibições e nas páginas de registro para todos os outros usuários.

* Os seguintes tipos de campos são atualizados automaticamente e não é possível editar seus valores manualmente:
   * Campos vinculados de outros registros
   * Campos do tipo fórmula
   * Campos do sistema (Criado por, Data de criação, Última modificação por, Última data de modificação)
* Se os registros exibidos estiverem vinculados a outros registros, as novas informações dos registros que você está editando serão refletidas nos registros vinculados.
* Não é possível editar registros em massa. <!--this will probably change-->
* Os URLs são reconhecidos como links em tipos de campo de texto de linha única somente quando começam com o seguinte: http://, https://, ftp:// ou www. .
* Você pode adicionar uma imagem de capa a cada registro. A imagem é exclusiva para cada registro e não se aplica a todos os registros do mesmo tempo.
* É possível editar a ordem dos campos em uma página de registro e adicionar uma imagem de capa para um registro. Para obter mais informações, consulte [Gerenciar o layout da página de registro](/help/quicksilver/planning/records/manage-the-record-page.md).

## Editar registros

É possível editar um registro das seguintes áreas:

* [Na exibição de tabela de um tipo de registro](#edit-a-record-inline-in-the-table-view-of-a-record-type)
* [Da visualização do registro em uma exibição](#edit-a-record-from-the-records-preview-in-a-view)
* [Da página do registro](#edit-a-record-from-the-records-page)
* [De um objeto do Workfront na seção Planejamento](#edit-a-record-from-a-workfront-object-in-the-planning-section)

### Editar um registro incorporado na exibição de tabela de um tipo de registro

Ao editar registros na exibição de tabela, há uma indicação de qual campo está sendo editado por outros usuários no momento em que você está visualizando o registro.

Para obter mais informações, consulte [Gerenciar exibições de registros](/help/quicksilver/planning/views/manage-record-views.md).

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros você deseja editar

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.
1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.
1. (Condicional) Clique na guia de um modo de exibição de tabela ou clique em **+ Modo de Exibição** para criar um modo de exibição de tabela. A exibição em tabela deve ser a padrão, a menos que você tenha visualizado o tipo de registro em outro tipo de exibição ao acessá-lo pela última vez.

   Os registros associados ao tipo de registro selecionado são exibidos na exibição de tabela.
1. Clique dentro da linha de um registro para começar a editar informações sobre o registro em linha.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Não é possível editar as informações dos seguintes campos, pois eles são somente leitura e o Workfront os atualiza automaticamente:
   >  
   >  * Campos vinculados criados pela conexão de tipos de registro. Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação, Campos de fórmula.

1. (Opcional e condicional) Ao editar um campo do tipo Parágrafo, use as seguintes opções de formatação de **Rich Text**:

   * Negrito
   * Itálico
   * Sublinhar
   * Adicionar um link
   * Adicionar uma lista com marcadores
   * Adicionar uma lista numerada

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Opcional) Clique duas vezes em um campo de registro conectado para adicionar registros ou objetos conectados a outro registro. Para obter mais informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
1. Pressione **Enter** no teclado ou clique fora de uma linha para salvar as alterações. As alterações são salvas automaticamente. Um indicador **Salvo** é exibido brevemente no canto superior direito da exibição de tabela para mostrar que as alterações foram salvas.


1. (Opcional) Para copiar e colar informações de um campo para outro, siga um destes procedimentos:

   * Copie um ou vários valores existentes de um campo e cole-os em um campo do mesmo tipo em outro registro
   * Clique no cabeçalho de uma coluna para selecioná-la e copiá-la, em seguida, clique no cabeçalho da coluna de outra coluna e cole o conteúdo da coluna copiada. As colunas devem conter tipos de campo semelhantes.
   * Com a tecla Shift pressionada, clique para selecionar várias linhas em uma tabela, copie as informações nas linhas selecionadas e, em seguida, clique em uma linha diferente e cole as informações selecionadas na nova linha e nas linhas seguintes depois disso.
   * Copie as informações de uma célula, selecione várias células e cole as mesmas informações em várias células. Você pode selecionar várias células e colar as mesmas informações em várias células de linhas e colunas adjacentes.
   * Selecione o canto inferior direito de uma célula existente que contenha as informações que você deseja copiar e, em seguida, arraste e solte-a nas células adjacentes onde deseja colar as mesmas informações. Todas as células devem conter o mesmo tipo de informação.

     ![](assets/dragable-lower-right-corner-for-copy-paste-in-table-view.png)

   >[!NOTE]
   >
   >Considere o seguinte:
   >
   >* Use os seguintes atalhos de teclado para copiar e colar informações:
   >   * Copiar: CTRL + C (⌘ + C para Mac)
   >   * Colar: CTRL + V (⌘ + V para Mac)
   >
   >* Não é possível copiar e colar valores de campo na página de registro. Essa funcionalidade é compatível somente na exibição de tabela de um tipo de registro.
   >* Não é possível copiar e colar valores de campo para os seguintes tipos de campo:
   >
   >
   >    * Campos vinculados (ou campos de pesquisa) que são criados pela conexão de tipos de registro. Você pode copiar e colar campos de registro vinculados. Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
   >    * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a edição ou a cópia e a colagem das informações do registro:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração

   >[!TIP]
   >
   >    Você pode usar os atalhos do teclado várias vezes seguidas para desfazer várias alterações.

1. (Opcional) Adicione uma miniatura a um registro. Para obter informações, consulte [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

### Editar um registro da visualização do registro em uma exibição

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros você deseja editar

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no registro

   Ou

   Na exibição de tabela, clique no ícone ![](assets/open-details-icon-in-table-name-field.png) de **Abrir detalhes** na primeira coluna. A visualização do registro é aberta na exibição.

   ![](assets/details-box.png)

1. (Opcional) Clique no menu **Mais** à direita do título do registro e clique em **Renomear**. Isso atualiza o campo que é exibido como o título do registro.

   O título do registro é o campo principal do registro quando exibido em uma exibição de tabela. Para obter informações, consulte [Visão geral do campo principal](/help/quicksilver/planning/fields/primary-field-overview.md).

1. Comece a editar as informações do campo na visualização do registro.

   >[!TIP]
   >
   >  Não é possível editar as informações dos seguintes campos, pois eles são somente leitura e o Workfront os atualiza automaticamente:
   >  
   >  * Campos de pesquisa de outros registros criados pela conexão de tipos de registro. Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação, Campos de fórmula.

1. (Opcional) Clique em **Adicionar capa** para adicionar uma imagem de capa ao registro. Para obter mais informações, consulte [Adicionar uma imagem de capa a um registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Opcional) Passe o mouse sobre o ícone de miniatura, em seguida, clique em **Mais** ![](assets/more-menu.png) > **Editar miniatura** para adicionar uma imagem em miniatura. Para obter informações, consulte [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   O Workfront salva suas alterações automaticamente.

1. (Opcional) Clique no menu ![](assets/export-icon-in-record-details-page.png) **Exportar** para exportar os detalhes do registro. Para obter informações, consulte [Exportar os detalhes de um registro](/help/quicksilver/planning/records/export-the-record-page.md).

1. (Opcional) Clique no ícone ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> de **Abrir em nova guia** no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia. Continue editando o registro conforme descrito na seção [Editar um registro da página do registro](#edit-a-record-from-the-records-page) deste artigo.

### Editar um registro da página do registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros você deseja editar

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Siga um destes procedimentos:

   * Em qualquer exibição, acesse a visualização do registro, conforme descrito na seção [Editar um registro da visualização do registro em uma exibição](#edit-a-record-from-the-records-preview-in-a-view) deste artigo, em seguida, clique no ícone ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> de **Abrir em nova guia** no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.

   * Na exibição **Tabela**, passe o mouse sobre o nome de um registro, em seguida, clique no menu **Mais** ![](assets/more-menu.png) e, em seguida, clique em **Exibir**

     ![](assets/contextual-menu-for-record-row.png)

     A página de registro é aberta.

     ![](assets/details-page.png)

1. (Opcional) Clique no menu **Mais** à direita do título do registro e clique em **Renomear**. Isso atualiza o campo que é exibido como o título do registro.

   O título do registro é o campo principal do registro quando exibido em uma exibição de tabela. Para obter informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

1. Clique em qualquer campo editável na página de registro para editá-lo.

   >[!TIP]
   >
   >  Não é possível editar as informações dos seguintes campos, pois eles são somente leitura e o Workfront os atualiza automaticamente:
   >  
   >  * Campos vinculados criados pela conexão de tipos de registro. Para obter mais informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
   >  * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação, Campos de fórmula.

1. <span class="preview">(Opcional) Clique no ícone de informações à direita de qualquer campo que o exiba para exibir a descrição de um campo. </span>
1. (Opcional) Clique em **Adicionar capa** para adicionar uma imagem de capa ao registro

   Ou

   Passe o mouse sobre a imagem de capa existente, em seguida, clique no menu **Mais** ![](assets/more-menu.png) > **Carregar** para adicionar uma nova imagem de capa para o registro.

   Para obter mais informações, consulte [Adicionar uma imagem de capa a um registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md).

1. (Opcional) Passe o mouse sobre uma miniatura existente ou sobre o **ícone de miniatura** ![](assets/record-thumbnail-icon-on-details-page.png) e clique no menu **Mais** ![](assets/more-menu.png) > **Editar miniatura** para adicionar uma miniatura para o registro.

   Para obter mais informações, consulte [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

   O Workfront salva suas alterações automaticamente.

1. (Opcional) Clique no menu ![](assets/export-icon-in-record-details-page.png) **Exportar** para exportar os detalhes do registro. Para obter informações, consulte [Exportar os detalhes de um registro](/help/quicksilver/planning/records/export-the-record-page.md).


## Editar um registro de um objeto do Workfront na seção Planejamento

Depois de conectar registros a objetos do Workfront, você pode editar os registros do Workfront Planning no Workfront na seção Planejamento do objeto.

Para obter mais informações, consulte [Gerenciar registros na seção Planning de objetos do Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).