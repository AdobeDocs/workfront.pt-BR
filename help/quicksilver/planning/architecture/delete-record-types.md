---
title: Excluir Tipos de Registro
description: É possível excluir tipos de registro quando eles não forem mais relevantes. A exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro, como seus registros, campos e exibições.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 2%

---


# Excluir tipos de registro

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

É possível excluir tipos de registro quando eles não forem mais relevantes.

No entanto, a exclusão de tipos de registro também exclui todas as informações associadas aos tipos de registro. Para obter mais informações, consulte a seção [Considerações ao excluir tipos de registro](#considerations-when-deleting-record-types) neste artigo.

Para obter informações sobre tipos de registros, consulte [Visão geral sobre tipos de registros](/help/quicksilver/planning/architecture/overview-of-record-types.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>plataforma Adobe Workfront</p></td> 
   <td> 
<p>A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para acessar todos os recursos do Workfront Planning.</p> 
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
   <td>   <p>Gerenciar permissões para um espaço de trabalho <span class="preview">e tipo de registro</span></p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p></td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Modelo de layout</p></td> 
   <td> <p>No ambiente de Produção, todos os usuários, inclusive os Administradores do Sistema, devem ser atribuídos a um modelo de layout que inclua o Planning.</p>
<p><span class="preview">No ambiente de Pré-visualização, os usuários do Standard e os administradores do sistema têm o Planning habilitado por padrão.</span></p></td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Considerações ao excluir tipos de registro

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* Você pode excluir somente tipos de registro de espaços de trabalho para os quais tem permissões de gerenciamento.
* A exclusão de tipos de registro remove as seguintes informações associadas a eles:

   * Todos os registros desse tipo.
   * Todos os campos associados ao tipo de registro.
   * Todas as exibições (incluindo filtros, agrupamentos e critérios de classificação) do tipo de registro.
* O tipo de registro é removido de todos os usuários que acessam o espaço de trabalho.
* Não é possível recuperar tipos de registros excluídos ou suas informações.
* É recomendável recriar os campos e os registros associados ao tipo de registro que você deseja excluir em outro tipo de registro antes de excluí-los.

## Excluir tipos de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja deletar,

   Ou

   Em um espaço de trabalho, expanda a seta apontando para baixo à direita do nome de um espaço de trabalho existente, procure um espaço de trabalho e selecione-o quando ele for exibido na lista.

   O espaço de trabalho é aberto e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de tipo de registro, clique no menu **Mais** e **Excluir**.
   * Clique no cartão do tipo de registro que deseja excluir e, na página de tipo de registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Excluir**.

   ![Excluir permanentemente a confirmação do tipo de registro](assets/permanently-delete-record-type-confirmation.png)

1. Digite **excluir** na caixa de confirmação e clique em **Excluir permanentemente**. Isso não diferencia maiúsculas de minúsculas.

   O tipo de registro selecionado, juntamente com seus campos, registros associados e exibições são excluídos e não podem ser recuperados.
