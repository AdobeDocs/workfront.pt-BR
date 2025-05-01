---
title: Excluir espaços de trabalho
description: É possível excluir espaços de trabalho quando eles não são mais relevantes.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: adec4b8e-2964-479b-8cf0-79d3afa27b2a
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '522'
ht-degree: 1%

---


# Excluir espaços de trabalho

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

No Adobe Workfront Planning, os espaços de trabalho são locais centralizados para as equipes planejarem o trabalho. Para obter mais informações, consulte [Criar espaços de trabalho](/help/quicksilver/planning/architecture/create-workspaces.md).

É possível excluir espaços de trabalho que não são mais relevantes.

Recomendamos recriar alguns ou todos os tipos de registros, registros, campos e views associados ao espaço de trabalho que você deseja excluir em outro espaço de trabalho antes de excluí-lo.

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
   <td><p> Padrão </p>
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
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
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

## Considerações sobre a exclusão de espaços de trabalho

* Quando você exclui espaços de trabalho, todos os tipos de registro, registros, campos e exibições também são excluídos.
* Os espaços de trabalho excluídos e as informações que eles contêm não podem ser recuperados.

## Excluir um espaço de trabalho

{{step1-to-planning}}

1. (Condicional) Se você for um administrador do Workfront, clique em **Espaços de trabalho em que estou** para acessar os espaços de trabalho que você criou ou em **Outros espaços de trabalho** para acessar os espaços de trabalho que outras pessoas compartilharam com você.

1. (Opcional) Clique em **Mostrar tudo** para exibir espaços de trabalho adicionais. O link **Mostrar tudo** é exibido somente quando há mais de duas linhas de cartões de espaço de trabalho.
1. (Opcional) Clique em K **Mostrar menos** para limitar o número de espaços de trabalho exibidos na tela.
1. Para deletar um espaço de trabalho, siga um destes procedimentos:

   * Passe o mouse sobre o cartão de espaço de trabalho e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão
Ou
   * Clique em um cartão de espaço de trabalho para abrir o espaço de trabalho e no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do espaço de trabalho.
1. Clique em **Excluir**.

   ![Excluir permanentemente a confirmação do espaço de trabalho](assets/permanently-delete-workspace-confirmation.png)

1. Digite &quot;**delete**&quot; no espaço fornecido e clique em **Excluir permanentemente**. Isso não diferencia maiúsculas de minúsculas.

   O espaço de trabalho foi excluído e não pode ser recuperado. Quaisquer tipos de registro, registros, campos e exibições associados a eles também são excluídos. <!--ensure this is right at or before GA-->
