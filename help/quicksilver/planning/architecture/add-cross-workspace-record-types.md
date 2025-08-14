---
title: Adicionar Tipos de Registro Entre Espaços de Trabalho
description: Os tipos de registro são os tipos de objeto do Adobe Workfront Planning. No Workfront Planning, você pode importar um tipo de registro existente de outro espaço de trabalho.
hidefromtoc: true
hide: true
exl-id: b977d5dd-8975-42c4-9968-a7ac357972e6
source-git-commit: b6ced451cdd6b38b5661a076b2311a34c2c70432
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 2%

---

<!-- add these to the metadata, when making this public: 

feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
-->

# Adicionar tipos de registro entre espaços de trabalho

<span class="preview">As informações nesta página se referem a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como gerenciador de espaço de trabalho, você pode importar ou adicionar um tipo de registro existente a outro espaço de trabalho.

Primeiro, você deve designar um tipo de registro como centralizado para que os gerentes de espaço de trabalho possam importá-lo para outros espaços de trabalho.

Você pode designar um tipo de registro como centralizado ao criá-lo ou editá-lo, conforme estiver definindo suas configurações entre espaços de trabalho.

Para obter informações, consulte [Configurar recursos entre espaços de trabalho para tipos de registro](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.  

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
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

## Visão geral dos tipos de registros centralizados

Considerações ao adicionar tipos de registro existentes de outro espaço de trabalho

* Quando não há tipos de registro configurados para serem adicionados a outro espaço de trabalho, a opção para importá-los de outro espaço de trabalho não é exibida ao criar um tipo de registro. <!--add this a tip in the steps below, and/ or add a Conditional step that this is possible only when these record types are first enabled-->
* Após adicionar o tipo de registro de outro espaço de trabalho, as seguintes informações também são adicionadas do tipo de registro existente:

   * Campos
   * Registros
   * Gravar conexões

* É possível editar o tipo de registro, incluindo seus campos, somente em seu espaço de trabalho original. Não é possível editá-lo nos espaços de trabalho em que foi adicionado.

## Criar um tipo de registro a partir de um tipo de registro existente

1. Comece a criar um tipo de registro, conforme descrito no artigo [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md), em seguida, clique em **Adicionar existente**. <!--check this - the option might have been renamed in the UI-->

   ![Modal para adicionar tipo de registro com opção para importar de outro espaço de trabalho](assets/add-record-type-from-existing-workspace-option-when-creating-records.png)

1. Clique em **Continuar**.
1. Na caixa **Escolher tipo de registro**, clique no cartão do tipo de registro que deseja adicionar de um espaço de trabalho existente e clique em **Adicionar**.

   O tipo de registro é adicionado ao espaço de trabalho selecionado e as seguintes situações ocorrem:

   * O **ícone de tipo de registro entre espaços de trabalho** ![ícone de conexão entre espaços de trabalho](assets/global-icon.png) foi adicionado ao cartão do tipo de registro importado.
   * O campo somente leitura **Workspace** é adicionado ao tipo de registro importado. O campo exibe em qual espaço de trabalho cada registro foi criado.

     >[!NOTE]
     >
     >* Não é possível editar o tipo de registro importado ou seus campos. É possível editar o tipo de registro e seus campos no espaço de trabalho original.

1. (Opcional) Clique no menu **Mais** ![Mais menu](assets/more-menu.png) no cartão do tipo de registro importado ou à direita do nome do tipo de registro em sua página e clique em **Excluir**.
1. (Condicional) Digite **delete** no campo fornecido e clique em **Excluir permanentemente**.

   Isso remove o tipo de registro importado do espaço de trabalho selecionado. O tipo de registro original e seus campos permanecem no espaço de trabalho original.

   <!--**************************ASK LILIT ON THIS ONE, NOT SURE IF THIS IS TRUE: Any records added in the current workspace are saved in the original workspace.**********-->



