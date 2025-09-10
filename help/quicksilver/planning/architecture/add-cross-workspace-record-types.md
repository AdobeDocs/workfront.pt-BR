---
title: Adicionar Tipos de Registro Existentes
description: Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, é possível adicionar um tipo de registro existente criado em outro espaço de trabalho.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: 38c397594449856a0f1404848a527b86083654b8
workflow-type: tm+mt
source-wordcount: '666'
ht-degree: 0%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Adicionar tipos de registro existentes

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como um gerenciador de espaço de trabalho, você pode adicionar um tipo de registro que existe em um espaço de trabalho a um espaço de trabalho gerenciado no Adobe Workfront Planning.

Primeiro, você deve designar um tipo de registro como centralizado para que os gerentes de espaço de trabalho possam adicioná-lo a outros espaços de trabalho como um tipo de registro existente.

Você pode designar um tipo de registro como centralizado ao criá-lo ou editá-lo, conforme estiver definindo suas configurações entre espaços de trabalho.

Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

Antes de adicionar registros a um espaço de trabalho a partir de um tipo de registro centralizado, consulte o artigo [Visão geral dos tipos de registro centralizado](/help/quicksilver/planning/architecture/centralized-record-types-overview.md).

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
E
<li><p>Pacote do Planning Plus</p></li></ul>
Ou:
<ul><li><p>Qualquer pacote de fluxo de trabalho</p> </li>
E
<li><p>Planejamento do pacote Prime ou Ultimate</p></li></ul>
<p>Para obter mais informações sobre o que está incluído em cada plano do Workfront Planning, entre em contato com seu gerente de conta da Workfront. </p> 
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
   >Quando não há tipos de registro configurados para serem adicionados a outro espaço de trabalho, a opção para adicioná-los de outro espaço de trabalho não é exibida ao criar um tipo de registro.

   As seguintes situações ocorrem:

   * As seguintes informações também são adicionadas do tipo de registro centralizado existente:

      * Todos os campos originais
      * Todas as conexões de registro
   * Você pode exibir registros adicionados de outros espaços de trabalho, somente quando tiver pelo menos permissões de Exibição para esses espaços de trabalho.
   * O ícone **tipo de registro centralizado** ![ícone do tipo de registro centralizado](assets/global-icon.png) é adicionado ao cartão do novo tipo de registro.
   * O campo somente leitura **Workspace** é adicionado à nova exibição de tabela do tipo de registro. O campo exibe em qual espaço de trabalho cada registro foi criado.

     >[!NOTE]
     >
     >* Não é possível editar a aparência, as configurações avançadas ou os campos originais do novo tipo de registro. É possível editar o tipo de registro e todos os campos e configurações originais somente no espaço de trabalho original.

1. (Opcional) Clique em, em seguida arraste e solte o tipo de registro recém-adicionado em qualquer seção no espaço de trabalho.

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no cartão do novo tipo de registro ou à direita do nome do tipo de registro em sua página e clique em **Compartilhar** para compartilhá-lo com outros usuários no mesmo espaço de trabalho.

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no cartão do novo tipo de registro ou à direita do nome do tipo de registro em sua página e clique em **Excluir**.
1. (Condicional) Digite **delete** no campo fornecido e clique em **Excluir permanentemente**.

   As seguintes situações ocorrem:

   * O tipo de registro criado de um tipo de registro centralizado é removido do espaço de trabalho selecionado.
   * O tipo de registro original e seus campos permanecem no espaço de trabalho original.
   * Todos os outros tipos de registro adicionados do mesmo tipo de registro centralizado permanecem em seus espaços de trabalho.
   * Os registros adicionados ao tipo de registro do espaço de trabalho atual são excluídos. Todos os outros registros adicionados de espaços de trabalho adicionais onde o tipo de registro centralizado foi adicionado são preservados.





