---
title: Adicionar uma imagem da capa a um registro
description: É possível editar informações de registro no Adobe Workfront Planning e associar cada registro a uma imagem de capa para personalizar a página do registro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '556'
ht-degree: 0%

---

<!--update the metadata with real information-->

# Adicionar uma imagem da capa a um registro

{{maestro-important-intro}}

É possível editar informações de registro no Adobe Workfront Planning e associar cada registro a uma imagem de capa para personalizar a página do registro.

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
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td>
   <td>
   <p>Qualquer</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configurações de nível de acesso</p></td>
   <td> <p>Não há controles de acesso para o Workfront Planning </p>  
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
   <td>  <p>Todos os usuários, incluindo administradores do Workfront, devem receber um modelo de layout que inclua a área Planejamento no Menu principal. </p> <p>Para obter informações, consulte <a href="/help/quicksilver/maestro/access/access-overview.md">Visão geral do Access</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Considerações sobre imagens de capa de página de registro

É possível personalizar a página de um registro adicionando uma imagem de capa a ela. A imagem é exclusiva de cada registro e não se aplica a todos os registros do mesmo tipo.

Considere o seguinte:

* Você pode adicionar somente arquivos de imagem como imagens de capa.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* Você pode adicionar uma imagem de capa a registros individuais da caixa de registro em qualquer exibição ou da página de registro.
* Não é possível adicionar imagens de capa integradas na exibição de tabela.

## Adicionar uma imagem da capa a um registro

É possível personalizar um registro adicionando uma imagem de capa na parte superior da caixa ou página do registro.

{{step1-to-maestro}}

O espaço de trabalho que você acessa por último é aberto.

1. (Opcional) Clique na seta para baixo à direita do nome do espaço de trabalho para selecionar o espaço de trabalho cujos registros você deseja atualizar.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique no nome de um registro

   Ou

   Na exibição de tabela, clique na guia **Abrir detalhes** ícone ![](assets/open-details-icon-in-table-name-field.png) à esquerda do nome de um registro.

   A caixa do registro é aberta na exibição.

   ![](assets/details-box.png)

   >[!TIP]
   >
   >É possível exibir a **Abrir detalhes** Ícone à esquerda do campo Nome de um registro em uma exibição de tabela somente quando o campo Nome é um campo primário.

1. (Opcional) Clique no link **Abrir em nova guia** ícone ![](assets/open-details-in-a-new-tab-icon.png) <!--check the icon; they are changing it--> no canto superior direito da caixa de registro para abrir a página do registro em uma nova guia.

   A página de registro é aberta.

   ![](assets/details-page.png)

1. Na caixa ou página do registro, clique em **Adicionar capa**. <!--check the casing here; I logged a bug for this-->
A variável **Gravar capa** é aberta.

1. Clique em **Selecione para fazer upload** e procure uma imagem em seu computador para selecionar, adicioná-la e, em seguida, clique em **Usar imagem**.

   A imagem é carregada na parte superior da caixa ou página de registro e as alterações são salvas automaticamente.

   ![](assets/record-page-with-cover-image.png)

1. (Opcional) Passe o mouse sobre a imagem e clique no link **Mais** menu ![](assets/more-menu.png) no canto inferior direito da imagem da capa, siga um destes procedimentos:

   * Clique em **Carregar** se quiser substituir a imagem da capa e repita o Passo 6 para carregar e salvar uma nova imagem.
   * Clique em **Reposicionar** e use o **Reposicionar** ferramenta ![](assets/reposition-tool-icon.png) para centralizar a imagem da capa, clique em **Salvar** quando terminar.
   * Clique em **Remover** para remover a imagem da tampa.

   O Workfront salva suas alterações automaticamente.