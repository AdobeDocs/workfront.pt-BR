---
title: Excluir Registros
description: É possível excluir registros criados por você ou por outro usuário.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '681'
ht-degree: 2%

---


# Excluir registros

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Você pode excluir registros que não são mais relevantes no Adobe Workfront Planning. É possível recuperar registros excluídos por 30 dias após a exclusão. Para obter informações sobre como recuperar registros excluídos, consulte [Recuperar registros excluídos](/help/quicksilver/planning/records/restore-deleted-records.md).

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
   <td>   <p>Permissões do Contribute ou superior para um espaço de trabalho e tipo de registro </a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p> </td> 
  </tr> 
</tbody> 
</table>

*Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre a exclusão de registros

* É possível excluir registros criados por você ou por outro usuário.
* É possível recuperar registros excluídos que você ou outras pessoas excluíram.
* Se os registros excluídos estiverem vinculados a outros registros, os registros vinculados não serão excluídos, mas as informações do registro excluído também serão excluídas.
* Não é possível excluir registros da linha do tempo ou das exibições do calendário.

## Excluir registros

É possível excluir um registro das seguintes áreas:

* [Da página do registro](#delete-a-record-from-the-records-page)
* [Na exibição de tabela de um tipo de registro](#delete-a-record-from-the-record-type-table-view)

### Excluir um registro da página do registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros você deseja deletar.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.
1. Siga um destes procedimentos:

   * Em uma exibição de Tabela, clique no nome de um registro.
   * Na exibição de Tabela, passe o mouse sobre o nome de um registro e clique no menu **Mais** ![Mais menu](assets/more-menu.png) e clique em **Exibir**

     ![Menu contextual da linha de registro](assets/contextual-menu-for-record-row.png)
   * Em uma exibição de Linha do tempo, clique em uma barra de registro.

   A página de registro é aberta.

1. Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do registro e clique em **Excluir** e depois em **Excluir** novamente para confirmar.

   ![Mais opções de menu da página de detalhes do registro](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
O registro é excluído.
1. (Opcional) Vá para a exibição de tabela da página de registro e clique no **ícone Desfazer** ![ícone Desfazer](assets/undo-icon.png) no canto superior direito da exibição e, em seguida, clique em **Excluído recentemente** para recuperar os registros excluídos.

Para obter informações sobre como recuperar registros excluídos, consulte [Recuperar registros excluídos](/help/quicksilver/planning/records/restore-deleted-records.md).

### Excluir um registro da exibição de tabela do tipo de registro

{{step1-to-planning}}

1. Clique no espaço de trabalho cujos registros você deseja deletar.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.
1. (Condicional) No menu suspenso **Exibir**, no canto superior esquerdo da tabela, selecione um modo de exibição de Tabela. Essa deve ser a exibição padrão, a menos que você tenha visualizado o tipo de registro na exibição de linha do tempo ao acessá-lo pela última vez.

   Os registros associados ao tipo de registro selecionado são exibidos na exibição de tabela.
1. Siga um destes procedimentos:

   * Clique com o botão direito do mouse em uma linha de registro e clique em **Excluir**.
   * Clique no menu **Mais** ![Mais menu](assets/more-menu.png) à direita do nome do registro e clique em **Excluir**.

     ![Menu contextual da linha de registro](assets/contextual-menu-for-record-row.png)

   * Clique no ícone **Abrir detalhes** ![Ícone Abrir detalhes no campo de nome de tabela](assets/open-details-icon-in-table-name-field.png) para abrir a caixa com as informações detalhadas do registro e clique no menu **Mais** ![Mais](assets/more-menu.png) à direita do nome do registro e **Excluir**.

   O registro é excluído.

1. (Opcional) Siga um destes procedimentos para desfazer ou refazer a exclusão de um registro:

   * Clique no ícone **Desfazer** ![Ícone Desfazer](assets/undo-icon.png) e **Excluído recentemente** para recuperar os registros excluídos. Para obter informações sobre como recuperar registros excluídos, consulte [Recuperar registros excluídos](/help/quicksilver/planning/records/restore-deleted-records.md).
   * Use os atalhos de teclado a seguir para desfazer ou refazer a exclusão de um registro:

      * CTRL + Z (⌘ + Z para Mac) para desfazer a exclusão de um registro
      * CTRL + Shift + Z (⌘ + Shift + Z para Mac) para refazer a exclusão do registro




