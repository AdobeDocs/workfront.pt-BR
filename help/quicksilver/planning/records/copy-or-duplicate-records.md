---
title: Registros Duplicados
description: Você pode duplicar um registro existente na exibição de tabela. Uma cópia idêntica do registro existente é adicionada à página de tipo de registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2fed8c96-0c9c-4662-a9c4-66dae507ff2a
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 2%

---

# Registros duplicados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

No Adobe Workfront Planning, um registro é uma instância de um tipo de registro.

Você pode duplicar um registro existente na exibição de tabela. Uma cópia idêntica do registro existente é adicionada à página de tipo de registro.

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
   <td>   <p>Contribuir com ou mais permissões para um espaço de trabalho e tipo de registro</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Duplicar um registro <!--in a record type table (I don't think you can create them elsewhere right now)-->

Você pode criar registros na exibição de tabela de uma página de tipo de registro duplicando uma existente. Um registro idêntico ao existente é criado e adicionado ao registro original.


{{step1-to-planning}}

1. Clique no espaço de trabalho ao qual deseja adicionar registros.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro. Para obter informações sobre como criar um tipo de registro, consulte [Criar tipos de registro](/help/quicksilver/planning/architecture/create-record-types.md).

   A página do tipo de registro é aberta na exibição acessada pela última vez. Por padrão, uma página do tipo de registro é aberta na exibição de tabela.
Todos os registros do tipo selecionado são exibidos na visualização.

1. (Condicional) Selecione uma exibição de tabela.

1. Siga um destes procedimentos:

   * Passe o mouse sobre o nome de um registro, em seguida, clique no menu **Mais** incorporado com o nome do registro e, em seguida, clique no ícone **Duplicar** ![Ícone duplicar cinza](assets/duplicate-icon-gray.png).

     ![Mais menus do registro na exibição de tabela](assets/more-menu-from-record-in-table-view.png)

   * Selecione um registro e clique no ícone **Duplicar** ![Ícone Duplicar branco e azul](assets/duplicate-icon-white-and-blue.png) na barra de ferramentas, na parte inferior da página.

     ![Duplicar ícone na barra de ferramentas na exibição de tabela](assets/duplicate-icon-in-toolbar-in-table-view.png)

   Um registro idêntico com um nome idêntico é criado abaixo do registro original. Todos os campos do novo registro são preenchidos com as mesmas informações do registro original.

1. (Opcional) Comece a atualizar as informações sobre o novo registro nos campos disponíveis na exibição de tabela ou clique no registro e atualize as informações na visualização ou página do registro.

   >[!NOTE]
   >
   >  * Não há campos obrigatórios para registros. No entanto, recomendamos adicionar informações para o campo principal de um registro, pois é útil identificar registros ao vincular registros uns aos outros. Para obter mais informações sobre campos primários, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md) e [Visão geral do campo primário](/help/quicksilver/planning/fields/primary-field-overview.md).
   >
   >  * Os campos que se referem a outros tipos de registro ou campos calculados são campos somente leitura.

   Para obter mais informações sobre como editar registros, consulte [Editar registros](/help/quicksilver/planning/records/edit-records.md).

1. (Opcional) Use os seguintes atalhos de teclado para desfazer ou refazer a adição de novos registros ou suas informações ao adicioná-los na exibição de tabela:

   * CTRL + Z (⌘ + Z para Mac) para desfazer uma alteração
   * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer uma alteração.
