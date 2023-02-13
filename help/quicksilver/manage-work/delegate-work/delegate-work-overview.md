---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Visão geral do trabalho delegado
description: Quando você planeja estar fora do escritório por um curto período de tempo, você pode delegar temporariamente seu trabalho a outros usuários para garantir que sua ausência não se torne um obstáculo para o trabalho que está sendo concluído.
author: Alina
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: f3ae487f53f7c4f8c389cf0d35323f21e76ece35
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 1%

---

# Visão geral do trabalho delegado

Quando você planeja estar fora do escritório por um curto período de tempo, você pode delegar temporariamente seu trabalho a outros usuários para garantir que sua ausência não se torne um obstáculo para o trabalho que está sendo concluído.

Por exemplo, se determinadas tarefas vencerem antes de retornar, mas você não tiver tempo para concluí-las antes de sair, é possível delegar as tarefas a outro usuário para que ele possa concluí-las a tempo e não atrasar a conclusão do projeto até que você retorne.

Você pode delegar os seguintes objetos em [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tarefas atribuídas a você
* Problemas atribuídos a você
* Projeto, tarefa, emissão, aprovações de documento atribuídas a você.

Este artigo contém informações gerais sobre delegação de tarefas e problemas.

Para obter informações sobre delegação de projeto, tarefa, emissão e aprovações de documento, consulte [Delegar solicitação de aprovação](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Para obter informações sobre como delegar tarefas e problemas, consulte [Delegar tarefas e problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

## Visão geral do trabalho delegado

Considere o seguinte ao delegar tarefas e problemas:

* Seu [!DNL Workfront] ou o administrador do grupo deve ativar as preferências da delegação no [!UICONTROL Configuração] antes de delegar seu trabalho a outros.

   Para obter mais informações, consulte [Configurar preferências de emissão e tarefa em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Você pode delegar tarefas e problemas somente do [!UICONTROL Início] área.
* Existem exceções para os seguintes tipos de licença:

   * Você pode delegar trabalho a Revisores ou Solicitantes, embora [!DNL Workfront] não o recomenda.
   * Os revisores podem delegar trabalhos a outros. Eles não podem exibir itens de trabalho em seus [!UICONTROL Início] área. Eles podem exibir somente aprovações.
   * Os solicitantes não podem delegar trabalho a outros. Eles não podem exibir itens de trabalho em seus [!UICONTROL Início] area
* Você só pode delegar as tarefas e os problemas atribuídos a você. Você não pode delegar tarefas e problemas que são atribuídos a outros usuários, equipes ou funções de trabalho.
* Você só pode delegar tarefas e problemas que não são concluídos antes da data de início da delegação.
* Se um item de trabalho for concluído durante o período de delegação, o item permanecerá na área Inicial do delegado e do destinatário por 2 semanas antes [!DNL Workfront] O remove automaticamente.
* Os usuários selecionados como delegados recebem as mesmas permissões que suas permissões nas tarefas e problemas que você delega a eles. As permissões devem funcionar em seus níveis de acesso e, às vezes, seus níveis de acesso podem ser menores do que os seus.

>[!NOTE]
>
>  Para itens que são atribuídos depois que a delegação já foi iniciada, pode levar até uma hora depois que o item foi atribuído para [!DNL Workfront] para compartilhar os itens recém-atribuídos com o delegado.

* Se tarefas e problemas adicionais forem atribuídos a você durante o tempo em que você selecionou que seu trabalho fosse delegado a outros usuários, o novo trabalho atribuído será delegado automaticamente à mesma pessoa pelo período selecionado, se as datas da tarefa ou da emissão estiverem dentro desse período.
* O mesmo usuário pode ser selecionado como delegado por vários usuários.
* As tarefas delegadas e os problemas não são exibidos nas ferramentas de gerenciamento de recursos, como o [!UICONTROL Balanceador de Carga de Trabalho] ou [!UICONTROL Planejador de recursos] para os utilizadores delegados.
* Você pode visualizar o trabalho delegado e nomes de delegados em várias áreas de [!DNL Workfront]. Para obter mais informações, consulte a seção &quot;Localizar trabalho delegado e informações delegadas&quot; no artigo [Gerenciar delegação de tarefa e emissão](../delegate-work/how-to-delegate-work.md).


   >[!IMPORTANT]
   >
   >  Se um usuário tiver somente o acesso à Exibição para tarefas em seu nível de acesso e tiver permissões de Gerenciamento nas tarefas que você delegar a ele, ele receberá permissões de Gerenciamento para as tarefas que você delegar a ele. No entanto, eles não poderão executar as mesmas ações que você nas tarefas delegadas. Eles devem solicitar Editar acesso às Tarefas pelo administrador do sistema para poder atualizar tarefas na sua ausência.

* Parar a delegação não remove as permissões concedidas aos usuários delegados sobre as tarefas e os problemas em que eles foram delegados.
* Se um sistema ou desativar o [!UICONTROL Permitir que usuários deleguem suas tarefas e problemas] na configuração do [!UICONTROL Configuração] , os usuários delegados atualmente são removidos das tarefas e problemas aos quais foram anteriormente delegados. Suas permissões para as tarefas ou problemas não são removidas.

## Diferenças e semelhanças entre atribuições e delegações

| Ação | Atribuições | Delegações |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Um usuário atribuído ou delegado pode editar ou excluir o item de trabalho ao qual está atribuído ou delegado | Com base em permissões e nível de acesso | Com base em permissões e nível de acesso |
| Um usuário atribuído ou delegado é exibido no cabeçalho do item de trabalho | Sim | Sim |
| As tarefas atribuídas ou delegadas ou os problemas são exibidos na área inicial do destinatário ou do delegado | Sim, até que o item esteja concluído | Sim, somente para o período de tempo da delegação |
| Você pode atribuir ou delegar trabalhos a usuários a partir da área inicial | Sim | Sim |
| Você pode atribuir ou delegar trabalhos a usuários usando a variável | Sim | não |
| Você pode atribuir ou delegar trabalho a usuários em uma lista ou a partir do cabeçalho de um item de trabalho | Sim | não |
| Qualquer usuário pode atribuir ou delegar outros usuários com itens de trabalho aos quais eles não estejam associados | Com base em permissões e nível de acesso | não. Somente o destinatário pode delegar seus próprios itens. |
| Horas Planejadas, Reais ou Orçadas para trabalho atribuído ou delegado a uma exibição de usuário para esse usuário nas ferramentas de gerenciamento de recursos | Sim | não |
