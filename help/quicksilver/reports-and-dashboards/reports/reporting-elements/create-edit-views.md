---
product-area: reporting
navigation-topic: reporting-elements
title: Criar ou editar exibições no Adobe Workfront
description: Você pode personalizar o tipo de informações exibidas na tela usando as exibições. Você pode usar vários tipos de exibições no Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# Criar ou editar exibições no Adobe Workfront

Você pode personalizar o tipo de informações exibidas na tela usando as exibições. Você pode usar vários tipos de exibições no Adobe Workfront.

Este artigo descreve como criar e editar exibições padrão para listas e relatórios, e como criar exibições ágil. Para obter mais informações, consulte [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Editar o acesso a Relatórios, Painéis, Calendários para criar uma visualização em um relatório</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Gerenciar permissões de um relatório para criar ou editar uma visualização em um relatório</p> <p>Gerenciar permissões em uma exibição para editá-la</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar ou personalizar uma exibição

O processo para criar ou personalizar uma exibição varia dependendo de você estar criando ou personalizando uma exibição padrão ou ágil.

* [Criar ou personalizar uma exibição padrão](#create-or-customize-a-standard-view)
* [Criar ou personalizar uma visualização ágil](#create-or-customize-an-agile-view)

### Criar ou personalizar uma exibição padrão {#create-or-customize-a-standard-view}

Você pode criar uma nova visualização padrão ou personalizar uma visualização padrão existente criada anteriormente.

1. Clique no botão **Exibir** menu suspenso em qualquer lista onde você deseja criar ou personalizar uma exibição.
1. (Opcional) Para personalizar uma exibição existente, selecione a Exibição padrão que deseja personalizar.\
   As Exibições padrão estão disponíveis em qualquer tipo de lista no Workfront, como um relatório, uma lista de projetos ou uma lista de tarefas.
1. Clique no botão **Exibir** menu suspenso e, em seguida, clique em **Personalizar exibição** ou **Nova exibição**.\
   O **Personalizar exibição** será exibida.

1. No **Visualização de coluna** siga um destes procedimentos:

   * Modifique o valor de qualquer coluna clicando no título da coluna e selecionando um novo campo.
   * Adicione uma coluna clicando em **Adicionar coluna**, comece digitando o nome da coluna que deseja adicionar e clique nela quando ela for exibida na lista suspensa.
   * Ajuste a ordem de exibição das colunas arrastando o título da coluna para um novo local.

      * (Opcional) Na seção **Configurações de coluna** clique no botão **Resumir esta coluna por** selecione uma das opções disponíveis para resumir as informações. Ao escolher essa opção, as informações na coluna são agregadas nos agrupamentos do relatório.\
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
         >As seguintes exceções se aplicam a objetos pai (por exemplo, tarefas pai) quando você está agregando valores para os seguintes campos em agrupamentos:
         >   
         >   * Todos os campos de número e moeda, exceto Horas Reais (por exemplo, Custo da Mão de obra Planejada/Real, Custo da Despesa Planejada/Real, Custo Planejado/Real, Horas Planejadas) agregam apenas os valores para as tarefas filhas e tarefas independentes. Eles não agregam os valores para as tarefas pai ou pais dos pais.
         >   * As Horas reais agregam os valores do principal e das tarefas independentes; eles não agregam os números dos pais das tarefas pai ou filho.
         >   * Os campos de dados personalizados para valores numéricos e de moeda agregam todas as tarefas: pais, filhos, pais e tarefas independentes.


         Para obter mais informações sobre o uso de agrupamentos em um relatório, consulte o artigo [Visão geral dos agrupamentos no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

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
           <td>Selecione o formato no qual deseja que os valores sejam exibidos para os campos na coluna .</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostrar esta coluna quando estiver em um Painel</strong></td> 
           <td><p>Selecione essa opção para mostrar essa coluna em um painel, quando o relatório for exibido lado a lado com outro relatório. Quando essa opção não está selecionada, essa coluna não é exibida ao exibir o relatório em um painel em que os relatórios são exibidos lado a lado.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Regras de colunas</strong></td> 
           <td><p>Clique em <strong>Adicionar uma regra para esta coluna</strong> para definir uma regra para a coluna. Após adicionar uma regra, é possível definir estilos de campo e texto para a forma como os campos que correspondem a essa regra são exibidos. Clique em <strong>Adicionar regra</strong> depois que terminar de definir a regra.</p></td> 
          </tr> 
         </tbody> 
        </table>

         Para obter mais informações sobre a formatação condicional de exibições em relatórios, consulte o artigo [Usar formatação condicional no Modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).



1. (Condicional) Se você clicou **Opções avançadas**, clique em **Concluído**.

1. Clique em **Salvar exibição** para criar uma nova exibição ou substituir a exibição atual por suas alterações.\
   Ou\
   Clique em **Salvar como nova exibição** para salvar as alterações como uma nova visualização.

   >[!TIP]
   >
   >O **Salvar como nova exibição** é a única opção disponível ao personalizar uma visualização integrada do Workfront.

   Seu acesso determina como a exibição é salva. Se você criou a exibição originalmente, é possível salvar as alterações; caso contrário, você será solicitado a salvar uma versão. Lembre-se de que as alterações feitas na exibição afetam os usuários com os quais a exibição foi compartilhada.

### Criar ou personalizar uma visualização ágil {#create-or-customize-an-agile-view}

Você pode criar uma nova visualização ágil ou personalizar uma visualização ágil existente criada anteriormente.

>[!IMPORTANT]
>
>As exibições ágil estão disponíveis somente ao visualizar um projeto.

Para obter mais informações sobre visualizações do Ágil, consulte o artigo [Gerenciar um projeto na Visualização ágil](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

Para criar ou personalizar uma visualização ágil:

1. Vá para a lista de tarefas em um projeto.
1. Clique no botão **Agile Storyboard** ícone ![](assets/agile-storyboard-nwe.png).

1. (Condicional) Para personalizar uma visualização ágil existente:

   1. Clique no botão **Exibir** selecione a exibição ágil que deseja personalizar.\
      Não é possível personalizar a visualização ágil padrão.

   1. Clique no botão **Exibir** menu suspenso novamente e clique em **Personalizar exibição**.\
      ![](assets/view-agile-customize.png)

1. (Condicional) Para criar uma nova exibição ágil, clique em **Nova exibição**.\
   O **Personalizar exibição ágil** será exibida.

1. No **Personalizar exibição ágil** , especifique um nome para a exibição ágil.\
   Recomendamos incluir a palavra &quot;Ágil&quot; no nome da exibição, para que os usuários saibam que é uma exibição ágil.\
   Esse nome é exibido no **Exibir** ao selecionar uma exibição.

1. Defina as colunas de status a serem exibidas no quadro de matérias na exibição ágil. Esses são os status da tarefa definidos pelo administrador do Workfront, conforme descrito em [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Somente os status do sistema estão disponíveis para uso na placa Histórias do ágil. Se um status estiver disponível somente para um grupo individual do qual você é membro, o status não estará disponível no quadro de história ágil. Além disso, as tarefas que estão em um status que está disponível somente para um grupo personalizado não ficam visíveis ao visualizar o projeto em uma visualização ágil.

   Os usuários podem mover histórias entre essas colunas de status no quadro de histórias em ágil.\
   Ao definir colunas de status, você pode fazer o seguinte:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reordenar colunas de status:</strong> </td> 
      <td> Arraste uma coluna de status para a ordem em que deseja exibi-la.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Remover colunas de status:</strong> </td> 
      <td>Clique no ícone (x) na coluna que deseja remover.<br>Não é possível remover o status "Novo" a menos que um status personalizado tenha sido adicionado à exibição e que o status personalizado seja igual a "Novo".<br>Para obter informações sobre como criar um status personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Adicionar colunas de status:</strong> </td> 
      <td> <p>Clique no botão <strong>Plus</strong> e selecione o status que deseja adicionar.<br>Todos os status padrão do sistema são exibidos, bem como todos os status personalizados que foram compartilhados com você.<br>Você pode configurar até 10 status para exibição.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. No **Associar cor do cartão a** selecione uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>História:</strong> </td> 
      <td>Todas as subtarefas correspondem à cor da tarefa pai, de modo que as cores de todas as histórias em uma determinada faixa sejam as mesmas.<br>As cores são atribuídas aleatoriamente a tarefas quando elas são criadas se a tarefa não tiver subtarefas ou não tiver uma tarefa pai.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Forma livre:</strong> </td> 
      <td> Todos os cartões são exibidos como azul por padrão até que o usuário altere a cor manualmente, conforme descrito no artigo <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorize as histórias por cor no quadro Soma</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridade:</strong> </td> 
      <td> <p> As cores estão associadas à prioridade da história, da seguinte maneira:</p> 
       <ul> 
        <li>Alto = Vermelho</li> 
        <li>Médio = Amarelo</li> 
        <li>Baixo = Verde<br>Se o administrador do Workfront tiver configurado prioridades personalizadas para seu sistema Workfront, a prioridade mais alta será vermelha, a segunda mais alta será amarela e as restantes serão verdes.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Proprietário da tarefa:</strong> </td> 
      <td> Todas as histórias com o mesmo destinatário principal têm a mesma cor.<br>O destinatário principal é o usuário que foi atribuído pela primeira vez à tarefa. </td> 
     </tr> 
    </tbody> 
   </table>

1. No **Ágil** na seção **Campos adicionais** , clique em **Adicionar campo** e, em seguida, selecione o campo que deseja adicionar aos cartões de história. (Esses são os mesmos campos que você pode adicionar ao criar personalização de uma exibição ou criação de colunas para um relatório.)\
   Repita esse processo para adicionar até três campos adicionais aos cartões de história.\
   Ao adicionar campos a cartões de história, os campos são somente visualização e são exibidos somente quando o campo é preenchido.

   Por padrão, os seguintes tipos de dados são exibidos no cartão de história:

   * Nome da história com um link diretamente para a tarefa
   * O nome do projeto com um link diretamente para o projeto\
      Esse link é exibido somente ao usar a visualização ágil em uma iteração; não é exibido ao usar uma visualização ágil em um projeto.
   * A descrição da tarefa
   * Compromisso atual
   * Exibir e editar a porcentagem concluída ajustando a porcentagem concluída ou ajustando o número de pontos ou horas concluídas
   * Usuários atribuídos

   Você pode exibir dados adicionais (incluindo dados personalizados) em cartões de história. Talvez você queira exibir campos adicionais em cartões de história por qualquer motivo. Por exemplo, talvez você queira exibir a ID do cliente se estiver trabalhando em histórias para vários clientes dentro do projeto ou quiser exibir a Data de início da tarefa.

1. Clique em **Salvar**.\
   Seu acesso determina como a exibição é salva. Se você criou a exibição originalmente, é possível salvar as alterações; caso contrário, você será solicitado a salvar uma versão. Lembre-se de que as alterações feitas na exibição afetam os usuários com os quais a exibição foi compartilhada.

1. (Opcional) Clique no botão **Exibição de lista** ícone ![](assets/list-view-in-agile-view-for-tasks.png) para retornar à lista de tarefas.
