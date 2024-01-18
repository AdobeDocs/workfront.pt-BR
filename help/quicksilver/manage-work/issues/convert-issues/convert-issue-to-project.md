---
product-area: projects
navigation-topic: convert-issues
title: Converter um problema em um projeto no Adobe Workfront
description: Converter um problema em um projeto no Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '1476'
ht-degree: 0%

---

# Converter um problema em um projeto no Adobe Workfront

Se for necessário trabalhar mais para concluir um problema depois que ele for enviado, você pode converter o problema em um projeto.

Você pode converter um problema em um novo projeto ou convertê-lo em um projeto usando um modelo. Este artigo descreve ambas as maneiras de converter problemas em projetos.

>[!IMPORTANT]
>
>Para obter informações gerais sobre como converter problemas, recomendamos que você também leia o artigo [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Ao criar um projeto a partir de um problema, alguns dos campos no projeto são preenchidos a partir de outros objetos. Para obter mais informações, consulte a seção &quot;Configurações padrão do novo projeto&quot; no artigo [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Problemas, Tarefas e Projetos</p> <p>Editar acesso a Dados Financeiros para atualizar informações financeiras de uma projeção convertida a partir da ocorrência</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o problema</p> <p>Você obtém permissões de Gerenciamento para o projeto após a conversão do problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o administrador do Workfront.

## Converter um problema em um projeto

Você pode converter um problema em um projeto em branco ou converter um problema em um projeto usando um modelo.

1. Vá para um projeto e clique em **[!UICONTROL Problemas]** no painel esquerdo.
1. Na lista de problemas que são exibidas, siga um destes procedimentos:

   * Para converter um problema em um projeto em branco, clique no nome do problema, clique no **[!UICONTROL Mais]** menu ![](assets/more-icon.png) à direita do nome do problema, clique em **[!UICONTROL Converter em um projeto em branco]**.


     Ou

     Selecione o problema na lista de problemas, clique na guia **[!UICONTROL Mais]** menu ![](assets/more-icon.png) na parte superior da lista, em seguida, clique em **[!UICONTROL Converter em um projeto em branco]**.

     >[!IMPORTANT]
     >
     >A opção Converter em um projeto em branco é exibida somente quando o administrador do sistema ou do grupo habilita a [!UICONTROL Permitir que os usuários criem projetos sem usar um modelo] preferência na variável [!UICONTROL Configuração] área. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Você deve adicionar tarefas manualmente ao projeto ou anexar um modelo ao projeto depois de converter o problema.

     Continue com a Etapa 3e abaixo.

     <!--
     Is this accurate?
     -->

     >[!TIP]
     >   
     >* Se o problema tiver sido criado usando uma fila de solicitações, o novo projeto herdará o grupo da fila de solicitações.
     >* Se o problema tiver sido criado adicionando-o à seção Problemas do projeto, o novo projeto herdará o Grupo do projeto do problema.

   * Para converter um problema em um projeto usando um modelo, siga um destes procedimentos:

      * Clique no nome de um problema e, em seguida, clique no link [!UICONTROL **Mais**] menu ![](assets/more-icon.png) à direita do nome do problema

        Ou

      * Selecione o problema na lista de problemas, em um relatório ou painel, clique no **Mais** menu ![](assets/more-icon.png) na parte superior da lista, em seguida, clique em **Converter para projeto a partir de Modelo** e comece digitando o nome de um modelo na variável **Modelo de pesquisa** e clique no nome do template quando ele for exibido na lista. Continue com a Etapa 3.

        <!--      
        (is this accurate?)      
        -->

     >[!TIP]
     >
     >Se você tiver adicionado modelos à sua lista Favoritos, poderá passar o mouse sobre a [!UICONTROL **Modelos favoritos**] e clique no template que deseja usar.

     A caixa Novo projeto a partir do modelo é exibida.

     ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

     >[!TIP]
     >
     >Se o problema estiver associado a um processo de aprovação ou já estiver associado a um objeto de resolução, o Workfront exibirá um aviso na parte superior da caixa Converter em projeto para notificar que a aprovação será removida ou o objeto de resolução será substituído durante a conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Condicional) Se você selecionou converter o problema em um projeto usando um modelo, continue com as seguintes etapas:

   1. Revise os detalhes do modelo à direita.

      Os detalhes do template incluem o seguinte:

      * Duração do modelo
      * Proprietário do modelo
      * O número de tarefas de nível superior que inclui os nomes das três principais tarefas
      * O número de todas as tarefas no modelo
      * Os nomes dos formulários personalizados do modelo

   1. (Opcional) Passe o mouse sobre o nome de um modelo e clique no ícone Favoritos ![](assets/favorites-icon-small.png) para marcá-la como favorita para uso futuro.

      >[!TIP]
      >
      >É possível marcar até 40 itens do Workfront como favoritos. Isso inclui modelos e outros itens.

   1. Clique em [!UICONTROL **Usar modelo**] para selecionar um modelo.

      A variável [!UICONTROL Converter em Projeto] é aberta.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Se um campo já estiver preenchido no modelo, ele será preenchido previamente na variável [!UICONTROL Converter em projeto] caixa. É possível editar os valores pré-preenchidos para melhor corresponder ao seu projeto. Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* O administrador do sistema ou do grupo pode adicionar ou remover campos no [!UICONTROL Caixa Converter em projeto] atualizando as informações de Detalhes do projeto em seu [!UICONTROL Modelo de layout].
      >
      >* Para atualizar campos na variável [!UICONTROL Finanças] na seção [!UICONTROL Converter em Projeto] caixa que você deve ter [!UICONTROL Editar] acesso a [!UICONTROL Dados financeiros] no seu nível de acesso. Se você tiver [!UICONTROL Exibir] acesso a [!UICONTROL Dados financeiros] no seu nível de acesso, todas as informações financeiras do modelo são transferidas para o novo projeto e você não pode editá-las enquanto converte o problema. Para obter informações, consulte [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

   1. (Opcional e condicional) Clique em [!UICONTROL **Opções**] no painel esquerdo, selecione uma das opções disponíveis:

      * [!UICONTROL **Conservar o problema original e vincular a sua resolução a este projeto**]

        Quando desmarcado, o problema original é excluído.

        >[!NOTE]
        >
        >Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema como estão convertendo-o, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:
        >
        >* [Conceder acesso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
        > 
        >* [Compartilhar um problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

      * [!UICONTROL **Permitir que (nome de usuário) tenha acesso a este projeto**]

        Se essa opção não estiver selecionada, as [!UICONTROL Contato Primário] não tem acesso à nova tarefa.

        >[!NOTE]
        >
        >As opções disponíveis aqui dependem de como o administrador do Workfront as configurou para todos no sistema ou para o seu grupo. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
        >
        >
        >Ou, se os grupos de nível superior em sua organização os configuraram separadamente, as opções disponíveis aqui dependem do grupo que você selecionou para o novo projeto na etapa 6. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Clique em [!UICONTROL **Forms personalizado**] e execute um dos procedimentos a seguir:

      * Revise os formulários personalizados anexados ao modelo. Eles serão transferidos para o novo projeto.
      * Verifique se todos os campos obrigatórios têm informações válidas.
      * Reorganizar os formulários personalizados arrastando-os ![](assets/drag-object-icon.png) onde você os quiser.
      * Clique em **x** ícone à direita de qualquer formulário que você não deseja transferir para o projeto.
      * Se necessário, transfira as informações de formulário personalizadas do problema para o projeto.

        >[!TIP]
        >
        >* Se um formulário personalizado de vários objetos anexado ao problema for configurado para uso com problemas e projetos, todas as informações salvas no formulário serão mantidas quando você fizer a conversão, se os campos existirem tanto no problema quanto nos formulários personalizados do projeto.
        >* Se um formulário personalizado de vários objetos com um campo calculado for anexado ao problema, bem como ao projeto, o problema e o projeto devem ser compatíveis com todos os campos referenciados nos campos personalizados calculados do formulário. Se houver uma incompatibilidade, uma mensagem o alertará para fazer ajustes. Para obter mais informações, consulte a seção &quot;Campos personalizados calculados em formulários personalizados de vários objetos&quot; na [Adicionar dados calculados a um formulário personalizado com o construtor de formulários herdado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).
        >* Se você estiver usando um modelo para a conversão e um formulário personalizado anexado ao modelo contiver um campo personalizado também encontrado em um formulário personalizado anexado ao problema, o valor do campo do problema será usado para o novo projeto. No entanto, se o campo personalizado estiver em branco no problema, o valor do template será usado.

   1. Clique em [!UICONTROL **Converter em projeto**].

      >[!TIP]
      >
      >Se você decidiu excluir o problema original, ele agora é um projeto.
      >   
      >Ou
      >  
      >Se você decidiu manter o problema original, ele agora está vinculado ao novo projeto e será concluído quando o projeto for concluído.
      >
      >Alguns campos de problema são transferidos para o projeto. A maioria dos campos definidos no modelo é transferida automaticamente para o projeto recém-criado se você não os alterou nas etapas anteriores. Para obter informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Opcional) Defina outros detalhes &#x200B; projeto (proprietário do projeto, datas do projeto) e tarefas, conforme necessário.
1. Clique em [!UICONTROL **Converter em projeto**].

   O problema foi convertido em um projeto.

1. Clique em [!UICONTROL **Ir para projeto**] dentro do [!UICONTROL Sucesso] no canto superior direito da página. Isso abre a página do projeto.
