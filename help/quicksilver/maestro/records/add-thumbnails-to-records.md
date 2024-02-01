---
title: Adicionar miniaturas aos registros
description: Você pode editar informações de registro no Adobe Maestro e associar cada registro com miniaturas individuais, para torná-los facilmente reconhecíveis.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Adicionar miniaturas aos registros

{{maestro-important-intro}}

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
   <td> <p>Contribuir com permissões ou mais altas para um espaço de trabalho </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td>  <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclui a área Maestro no menu principal. </p> <p>Para obter informações, consulte <a href="/help/quicksilver/maestro/access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Considerações sobre miniaturas de registro

Para distinguir visualmente entre registros em uma exibição de tabela, você pode associar uma imagem em miniatura exclusiva a cada registro.

Considere o seguinte:

* Você pode adicionar somente arquivos de imagem como miniaturas.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Você pode adicionar uma imagem em miniatura a registros individuais na exibição de tabela.
* As miniaturas pertencem às informações de registro e são exibidas em exibições nas quais os registros são exibidos. Por exemplo, as miniaturas são exibidas ao lado das informações de registro nas seguintes áreas:

   * O campo principal de um registro na exibição de tabela
   * A barra de registro na exibição de linha do tempo.
* Não é possível adicionar miniaturas de registro na página Detalhes do registro ou na exibição de linha do tempo.
* As miniaturas não são exibidas na página Detalhes do registro.

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
1. (Condicional) Se você tiver pelo menos permissões do Contribute para a exibição de tabela, clique em **Campos** no canto superior direito da exibição em tabela.
1. Selecione o **Miniatura** para exibir a miniatura. Essa opção é desmarcada por padrão.

   ![](assets/thumbnail-toggle-in-fields-menu-deselected.png)

   A miniatura é exibida à esquerda do valor do campo principal.
1. (Opcional e condicional) Se você não tiver permissões do Contribute ou superiores para a exibição, selecione uma nova exibição na **Exibir** ou crie uma visualização.
1. (Opcional) Para remover a miniatura, passe o mouse sobre o campo principal e clique no link **Mais** menu ![](assets/more-menu.png)> **Miniatura** > o **Remover** ícone ![](assets/remove-image-icon.png)e, em seguida, clique em **Salvar alterações**.
