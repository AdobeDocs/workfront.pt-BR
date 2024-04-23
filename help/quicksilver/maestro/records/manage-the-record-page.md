---
title: Gerenciar a página de registros
description: É possível editar e gerenciar o layout da caixa de registro e da página no Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: c044b4df-f61d-48e0-be9b-e9fa151b092b
source-git-commit: 6bea34403e45c2b50986f79272f7a46959d67c6d
workflow-type: tm+mt
source-wordcount: '520'
ht-degree: 0%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Gerenciar a página de registros

{{maestro-important-intro}}

É possível editar e gerenciar o layout da caixa de registro e da página no Adobe Workfront Planning. Você pode exibir a caixa de registro em uma visualização de registro.

A caixa de registro é uma exibição menor da página de registro exibida na exibição de um tipo de registro.

Quando você altera o layout de uma caixa e de uma página de registro, a caixa e a página são alteradas para todos os registros do mesmo tipo.

Você deve criar tipos de registro e registros antes de começar a editar páginas de registro.

Para obter informações, consulte os seguintes artigos:

* [Criar tipos de registro](../architecture/create-record-types.md)

* [Criar registros](/help/quicksilver/maestro/records/create-records.md)

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
   <td> <p>Gerenciar ou aumentar as permissões de um espaço de trabalho</a> </p>  
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

## Considerações sobre a edição de páginas de registro

* A reorganização de campos na caixa de registro ou página reorganiza os campos para todos os registros desse tipo e para todos os usuários que acessam esses registros.
* A adição de uma imagem de capa a um registro não faz parte do layout geral da caixa ou página do registro. Você pode adicionar imagens de capa exclusivas a cada registro. Para obter informações, consulte [Adicionar uma imagem da capa a um registro](/help/quicksilver/maestro/records/add-a-cover-image-to-a-record.md).

## Reorganizar campos na caixa ou página de registro

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

1. Na caixa ou página do registro, clique no ícone de captura ![](assets/grab-icon.png) à esquerda de um nome de campo, arraste e solte-o no ponto desejado.

   A nova posição do campo é atualizada na caixa e na página de todos os registros do mesmo tipo para todos os usuários que visualizam os registros.

   Todas as alterações no layout da caixa de registro ou página são salvas automaticamente.

