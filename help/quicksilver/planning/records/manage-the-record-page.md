---
title: Gerenciar o layout da página de registros
description: É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 869a1f9e4fd7e3b65591050530b96d6dae9e230c
workflow-type: tm+mt
source-wordcount: '1066'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Gerenciar o layout da página de registros

{{planning-important-intro}}

É possível editar o layout da visualização de registro e da página no Adobe Workfront Planning.

A visualização do registro é uma exibição menor da página do registro exibida na exibição de um tipo de registro.

Quando você altera o layout de uma visualização e página de registro, as alterações afetam as caixas de visualização e as páginas de detalhes de todos os registros do mesmo tipo.

Este artigo descreve como alterar o layout e a aparência de uma caixa de visualização de registro ou de uma página de registro. Para obter informações sobre edição de registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Você deve criar tipos de registro e registros antes de começar a editar páginas de registro.

Para obter informações, consulte os seguintes artigos:

* [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md)

* [Criar registros](/help/quicksilver/planning/records/create-records.md)

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
<p>Sua organização deve estar inscrita no estágio de acesso antecipado do Workfront Planning </p>
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
   <td> <p>Gerenciar ou aumentar as permissões de um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área do Planning ao modelo de layout. Para obter informações, consulte <a href="/help/quicksilver/planning/access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Considerações sobre a edição de páginas de registro

* Por padrão, os detalhes e as páginas de visualização de um registro exibem todos os campos associados ao registro.

* Não é possível adicionar novos campos a um registro na página de visualização ou de detalhes. Você deve adicionar novos campos na exibição de tabela para exibi-los nas páginas de visualização e detalhes.

* É possível adicionar seções a uma visualização de registro ou página de detalhes para organizar as informações por critérios comuns e facilitar a localização.

* As alterações a seguir afetam todos os registros do mesmo tipo e são visíveis para todos os usuários que acessam esses registros:

   * Reorganização de campos
   * Adição ou remoção de seções

* As alterações de exibição feitas na visualização do registro ficam imediatamente visíveis na página de detalhes do registro. As alterações feitas na página de registro também estão visíveis na caixa de visualização do registro.

* Adicionar uma imagem de capa ou uma miniatura a um registro não faz parte do layout geral da pré-visualização ou página do registro. É possível adicionar imagens de capa ou miniaturas exclusivas a cada registro. Para obter informações, consulte [Adicionar uma imagem da capa a um registro](/help/quicksilver/planning/records/add-a-cover-image-to-a-record.md) e [Adicionar uma miniatura a um registro](/help/quicksilver/planning/records/add-thumbnails-to-records.md).

## Adicionar seções a uma visualização ou página de registro

Considere o seguinte ao adicionar seções a uma página de registro:

* Não há limite para quantas seções você pode ter em uma página.
* Você não pode ter uma seção vazia. Você deve ter pelo menos um campo em uma seção.
* Você pode arrastar e soltar campos de uma seção para outra. Para obter mais informações, consulte a seção [Reorganizar campos na página de visualização ou detalhes do registro](#rearrange-fields-in-the-record-preview-or-details-page) neste artigo.
* Ao remover todos os campos de uma seção, ela é automaticamente excluída e não pode ser recuperada.

Para adicionar uma seção a uma visualização de registro ou página:

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no nome de um registro

   Ou

   Na exibição de tabela, clique na guia **Abrir detalhes** ícone ![](assets/open-details-icon-in-table-name-field.png) na primeira coluna.

   A visualização do registro é aberta na exibição.

   ![](assets/details-box.png)

1. (Opcional) Clique no link **Abrir em nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.

   A página de registro é aberta.

   ![](assets/details-page.png)

1. Na visualização do registro ou página, passe o mouse sobre o espaço em branco à esquerda dos campos e clique no botão **Adicionar seção** ícone ![](assets/add-section-icon.png) para adicionar uma seção.
1. Clique dentro do nome da seção e substitua **Seção sem título** com um nome, em seguida, clique em Enter. Os campos exibidos abaixo da seção fazem parte automaticamente da nova seção.
1. Comece a arrastar e soltar campos na nova seção, conforme descrito na seção [Reorganizar campos na página de visualização ou detalhes do registro](#rearrange-fields-in-the-record-preview-or-details-page) neste artigo.

1. (Opcional) Passe o mouse sobre o nome de uma seção e clique no link **Mais** menu ![](assets/more-menu.png).

   ![](assets/more-menu-options-for-section-on-record-page.png)
1. (Opcional) Siga um destes procedimentos para editar a seção:

   * Clique em **Renomear** para renomear a seção

     >[!TIP]
     >
     > É possível renomear uma seção em linha clicando no nome.

   * Clique em **Mover para cima** para mover a seção uma posição acima

     Ou

     Clique em **Mover para baixo** para mover a seção uma posição para baixo.
Todos os campos na seção se movem com a seção.

   * Clique em **Excluir** para excluir a seção. A seção é excluída e não pode ser recuperada. Todos os usuários que acessarem os registros desse tipo não visualizarão mais a seção excluída.

1. Clique na seta apontando para baixo à esquerda do nome de uma seção para recolhê-la ou na seta apontando para a direita para expandi-la.
Todas as seções são expandidas por padrão.

1. (Opcional) Clique no link **agarrar** ícone ![](assets/grab-icon.png) à esquerda do nome de uma seção, arraste-a e solte-a no local desejado.

   A nova posição da seção atualiza na pré-visualização e na página de todos os registros do mesmo tipo para todos os usuários que visualizam os registros.

   Todas as alterações nas seções e na ordem dos campos são salvas automaticamente.

## Reorganizar campos na página de visualização ou detalhes do registro

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no nome de um registro

   Ou

   Na exibição de tabela, clique na guia **Abrir detalhes** ícone ![](assets/open-details-icon-in-table-name-field.png) na primeira coluna.

   A visualização do registro é aberta na exibição.

   ![](assets/details-box.png)

1. (Opcional) Clique no link **Abrir em nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.

   A página de registro é aberta.

   ![](assets/details-page.png)

1. Na visualização ou página do registro, clique na guia **agarrar** ícone ![](assets/grab-icon.png) à esquerda de um nome de campo, arraste e solte-o no ponto desejado. <!--You can drag and drop fields to another section. You must have at least one field in a section.-->

   A nova posição do campo é atualizada na pré-visualização e na página de todos os registros do mesmo tipo para todos os usuários que visualizam os registros.

   Todas as alterações no layout da visualização do registro ou na página são salvas automaticamente.

