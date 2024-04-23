---
title: Editar registros
description: É possível editar informações de registro no Adobe Workfront Planning. Você deve criar tipos de registro antes de começar a criar e editar registros.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '1495'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Editar registros

{{maestro-important-intro}}

É possível editar informações de registro no Adobe Workfront Planning editando os valores dos campos associados aos registros.

Você deve criar tipos de registro antes de começar a criar e editar registros.

Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

Para obter informações sobre como criar registros, consulte [Criar registros](/help/quicksilver/maestro/records/create-records.md).

&lt;!— mencione aqui que os campos na exibição Detalhes são os mesmos da exibição de tabela — este artigo é vinculado da opção Gerenciar exibições de registro para fazer referência a essas informações—>

## Requisitos de acesso

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
   <p> Produto</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>contrato do Adobe Workfront</p></td>
   <td>
<p>Sua organização deve estar inscrita no programa beta de Planejamento do Adobe Workfront. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença da Adobe Workfront*</p></td>
   <td>
   <p>Novo: Claro ou superior</p>
   Ou
   <p>Atual: trabalho ou superior</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Adobe Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Contribuir com permissões ou mais altas para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerações sobre a edição de registros

* É possível editar registros criados ou registros criados por outras pessoas, se você tiver recebido permissões para o espaço de trabalho.
* É possível editar campos de registro nas seguintes áreas:

   * A caixa do registro em uma visualização de registro
   * A página do registro
   * Em linha, em uma exibição de tabela.

* Os seguintes tipos de campos são atualizados automaticamente e não é possível editar seus valores manualmente:
   * Campos vinculados de outros registros
   * Campos do tipo fórmula
   * Campos do sistema (Criado por, Data de criação, Última modificação por, Última data de modificação)
* Se os registros exibidos estiverem vinculados a outros registros, as novas informações dos registros que você está editando serão refletidas nos registros vinculados.
* Não é possível editar registros em massa. <!--this will probably change-->
* Os URLs são reconhecidos como links em tipos de campo de texto de linha única somente quando começam com o seguinte: http://, https://, ftp:// ou www. .
* Você pode adicionar uma imagem de capa a cada registro. A imagem é exclusiva para cada registro e não se aplica a todos os registros do mesmo tempo.
* É possível editar a ordem dos campos em uma página de registro e adicionar uma imagem de capa para um registro. Para obter mais informações, consulte [Gerenciar a página de registros](/help/quicksilver/maestro/records/manage-the-record-page.md).

## Editar registros

É possível editar um registro das seguintes áreas:

* [Na exibição de tabela de um tipo de registro](#edit-a-record-from-the-table-view-of-a-record-type)
* [Na caixa do registro em uma exibição](#edit-a-record-from-the-records-box-in-a-view)
* [Da página do registro](#edit-a-record-from-the-records-page)

### Editar um registro incorporado na exibição de tabela de um tipo de registro

{#step1-to-maestro}

O espaço de trabalho que você acessou por último é aberto.

1. (Opcional) Clique na seta para baixo à direita do nome do espaço de trabalho para selecionar o espaço de trabalho cujos registros você deseja atualizar.
1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.
1. (Condicional) Clique na guia de uma exibição de tabela ou clique em **+ Exibir** para criar uma visualização de tabela. A exibição em tabela deve ser a padrão, a menos que você tenha visualizado o tipo de registro em outro tipo de exibição ao acessá-lo pela última vez.

   Os registros associados ao tipo de registro selecionado são exibidos na exibição de tabela.
1. Clique dentro da linha de um registro para começar a editar informações sobre o registro em linha.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)

   >[!TIP]
   >
   >  Não é possível editar as informações dos seguintes campos, pois eles são somente leitura e o Workfront os atualiza automaticamente:
   >  
   >  * Campos vinculados criados pela conexão de tipos de registro. Para obter mais informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).
   >  * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação, Campos de fórmula.

1. (Opcional e condicional) Ao editar um campo do tipo Parágrafo, use o seguinte **Rich Text** opções de formatação:

   * Negrito
   * Itálico
   * Sublinhar
   * Adicionar um link
   * Adicionar uma lista com marcadores
   * Adicionar uma lista numerada

   ![](assets/rich-text-toolbar-on-paragraph-field.png)

1. (Opcional) Clique duas vezes em um campo de registro conectado para adicionar registros ou objetos conectados a outro registro. Para obter mais informações, consulte [Conectar registros](/help/quicksilver/maestro/records/connect-records.md).
1. Pressione **Enter** no teclado ou clique fora de uma linha para salvar as alterações. As alterações são salvas automaticamente. A **Salvo** O indicador é exibido brevemente no canto superior direito da exibição de tabela para mostrar que as alterações foram salvas.


1. (Opcional) Para copiar e colar informações de um campo para outro, siga um destes procedimentos:

   * Copie um ou vários valores existentes de um campo e cole-os em um campo do mesmo tipo em outro registro
   * Clique no cabeçalho de uma coluna para selecioná-la e copiá-la, em seguida, clique no cabeçalho da coluna de outra coluna e cole o conteúdo da coluna copiada. As colunas devem conter tipos de campo semelhantes.
   * Com a tecla Shift pressionada, clique para selecionar várias linhas em uma tabela, copie as informações nas linhas selecionadas e, em seguida, clique em uma linha diferente e cole as informações selecionadas na nova linha e nas linhas seguintes depois disso.
   * Copie as informações de uma célula, selecione várias células e cole as mesmas informações em várias células. Você pode selecionar várias células e colar as mesmas informações em várias células de linhas e colunas adjacentes.

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
   >    * Campos vinculados (ou campos de pesquisa) que são criados pela conexão de tipos de registro. Você pode copiar e colar campos de registro vinculados. Para obter mais informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).
   >    * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a edição ou a cópia e a colagem das informações do registro:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração

   >[!TIP]
   >
   >    Você pode usar os atalhos do teclado várias vezes seguidas para desfazer várias alterações.

1. (Opcional) Adicione uma miniatura a um registro. Para obter informações, consulte [Adicionar uma miniatura a um registro](/help/quicksilver/maestro/records/add-thumbnails-to-records.md).

### Editar um registro da caixa do registro em uma exibição

{{step1-to-maestro}}

O espaço de trabalho que você acessa por último é aberto.

1. (Opcional) Clique na seta para baixo à direita do nome do espaço de trabalho para selecionar o espaço de trabalho cujos registros você deseja atualizar.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no nome de um registro

   Ou

   Na exibição de tabela, clique no botão **Abrir detalhes** ícone ![](assets/open-details-icon-in-table-name-field.png) à esquerda do nome de um registro. A caixa do registro é aberta na exibição.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >É possível exibir a **Abrir detalhes** Ícone à esquerda do campo Nome de um registro em uma exibição de tabela somente quando o campo Nome é um campo primário.

1. Comece a editar as informações do campo na caixa do registro.

   >[!TIP]
   >
   >  Não é possível editar as informações dos seguintes campos, pois eles são somente leitura e o Workfront os atualiza automaticamente:
   >  
   >  * Campos vinculados criados pela conexão de tipos de registro. Para obter mais informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).
   >  * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação, Campos de fórmula.

1. (Opcional) Clique em **Adicionar capa** para adicionar uma imagem da capa ao registro. Para obter mais informações, consulte [Adicionar uma imagem da capa a um registro](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

   O Workfront salva suas alterações automaticamente.

1. (Opcional) Clique no link **Abrir em nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> no canto superior direito da caixa do registro para abrir a página do registro em uma nova guia. Continue editando o registro conforme descrito em [Editar um registro da página do registro](#edit-a-record-from-the-records-page) neste artigo.

### Editar um registro da página do registro

{{step1-to-maestro}}

O espaço de trabalho que você acessa por último é aberto.

1. (Opcional) Clique na seta para baixo à direita do nome do espaço de trabalho para selecionar o espaço de trabalho cujos registros você deseja atualizar.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Siga um destes procedimentos:

   * Em qualquer exibição, acesse a caixa do registro, conforme descrito na seção [Editar um registro da caixa do registro em uma exibição](#edit-a-record-from-the-records-box-in-a-view) neste artigo, em seguida, clique no link **Abrir em nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> no canto superior direito da caixa de registro para abrir a página do registro em uma nova guia.

   * No **Tabela** exibir, passe o mouse sobre o nome de um registro, em seguida, clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Exibir**

     ![](assets/contextual-menu-for-record-row.png)

     A página de registro é aberta.

     ![](assets/details-page.png)

1. Clique em qualquer campo editável na página de registro para editá-lo.

   >[!TIP]
   >
   >  Não é possível editar as informações dos seguintes campos, pois eles são somente leitura e o Workfront os atualiza automaticamente:
   >  
   >  * Campos vinculados criados pela conexão de tipos de registro. Para obter mais informações, consulte [Conectar tipos de registro](../architecture/connect-record-types.md).
   >  * Campos dos seguintes tipos: Criado por, Data de criação, Última modificação por, Data da última modificação, Campos de fórmula.

1. (Opcional) Clique em **Adicionar capa** para adicionar uma imagem da capa ao registro. Para obter mais informações, consulte [Adicionar uma imagem da capa a um registro](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

   O Workfront salva suas alterações automaticamente.

