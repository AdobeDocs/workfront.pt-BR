---
title: Adicionar miniaturas aos registros
description: Você pode editar informações de registro no Adobe Maestro e associar cada registro com miniaturas individuais, para torná-los facilmente reconhecíveis.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 7448f6b8a622bc814604e59d4654644b3d7a1e12
workflow-type: tm+mt
source-wordcount: '559'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Adicionar miniaturas aos registros

>[!IMPORTANT]
>
>As informações neste artigo referem-se ao Adobe Maestro, que é uma nova oferta da Adobe Workfront.
>
>Atualmente, o Adobe Maestro faz parte de um programa beta aberto a um número limitado de clientes. Você deve ser um cliente do Workfront para usar os recursos do Maestro.
>
>Entre em contato com seu representante de conta para obter mais informações sobre como participar do programa beta para o Maestro.
>
>Para obter informações, consulte [Visão geral do Adobe Maestri](../maestro-overview.md).

Você pode associar registros com miniaturas únicas no Adobe Maestro, para torná-los facilmente reconhecíveis.

Você deve criar tipos de registro antes de começar a criar e editar registros.
Para obter informações, consulte [Criar tipos de registro](../architecture/create-record-types.md).

## Requisitos de acesso

<!--************double-check permissions here - asking Isk and Lilit what permissions users need for adding thumbnails-->

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
<p>Sua organização deve estar inscrita no programa beta fechado do Adobe Maestro. Entre em contato com seu representante de conta para obter mais informações sobre esta nova oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plano do Adobe Workfront</p></td>
   <td>
<p>Qualquer</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Maestro </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissões</p></td>
   <td> <p>Exibir ou aumentar as permissões de um espaço de trabalho </p>  
   <p>Exibir permissões ou mais altas para a exibição de tabela </p> 
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> <p>O administrador do Workfront ou do grupo deve adicionar a área Maestri no modelo de layout. Para obter informações, consulte <a href="../access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>


## Considerações sobre miniaturas de registro

Para distinguir visualmente entre registros em uma exibição de tabela, você pode associar uma imagem em miniatura exclusiva a cada registro.

Considere o seguinte:

* Você pode adicionar somente arquivos de imagem como miniaturas.
* Você pode adicionar uma imagem em miniatura a registros individuais na exibição de tabela.
* Não é possível adicionar miniaturas de registro na página Detalhes do registro ou na exibição de linha do tempo.
* A imagem em miniatura é sempre exibida à esquerda do campo principal de cada registro, independentemente do tipo do campo.

  Os campos que são texto de linha única, números ou fórmulas podem ser designados como campos primários.
Para obter mais informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/maestro/views/manage-the-table-view.md).

<!--above: when you know exactly what type of files are allowed, add the exact extensions above-->

## Adicionar uma miniatura a um registro

{{step1-to-maestro}}

1. Selecione o espaço de trabalho cujos registros deseja adicionar miniaturas e clique no cartão de tipo de registro.

   Isso abre a página do tipo de registro.
1. Selecione uma exibição de tabela na **Exibir** menu suspenso. Todos os registros do tipo selecionado são exibidos em uma tabela.
1. Passe o mouse sobre as informações do campo principal, clique no **Mais** menu ![](assets/more-menu.png)e, em seguida, clique em **Miniatura**.

   ![](assets/record-more-menu-expanded.png)

   >[!TIP]
   >
   >   O campo principal é aquele exibido na primeira coluna de uma exibição de tabela. O campo principal é sempre congelado e não pode ser oculto ou realocado.

   A variável **Miniatura de registro** é aberta.

   ![](assets/record-thumbnail-box-for-upload.png)

   <!--update screen shot with correct casing-->

1. No **Carregar** arraste e solte um arquivo para adicionar como miniatura ou clique em **Selecione para fazer upload** e procure um arquivo de imagem para adicionar. O arquivo deve ser salvo no computador.
1. (Opcional) Use a ferramenta de dimensionamento para cortar e redimensionar a imagem.
1. Clique em **Usar imagem** para adicionar a imagem como miniatura.
Isso fecha o **Miniatura de registro** caixa.
1. Clique em Campos no canto superior direito da exibição em tabela.
1. Selecione o **Miniatura** para exibir a miniatura. Essa opção é desmarcada por padrão.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   A miniatura é exibida à esquerda do valor do campo principal.
1. (Opcional) Para remover a miniatura, passe o mouse sobre o campo principal e clique no link **Mais** menu ![](assets/more-menu.png)> **Miniatura** > o **Remover** ícone ![](assets/remove-image-icon.png)e, em seguida, clique em **Salvar alterações**.