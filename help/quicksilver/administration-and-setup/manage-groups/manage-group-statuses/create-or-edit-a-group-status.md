---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Criar ou editar um status de grupo
description: Como administrador de grupo, você pode criar status personalizados para um grupo que você gerencia. Isso ajuda a eliminar a necessidade de dezenas de status personalizados em toda a empresa e permite mais autonomia nas hierarquias do grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: 027d636e8256c6a12d552af736884f6f27886114
workflow-type: tm+mt
source-wordcount: '1313'
ht-degree: 1%

---

# Criar ou editar um status de grupo

Como administrador de grupo, você pode criar status personalizados para um grupo que você gerencia. Isso ajuda a eliminar a necessidade de dezenas de status personalizados em toda a empresa e permite mais autonomia nas hierarquias do grupo.

Também é possível editar um status de nível de sistema para um grupo que você gerencia se um administrador do Workfront tiver desbloqueado o status. Para obter mais informações, consulte [Status de nível de sistema bloqueados e desbloqueados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Se houver algum grupo acima do seu grupo, os administradores também poderão fazer essas tarefas para o seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>Os status do grupo personalizado não podem ser exibidos em um projeto ao exibi-lo em uma visualização ágil. Somente os status padrão e personalizado bloqueados ficam visíveis ao visualizar um projeto em uma visualização ágil. Para obter informações sobre como personalizar uma visualização ágil para um projeto, consulte a seção [Criar ou personalizar uma visualização ágil](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md#customizing-an-agile-view) no artigo [Visão geral das exibições no Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

Para obter informações gerais sobre status, consulte [Visão geral dos status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Workfront*</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> <p>Você deve ser um administrador de grupo do grupo ou um administrador do Workfront. Para obter mais informações, consulte <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Administradores do grupo</a> e <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Se precisar descobrir qual plano ou tipo de licença você tem, entre em contato com o administrador da Workfront.

## Criar ou editar um status para um grupo

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Grupos** ![](assets/groups-icon.png).

1. Clique no nome do grupo em que deseja criar ou personalizar os status.
1. No painel esquerdo, clique em **Status**.

   Se o grupo que você está visualizando for de nível superior, a lista exibida incluirá o seguinte:

   * Status bloqueados no nível do sistema.
   * Status personalizados já criados para o grupo.

   Além disso, se o grupo que você está visualizando for um subgrupo, a lista também inclui:

   * Status bloqueados pertencentes aos grupos acima do subgrupo.
   * Status desbloqueados que pertenciam aos grupos acima do subgrupo quando ele foi criado.

      Após a criação de um subgrupo, os status desbloqueados criados nos grupos acima dele não serão incluídos na lista de status do subgrupo. No entanto, se alguém bloquear um deles posteriormente, ele será incluído na lista de status do subgrupo. Para obter mais informações, consulte [Como os grupos herdam os status](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).


1. Selecione a guia do tipo de objeto (**Projeto**, **Tarefas** ou **Problemas**) que você deseja associar ao status.

1. (Condicional) Se o status for um status de problema, verifique se **Lista principal** está selecionada.

   ![](assets/master-list.png)

   Para obter informações sobre como personalizar os outros tipos de problema (Relatório de erros, Ordem de alteração, Ocorrência, Solicitação), consulte [Personalizar tipos de problemas padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Condicional) Para criar um novo status, clique em **Adicionar um novo status**.

   Ou

   Para editar um status existente, passe o mouse sobre o status que deseja editar e clique no botão **Editar** que é exibida à extrema direita.

   ![](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Você pode editar um status para seu grupo somente se:
   >      
   >* Você gerencia o grupo para o qual o status foi criado
   >* Um administrador do Workfront desbloqueou o status no nível do sistema
   >* Um administrador de grupo de um grupo acima do seu grupo desbloqueou o status

   >      
   >      
   >Ao editar um status existente, você pode alterar somente seu nome, descrição e cor.
   >
   >Ao editar um status bloqueado, suas alterações afetam todos os subgrupos que herdaram o status do seu grupo.
   >   
   >Por outro lado, editar um status desbloqueado não afeta os subgrupos que herdaram o status do seu grupo.

1. Especifique as seguintes informações.

   Se você estiver editando um status, somente as 3 primeiras configurações poderão ser alteradas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do status</td> 
      <td> <p>Digite um nome para o status. Este campo é obrigatório.</p> <p>Ao criar um nome de status, esteja ciente de que outros usuários no sistema podem criar um status com o mesmo nome. Recomendamos usar um nome exclusivo para evitar confusão ao selecionar status no Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>(Opcional) Digite uma descrição do status. Isto comunica o seu objetivo a quem o utiliza.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Personalize a cor do status clicando no campo de cor e selecionando uma cor no painel de amostra. Também é possível inserir um número hexadecimal no campo .</p> <p>A cor do status é exibida no canto superior direito do Workfront quando um usuário exibe o objeto.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Correspondente</td> 
      <td> <p>Selecione uma das opções na lista que melhor descreve a função do status. Por exemplo, se o nome do status for Concluído, a opção com a qual ele equivale deve ser Concluído.</p> <p>Cada status deve ser igual a uma dessas opções, pois isso determina como o status funciona.</p> <p>Essa opção não pode ser modificada após a criação do status.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chave</td> 
      <td> <p>Se estiver criando um novo status, digite um código ou abreviação para o status ou use o que foi gerado para você. Essa chave deve ser exclusiva no Workfront, pois pode ser usada para fins de relatório. Se você tentar especificar uma chave que já está sendo usada no sistema, o campo ficará vermelho.</p> <p>Pode ser útil usar uma abreviação que seja reconhecível para aqueles que a usarão.</p> <p>Essa opção não pode ser modificada após a criação do status.</p> <p>Não é possível alterar o código de chave dos status Planejamento, Atual e Concluído. Isso é importante se você estiver criando um relatório no modo de texto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar Status</td> 
      <td> <p>(Status do projeto e da tarefa somente)</p> <p>Ative essa opção se desejar que o status fique oculto dos usuários. Quando estiver desativado (a configuração padrão), todos os subgrupos abaixo do grupo poderão usar o status .</p> <p>Dica: É possível ocultar um status de Ocorrência desativando todos os quatro tipos de problema (Relatório de erros, Pedido de alteração, Ocorrência, Solicitação).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear para todos os grupos</td> 
      <td> 
       <p>Se deixar essa opção ativada, os usuários do grupo e de seus subgrupos poderão visualizar e usar o status e os administradores de grupo não poderão personalizá-la para subgrupos inferiores.</p> 
       <p>Quando essa opção estiver desativada, os administradores de grupo poderão personalizar o status de subgrupos inferiores.</p> 
       <p><b>OBSERVAÇÃO</b>: Você pode usar os status bloqueado e desbloqueado em um processo de aprovação de grupo. Se você criar um processo de aprovação de grupo com um status de grupo desbloqueado, os usuários poderão anexar o processo de aprovação a qualquer projeto, tarefa ou problema associado ao grupo.</p> 
       <p>Para obter mais informações sobre o bloqueio de status, consulte <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Status dos grupos bloqueados e desbloqueados</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Clique em **Salvar**.

   O status agora está disponível para todos os projetos associados ao seu grupo ou subgrupo. Se você bloqueou, ele está disponível para uso por qualquer subgrupo inferior.

   Você pode configurar o status para que seja um status padrão do grupo. Para obter mais informações, consulte [Usar um status personalizado como status padrão para um grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Criar um status personalizado para vários grupos

Se você for um administrador do Workfront, poderá criar um status personalizado para vários grupos criando um status em todo o sistema e ocultando esse status de qualquer grupo que não precise dele.

Se você for um administrador de grupo (ou um administrador do Workfront), poderá criar um status personalizado para vários subgrupos dentro de uma hierarquia de grupo que você gerencia criando um status para um grupo de nível superior e, em seguida, ocultando esse status de qualquer subgrupo inferior que não precise dele.

1. Se você for um administrador do Workfront, crie um status desbloqueado em todo o sistema, conforme descrito em [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. Na caixa no canto superior direito, exclua **Status do sistema**, comece digitando o nome de um grupo onde deseja ocultar o status e clique no nome quando ele for exibido.
1. Passe o mouse sobre o status que deseja ocultar do grupo e clique em **Editar** quando for exibido.

   ![](assets/hover-click-edit.jpg)

1. Ative o **Ocultar Status** que é exibida.

   ![](assets/hide-group-status.png)

1. Clique em **Salvar**.

   O status está esmaecido e não é mais visível para todos os usuários nesse grupo.

1. Repita as etapas de 3 a 5 para ocultar o status personalizado de qualquer outro grupo que não precise dele.
