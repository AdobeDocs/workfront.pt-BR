---
title: Configurar a área de configurações de um tipo de registro
description: Você poderá editar os tipos de registro depois que eles forem salvos na página Configurações.
hide: true
hidefromtoc: true
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---


<!--add better metadata at release:

title: Configure Record Type Settings
description: You can edit record types after they have been saved in the Settings page. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog 

-->

# Definir a área Configurações de um tipo de registro

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode definir configurações adicionais para um tipo de registro depois que elas tiverem sido salvas no Adobe Workfront Planning.

Dependendo dos recursos que deseja definir para um tipo de registro, é possível definir configurações adicionais para ele ao seguir um destes procedimentos:

<!--the above will need to be reworded when we add automations and manage request forms to this area-->

* Editá-los

  Para obter informações, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).

* Definição da página Configurações de um tipo de registro.

  Este artigo descreve como editar um tipo de registro definindo sua página Configurações.

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
<ul><li><p>Qualquer pacote do Workfront</p></li>
<p>E</p>
<li><p>Qualquer pacote do Planning para criar tipos de registro conectáveis</p></li>
<li><p>Pacote do Planning Plus para criar tipos de registro centralizados</p></li>
</ul>
<p>Ou:</p>
<ul><li><p>Um pacote do Workflow e do Planning Prime ou Ultimate</p> </li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> 

-->

## Configurar informações de tipo de registro na página Configurações

Você pode definir recursos entre espaços de trabalho para um tipo de registro, configurando as informações na página Configurações.

<!--the intro above will change when we can configure more in this area -->

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos tipos de registro você deseja editar,

   A página do espaço de trabalho é aberta e os tipos de registro são exibidos.
1. Siga um destes procedimentos:

   * Passe o mouse sobre o cartão de um tipo de registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) no canto superior direito do cartão de tipo de registro e clique em **Configurações**
Ou
   * Clique em um cartão de tipo de registro para abrir a página de tipo de registro, clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do tipo de registro e clique em **Configurações**.

   <!--update screen shot at release-->

   ![Mais opções de menu do cartão de tipo de registro](assets/more-menu-options-from-record-type-card.png)

1. A seção **Configurações entre espaços de trabalho** está selecionada por padrão.
1. Ative ou desative uma das seguintes configurações:

   * **Permitir a adição deste tipo de registro a outros espaços de trabalho** para indicar que este é um tipo de registro global
   * **Permitir a conexão com este tipo de registro em outros espaços de trabalho** para indicar que este é um tipo de registro conectável.

   As configurações estão desativadas por padrão.

   Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)