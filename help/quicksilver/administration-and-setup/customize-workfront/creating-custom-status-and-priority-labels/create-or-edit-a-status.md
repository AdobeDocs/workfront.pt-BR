---
title: Criar ou editar um status
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
description: Como administrador do Adobe Workfront, você pode criar status personalizados para projetos, tarefas e problemas.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 35c804b5-569d-4ba8-84b8-6129f0ffbc7f
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 2%

---

# Criar ou editar um status

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT THROUGH CONTEXT SENSITIVE HELP LINKS.-->

Como administrador do Adobe Workfront, você pode criar status personalizados para projetos, tarefas e problemas. Eles podem ser para usuários em todo o sistema Workfront ou para grupos ou subgrupos específicos. Para obter mais informações sobre status, consulte [Visão geral dos status](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md).

>[!NOTE]
>
>Os administradores de grupo também podem criar seus próprios status de grupo, para uso somente por seus grupos. Para obter mais informações, consulte [Criar ou editar o status de um grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
     <p>Novo: Padrão</p>
     <p>ou</p>
     <p>Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar ou editar um status personalizado

Você pode adicionar um status personalizado para ser usado por toda a organização ou por um único grupo.

Ao criar um status personalizado para toda a organização, você pode configurá-lo para que todos os grupos no sistema possam usá-lo sem editá-lo. Ou você pode configurá-lo para que os administradores de grupos possam modificá-lo para seus grupos, conforme explicado em [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Preferências do projeto** > **Status**.

1. (Condicional) Se você estiver criando ou editando um status para uso em todo o sistema, verifique se **Status do Sistema** está selecionado na caixa no canto superior direito.

   ![](assets/system-statuses-in-upper-rt-corner-new.jpg)

   Ou

   Se o status for para um grupo ou subgrupo, comece digitando o nome do grupo no canto superior direito e selecione-o quando ele for exibido.

   ![](assets/system-statuses-in-upper-rt-corner-group.jpg)

1. Selecione a guia do tipo de objeto (**Projeto**, **Tarefas** ou **Problemas**) que você deseja associar ao status.

1. Se você estiver criando um novo status, clique em **Adicionar um Novo Status**.

   Ou

   Se você estiver editando um status existente, passe o mouse sobre ele e clique no ícone **Editar**, que é exibido na extremidade direita.

   ![](assets/custom-status-edit.png)

1. Configure o status usando as seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome do status</td> 
      <td> <p>Digite um nome para o status. Este campo é obrigatório.</p> <p>Ao criar um nome de status, esteja ciente de que outras pessoas no sistema podem criar um status com o mesmo nome. Recomendamos usar um nome exclusivo para evitar confusão ao selecionar status no Workfront.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição</td> 
      <td>(Opcional) Digite uma descrição do status. Isso comunica seu propósito para aqueles que o usam.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cor</td> 
      <td> <p>Personalize a cor do status clicando no campo de cor e selecionando uma cor no painel de amostra. Você também pode inserir um número hexadecimal no campo.</p> <p>A cor do status é exibida no canto superior direito do Workfront quando um usuário visualiza o objeto.</p> <img src="assets/status-color.png" style="width: 350;height: 211;"> </p> </td> 
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
      <td> <p>(Somente status de projeto e tarefa)</p> <p>Ative essa opção se desejar que o status seja oculto dos usuários. Quando essa opção está desativada (a configuração padrão), todos os usuários no sistema podem usar o status.</p> <p>Você pode ocultar o status de um problema desativando essa opção para todos os 4 tipos de problemas (Relatório de erros, Pedido de alteração, Ocorrência, Solicitação).</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear para todos os grupos</td> 
      <td>
       <p>Quando um status é bloqueado, os usuários em todo o sistema podem visualizá-lo e usá-lo, e os administradores de grupo não podem personalizá-lo para seus grupos.</p> 
       <p>Quando um status é desbloqueado, os administradores de grupo podem personalizá-lo para seus grupos individuais.</p>

   <div>
       <p>Você pode usar os status bloqueado e desbloqueado em um processo de aprovação do sistema. Se você criar um processo de aprovação do sistema com um status de sistema desbloqueado, os usuários em todo o sistema poderão anexar o processo de aprovação a qualquer projeto, tarefa ou problema no sistema.</p>
       <p> Nos seguintes cenários, mensagens de aviso são exibidas para ajudar você e seus usuários a entender os resultados do desbloqueio de um status:</p>
       <ul>
       <li>Um administrador desbloqueia um status de nível de sistema que é usado em um processo de aprovação. Uma mensagem avisa que a pode excluir o status desbloqueado de seus grupos, o que impediria que os membros do grupo usassem esse processo de aprovação corretamente para objetos atribuídos a seus grupos.</li>
       <li>Um usuário começa a editar um processo de aprovação que usa um status desbloqueado. Uma mensagem alerta o usuário sobre o status desbloqueado para que ele possa avaliar se seria uma boa ideia bloqueá-lo novamente ou substituí-lo.</li>
       <li>Um processo de aprovação em nível de sistema com status desbloqueado é anexado a um objeto e o status foi excluído para o grupo atribuído ao objeto. Quando um membro do grupo vai para a seção Aprovações do objeto, uma mensagem explica que o processo de aprovação não pode ser iniciado para o objeto.</li>
       </ul>
       <p>Para obter mais informações sobre status de bloqueio, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/lock-or-unlock-a-custom-system-level-status.md" class="MCXref xref">Status de nível de sistema bloqueados e desbloqueados</a>.</p>
       </div>
      </td>
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

   Para obter instruções sobre como tornar este status padrão, consulte [Usar status personalizados como status padrão](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

Para obter informações sobre como reordenar os status de grupo, consulte [Reordenar os status de grupo e de nível de sistema](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).
