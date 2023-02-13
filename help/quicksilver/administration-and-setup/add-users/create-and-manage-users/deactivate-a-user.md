---
title: Desativar ou reativar um usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Como administrador do Workfront, você pode desativar ou reativar um usuário.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aba243ba-46c2-4eb7-b704-4368bf0ae3cc
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 0%

---

# Desativar ou reativar um usuário

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para obter instruções sobre como desativar um usuário no Adobe Admin Console, consulte a seção &quot;Remover usuários&quot; no artigo [Gerenciar usuários individualmente](https://helpx.adobe.com/enterprise/using/manage-users-individually.html) ou entre em contato com o administrador do Adobe Admin Console.
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Seus usuários podem sair da organização e talvez seja necessário removê-los da Adobe Workfront. Eles não devem permanecer ativos no sistema, pois isso criaria confusão para outros usuários ao adicioná-los a atualizações ou atribuí-los trabalho. Quando você desativar um usuário, outros usuários não verão mais seu nome quando pesquisarem por pessoas no sistema.

Os administradores podem ver usuários inativos na área Configuração .

Você pode reativar um usuário a qualquer momento.

>[!IMPORTANT]
>
>Recomendamos desativar os usuários que saíram da organização em vez de excluí-los. Se um usuário for excluído, todo o histórico no Workfront associado a esse usuário será perdido. Isso inclui suas atribuições de trabalho, sua associação com notas, horas, documentos e todos os outros objetos que eles criaram depois.
>
>Desativar um usuário no Workfront remove as licenças do usuário para a prova digital e do Workfront. Além disso, o usuário não pode mais receber trabalho. Quando um usuário é desativado, a licença Workfront e a licença de prova desse usuário ficam disponíveis para uso por outro usuário; todas as outras informações no perfil do usuário desativado permanecem como estão.
>
>Para obter mais informações sobre o impacto da exclusão e da desativação de usuários, consulte [Excluir usuários](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td> <p>Plano </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do Administrador do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p><b>Usuários</b> na configuração do seu nível de acesso configurado como <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador do usuário</b> opções ativadas em <b>Ajustar as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se Usuário <b>Administrador (usuários do grupo)</b> estiver habilitado, você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> <p>Para obter mais informações sobre o <b>Usuários</b> configurar em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Desativar um usuário

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Selecione um usuário, clique no ícone Mais ![](assets/more-icon.png), depois clique em **Desativar**.

1. Clique em **Desativar** na caixa exibida.

## Agendar usuários para desativação

Como gerente, talvez você queira marcar os usuários como desativados antes de eles realmente deixarem sua organização. Por exemplo, se você estiver trabalhando com um usuário vinculado por contrato, ele estará em seu sistema por um período limitado e você saberá a data de término. Você pode programá-los para ficarem desativados nessa data.

Os administradores do Workfront e usuários da licença do Plan podem ver a data de desativação em seu perfil de usuário.

Para agendar um usuário para desativação:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Selecione o nome do usuário.

   Ou

   (Opcional) Selecione vários usuários para agendá-los para desativação em massa.

1. Clique no ícone Editar ![](assets/edit-icon.png).
1. Na caixa Editar usuário que é exibida, clique em **Planejamento de recursos** ir para aquela área.
1. Ative o **Agendar desativação** opção.

1. No calendário exibido, especifique a data e a hora para a **Data de desativação programada**.

   >[!NOTE]
   >
   >* Na caixa de tempo, você pode selecionar apenas incrementos de hora inteira, não minutos.
   >* Se você selecionar uma hora para o dia atual que passou, o Workfront agendará a desativação para o dia seguinte às 12:00 AM. A hora selecionada corresponde ao fuso horário do computador do usuário que está agendando a desativação.


1. Clique em **Salvar alterações**.

   O usuário é desativado no dia selecionado, às vezes depois do horário selecionado. Se você selecionou vários usuários para desativarem em massa, todos os usuários selecionados são desativados no dia selecionado, às vezes após o tempo selecionado.

Recomendamos que você crie um relatório para os usuários que você agendou para desativação, para manter-se informado sobre o que os usuários estão começando a ser desativados. Não há confirmação de que a desativação tenha ocorrido assim que os usuários forem desativados.

## Reativar um usuário

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Usuários** ![](assets/users-icon-in-main-menu.png).

1. Selecione um usuário, clique no ícone Mais ![](assets/more-icon.png), depois clique em **Ativar**.

1. Atribua um novo **Nível de acesso** no menu suspenso.

### A revisão de texto afeta ao reativar um usuário

Os usuários desativados perdem a função de prova padrão atribuída e a licença de prova (se você estiver em um Workfront Premium Legacy Plan). Se você optar por reativar o usuário, deverá:

* Atribua novamente a licença (se estiver em um Plano herdado do Workfront Premium). Para obter mais informações sobre os planos de prova do Workfront, consulte [Acesso à funcionalidade de prova no Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).
* Verifique se eles têm a função de prova correta. Os usuários de prova reativados recebem o que for especificado como a função de prova padrão para novos usuários. Consulte [Configurar funções de prova padrão](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proofing-roles.md) para obter mais informações.

## Sobre a desativação de administradores do Workfront e de usuários de licença do Plan

Antes de desativar um administrador do Workfront ou um usuário com uma licença do Plan , é importante verificar objetos e atividades do Workfront envolvendo essa pessoa e associá-los a outro administrador do Workfront ou usuário de licença do Plan , conforme necessário.

Esses objetos e atividades podem incluir o seguinte:

* Tarefas ou problemas atribuídos ao usuário
* Projetos pertencentes ao usuário
* Relatórios configurados para serem executados com os direitos de acesso do usuário
* Modelos de propriedade do usuário
* Projetos e modelos nos quais o usuário foi definido como um gerenciador de recursos
* Solicitar regras de roteamento de fila em que o administrador do Workfront ou o usuário de licença do Plano é o Destinatário Padrão
* Processos de aprovação que têm um estágio incluindo o usuário (especialmente se eles forem o único aprovador no palco)
* Folhas de horas que listam o usuário como aprovador
* Perfis de folha de horas que listam o usuário como aprovador
* Revisar fluxos de trabalho automatizados que incluem o usuário

## Impacto do planejamento de recursos ao agendar um usuário para desativação

Quando você agenda um usuário para desativação, ele não é mais exibido no Planejador de Recursos como estando disponível para as horas do orçamento. Se eles permanecerem parte dos Pools de Recursos, eles aparecerão no Planejador de Recursos, mas sua disponibilidade será definida para zero horas a partir da data de sua desativação programada.

O Planejador de Recursos leva em conta todas as funções de cargo dos usuários e Datas de Conclusão Planejadas das tarefas e calcula os recursos de acordo.

Para obter mais informações sobre o Planejador de Recursos, consulte [Visão geral do Planejador de recursos](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).
