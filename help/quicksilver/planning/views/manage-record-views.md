---
title: Gerenciar Visualizações de Registro
description: É possível exibir registros em uma exibição de tabela, linha do tempo ou calendário ao usar o Adobe Workfront Planning. Este artigo descreve como criar uma visualização e editar uma existente.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '1145'
ht-degree: 1%

---


# Gerenciar exibições de registro


<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Depois de selecionar um tipo de registro na área Adobe Workfront Planning, você pode exibir todos os registros desse tipo nas seguintes exibições:

* Tabela

  Para obter mais informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).

* Linha do tempo

  Para obter mais informações, consulte [Gerenciar a exibição da linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md).

* Calendário

  Para obter mais informações, consulte [Gerenciar a exibição de calendário](/help/quicksilver/planning/views/manage-the-calendar-view.md).

Este artigo descreve as seguintes informações sobre visualizações de registro:

* [Criar e editar um modo de exibição](#create-or-edit-record-views)
* [Habilitar os indicadores de presença em tempo real em uma exibição](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Para obter mais informações sobre o gerenciamento de exibições de registros do Workfront Planning, consulte também os seguintes artigos:

* [Excluir visualizações de registros](/help/quicksilver/planning/views/delete-record-views.md)
* [Exibições de registro duplicadas](/help/quicksilver/planning/views/duplicate-record-views.md)
* [Compartilhar exibições](/help/quicksilver/planning/access/share-views.md)


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
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
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
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## Considerações ao trabalhar com visualizações de registro

* As exibições no Workfront Planning são específicas do tipo de registro. Não é possível aplicar a mesma exibição a dois tipos de registro diferentes.
* As exibições criadas estão visíveis somente para você e os usuários com os quais você compartilha as exibições.
* Quando você modifica ou exclui uma exibição, ela é modificada e excluída para todos os usuários que têm permissões para a exibição.
* Cada usuário pode criar no máximo 100 visualizações. Você pode exibir mais de 100 visualizações para um tipo de registro, mas um usuário pode criar apenas 100 visualizações.
* Embora alguns elementos de exibição possam ser aplicados a várias exibições para o mesmo registro, eles são exclusivos para cada exibição de registro:

   * Filtro
   * Agrupamento (para as exibições de tabela e linha do tempo)
   * Aparência da barra (para as visualizações de linha do tempo e calendário)

  Por exemplo, ao criar um filtro em uma exibição de tabela, os resultados do filtro ficam visíveis somente na exibição selecionada (a exibição de tabela) e não em todas as exibições associadas ao tipo de registro.

  >[!TIP]
  >
  >Alguns elementos de visualização não estão disponíveis para todas as visualizações.


## Semelhanças e diferenças entre visualizações de registro

A tabela a seguir mostra as semelhanças e diferenças entre as exibições de tabela, linha do tempo e calendário:

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| Recurso | Exibição em tabela | Exibição da linha do tempo | Visualização de calendário |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| Exibir registros em uma lista ou tabela | ✓ |              | |
| Exibir todos os campos como colunas na tabela, por padrão | ✓ |              |    |
| Ocultar ou mostrar campos (ou colunas) | ✓ |               |    |
| Editar valores de campo para cada registro | ✓ |               |             |
| Adicionar registros como novas linhas na exibição | ✓ |               |        |
| Adicionar campos como novas colunas na exibição | ✓ |               |         |
| Copiar linhas de uma lista externa e colá-las em uma tabela | ✓ |               |          |
| Exibir registros em uma linha do tempo |            | ✓ |             |
| Filtrar registros | ✓ | ✓ | ✓ |
| Exibir registros em um calendário |           |              | ✓ |
| Registros de grupo | ✓ | ✓ |
| Classificar registros | ✓ |              |
| Registros de código de cores | ✓ | ✓ | ✓ |
| Agrupamentos de código de cores |           | ✓ |
| Pesquisar registros específicos | ✓ | ✓ |
| Compartilhar a exibição com outras pessoas | ✓ | ✓ | ✓ |
| Abrir a página do registro na exibição | ✓ | ✓ |    |
| Exibir registros por ano e trimestre |           | ✓ |    |
| Exibir registros por mês |           | ✓ | ✓ |
| Exibir registros por semana |           |               | ✓ |
| Exportar informações de uma visualização | ✓ |               |    |
| Exibir em tela inteira | ✓ | ✓ | ✓ |
| Criar registros na exibição | ✓ | ✓ | ✓ |

## Criar ou editar exibições {#create-or-edit-views}

{{step1-to-planning}}


1. Clique no cartão de um espaço de trabalho.

   O espaço de trabalho é aberto e os tipos de registro são exibidos como cartões.

1. Clique em um cartão de tipo de registro.

   A página de tipo de registro é aberta.

   Por padrão, todos os registros do tipo selecionado são exibidos na exibição de tabela.

1. Clique no ícone suspenso ![Ícone suspenso](assets/drop-down-icon.png) ao lado do nome do modo de exibição atual e clique em **+Novo modo de exibição**.

1. Selecione entre os seguintes tipos de exibições:

   * Tabela
   * Linha do tempo
   * Calendário

1. Escolha um tipo de exibição e clique em **Criar**. Uma nova visualização é adicionada ao menu suspenso.

   >[!TIP]
   >
   >Quando você cria um tipo de registro, a exibição de tabela também é criada por padrão.
   >
   >Para criar uma exibição de linha do tempo ou calendário, o tipo de registro para o qual você cria a exibição deve ter pelo menos dois campos de data.
   >
   >Caso contrário, as opções Linha do tempo e Calendário estarão esmaecidas.
   >  

   ![Criar caixa de exibição](assets/create-view-box.png)

1. (Opcional) Para editar um modo de exibição existente, clique no menu suspenso à direita do nome do modo de exibição atual, digite o nome de um modo de exibição no campo **Pesquisa** e pressione Enter no teclado.
1. (Opcional) No menu suspenso Exibir, arraste e solte as exibições na ordem de sua preferência.

   ![Exibir lista suspensa de tipos de registro](assets/view-types-drop-down-from-record-type-list.png)

1. (Condicional) Clique em **Avançar** ao criar uma exibição de linha do tempo ou calendário.

   Por padrão, o Workfront atribui à exibição um dos seguintes nomes:

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   O número é um incremento gerado automaticamente.

1. (Condicional) Selecione as **Datas de início** e **datas de término** para os registros que serão exibidos na exibição de linha do tempo ou calendário.

   >[!NOTE]
   >
   >    Você pode selecionar entre campos de data de registro ou campos de data de pesquisa a partir de tipos de objeto ou registro conectados.
   >
   >Você deve usar agregadores para campos de data (MAX ou MIN) ao selecionar campos de pesquisa ao conectar tipos de registro. Apenas a adição dos agregadores permite usar as datas das conexões como datas de Início e Término para as exibições de linha do tempo e calendário.
   >
   >Para obter informações, consulte [Tipos de registro de conexão](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Clique em **Criar**.

   A visualização é exibida como uma nova guia. As exibições são exibidas na ordem cronológica de quando foram criadas ou compartilhadas com você.
1. (Opcional) Clique no menu **Mais** ![Mais exibições de ícones de seta para baixo](assets/more-caret-down-icon-views.png) ao lado da última exibição para exibir todas as exibições do tipo de registro selecionado.

   Exibições adicionais são exibidas no menu **Mais** após a última guia de exibição. O número ao lado do menu **Mais** mostra o número de exibições adicionais.
1. (Opcional) Para renomear uma exibição depois de sua criação, clique no menu suspenso exibição e no menu **Mais** ![Mais menu](assets/more-menu.png) > **Renomear** para atualizar o nome da exibição

   Ou

   Clique duas vezes no nome da exibição e comece a digitar o novo nome.  <!--ensure there is not another saving step here?!-->

1. (Opcional) Clique no ícone **Tela cheia** ![Abrir ícone de tela cheia](assets/open-full-screen-icon.png) para abrir qualquer modo de exibição em tela cheia, em seguida no ícone **Sair da tela cheia** ![Sair do ícone de tela cheia](assets/exit-full-screen-icon.png) ou em Escape no teclado para sair da tela cheia.

1. (Opcional) Para gerenciar um tipo específico de visualização, consulte os seguintes artigos:

   * [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [Gerenciar a exibição de linha do tempo](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [Gerenciar a exibição de calendário](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## Ativar o indicador de presença em tempo real em uma exibição

Você pode ver se outros usuários estão editando registros ao mesmo tempo que você seguindo os indicadores de presença em tempo real na exibição.

Os avatares de outros usuários que estão editando informações de registro ao mesmo tempo que você exibe no canto superior direito de todas as visualizações de registro, por padrão.

Ao exibir a visualização de tabela, você também pode visualizar qual campo outro usuário está editando no momento em que você está visualizando o registro.

Para obter mais informações, consulte [Gerenciar a exibição de tabela](/help/quicksilver/planning/views/manage-the-table-view.md).



<!--## Add a view as a favorite - this is not possible yet-->
