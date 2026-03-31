---
title: Gerenciar a Exibição de Lista no Adobe Workfront Planning
description: Você pode exibir objetos e seus campos em uma exibição de lista, ao acessá-los na página Registros conectados de um registro, no Adobe Workfront Planning. Este artigo descreve como criar ou editar uma exibição de lista na página Registros conectados de um registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1c7e6973-6e9e-4c93-9d3b-89ed90df9d14
source-git-commit: ddf10844646a79c43accaffa1789caf24290cc8a
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 0%

---


# Gerenciar a exibição de lista no Adobe Workfront Planning

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode exibir objetos na exibição de lista nas seguintes áreas do Workfront Planning:

* Uma página de registros conectada para projetos na área de detalhes de um registro

  ![Projetos na página de registros conectados na exibição de lista](assets/projects-on-connected-records-page-list-view.png)

* Uma lista de formulários de solicitação no nível do tipo de registro

  ![Solicitar formulários na exibição de lista](assets/request-forms-in-list-view.png)

Este artigo descreve como navegar, criar ou editar uma exibição de lista que exibe objetos no Workfront Planning. <!--change 'projects' to other objects when they become available and the location of the list view-->

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

* Considere o seguinte para a exibição da lista de páginas de registros conectados:

   * Você só pode exibir projetos na exibição de lista na página de registros conectados de um registro. A exibição de lista não está disponível para nenhum outro objeto ou tipo de registro em uma página de registros conectada.

  Para obter informações sobre como criar uma página de registros conectados, consulte [Adicionar uma página de registros conectados a um registro](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).
   * Antes de exibir uma exibição de lista em uma página de registros conectados de um registro, você deve conectar os projetos Workfront com os tipos de registro do Planning. Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).
   * É possível criar várias exibições de lista para projetos na página de registros conectados de um registro.

* Considere o seguinte para a exibição de lista dos formulários de solicitação:

   * Não é possível criar ou editar exibições de lista adicionais para formulários de solicitação do Planning. O Workfront cria uma exibição de lista para formulários de solicitação. <!--this will change-->

     Para obter informações sobre formulários de solicitação, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
* Dependendo de onde for exibida, nem todas as exibições de lista têm os mesmos elementos descritos neste artigo.


## Gerenciar uma exibição de lista {#manage-a-list-view}

As exibições de lista são semelhantes às listas aprimoradas. A maioria dos elementos das exibições aprimoradas também existe nas exibições de lista no Workfront Planning.

Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

<!--
{{step1-to-planning}}

1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card. 
    1. From any view, click the name of a record to open the record's preview or details page. 
    1. Add a **Connected records page** for connected projects as described in the article [Add a Connected records page to a record](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md).

    The Connected records page displays projects connected to the record in the list view. 

    ![Projects on connected records page in list view](assets/projects-on-connected-records-page-list-view.png)

1. (Conditional) To access a list of request forms, do the following: 

    1. {{step1-to-planning}}

    1. (Conditional) To access a projects connected page, do the following: 

    1. Click a workspace card, then click a record type card.
    1. Click the **More** menu ![More menu](assets/more-menu.png) to the right of the record name in the header, then click **Manage request forms**.

        A list of request forms displays.

-->

1. Vá para uma exibição de lista em uma das seguintes áreas:

   * Página de registros conectados na área de detalhes de um registro
   * A página Formulários de solicitação de um registro

1. (Condicional) Quando disponível, execute um dos procedimentos a seguir para modificar a exibição de lista:

   1. Expanda o menu suspenso de modos de exibição no canto superior esquerdo da lista para selecionar outro modo de exibição ou clique em **Novo modo de exibição** e crie outro.

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
      >* <span class="preview">Você pode redefinir um modo de exibição compartilhado com você para o qual tem permissão apenas para Exibir, depois de modificá-lo para restaurar suas preferências originais, ou pode copiá-lo com suas alterações e compartilhar a cópia. Para obter mais informações, consulte [Usar listas aprimoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). </span>

      <!--
        And hide everything else below for these elements, after moving it to the Use enhanced lists article: 
        1. <span class="preview">To update one of the following view elements, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md):</span>
            <div class="preview">
            * Filter
            * Columns
            * Format cells
            * Row height
            </div>
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

   1. <span class="preview">Clique no ícone **Formatar células** ![Ícone Formatar células](assets/format-cells-icon.png). A caixa **Formato** é aberta.</span> <!--change the name of the box when they update it-->
      <span class="preview">Faça o seguinte: </span>

      1. Clique em **Adicionar condição**.
      1. <span class="preview">Na linha **If**, selecione um campo, escolha um valor de campo e adicione um modificador. Os modificadores mudam, dependendo do tipo de campo escolhido. </span>

         >[!TIP]
         >
         ><span class="preview">Somente os campos visíveis na exibição de lista estão disponíveis para formatação condicional.</span>

      1. <span class="preview">(Opcional) Em vez de adicionar um valor de campo, clique no ícone **Comparar com outro campo** ![Comparar com outro campo](assets/compare-to-another-field-icon.png) e escolha um campo cujo valor você deseja comparar ao valor do campo selecionado. Por exemplo, você pode filtrar por projetos cujo Proprietário do projeto corresponde ao Patrocinador do projeto. </span>

         >[!TIP]
         >
         ><span class="preview">Somente os campos visíveis na exibição de lista estão disponíveis para formatação condicional.</span>

      1. <span class="preview">(Opcional) Clique em **Adicionar condição** na linha **If** para adicionar mais condições à mesma regra.</span>

         >[!TIP]
         >
         ><span class="preview">Você pode adicionar até 10 condições em uma regra de condição e pode ter até 20 regras para um campo.</span>

      <div class="preview">

      1. Clique no conector **Or** entre as condições para alterar para **And** e indicar que várias condições devem ser atendidas ao mesmo tempo. **Or** é o conector padrão.
      1. Na linha **Formatar**, selecione um campo para indicar qual coluna será formatada. <!--edit this area, if it changes names??-->
      1. (Opcional) Clique no **ícone do círculo de cores** ![ícone do círculo de cores](assets/color-circle.png) ao lado do campo selecionado, para expandi-lo e escolher outra cor <!--for a cell or the text of the cell that matches your criteria-->. <!--is this where the bold, italic is? I had no UI for this when I wrote it-->
      1. Ative a configuração **Aplicar à linha** para aplicar a formatação à linha inteira do campo que atende às condições.
      1. (Opcional) Clique em **Adicionar condição** na caixa **Formatar** para adicionar outra regra a outro campo e repetir as etapas acima.
      1. (Opcional) Clique em **Limpar tudo** para remover toda a formatação.
      1. Clique fora da caixa **Formatar** para fechá-la.

         Isso retornará à exibição em lista.
A formatação é aplicada imediatamente à exibição de lista.
Há um ponto azul ao lado do ícone **Formatar células** para indicar que a exibição tem formatação especial aplicada.

      </div>

   <!--leave these here-->

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

   Selecione um ou mais itens, observe a barra de ações na parte inferior da lista e clique em uma das opções a seguir, quando disponível:

   * **Excluir** para excluir o item. A exclusão de um projeto o desconecta do registro e o move para a Lixeira do Workfront. Os administradores do Workfront podem recuperar projetos excluídos até 30 dias após a exclusão. A exclusão de um formulário não exclui as solicitações ou os registros criados quando o formulário foi enviado.
   * **Desconectar** para desconectar o projeto do registro. Desconectar um projeto o remove e todos os valores de seus campos de pesquisa do registro atual.

   ![Barra de ações na exibição de Lista da página Registros conectados](assets/actions-bar-connected-records-page-list-view.png)

