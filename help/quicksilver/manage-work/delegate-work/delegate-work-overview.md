---
filename: delegate-work-overview
content-type: overview
navigation-topic: delegate-work
title: Delegar visão geral do trabalho
description: Quando você planeja ficar fora do escritório por um curto período de tempo, pode delegar temporariamente seu trabalho a outros usuários para garantir que sua ausência não se torne um obstáculo para a conclusão do trabalho.
author: Alina
feature: Work Management
exl-id: aec2ce78-278f-48d2-af8c-e4e5b31ac856
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 1%

---

# Delegar visão geral do trabalho

Quando você planeja ficar fora do escritório por um curto período de tempo, pode delegar temporariamente seu trabalho a outros usuários para garantir que sua ausência não se torne um obstáculo para a conclusão do trabalho.

Por exemplo, se determinadas tarefas vencerem antes de você retornar, mas não houver tempo para concluí-las antes de sair, você poderá delegar suas tarefas a outro usuário para que ele possa concluí-las no prazo e não atrasar a conclusão do projeto até depois que você retornar.

Você pode delegar os seguintes objetos em [!DNL Adobe Workfront]:

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Projects where you are designated as the Project Owner (not yet, not for the MVP)</p> </li>
  -->

* Tarefas atribuídas a você
* Problemas atribuídos a você
* Aprovações de projetos, tarefas, problemas e documentos atribuídas a você.

Este artigo contém informações gerais sobre a delegação de tarefas e problemas.

Para obter informações sobre como delegar aprovações de projetos, tarefas, problemas e documentos, consulte [Delegar solicitação de aprovação](../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

Para obter informações sobre como delegar tarefas e problemas, consulte [Delegar tarefas e problemas](../../manage-work/delegate-work/how-to-delegate-work.md).

## Delegar visão geral do trabalho

Considere o seguinte ao delegar tarefas e problemas:

* Seu [!DNL Workfront] ou o administrador de grupo deve ativar as preferências de Delegação no [!UICONTROL Configuração] antes de delegar seu trabalho a outras pessoas.

  Para obter informações, consulte [Configurar preferências de tarefas e problemas em todo o sistema](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).
* Você pode delegar tarefas e problemas somente a partir do [!UICONTROL Início] área.
* Existem exceções para os seguintes tipos de licença:

   * Você pode delegar trabalho a Revisores ou Solicitantes, embora [!DNL Workfront] não recomenda.
   * Os revisores podem delegar trabalho a outros. Eles não podem exibir itens de trabalho em seus [!UICONTROL Início] área. Eles podem exibir somente aprovações.
   * Os solicitantes não podem delegar trabalho a outras pessoas. Eles não podem exibir itens de trabalho em seus [!UICONTROL Início] área
* Você só pode delegar tarefas e problemas atribuídos a você. Não é possível delegar tarefas e problemas atribuídos a outros usuários, equipes ou funções de trabalho.
* Você só pode delegar tarefas e problemas que não tenham sido concluídos antes da data de início da delegação.
* Se um item de trabalho for concluído durante o período de delegação, ele permanecerá na área inicial do delegado e do destinatário por duas semanas antes [!DNL Workfront] o remove automaticamente.
* Os usuários selecionados como delegados recebem as mesmas permissões que suas permissões nas tarefas e problemas que você delega a eles. As permissões devem funcionar dentro de seus níveis de acesso e, às vezes, seus níveis de acesso podem ser inferiores aos seus.

>[!NOTE]
>
>  Para itens atribuídos após a delegação já iniciada, pode levar até uma hora depois que o item foi atribuído para [!DNL Workfront] para compartilhar os itens recentemente atribuídos com o delegado.

* Se tarefas e problemas adicionais forem atribuídos a você durante o período selecionado para que seu trabalho seja delegado a outros usuários, o novo trabalho atribuído será automaticamente delegado à mesma pessoa para o período selecionado se as datas da tarefa ou problema estiverem dentro desse período.
* O mesmo usuário pode ser selecionado como delegado por vários usuários.
* As tarefas e problemas delegados não são exibidos nas ferramentas de gerenciamento de recursos, como o [!UICONTROL Balanceador de carga de trabalho] ou o [!UICONTROL Planejador de recursos] para os usuários delegados.
* Você pode exibir o trabalho delegado e os nomes de delegados em várias áreas do [!DNL Workfront]. Para obter mais informações, consulte a seção &quot;Localizar trabalho delegado e informações delegadas&quot; no artigo [Gerenciar delegação de tarefas e problemas](../delegate-work/how-to-delegate-work.md).


  >[!IMPORTANT]
  >
  >  Se um usuário tiver somente o acesso de Visualização às tarefas em seu nível de acesso e você tiver permissões de Gerenciamento nas tarefas que você delegar a ele, ele receberá permissões de Gerenciamento para as tarefas que você delegar a ele. No entanto, eles não poderão executar as mesmas ações que você nas tarefas delegadas. Eles devem solicitar ao administrador do sistema o acesso para Editar tarefas para poderem atualizá-las quando estiverem ausentes.

* Interromper a delegação não remove as permissões concedidas aos usuários delegados sobre as tarefas e problemas em que foram delegados.
* Se um sistema ou desativar o [!UICONTROL Permitir que os usuários deleguem tarefas e problemas] configuração no [!UICONTROL Configuração] , os usuários atualmente delegados serão removidos das tarefas e problemas para os quais foram delegados anteriormente. As permissões para as tarefas ou problemas não são removidas.

## Diferenças e semelhanças entre atribuições e delegações

| Ação | Atribuições | Delegações |
|--------------------------------------------------------------------------------------------------------------------------------|---------------------------------------|-----------------------------------------------------|
| Um usuário atribuído ou delegado pode editar ou excluir o item de trabalho ao qual está atribuído ou ao qual está delegado | Com base em permissões e nível de acesso | Com base em permissões e nível de acesso |
| Um usuário atribuído ou delegado é exibido no cabeçalho do item de trabalho | Sim | Sim |
| As tarefas ou problemas atribuídos ou delegados são exibidos na área Página inicial do destinatário ou delegado | Sim, até que o item seja concluído | Sim, somente para o período da delegação |
| Você pode atribuir ou delegar trabalho a usuários na área Página inicial | Sim | Sim |
| Você pode atribuir ou delegar trabalho aos usuários usando a | Sim | Não |
| Você pode atribuir ou delegar trabalho aos usuários em uma lista ou a partir do cabeçalho de um item de trabalho | Sim | Não |
| Qualquer usuário pode atribuir ou delegar outros usuários com itens de trabalho aos quais eles não estão associados | Com base em permissões e nível de acesso | Não. Somente o destinatário pode delegar seus próprios itens. |
| As horas planejadas, reais ou orçadas do trabalho atribuído ou delegado a um usuário são exibidas para esse usuário nas ferramentas de gerenciamento de recursos | Sim | Não |
