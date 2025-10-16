---
title: Duplicar Visualizações de Registro
description: Se quiser manter várias versões de uma exibição e fazer pequenas alterações entre as versões, você poderá duplicar uma exibição no Adobe Workfront Planning. Este artigo descreve como duplicar uma visualização.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 441a53d1-ad39-41b7-93fe-2ae1836476c9
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

# Exibições de registro duplicadas

<!--remove preview and production references-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>


{{planning-important-intro}}

Se quiser manter várias versões de uma exibição e fazer pequenas alterações entre as versões, você poderá duplicar uma exibição no Adobe Workfront Planning.

A duplicação de uma exibição cria cópias idênticas de uma exibição existente.

As permissões de compartilhamento da exibição original não são transferidas para a exibição duplicada.

A duplicação de exibições é idêntica para todos os tipos de exibições no Workfront Planning.

## Requisitos de acesso

+++ Expanda para exibir os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Qualquer Workfront e qualquer pacote do Planning</p></li>
Ou
<li><p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para uma exibição</p>  
   <p>Permissões de exibição para uma exibição para alterar temporariamente as configurações de exibição ou duplicá-las.</p> </td> 
  </tr>   
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard </p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it.</p> </td> 
  </tr> 
</tbody> 
</table> -->

## Duplicar uma visualização de registro

{{step1-to-planning}}

1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.
Por padrão, todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. Dependendo do ambiente usado, faça o seguinte:

   * No ambiente de Produção, passe o mouse sobre um dos nomes de exibição na guia de exibição e clique em **Mais** ![Mais menu](assets/more-menu.png) à esquerda do nome da exibição e clique em **Duplicar**.
   * <span class="preview">No ambiente de Visualização, clique no ícone suspenso ![Ícone suspenso](assets/drop-down-icon.png) ao lado do nome da exibição atual, passe o mouse sobre o nome de uma exibição, clique em **Mais** e em **Duplicar**.</span>

     ![Mais menu no modo de exibição com opções](assets/more-menu-for-views-expanded-with-delete-option.png)

     A exibição está duplicada e o nome da nova exibição segue o seguinte padrão: `Original view's name (Copy)`. A nova guia de exibição é exibida no final de todas as guias de exibição.
