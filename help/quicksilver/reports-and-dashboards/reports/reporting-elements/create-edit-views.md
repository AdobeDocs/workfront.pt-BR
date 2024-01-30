---
product-area: reporting
navigation-topic: reporting-elements
title: Criar ou editar exibições no Adobe Workfront
description: Você pode personalizar o tipo de informação exibida na tela usando visualizações. Você pode usar vários tipos de visualizações no Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: dda00a43c5122a233ce2849d828d2e5e4555d2d9
workflow-type: tm+mt
source-wordcount: '1777'
ht-degree: 1%

---

# Criar ou editar exibições no Adobe Workfront

Você pode personalizar o tipo de informação exibida na tela usando visualizações. Você pode usar vários tipos de visualizações no Adobe Workfront.

Este artigo descreve como criar e editar exibições padrão para listas e relatórios, e como criar exibições Agile. Para obter mais informações, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p> <p>Editar acesso a Relatórios, Painéis, Calendários para criar uma visualização em um relatório</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões para um relatório para criar ou editar uma visualização em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Criar ou personalizar um modo de exibição

O processo para criar ou personalizar uma view difere dependendo se você está criando ou personalizando uma view padrão ou uma view ágil.

* [Criar ou personalizar um modo de exibição padrão](#create-or-customize-a-standard-view)
* [Criar ou personalizar uma visualização Agile](#create-or-customize-an-agile-view)

### Criar ou personalizar um modo de exibição padrão {#create-or-customize-a-standard-view}

Você pode criar uma nova view-padrão ou personalizar uma view-padrão existente criada anteriormente.

1. Clique em **Exibir** menu suspenso em qualquer lista em que você deseja criar ou personalizar uma visualização.
1. (Opcional) Para personalizar uma exibição existente, selecione a exibição padrão que deseja personalizar.\
   As Exibições padrão estão disponíveis em qualquer tipo de lista no Workfront, como um relatório, lista de projetos ou lista de tarefas.
1. Clique em **Exibir** e, em seguida, clique em **Personalizar visualização** ou **Nova visualização**.\
   A variável **Personalizar visualização** é exibida.

1. No **Visualização da coluna** execute um dos procedimentos a seguir:

   * Modifique o valor de qualquer coluna clicando no título da coluna e selecionando um novo campo.
   * Adicionar uma coluna clicando em **Adicionar coluna**, comece digitando o nome da coluna que deseja adicionar e, em seguida, clique nela quando ela aparecer na lista suspensa.
   * Ajuste a ordem em que as colunas aparecem arrastando o título da coluna para um novo local.

      * (Opcional) Na **Configurações de coluna** clique na guia **Resumir esta coluna por** e, em seguida, selecione uma das opções disponíveis para resumir as informações. Quando você escolhe essa opção, as informações em sua coluna são agregadas nos agrupamentos do relatório.\
        Para campos de data, é possível resumir os valores pelas seguintes opções:

         * Máximo
         * Mínimo

        Para campos de número e moeda, é possível resumir os valores pelas seguintes opções:

         * Contagem
         * Sum
         * Média
         * Máximo
         * Mínimo

        >[!NOTE]
        >
        >As exceções a seguir se aplicam a objetos pai (por exemplo, tarefas pai) quando você está agregando valores para os seguintes campos em agrupamentos:
        >   
        >   * Todos os campos de número e moeda, exceto Horas Reais (por exemplo, Custo de Trabalho Planejado/Efetivo, Custo de Despesas Planejado/Efetivo, Custo Planejado/Efetivo, Horas Planejadas) agregam apenas os valores das tarefas filhas e tarefas independentes. Eles não agregam os valores das tarefas pai ou pai dos pais.
        >   * As Horas Reais agregam os valores das tarefas pai principal e independente; elas não agregam os números para as tarefas pai ou filho.
        >   * Os campos de dados personalizados para valores de número e moeda agregam todas as tarefas: pais, filhos, pais dos pais e tarefas independentes.
        >   
        >

        Para obter mais informações sobre o uso de agrupamentos em um relatório, consulte o artigo [Visão geral de agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Opcional) Clique em **Opções avançadas** para especificar as seguintes informações para a coluna:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Personalizar rótulo da coluna</strong></td> 
           <td><p>Especifique um rótulo personalizado para a coluna. Esse rótulo substitui o rótulo padrão.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Formato do campo</strong></td> 
           <td>Selecione o formato no qual deseja que os valores sejam exibidos para os campos na coluna.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostrar esta coluna quando estiver em um Painel</strong></td> 
           <td><p>Selecione essa opção para mostrar essa coluna em um painel, quando o relatório for exibido lado a lado com outro relatório. Quando essa opção não está selecionada, essa coluna não é exibida ao visualizar o relatório em um painel em que os relatórios são exibidos lado a lado.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Regras de colunas</strong></td> 
           <td><p>Clique em <strong>Adicionar uma Regra para esta Coluna</strong> para definir uma regra para a coluna. Após adicionar uma regra, é possível definir estilos de campo e texto para a forma como os campos que correspondem a essa regra são exibidos. Clique em <strong>Adicionar regra</strong> após concluir a definição da regra.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Para obter mais informações sobre a formatação condicional de exibições nos relatórios, consulte o artigo [Usar formatação condicional no Modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Condicional) Se você clicou em **Opções avançadas**, clique em **Concluído**.

1. Clique em **Salvar visualização** para criar um novo modo de exibição ou substituir o modo de exibição atual por suas alterações.\
   Ou\
   Clique em **Salvar como nova visualização** para salvar as alterações como uma nova visualização.

   >[!TIP]
   >
   >A variável **Salvar como nova visualização** O é a única opção disponível ao personalizar uma visualização integrada do Workfront.

   Seu acesso determina como a visualização é salva. Se você criou a visualização originalmente, é possível salvar as alterações; caso contrário, será solicitado que você salve uma versão. Lembre-se de que as alterações feitas na exibição afetam os usuários com os quais a exibição foi compartilhada.

### Criar ou personalizar uma visualização Agile {#create-or-customize-an-agile-view}

É possível criar uma visualização Agile ou personalizar uma visualização Agile existente criada anteriormente.

>[!IMPORTANT]
>
>As visualizações Agile estão disponíveis somente ao visualizar um projeto.

Para obter mais informações sobre visualizações Agile, consulte o artigo [Gerenciar um projeto na visualização Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
>Esse procedimento se aplica somente à visualização Agile herdada, não à visualização de quadro de um projeto.

Para criar ou personalizar uma visualização Agile:

1. Vá para a lista de tarefas em um projeto.
1. Clique em **Quadro** ícone ![Ícone do painel](assets/board-icon-for-agile-view.png)e clique em **Usar ágil legado** na exibição do quadro.

1. (Condicional) Para personalizar uma exibição Agile existente:

   1. Clique em **Exibir** e selecione a visualização Agile que deseja personalizar.\
      Não é possível personalizar a visualização Agile padrão.

   1. Clique em **Exibir** menu suspenso novamente e clique em **Personalizar visualização**.\
      ![](assets/view-agile-customize.png)

1. (Condicional) Para criar uma nova exibição Agile, clique em **Nova visualização**.\
   A variável **Personalizar visualização Agile** é exibida.

1. No **Personalizar visualização Agile** especifique um nome para a exibição Agile.\
   Recomendamos que você inclua a palavra &quot;Agile&quot; no nome da visualização para que os usuários saibam que esta é uma visualização Agile.\
   Esse nome é exibido no campo **Exibir** menu suspenso ao selecionar uma exibição.

1. Defina as colunas de status a serem exibidas no storyboard na exibição ágil. Esses são os status de tarefa definidos pelo administrador do Workfront, conforme descrito em [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Somente os status do sistema estão disponíveis para uso no storyboard Agile. Se um status estiver disponível somente para um grupo individual do qual você é membro, o status não estará disponível no storyboard do Agile. Além disso, as tarefas com um status que está disponível somente para um grupo personalizado não ficam visíveis ao visualizar o projeto em uma visualização Agile.

   Os usuários podem mover matérias entre essas colunas de status no storyboard Agile.\
   Ao definir colunas de status, você pode fazer o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reordenar colunas de status:</strong> </td> 
      <td> Arraste uma coluna de status para a ordem em que você deseja que ela apareça.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remover colunas de status:</strong> </td> 
      <td>Clique no ícone (x) na coluna que deseja remover.<br>Não é possível remover o status "Novo", a menos que um status personalizado tenha sido adicionado à exibição e que o status personalizado seja igual a "Novo".<br>Para obter informações sobre como criar um status personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Adicionar colunas de status:</strong> </td> 
      <td> <p>Clique em <strong>Plus</strong> e selecione o status que deseja adicionar.<br>Todos os status padrão do sistema são exibidos, bem como todos os status personalizados que foram compartilhados com você.<br>Você pode configurar até 10 status para serem exibidos.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. No **Associar cor do cartão a** selecione entre as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>História:</strong> </td> 
      <td>Qualquer subtarefa corresponde à cor da tarefa pai, de modo que as cores de todas as histórias em qualquer raia sejam as mesmas.<br>As cores são atribuídas aleatoriamente às tarefas quando são criadas se a tarefa não tiver subtarefas ou não tiver uma tarefa pai.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Forma livre:</strong> </td> 
      <td> Todos os cartões são exibidos em azul por padrão até que um usuário altere a cor manualmente, conforme descrito no artigo <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorizar histórias por cor no quadro Scrum</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridade:</strong> </td> 
      <td> <p> As cores são associadas à prioridade da matéria, da seguinte maneira:</p> 
       <ul> 
        <li>Alto = Vermelho</li> 
        <li>Médio = Amarelo</li> 
        <li>Baixo = Verde<br>Se o administrador do Workfront tiver configurado prioridades personalizadas para o seu sistema Workfront, a prioridade mais alta será vermelha, a segunda mais alta será amarela e a restante será verde.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Proprietário da tarefa:</strong> </td> 
      <td> Todas as matérias com o mesmo destinatário primário têm a mesma cor.<br>O principal responsável é o usuário que foi atribuído pela primeira vez à tarefa. </td> 
     </tr> 
    </tbody> 
   </table>

1. No **Agile** seção, no campo **Campos Adicionais** clique em **Adicionar campo**, em seguida, selecione o campo que deseja adicionar aos cartões de história. (Esses são os mesmos campos que você pode adicionar ao criar ou personalizar uma visualização ou criar colunas para um relatório.)\
   Repita esse processo para adicionar até três campos adicionais aos cartões de história.\
   Ao adicionar campos a cartões de matéria, os campos são somente visualização e são exibidos somente quando o campo é preenchido.

   Por padrão, os seguintes tipos de dados são exibidos no cartão de história:

   * Nome da história com um link diretamente para a tarefa
   * O nome do projeto com um link direto para o projeto\
     Esse link é exibido somente ao usar a visualização Agile em uma iteração; ele não é exibido ao usar uma visualização Agile em um projeto.
   * A descrição da tarefa
   * Compromisso atual
   * Exiba e edite o percentual concluído ajustando o próprio percentual concluído ou ajustando o número de pontos ou horas concluídos
   * Usuários atribuídos

   É possível exibir dados adicionais (incluindo dados personalizados) em cartões de história. Talvez você queira exibir campos adicionais em cartões de história por vários motivos. Por exemplo, você pode exibir a ID do cliente se estiver trabalhando em histórias para vários clientes dentro do projeto, ou exibir a Data de início da tarefa.

1. Clique em **Salvar**.\
   Seu acesso determina como a visualização é salva. Se você criou a visualização originalmente, é possível salvar as alterações; caso contrário, será solicitado que você salve uma versão. Lembre-se de que as alterações feitas na exibição afetam os usuários com os quais a exibição foi compartilhada.

1. (Opcional) Clique no link **Lista** ícone para retornar à lista de tarefas.
