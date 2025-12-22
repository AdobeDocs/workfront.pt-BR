---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Criar ou editar um status de grupo
description: Como administrador de grupo, você pode criar status personalizados para um grupo gerenciado por você. Isso ajuda a eliminar a necessidade de dezenas de status personalizados em toda a empresa e permite mais autonomia nas hierarquias do grupo.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 75018e0e-ff74-4afb-9a99-34bbb39b6e14
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1321'
ht-degree: 2%

---

# Criar ou editar um status de grupo

Como administrador de grupo, você pode criar status personalizados para um grupo gerenciado por você. Isso ajuda a eliminar a necessidade de dezenas de status personalizados em toda a empresa e permite mais autonomia nas hierarquias do grupo.

Você também pode editar um status de nível de sistema para um grupo gerenciado se um administrador do Workfront tiver desbloqueado o status. Para obter mais informações, consulte [Status de nível de sistema bloqueados e desbloqueados](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md).

Se houver algum grupo acima do seu, os administradores também poderão fazer essas coisas pelo seu grupo. O mesmo se aplica aos administradores do Workfront (para qualquer grupo).

>[!NOTE]
>
>Status de grupo personalizados não podem ser exibidos em um projeto ao visualizar o projeto em uma visualização Agile. Somente os status bloqueados padrão e personalizados ficam visíveis ao visualizar um projeto em uma visualização Agile. Para obter informações sobre como personalizar um modo de exibição Agile para um projeto, consulte a seção [Criar ou personalizar um modo de exibição Agile](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md#create-or-customize-an-agile-view) no artigo [Criar ou editar modos de exibição no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-edit-views.md).

Para obter informações gerais sobre status, consulte [Visão geral dos status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr>
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador de grupo do grupo ou um administrador do sistema.</td>
  </tr>
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar ou editar um status para um grupo

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Grupos** ![Grupos](assets/groups-icon.png).

1. Clique no nome do grupo no qual deseja criar ou personalizar os status.
1. No painel esquerdo, clique em **Status**.

   Se o grupo que você está visualizando for um grupo de nível superior, a lista exibida incluirá o seguinte:

   * Status bloqueados no nível do sistema.
   * Status personalizados já criados para o grupo.

   Além disso, se o grupo que você está visualizando for um subgrupo, a lista também incluirá:

   * Status bloqueados pertencentes aos grupos acima do subgrupo.
   * Status desbloqueados que pertenciam aos grupos acima do subgrupo quando ele foi criado.

     Após a criação de um subgrupo, os status desbloqueados criados nos grupos acima dele não são incluídos na lista de status do subgrupo. No entanto, se alguém bloquear um deles posteriormente, ele será incluído na lista de status do subgrupo. Para obter mais informações, consulte [Como os grupos herdam os status](../../../administration-and-setup/manage-groups/manage-group-statuses/how-groups-inherit-statuses.md).

1. Selecione a guia do tipo de objeto (**Projeto**, **Tarefas** ou **Problemas**) que você deseja associar ao status.

1. (Condicional) Se o status for um problema, verifique se **Lista Mestra** está selecionada.

   ![Lista mestra](assets/master-list.png)

   Para obter informações sobre como personalizar outros tipos de problemas (Relatório de Erros, Pedido de Alteração, Problema, Solicitação), consulte [Personalizar tipos de problemas padrão](../../../administration-and-setup/set-up-workfront/configure-system-defaults/customize-default-issue-types.md).

1. (Condicional) Para criar um novo status, clique em **Adicionar um novo status**.

   Ou

   Para editar um status existente, passe com o mouse sobre o status que deseja editar, em seguida, clique na opção **Editar** que é exibida na extremidade direita.

   ![Status do grupo](assets/group-statuses-edit.jpg)

   >[!NOTE]
   >Você pode editar um status para o seu grupo somente se:
   >      
   >* Você gerencia o grupo para o qual o status foi criado
   >* Um administrador do Workfront desbloqueou o status no nível do sistema
   >* Um administrador de grupo de um grupo acima do seu grupo desbloqueou o status
   >      
   >      
   >Ao editar um status existente, é possível alterar apenas seu nome, descrição e cor.
   >
   >Quando você edita um status bloqueado, as alterações afetam todos os subgrupos que herdaram o status do seu grupo.
   >   
   >Por outro lado, editar um status desbloqueado não afeta os subgrupos que herdaram o status do seu grupo.

1. Especifique as informações a seguir.

   Se você estiver editando um status, apenas as três primeiras configurações poderão ser alteradas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do status</td> 
      <td> <p>Digite um nome para o status. Este campo é obrigatório.</p> <p>Ao criar um nome de status, esteja ciente de que outras pessoas no sistema podem criar um status com o mesmo nome. Recomendamos usar um nome exclusivo para evitar confusão ao selecionar status no Workfront.</p><p>Se houver status duplicados, o administrador do grupo deverá atualizar os nomes para diferenciá-los. O único indicador de exclusividade no sistema é a Chave de status.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>(Opcional) Digite uma descrição do status. Isso comunica seu propósito para aqueles que o usam.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Personalize a cor do status clicando no campo de cor e selecionando uma cor no painel de amostra. Você também pode inserir um número hexadecimal no campo.</p> <p>A cor do status é exibida no canto superior direito do Workfront quando um usuário visualiza o objeto.</p> <p> <img src="assets/status-color.png"> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Correspondente</td> 
      <td> <p>Selecione na lista uma das opções que melhor descrevem a função do status. Por exemplo, se o nome do status for Concluído, a opção com a qual ele é igual deverá ser Concluído.</p> <p>Cada status deve ser igual a uma dessas opções, pois isso determina como o status funciona.</p> <p>Esta opção não pode ser modificada após a criação do status.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Chave</td> 
      <td> <p>Se estiver criando um novo status, digite um código ou abreviação para o status ou use o gerado para você. Essa chave deve ser exclusiva no Workfront, pois pode ser usada para fins de relatório. Se você tentar especificar uma chave que já está em uso no sistema, o campo ficará vermelho.</p> <p>Pode ser útil usar uma abreviação que seja reconhecível por aqueles que a utilizarão.</p> <p>Esta opção não pode ser modificada após a criação do status.</p> <p>Não é possível alterar o código-chave para os status Planejamento, Atual e Concluído. Isso é importante se você estiver criando um relatório em modo de texto.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ocultar Status</td> 
      <td> <p>(Somente status de projeto e tarefa)</p> <p>Ative essa opção se desejar que o status seja oculto dos usuários. Quando está desativado (a configuração padrão), todos os subgrupos abaixo do grupo podem usar o status.</p> <p>Dica: você pode ocultar o status de um problema desativando todos os 4 tipos de problemas (Relatório de erros, Pedido de alteração, Problema, Solicitação).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear para todos os grupos</td> 
      <td> 
       <p>Se você deixar essa opção ativada, os usuários no seu grupo e seus subgrupos poderão ver e usar o status e os administradores de grupo não poderão personalizá-lo para subgrupos inferiores.</p> 
       <p>Quando essa opção está desativada, os administradores de grupo podem personalizar o status para subgrupos inferiores.</p> 
       <p><b>OBSERVAÇÃO</b>: você pode usar os status bloqueado e desbloqueado em um processo de aprovação de grupo. Se você criar um processo de aprovação de grupo com um status de grupo desbloqueado, os usuários poderão anexar o processo de aprovação a qualquer projeto, tarefa ou problema associado ao grupo.</p> 
       <p>Para obter mais informações sobre status de bloqueio, consulte <a href="../../../administration-and-setup/manage-groups/manage-group-statuses/lock-or-unlock-a-custom-group-status.md" class="MCXref xref">Status de grupos bloqueados e desbloqueados</a>.</p> 
       </td> 
     </tr>
    </tbody> 
   </table>

1. Clique em **Salvar**.

   O status agora está disponível para todos os projetos associados ao seu grupo ou subgrupo. Se você o bloqueou, ele está disponível para uso por qualquer subgrupo inferior.

   Você pode configurar o status para ser um status padrão do grupo. Para obter mais informações, consulte [Usar um status personalizado como status padrão para um grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/use-custom-statuses-as-default-statuses-group.md).

## Criar um status personalizado para vários grupos

Se você for um administrador do Workfront, poderá criar um status personalizado para vários grupos criando um status de todo o sistema e, em seguida, ocultando esse status de todos os grupos que não precisam dele.

Se você for um administrador de grupo (ou um administrador do Workfront), poderá criar um status personalizado para vários subgrupos dentro de uma hierarquia de grupo gerenciada criando um status para um grupo de nível superior e, em seguida, ocultando esse status de qualquer subgrupo inferior que não precise dele.

1. Se você for um administrador do Workfront, crie um status desbloqueado em todo o sistema, conforme descrito em [Criar ou editar um status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
1. Na caixa no canto superior direito, exclua **Status do Sistema**, comece digitando o nome de um grupo no qual deseja ocultar o status e, em seguida, clique no nome quando ele for exibido.
1. Passe o cursor do mouse sobre o status que deseja ocultar do grupo e clique em **Editar** quando ele aparecer.

   ![Editar status](assets/hover-click-edit.jpg)

1. Habilite a opção **Ocultar Status** que aparece.

   ![Ocultar status](assets/hide-group-status.png)

1. Clique em **Salvar**.

   O status fica esmaecido e não fica mais visível para todos os usuários nesse grupo.

1. Repita as etapas de 3 a 5 para ocultar o status personalizado de qualquer outro grupo que não precise dele.

