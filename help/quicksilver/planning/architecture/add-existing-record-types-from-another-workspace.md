---
title: Adicionar tipos de registro existentes de outro Workspace
description: Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível adicionar um tipo de registro existente criado em outro espaço de trabalho.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 7d37481fc5b468f6f8ea1fce6ccd7ae064f00251
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Adicionar tipos de registro existentes de outro espaço de trabalho

{{planning-important-intro}}

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como um gerenciador de espaço de trabalho, você pode adicionar um tipo de registro que existe em outro espaço de trabalho a um espaço de trabalho gerenciado no Adobe Workfront Planning.

Um gerenciador de espaço de trabalho deve primeiro designar um tipo de registro como um tipo de registro global antes que você possa adicioná-lo aos espaços de trabalho que você gerencia como um tipo de registro existente. Os gerentes do Workspace podem designar um tipo de registro como global ao criá-lo ou editá-lo, definindo as configurações entre espaços de trabalho do tipo de registro.

Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Este artigo descreve como adicionar um tipo de registro a partir de um existente e como excluí-lo, se ele não for mais necessário.

Antes de adicionar registros a um espaço de trabalho a partir de um tipo de registro global, consulte também o artigo [Visão geral dos tipos de registro entre espaços de trabalho](/help/quicksilver/planning/architecture/cross-workspace-record-types-overview.md).


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
<li><p>Um pacote do Planning Plus para criar tipos de registros globais</p></li>
</ul>
Ou:
<ul><li><p>Um pacote de fluxo de trabalho do Prime ou Ultimate</p> </li>
E
<li><p>Um pacote do Planning Prime ou Ultimate</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
   </td>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e para o tipo de registro </a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Criar um tipo de registro adicionando um existente de outro espaço de trabalho

>[!NOTE]
>
>Verifique se há pelo menos um tipo de registro designado como global em pelo menos um outro espaço de trabalho.

1. Comece a criar um tipo de registro, conforme descrito no artigo [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md), em seguida, clique em **Adicionar existente**. <!--check this - the option might have been renamed in the UI-->

   ![Modal para adicionar tipo de registro com opção para adicionar de outro espaço de trabalho](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

   >[!TIP]
   >
   >Quando não há tipos de registro configurados para serem adicionados a outros espaços de trabalho em seu sistema, a opção **Adicionar existente** não é exibida.

1. Clique em **Continuar**.
1. Na caixa **Escolher o tipo de registro**, clique no cartão do tipo de registro que deseja adicionar de um espaço de trabalho existente e clique em **Adicionar**.

   O tipo de registro é adicionado ao espaço de trabalho selecionado e o ícone **do** tipo de registro global![](assets/global-icon.png) é exibido no cartão do tipo de registro.

   As seguintes situações ocorrem:

   * As seguintes informações também são adicionadas do tipo de registro global existente:

      * Todos os campos originais
      * Todas as conexões de registro
   * Você pode exibir registros adicionados de outros espaços de trabalho que usam o mesmo tipo de registro global, somente quando tiver pelo menos permissões de Exibição para esses espaços de trabalho.
   * O campo somente leitura **Workspace** é adicionado à nova exibição de tabela do tipo de registro. O campo exibe o espaço de trabalho onde cada registro foi criado.

     >[!NOTE]
     >
     >Não é possível editar a aparência do novo tipo de registro, as configurações adicionais ou os campos originais. É possível editar o tipo de registro e todos os campos e configurações originais somente no espaço de trabalho original.

1. (Opcional) Clique em, em seguida arraste e solte o tipo de registro recém-adicionado em qualquer seção no espaço de trabalho.

<!--This will be released later with another epic: 
1. In the table view, click the **+** icon in the upper-right corner to add new fields. For information, see [Create fields](/help/quicksilver/planning/fields/create-fields.md).
1. (Optional) Click the **More** menu ![More menu](assets/more-menu.png) in the new record type's card, or to the right of the record type's name on its page, then click **Share** to share it with other users in the same workspace, or adjust their permissions to the record type.
-->

&lt;!—verificando com Lilit se podemos adicionar automações ou solicitar formulários para RTs globais secundários??—adicione etapa com links para esses artigos se/ quando sim—>

## Excluir um tipo de registro global de um espaço de trabalho secundário

É possível excluir um tipo de registro adicionado de outro espaço de trabalho se não for mais necessário. Excluí-lo somente o removerá do espaço de trabalho secundário.

Quando você deleta um tipo de registro global de um espaço de trabalho secundário, os itens a seguir também são deletados:

* Os registros adicionados do espaço de trabalho secundário.
* Os campos adicionados do espaço de trabalho secundário.

Os tipos de registro global excluídos de seus espaços de trabalho secundários não podem ser recuperados.

O tipo de registro original permanece em seu espaço de trabalho original, bem como em outros espaços de trabalho aos quais foi adicionado.

Para deletar um tipo de registro global de um espaço de trabalho secundário:

1. Vá para o tipo de registro global no espaço de trabalho secundário.

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no cartão do tipo de registro ou à direita do nome do tipo de registro em sua página e clique em **Excluir**.
1. (Condicional) Digite **delete** no campo fornecido e clique em **Excluir permanentemente**.

   ![Excluir caixa de confirmação do tipo de registro global secundário](assets/delete-secondary-global-record-type.png)

   As seguintes situações ocorrem:

   * O tipo de registro criado a partir de um tipo de registro global é removido do espaço de trabalho selecionado.
   * O tipo de registro original e seus campos permanecem no espaço de trabalho original.
   * O tipo de registro permanece em todos os outros espaços de trabalho aos quais foi adicionado.
   * Os registros e campos adicionados ao tipo de registro do espaço de trabalho atual são excluídos. Todos os outros registros adicionados de espaços de trabalho adicionais onde o tipo de registro global foi adicionado são preservados. Os campos são preservados nos espaços de trabalho onde foram adicionados.





