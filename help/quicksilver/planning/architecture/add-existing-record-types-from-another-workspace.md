---
title: Adicionar tipos de registro existentes de outro Workspace
description: Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível adicionar um tipo de registro existente criado em outro espaço de trabalho.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: eacc6b26bd30ac7da363c6aa1d759a65a20cd9f4
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Adicionar tipos de registro existentes de outro espaço de trabalho

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como um gerenciador de espaço de trabalho, você pode adicionar um tipo de registro que existe em outro espaço de trabalho a um espaço de trabalho gerenciado no Adobe Workfront Planning.

Este artigo descreve como adicionar um tipo de registro a partir de um existente e como excluí-lo, se ele não for mais necessário.

Um gerenciador de espaço de trabalho deve primeiro designar um tipo de registro como centralizado antes que você possa adicioná-lo aos espaços de trabalho que você gerencia como um tipo de registro existente.

Você pode designar um tipo de registro como centralizado ao criá-lo ou editá-lo, conforme estiver definindo suas configurações avançadas.

Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Antes de adicionar registros a um espaço de trabalho a partir de um tipo de registro centralizado, consulte o artigo [Visão geral dos tipos de registro entre espaços de trabalho](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<!--Or:
<ul><li><p>Any Workflow package</p> </li>
And
<li><p>Planning Prime or Ultimate package</p></li></ul>-->
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

## Criar um tipo de registro a partir de um tipo de registro existente

1. Comece a criar um tipo de registro, conforme descrito no artigo [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md), em seguida, clique em **Adicionar existente**. <!--check this - the option might have been renamed in the UI-->

   ![Modal para adicionar tipo de registro com opção para adicionar de outro espaço de trabalho](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Clique em **Continuar**.
1. Na caixa **Escolher tipo de registro**, clique no cartão do tipo de registro que deseja adicionar de um espaço de trabalho existente e clique em **Adicionar**.

   O tipo de registro é adicionado ao espaço de trabalho selecionado.

   >[!TIP]
   >
   >Quando não há tipos de registro configurados para serem adicionados a outro espaço de trabalho, a opção para adicioná-los de outro espaço de trabalho não é exibida.

   As seguintes situações ocorrem:

   * As seguintes informações também são adicionadas do tipo de registro centralizado existente:

      * Todos os campos originais
      * Todas as conexões de registro
   * É possível exibir registros adicionados de outros espaços de trabalho que usam o mesmo tipo de registro centralizado, somente quando você tem pelo menos permissões de Exibição para esses espaços de trabalho.
   * O ícone **tipo de registro centralizado** ![ícone do tipo de registro centralizado](assets/global-icon.png) é adicionado ao cartão do novo tipo de registro.
   * O campo somente leitura **Workspace** é adicionado à nova exibição de tabela do tipo de registro. O campo exibe em qual espaço de trabalho cada registro foi criado.

     >[!NOTE]
     >
     >Não é possível editar a aparência, as configurações avançadas ou os campos originais do novo tipo de registro. É possível editar o tipo de registro e todos os campos e configurações originais somente no espaço de trabalho original.

1. (Opcional) Clique em, em seguida arraste e solte o tipo de registro recém-adicionado em qualquer seção no espaço de trabalho.

<!--This will be released later with another epic: 1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.-->

## Excluir um tipo de registro centralizado de um espaço de trabalho secundário

É possível excluir um tipo de registro adicionado de outro espaço de trabalho se não for mais necessário. Excluí-lo apenas o removerá do espaço de trabalho secundário e excluirá os registros adicionados desse espaço de trabalho. O tipo de registro original permanece em seu espaço de trabalho original e em outros espaços de trabalho aos quais foi adicionado.

Para deletar um tipo de registro centralizado de um espaço de trabalho secundário:

1. Vá para o tipo de registro centralizado no espaço de trabalho secundário.

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no cartão do tipo de registro ou à direita do nome do tipo de registro em sua página e clique em **Excluir**.
1. (Condicional) Digite **delete** no campo fornecido e clique em **Excluir permanentemente**.

   As seguintes situações ocorrem:

   * O tipo de registro criado de um tipo de registro centralizado é removido do espaço de trabalho selecionado.
   * O tipo de registro original e seus campos permanecem no espaço de trabalho original.
   * O tipo de registro permanece em todos os outros espaços de trabalho aos quais foi adicionado.
   * Os registros adicionados ao tipo de registro do espaço de trabalho atual são excluídos. Todos os outros registros adicionados de espaços de trabalho adicionais onde o tipo de registro centralizado foi adicionado são preservados.





