---
product-area: projects
navigation-topic: convert-issues
title: Converter um problema em um projeto no Adobe Workfront
description: Converter um problema em um projeto no Adobe Workfront
author: Alina
feature: Work Management
exl-id: e3ba15a3-6169-466c-9912-32a8afdcc68d
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1975'
ht-degree: 1%

---

# Converter um problema em um projeto no Adobe Workfront

<!--Audited: 01/2024-->

Se for necessário trabalhar mais para concluir um problema depois que ele for enviado, você pode converter o problema em um projeto.

Você pode converter um problema em um novo projeto ou convertê-lo em um projeto usando um modelo. Este artigo descreve ambas as maneiras de converter problemas em projetos.

>[!IMPORTANT]
>
>Para obter informações gerais sobre a conversão de problemas, recomendamos que você também leia o artigo [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

Ao criar um projeto a partir de um problema, alguns dos campos no projeto são preenchidos a partir de outros objetos. Para obter mais informações, consulte a seção &quot;Configurações padrão do novo projeto&quot; no artigo [Criar um projeto](../../../manage-work/projects/create-projects/create-project.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão </p> 
    <p>Atual: Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Problemas, Tarefas e Projetos</p> <p>Editar acesso a Dados Financeiros para atualizar informações financeiras de uma projeção convertida a partir da ocorrência</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o problema</p> <p>Você obtém permissões de Gerenciamento para o projeto após a conversão do problema</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Converter um problema em um projeto

Você pode converter um problema em um projeto em branco.

1. Vá para um projeto e clique em **[!UICONTROL Problemas]** no painel esquerdo.
1. Na lista de problemas que são exibidas, siga um destes procedimentos:

   * Para converter um problema em um projeto em branco, clique no nome do problema, clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon.png) à direita do nome do problema e clique em **[!UICONTROL Converter em um projeto em branco]**.


     Ou

     Selecione o problema na lista de problemas, clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon.png) na parte superior da lista e clique em **[!UICONTROL Converter em um projeto em branco]**.

     >[!IMPORTANT]
     >
     >A opção Converter em um projeto em branco é exibida somente quando o administrador do sistema ou do grupo habilita a preferência [!UICONTROL Permitir que os usuários criem projetos sem usar um modelo] na área [!UICONTROL Instalação]. Para obter mais informações, consulte [Configurar preferências de projeto do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).


     Você deve adicionar tarefas manualmente ao projeto ou anexar um modelo ao projeto depois de converter o problema.

     >[!TIP]
     >   
     >* Se o problema tiver sido criado usando uma fila de solicitações, o novo projeto herdará o grupo da fila de solicitações.
     >* Se o problema tiver sido criado adicionando-o à seção Problemas do projeto, o novo projeto herdará o Grupo do projeto do problema.

     >[!TIP]
     >
     >Se o problema estiver associado a um processo de aprovação ou já estiver associado a um objeto de resolução, o Workfront exibirá um aviso na parte superior da caixa Converter em projeto para notificar que a aprovação será removida ou o objeto de resolução será substituído durante a conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

1. (Opcional e condicional) Clique em [!UICONTROL **Opções**] no painel esquerdo e selecione uma das opções disponíveis:

   * [!UICONTROL **Manter o problema original e vincular a sua resolução a este projeto**]

     Quando desmarcado, o problema original é excluído.

     >[!NOTE]
     >
     >Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema como estão convertendo-o, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:
     >
     >* [Conceder acesso aos problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Compartilhar um problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Permitir que (Nome de Usuário) tenha acesso a este projeto**]

     Se desmarcada, o [!UICONTROL Contato Primário] do problema não terá acesso à nova tarefa.

     >[!NOTE]
     >
     >As opções disponíveis aqui dependem de como o administrador do Workfront as configurou para todos no sistema ou para o seu grupo. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Ou, se os grupos de nível superior em sua organização os configuraram separadamente, as opções disponíveis aqui dependem do grupo que você selecionou para o novo projeto na etapa 6. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

1. Clique em [!UICONTROL **Forms Personalizado**] e siga um destes procedimentos:

   * Revise os formulários personalizados anexados ao problema. Eles serão transferidos para o novo projeto se também forem formulários personalizados de projeto.
   * Adicionar mais formulários personalizados
   * Verifique se todos os campos obrigatórios têm informações válidas.
   * Reorganize os formulários personalizados arrastando-os ![ícone de Arrastar](assets/drag-object-icon.png) onde você desejar.
   * Clique no ícone **x** à direita de qualquer formulário que você não deseja transferir para o projeto. Isso remove o formulário do projeto.
   * Se necessário, transfira as informações de formulário personalizadas do problema para o projeto.

     >[!TIP]
     >
     >* Se um formulário personalizado de vários objetos anexado ao problema for configurado para uso com problemas e projetos, todas as informações salvas no formulário serão mantidas quando você fizer a conversão, se os campos existirem tanto no problema quanto nos formulários personalizados do projeto.
     >* Se um formulário personalizado de vários objetos com um campo calculado for anexado ao problema, bem como ao projeto, o problema e o projeto devem ser compatíveis com todos os campos referenciados nos campos personalizados calculados do formulário. Se houver uma incompatibilidade, uma mensagem o alertará para fazer ajustes. Para obter mais informações, consulte a seção &quot;Campos personalizados calculados em formulários personalizados de vários objetos&quot; em [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).

1. Clique em [!UICONTROL **Converter para projeto**].

   >[!TIP]
   >
   >Se você decidiu excluir o problema original, ele agora é um projeto.
   >   
   >Ou
   >  
   >Se você decidiu manter o problema original, ele agora está vinculado ao novo projeto e será concluído quando o projeto for concluído.
   >
   >As informações em alguns campos de problema são transferidas para o projeto, se você não as alterou durante a conversão.

1. (Opcional) Defina outros detalhes &#x200B; projeto (proprietário do projeto, datas do projeto) e tarefas, conforme necessário.
1. Clique em [!UICONTROL **Converter para projeto**].

   O problema foi convertido em um projeto. A página do projeto é exibida.

## Converter um problema em um projeto usando um modelo

Você pode converter um problema em um projeto usando um modelo.

1. Vá para um projeto e clique em **[!UICONTROL Problemas]** no painel esquerdo.
1. Na lista de problemas exibida, clique no nome do problema, clique no menu **[!UICONTROL Mais]** ![Mais menu](assets/more-icon.png) à direita do nome do problema, clique em **Converter em projeto de Modelo** e comece a digitar o nome de um modelo na caixa **Modelo de Pesquisa** e clique no nome do modelo quando ele for exibido na lista. Continue com a Etapa 3.

   >[!TIP]
   >
   >Se você tiver adicionado modelos à sua lista Favoritos, passe o mouse sobre o menu [!UICONTROL **Modelos favoritos**] e clique no modelo que deseja usar.

   A caixa Novo projeto a partir do modelo é exibida.

   ![Novo projeto do modelo](assets/new-project-from-template-small-box-with-template-details-panel-nwe-350x279.png)

   >[!TIP]
   >
   >* Se o problema estiver associado a um processo de aprovação ou já estiver associado a um objeto de resolução, o Workfront exibirá um aviso na parte superior da caixa Converter em projeto para notificar que a aprovação será removida ou o objeto de resolução será substituído durante a conversão. Para obter mais informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).
   >   
   >* Se o problema tiver sido criado usando uma fila de solicitações, o novo projeto herdará o grupo da fila de solicitações.
   >* Se o problema tiver sido criado adicionando-o à seção Problemas do projeto, o novo projeto herdará o Grupo do projeto do problema.

1. Revise os detalhes do modelo à direita.

   Os detalhes do template incluem o seguinte:

   * Duração do modelo
   * Proprietário do modelo
   * O número de tarefas de nível superior que inclui os nomes das três principais tarefas
   * O número de todas as tarefas no modelo
   * Os nomes dos formulários personalizados do modelo

1. (Opcional) Passe o mouse sobre o nome de um modelo e clique no ícone **Favoritos** ![Favoritos](assets/favorites-icon-small.png) para marcá-lo como favorito para uso futuro.

   >[!TIP]
   >
   >É possível marcar até 40 itens do Workfront como favoritos. Isso inclui modelos e outros itens.

1. Clique em [!UICONTROL **Usar modelo**] para selecionar um modelo.

   A caixa [!UICONTROL Converter em Projeto] é aberta.

   ![Converter para projeto](assets/convert-to-project-from-template-large-project-box-nwe-350x291.png)

1. Se um campo já estiver preenchido no modelo, ele será preenchido na caixa [!UICONTROL Converter em projeto]. É possível editar os valores pré-preenchidos para melhor corresponder ao seu projeto. Para obter mais informações, consulte [Editar projetos](../../../manage-work/projects/manage-projects/edit-projects.md).

   >[!TIP]
   >
   >* O administrador do sistema ou do grupo pode adicionar ou remover campos na [!UICONTROL caixa Converter em Projeto] atualizando as informações de Detalhes do Projeto em seu [!UICONTROL Modelo de Layout].
   >
   >* Para atualizar campos na seção [!UICONTROL Finanças] da caixa [!UICONTROL Converter em Projeto], você deve ter acesso de [!UICONTROL Edição] a [!UICONTROL Dados Financeiros] no seu nível de acesso. Se você tiver acesso de [!UICONTROL Visualização] a [!UICONTROL Dados Financeiros] no seu nível de acesso, todas as informações financeiras do modelo serão transferidas para o novo projeto e você não poderá editá-las enquanto converter o problema. Para obter informações, consulte [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md) e [Compartilhar um modelo](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. (Opcional e condicional) Clique em [!UICONTROL **Opções**] no painel esquerdo e selecione uma das opções disponíveis:

   * [!UICONTROL **Manter o problema original e vincular a sua resolução a este projeto**]

     Quando desmarcado, o problema original é excluído.

     >[!NOTE]
     >
     >Os usuários sem acesso ou permissões para excluir problemas não poderão excluir o problema como estão convertendo-o, independentemente do status dessa configuração. Para obter informações sobre acesso e permissões para problemas, consulte:
     >
     >* [Conceder acesso aos problemas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
     > 
     >* [Compartilhar um problema](../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md)

   * [!UICONTROL **Permitir que (Nome de Usuário) tenha acesso a este projeto**]

     Se desmarcada, o [!UICONTROL Contato Primário] do problema não terá acesso à nova tarefa.

     >[!NOTE]
     >
     >As opções disponíveis aqui dependem de como o administrador do Workfront as configurou para todos no sistema ou para o seu grupo. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas do sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
     >
     >
     >Ou, se os grupos de nível superior em sua organização os configuraram separadamente, as opções disponíveis aqui dependem do grupo que você selecionou para o novo projeto na etapa 6. Para obter mais informações, consulte [Configurar preferências de tarefas e problemas para um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

   1. Clique em [!UICONTROL **Forms Personalizado**] e siga um destes procedimentos:

      * Revise os formulários personalizados anexados ao modelo. Eles serão transferidos para o novo projeto.
      * Revise os formulários personalizados anexados ao problema. Eles serão transferidos para o projeto se também forem formulários de projeto.
      * Verifique se todos os campos obrigatórios têm informações válidas.
      * Reorganize os formulários personalizados arrastando-os ![ícone de Arrastar](assets/drag-object-icon.png) onde você desejar.
      * Clique no ícone **x** à direita de qualquer formulário que você não deseja transferir para o projeto.
      * Se necessário, transfira as informações de formulário personalizadas do problema para o projeto.

        >[!TIP]
        >
        >* Se um formulário personalizado de vários objetos anexado ao problema for configurado para uso com problemas e projetos, todas as informações salvas no formulário serão mantidas quando você fizer a conversão, se os campos existirem tanto no problema quanto nos formulários personalizados do projeto.
        >* Se um formulário personalizado de vários objetos com um campo calculado for anexado ao problema, bem como ao projeto, o problema e o projeto devem ser compatíveis com todos os campos referenciados nos campos personalizados calculados do formulário. Se houver uma incompatibilidade, uma mensagem o alertará para fazer ajustes. Para obter mais informações, consulte [Adicionar campos calculados a um formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/add-a-calculated-field.md).
        >* Se um formulário personalizado anexado ao modelo contiver um campo personalizado também encontrado em um formulário personalizado anexado ao problema, o valor do campo do problema será usado para o novo projeto. No entanto, se o campo personalizado estiver em branco no problema, o valor do template será usado.

1. (Opcional) Defina outros detalhes &#x200B; projeto (proprietário do projeto, datas do projeto) e tarefas, conforme necessário.

   1. Clique em [!UICONTROL **Converter para projeto**].

      >[!TIP]
      >
      >Se você decidiu excluir o problema original, ele agora é um projeto.
      >   
      >Ou
      >  
      >Se você decidiu manter o problema original, ele agora está vinculado ao novo projeto e será concluído quando o projeto for concluído.
      >
      >Alguns campos de problema são transferidos para o projeto. A maioria dos campos definidos no modelo é transferida automaticamente para o projeto recém-criado se você não os alterou nas etapas anteriores. Para obter informações, consulte [Visão geral da conversão de problemas no Adobe Workfront](../../../manage-work/issues/convert-issues/convert-issues.md).

   O problema foi convertido em um projeto. A página do projeto é exibida.