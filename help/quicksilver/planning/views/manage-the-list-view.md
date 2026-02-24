---
title: Gerenciar a Exibição de Lista no Adobe Workfront Planning
description: Você pode exibir objetos e seus campos em uma exibição de lista, ao acessá-los na página Registros conectados de um registro, no Adobe Workfront Planning. Este artigo descreve como criar ou editar uma exibição de lista na página Registros conectados de um registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: 11b72c797203dcf364281665bc60cf67d25c8b5d
workflow-type: tm+mt
source-wordcount: '1001'
ht-degree: 1%

---


# Gerenciar a exibição de lista no Adobe Workfront Planning

<!--<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Você pode exibir objetos e seus campos em uma exibição de lista, ao acessá-los na página Registros conectados de um registro, no Adobe Workfront Planning.

Este artigo descreve como criar ou editar uma exibição de lista na página Registros conectados de um registro e como editar os objetos na exibição.

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
<p>Qualquer Workfront e qualquer pacote do Planning</p>
<p>Qualquer fluxo de trabalho e qualquer pacote de planejamento</p>
<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p> Padrão para criar e excluir visualizações</p>
   <p>Colaborador ou superior para atualizar elementos de visualização</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para uma exibição</p>  
   <p>Exibir permissões de um modo de exibição para alterar temporariamente as configurações de modo de exibição ou duplicá-lo</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Modelo de layout</p></td>
   <td> Os usuários com uma licença Light ou Contributor devem receber um modelo de layout que inclua o Planning.
   <p>Usuários padrão e Administradores do sistema têm as áreas do Planning habilitadas por padrão.</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Considerações sobre exibições de lista

* Não é possível exibir registros nas páginas de tipo de registro em uma exibição de lista. Você só poderá exibir os seguintes objetos em uma exibição de lista quando visualizá-los na página Registros conectados de um registro:

   * Projetos Workfront

  Para obter informações sobre como criar uma página de registros conectados, consulte [Adicionar uma página de registros conectados a um registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
* Antes de exibir uma exibição de lista em uma página de registros conectados de um registro, você deve conectar os projetos Workfront com os tipos de registro do Planning. Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
* As Exibições de lista são semelhantes às Listas aprimoradas. Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).


## Gerenciar uma exibição de lista {#manage-a-list-view}

Para obter mais informações sobre como gerenciar exibições de lista no Workfront, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

{{step1-to-planning}}

1. Clique em um cartão de espaço de trabalho e, em seguida, clique em um cartão de tipo de registro.
1. Em qualquer exibição, clique no nome de um registro para abrir a página de visualização ou detalhes do registro.
1. Adicione uma **página Registros conectados** para projetos conectados, conforme descrito no artigo [Adicionar uma página Registros conectados a um registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

   A página Registros conectados exibe projetos conectados ao registro na exibição de lista.

   <!--add new screen shot when they release Conditional formatting MVP -->

   ![Projetos na página de registros conectados na exibição de lista](assets/projects-on-connected-records-page-list-view.png)

1. (Opcional) Siga um destes procedimentos para modificar a exibição em lista:

   1. Expanda o menu suspenso de exibições no canto superior direito da lista para selecionar outro modo de exibição ou clique em **Novo modo de exibição** e crie outro.

      As visualizações são compartilhadas em todo o sistema. Se você criar uma visualização Projetos para um tipo de registro, poderá visualizá-la em outros tipos de registro que exibem projetos conectados.

   1. Passe o mouse sobre o nome de um modo de exibição existente e clique no menu **Mais** ![Mais menu](assets/more-menu.png), em seguida, clique em um dos seguintes:
      * **Renomear**, para dar um novo nome à exibição
      * **Compartilhar**, para compartilhar a exibição com outras pessoas
      * **Excluir**, para excluir o modo de exibição.

      >[!NOTE]
      >
      >* Você deve ter permissões de gerenciamento para um modo de exibição para poder editá-lo, compartilhá-lo ou excluí-lo.
      >
      >* Não é possível modificar as Exibições de sistema.
      >
      <!--For Feb 26 and add the Preview disclaimer at the top: * <span class="preview">You can reset a view that was shared with you after you modified it to restore its original preferences, or you can copy it with your changes and share the copy. For more information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>
        -->
   1. Clique no ícone **Filtro** ![Ícone Filtro](assets/filter-icon.png) para adicionar um filtro ao modo de exibição. Os resultados são filtrados imediatamente na lista. Não é possível salvar e nomear filtros. Os filtros são lembrados quando você acessa a página no futuro e fazem parte de exibições compartilhadas.
   1. Clique no ícone **Colunas** ![Ícone Colunas](assets/columns-icon.png) para selecionar quais colunas exibir ou ocultar no modo de exibição.
   1. Passe o mouse sobre o nome de uma coluna, clique na seta para baixo à esquerda do nome da coluna e clique em uma das seguintes opções:
      * **Renomear**, para adicionar um **Rótulo personalizado** para a coluna. O nome do campo original no Workfront não é alterado.
      * **Classificar**, para classificar a lista pelo campo selecionado. Um ícone de classificação que indica a direção da classificação é adicionado ao cabeçalho da coluna.
   1. Clique no ícone **+** no canto superior direito da lista para adicionar ou remover colunas à lista e clique em **Salvar**.

      O **Gerenciador de colunas** se abre.

      Você pode adicionar somente campos existentes à exibição de lista.
Não é possível remover o campo principal na exibição de lista exibida na primeira coluna.


   <!--For Feb 26: make available at release and fix the formatting - this will be broken, if not: 
    1. <span class="preview">Click the **Format cells** icon ![Format cells icon](assets/format-cells-icon.png). The **Format** box opens. (*********change the name of the box when they update it***********)</span>
        <span class="preview">Do the following: </span>
        <div class="preview">
        1. In the **If** line, click **Add condition**, then select a field you want to format by and choose a field value. 
            >[!TIP]
            >
            >Only fields visible in the list view are available for conditional formatting.
        1. (Optional) Click **Add condition** in the **If** line to add more conditions to same rule. 
            >[!TIP]
            >
            >You can add up to 10 conditions in a conditioning rule and you can have up to 20 rules for a field.
        1. Click the **Or** connector between conditions to change to **And** and to indicate that multiple conditions must be met at the same time. **Or** is the default connector.  
        1. In the **Format** line, select a field to indicate which column will be formatted. (*******edit this area, if it changes names??***********)
        1. (Optional) Click the **color circle** icon ![Color circle icon](assets/color-circle.png) next to the field selected, to expand it and choose another color.
        1. Turn on the **Apply to row** setting to apply the formatting to the entire row of the field that meets the conditions. 
        1. (Optional) Click **Add condition** in the **Format** box to add another rule for another field and the repeat the steps above. 
        1. (Optional) Click **Clear all** to remove all formatting.
        1. Click outside the **Format** box to close it. 
            This returns you to the list view. 
            The formatting is applied immediately to the list view.
            There is a blue dot next to the **Format cells** icon to indicate that the view has special formatting applied.
        </div>
    -->

1. (Opcional) Adicione uma palavra-chave na caixa de pesquisa no canto superior direito da lista para procurar um item.


   Os itens que correspondem ao termo de pesquisa são destacados na lista.
1. (Opcional) Para adicionar mais itens à lista e conectá-los automaticamente ao registro selecionado, siga um destes procedimentos:

   * Clique em **Conectar registros** no canto superior direito da lista para adicionar itens existentes.
   * Clique em **Nova linha** na parte inferior da lista para adicionar novos itens.
1. Clique no nome de um item conectado na lista para abri-lo em outra guia do navegador.
1. Clique duas vezes dentro de uma célula na lista para editar as informações de um campo, em seguida, pressione Enter para salvar suas alterações.

   Alguns campos são somente leitura. Por exemplo, o percentual concluído de um projeto é um campo calculado pelo sistema e não pode ser editado manualmente.

1. Passe o mouse sobre o nome de um item na lista, clique no menu **Mais** [Mais menu](assets/more-menu.png) e clique em **Exibir** para abrir o projeto em outra guia

   Ou

   Selecione um ou mais itens, observe a barra de ações na parte inferior da lista e clique em uma das seguintes opções:

   * **Excluir** para excluir o projeto. A exclusão de um projeto o desconecta do registro e o move para a Lixeira do Workfront. Os administradores do Workfront podem recuperar projetos excluídos até 30 dias após a exclusão.
   * **Desconectar** para desconectar o projeto do registro. Desconectar um projeto o remove e todos os valores de seus campos de pesquisa do registro atual.

   ![Barra de ações na exibição de Lista da página Registros conectados](assets/actions-bar-connected-records-page-list-view.png)

