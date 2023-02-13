---
product-area: projects
navigation-topic: convert-issues
title: Converter um problema em um projeto no Adobe Workfront
description: Converter um problema em um projeto no Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '1340'
ht-degree: 0%

---

# Converter um problema em um projeto no Adobe Workfront

Se precisar de mais trabalho para concluir um problema após o envio, é possível converter o problema em um projeto.

É possível converter um problema em um novo projeto ou convertê-lo em um projeto usando um modelo. Este artigo descreve ambas as maneiras de converter problemas em projetos.

Para obter informações gerais sobre conversão de problemas, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a ocorrências, tarefas e projetos</p> <p>Edite o acesso a Dados Financeiros para atualizar informações financeiras de uma conversão projetada do problema</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o problema</p> <p>Você obtém permissões de gerenciamento para o projeto após a conversão do problema</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Converter um problema em um projeto

É possível converter um problema em um projeto em branco ou converter um problema em um projeto usando um modelo.

1. Vá para um projeto e clique em **[!UICONTROL Problemas]** no painel esquerdo.
1. Na lista de problemas exibidos, execute um dos seguintes procedimentos:

   * Para converter um problema em um projeto em branco, clique no nome do problema e clique no botão **[!UICONTROL Mais]** menu ![](assets/more-icon.png) à direita do nome da ocorrência e clique em **[!UICONTROL Converter em um projeto em branco]**.


      Ou

      Selecione o problema na lista de problemas, clique no botão **[!UICONTROL Mais]** menu ![](assets/more-icon.png) na parte superior da lista, em seguida, clique em **[!UICONTROL Converter em um projeto em branco]**.

      >[!IMPORTANT]
      >
      >A opção Converter em um projeto em branco é exibida somente quando o administrador do sistema ou do grupo ativou a variável [!UICONTROL Permitir que os usuários criem projetos sem usar um modelo] na preferência de [!UICONTROL Configuração] área. Para obter mais informações, consulte [Configurar preferências de projeto em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


      Você deve adicionar tarefas manualmente ao projeto ou anexar um modelo ao projeto após converter o problema.

      Continue para a Etapa 3e abaixo.

      <!--
     Is this accurate?
     -->

      >[!TIP]
      >   
      >* Se o problema foi criado usando uma fila de solicitações, o novo projeto herda o Grupo da fila de solicitações.
      >* Se o problema tiver sido criado ao adicioná-lo à seção Problemas do projeto, o novo projeto herdará o Grupo se o projeto do problema tiver sido criado.


   * Para converter um problema em um projeto usando um modelo, execute um dos seguintes procedimentos:

      * Clique no nome de um problema e, em seguida, clique no botão [!UICONTROL **Mais**] menu ![](assets/more-icon.png) à direita do nome da emissão

         ![](assets/issue-more-menu-expanded-with-convert-to-project-options-nwe-350x213.png)

         Ou

      * Selecione o problema na lista de problemas, em um relatório ou painel, clique no botão **Mais** menu ![](assets/more-icon.png) na parte superior da lista, em seguida, clique em **Converter em projeto a partir de modelo** e comece a digitar o nome de um template no **Pesquisar modelo** , em seguida, clique no nome do modelo quando ele for exibido na lista. Continue para a Etapa 3.

         <!--      
        (is this accurate?)      
        -->
      >[!TIP]
      >
      >Se você adicionou modelos à sua lista de Favoritos, é possível passar o mouse sobre [!UICONTROL **Modelos favoritos**] e clique no modelo que deseja usar.

      A caixa Novo projeto a partir de modelo é exibida.

      ![](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

      >[!TIP]
      >
      >Se o problema estiver associado a um processo de aprovação ou já estiver associado a um objeto de resolução, o Workfront exibirá um aviso na parte superior da caixa Converter em projeto para notificá-lo de que a aprovação será removida ou o objeto de resolução será substituído durante a conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).


1. (Condicional) Se você selecionou converter o problema em um projeto usando um modelo, continue com as seguintes etapas:

   1. Revise os detalhes do modelo à direita.

      Os detalhes do modelo incluem:

      * Duração do modelo
      * Proprietário do modelo
      * O número de tarefas de nível superior que inclui os nomes das três principais tarefas
      * O número de todas as tarefas no modelo
      * Os nomes dos formulários personalizados do modelo
   1. (Opcional) Passe o mouse sobre o nome de um modelo e clique no ícone Favoritos ![](assets/favorites-icon-small.png) para marcá-lo como favorito para uso futuro.

      >[!TIP]
      >
      >É possível ter até 40 itens do Workfront marcados como favoritos. Isso inclui modelos e outros itens.

   1. Clique em [!UICONTROL **Usar modelo**] para selecionar um template.

      O [!UICONTROL Converter em projeto] será aberta.

      ![](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

   1. Se um campo já estiver preenchido no modelo, ele será preenchido previamente no campo [!UICONTROL Converter em projeto] caixa. Você pode editar os valores pré-preenchidos para corresponder melhor ao seu projeto. Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

      >[!TIP]
      >
      >* O administrador do sistema ou do grupo pode adicionar ou remover campos na [!UICONTROL Caixa Converter em projeto] atualizando as informações de Detalhes do projeto no [!UICONTROL Modelo de layout].
      >
      >* Para atualizar os campos no [!UICONTROL Finanças] na seção [!UICONTROL Converter em projeto] deve ter [!UICONTROL Editar] acesso a [!UICONTROL Dados financeiros] no seu nível de acesso. Se tiver [!UICONTROL Exibir] acesso a [!UICONTROL Dados financeiros] no seu nível de acesso, todas as informações financeiras do modelo são transferidas para o novo projeto e não é possível editá-las enquanto você converte o problema. Para obter mais informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).


   1. (Opcional e condicional) Clique em [!UICONTROL **Opções**] no painel esquerdo, selecione as opções disponíveis:

      * [!UICONTROL **Mantenha o problema original e vincule sua resolução a este projeto**]

         Quando desmarcado, o problema original é excluído.

         >[!NOTE]
         >
         >Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema à medida que o convertem, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:
         >
         >* [Conceder acesso a problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
         > 
         >* [Compartilhar um problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)


      * [!UICONTROL **Permitir que (Nome de Usuário) tenha acesso a este projeto**]

         Se não estiver selecionado, o [!UICONTROL Contato Principal] não tem acesso à nova tarefa.

         >[!NOTE]
         >
         >As opções disponíveis aqui dependem de como o administrador do Workfront as configurou para todos no sistema ou para o seu grupo. Para obter mais informações, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
         >
         >
         >Ou, se os grupos de nível superior em sua organização os configurarem separadamente, as opções disponíveis aqui dependerão do grupo selecionado para o novo projeto na etapa 6. Para obter mais informações, consulte [Configurar preferências de tarefa e emissão para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).
   1. Clique em [!UICONTROL **Forms personalizada**] e execute um dos seguintes procedimentos:

      * Revise os formulários personalizados anexados ao modelo. Eles serão transferidos para o novo projeto.
      * Verifique se todos os campos obrigatórios têm informações válidas.
      * Reorganize os formulários personalizados arrastando-os ![](assets/drag-object-icon.png) onde quiser.
      * Clique no botão **x** à direita de qualquer formulário que não deseja transferir para o projeto.
      * Se necessário, transfira as informações do formulário personalizado do problema para o projeto.

         >[!TIP]
         >
         >* Se um formulário personalizado de vários objetos anexado ao problema for configurado para uso com problemas e projetos, todas as informações salvas no formulário serão retidas quando você fizer a conversão.
         >
         >* Se você estiver usando um modelo para a conversão e um formulário personalizado anexado ao modelo contiver um campo personalizado também encontrado em um formulário personalizado anexado ao problema, o valor do campo do problema será usado para o novo projeto. No entanto, se o campo personalizado estiver em branco sobre o problema, o valor do modelo será usado.

   1. Clique em [!UICONTROL **Converter em projeto**].

      >[!TIP]
      >
      >Se você decidir excluir o problema original, o problema agora é um projeto.
      >   
      >Ou
      >  
      >Se você decidir manter o problema original, o problema agora é vinculado ao novo projeto e será concluído quando o projeto for concluído.
      >
      >Alguns campos de edição são transferidos para o projeto. A maioria dos campos definidos no modelo são transferidos automaticamente para o projeto recém-criado se você não os alterou nas etapas anteriores. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).




1. (Opcional) Defina quaisquer detalhes adicionais do projeto &#x200B;(proprietário do projeto, datas do projeto) e tarefas, conforme necessário.
1. Clique em [!UICONTROL **Converter em projeto**].

   O problema agora é convertido em um projeto.

1. Clique em [!UICONTROL **Ir para o projeto**] dentro do [!UICONTROL Sucesso] no canto superior direito da página. Isso abre a página do projeto.
