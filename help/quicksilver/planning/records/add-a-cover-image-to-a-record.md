---
title: Adicionar uma imagem da capa a um registro
description: É possível personalizar registros adicionando uma imagem de capa à página de registro no Adobe Workfront Planning, ao editar um registro.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 93c6bc15-d945-4cfc-8e87-f5b4e6fac2f4
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '820'
ht-degree: 1%

---


# Adicionar uma imagem da capa a um registro

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

É possível personalizar registros adicionando uma imagem de capa à página de registro no Adobe Workfront Planning, ao editar um registro.

Para obter informações sobre como editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

Você deve criar tipos de registro antes de começar a criar e editar registros.

Para obter informações, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

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
<p>Qualquer </p> 
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
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
   <td><p> Padrão</p>
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
   <td>   <p>Permissões do Contribute ou superior para um espaço de trabalho <span class="preview">e tipo de registro</span>  </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>No ambiente de Produção, todos os usuários, inclusive os Administradores do Sistema, devem ser atribuídos a um modelo de layout que inclua o Planning.</p>
<p><span class="preview">No ambiente de Pré-visualização, os usuários do Standard e os administradores do sistema têm o Planning habilitado por padrão.</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre imagens de capa de página de registro

É possível personalizar a página de um registro adicionando uma imagem de capa a ela.

Considere o seguinte:

* Uma imagem de capa é exclusiva a um registro e não se aplica a todos os registros do mesmo tipo.
* Você pode adicionar somente arquivos de imagem como imagens de capa.
  <!--above: when you know exactly what type of files are allowed, add the exact extensions above-->
* É possível adicionar uma imagem de capa a registros individuais a partir da pré-visualização do registro em qualquer exibição ou da página do registro.
* Não é possível adicionar imagens de capa a partir de uma visualização de registro.
* O Workfront faz o upload de uma imagem de capa automaticamente toda vez que você cria um registro. Posteriormente, você poderá modificar essa imagem.

## Adicionar uma imagem da capa a um registro

É possível personalizar um registro adicionando uma imagem de capa na parte superior da pré-visualização ou página do registro.

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros você deseja personalizar,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

1. Em uma exibição de qualquer tipo, clique em um registro

   Ou

   Na exibição de tabela, clique no ícone **Abrir detalhes** ![Ícone Abrir detalhes](assets/open-details-icon-in-table-name-field.png) na primeira coluna.

   A visualização do registro é aberta na exibição.

   ![Caixa de visualização de detalhes](assets/details-box.png)


1. (Opcional) Clique no ícone !&lbrack;Abrir em nova guia **<!--check the icon; they are changing it--> no canto superior direito da visualização do registro para abrir a página do registro em uma nova guia.**&rbrack;(assets/open-details-in-a-new-tab-icon.png)

   A página de registro é aberta.

   ![Página de detalhes](assets/details-page.png)

1. Na página de visualização ou detalhes do registro, passe o mouse sobre o espaço acima do nome do registro e clique em **Adicionar capa**.

   Ou

   Passe o mouse sobre uma imagem de capa existente, clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Carregar**. <!--check the casing here; I logged a bug for this-->
A caixa **Capa de registro** é aberta na guia **Carregar**.

   ![Caixa de capa de registro para carregamento](assets/record-cover-box-for-upload.png)

1. Clique em **Procurar imagens** e procure uma imagem em seu computador para selecioná-la e adicioná-la.

1. (Opcional) Para remover a imagem antes de salvá-la, clique no **ícone Carregar nova imagem** ![ícone Carregar nova imagem](assets/upload-new-image-icon.png) e carregue uma nova imagem.

1. (Opcional) Clique na guia **Galeria** e clique em uma imagem na galeria de imagens. A galeria de imagens não pode ser modificada.

   ![Caixa de capa de registro para galeria](assets/record-cover-box-for-gallery.png)

1. Clique em **Usar imagem**.

   A imagem é carregada na parte superior da página de visualização ou detalhes do registro e as alterações são salvas automaticamente.

   ![Gravar página com imagem de capa](assets/record-page-with-cover-image.png)

1. (Opcional) Passe o mouse sobre a imagem e clique no menu **Mais** ![Mais menu](assets/more-menu.png), no canto inferior direito da imagem da capa, e siga um destes procedimentos:

   * Clique em **Carregar** se quiser substituir a imagem de capa e repita a Etapa 6 para carregar e salvar uma nova imagem.
   * Clique em **Reposicionar** e use a ferramenta **Reposicionar** ![Ícone da ferramenta Reposicionar](assets/reposition-tool-icon.png) para centralizar a imagem da capa e, em seguida, clique em **Salvar** quando terminar.
   * Clique em **Remover** para remover a imagem da capa.

   O Workfront salva suas alterações automaticamente.
