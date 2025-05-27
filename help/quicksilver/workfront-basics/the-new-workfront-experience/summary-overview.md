---
content-type: overview
title: Visão geral do resumo
description: Você pode usar o painel Resumo para revisar e atualizar as informações do item de trabalho diretamente de uma lista de tarefas, problemas, documentos ou de outras áreas do  [!DNL Adobe Workfront]  que exibem tarefas e problemas.
feature: Get Started with Workfront
author: Nolan
exl-id: 5e4026b2-5f2f-45c1-bef1-04e20c62ed8a
source-git-commit: 66fc75ed9a7fca4b44ac776c314a6e08a6fbd450
workflow-type: tm+mt
source-wordcount: '986'
ht-degree: 2%

---

# Visão geral do [!UICONTROL Resumo]

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span> -->

Você pode usar o painel [!UICONTROL Resumo] para revisar e atualizar informações de item de trabalho diretamente de uma lista de tarefas, problemas, documentos ou de outras áreas do [!DNL Adobe Workfront] que exibem tarefas e problemas.

O administrador do Workfront ou de grupo pode modificar as áreas e os campos exibidos no painel Resumo. Eles podem adicionar até 16 campos ao painel Resumo.

>[!IMPORTANT]
>
>Recomendamos adicionar campos que você deve atualizar com frequência no Painel de resumo, para que possa acessá-los e atualizá-los facilmente sem acessar a página principal do objeto.
>
>Por exemplo, você pode adicionar os seguintes campos atualizados com frequência aos painéis Resumo de tarefas e problemas:
>
>* Status
>* Percentual concluído
>* Data de confirmação
>* Data de conclusão planejada
>* Condição



A tabela a seguir exibe as áreas em que você pode localizar e usar o painel [!UICONTROL Resumo]:

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td><b>Tarefas</b></td> 
  </tr> 
  <tr> 
   <td> <p>Listas de tarefas em um</p> 
    <ul> 
     <li>Projeto</li> 
     <li>Subtarefa</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>Tarefas nas áreas de trabalho [!UICONTROL Não atribuído] e [!UICONTROL Atribuído] do [!UICONTROL Balanceador de carga de trabalho]</td> 
  </tr> 
   <tr> 
   <td>Tarefas em uma [!UICONTROL Planilha de Horas]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><b>Problemas</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Listas de problemas em um</p> 
    <ul> 
     <li>Projeto</li> 
     <li>Tarefa</li> 
     <li>Subtarefa</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemas na área [!UICONTROL Trabalho atribuído] do [!UICONTROL Balanceador de carga de trabalho]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Problemas na seção [!UICONTROL Enviado] da área [!UICONTROL Solicitações]</td> 
  </tr> 
</tr> 
   <tr> 
   <td>Problemas em uma [!UICONTROL Planilha de Horas]</td> 
  </tr>

<tr data-mc-conditions=""> 
   <td><b>Documentos</b></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Área [!UICONTROL Documentos]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Seção [!UICONTROL Documentos] de qualquer objeto (projeto, tarefa, problema, programa, portfólio, modelo, tarefa de modelo, usuário)</td> 
  </tr> 
 </tbody> 
</table>

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront administrators can customize the Summary in the Layout Template. For more information, see <a href="../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md" class="MCXref xref">Create and manage layout templates</a>.</p>
-->

Este artigo descreve como acessar e usar o painel [!UICONTROL Resumo] para tarefas e problemas em listas.

Para obter informações sobre como acessar o [!UICONTROL Resumo] no [!UICONTROL Balanceador de carga de trabalho], consulte [Atualizar itens de trabalho no [!UICONTROL Balanceador de carga de trabalho] usando o [!UICONTROL Resumo]](../../resource-mgmt/workload-balancer/update-items-in-summary-panel-in-workload-balancer.md).

Para obter informações sobre como acessar o [!UICONTROL Resumo] de documentos, consulte o [[!UICONTROL Resumo] para obter a visão geral dos documentos](../../documents/managing-documents/summary-for-documents.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>Novo: Colaborador ou superior</p>
   Ou
   <p>Atual:[!UICONTROL Request] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuração do nível de acesso</strong></td> 
   <td> <p>[!UICONTROL Exibir] ou superior acesso a Tarefas, Problemas, Documentos</p> <p>[!UICONTROL Exibir] ou maior acesso a quaisquer objetos para os quais você deseja exibir documentos [!UICONTROL Resumo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>[!UICONTROL Exibir] ou permissões superiores para uma tarefa, problema ou documento</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront]. Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Exiba o painel [!UICONTROL Resumo] em uma lista de tarefas ou problemas

1. Vá para uma tarefa ou problema e selecione um item na lista.
1. Clique no ícone ![](assets/qs-summary-in-new-toolbar-small.png) do **[!UICONTROL Resumo]**

   ou

   Clique no ícone ![](assets/open-summary-with-text-nwe.png) do **[!UICONTROL Abrir Resumo]** na seção [!UICONTROL Enviado] da área [!UICONTROL Solicitações].

   Após abrir o Resumo, ele permanece aberto quando você clica ou seleciona outras tarefas ou problemas e permanece aberto até que você o feche manualmente.

   >[!TIP]
   >
   >Você só pode selecionar uma tarefa ou um problema por vez para exibir seus detalhes no painel [!UICONTROL Resumo].

   ![Painel de resumo](assets/summary-panel-for-task-new-comments.png)

1. (Opcional) Para fechar o painel [!UICONTROL Resumo], siga um destes procedimentos:

   * Em uma lista de tarefas ou problemas, clique no ícone ![](assets/summary-panel-icon.png) **[!UICONTROL Abrir resumo]**

     Ou

     Clique no ícone **X** no canto superior direito do painel [!UICONTROL Resumo].

   * Na seção [!UICONTROL Enviado] da área [!UICONTROL Solicitações], clique no ícone ![](assets/close-summary-with-text-nwe.png) de **[!UICONTROL Fechar Resumo]**

     Ou

     Clique no ícone **X** no canto superior direito do painel Resumo.

## [!UICONTROL Percentual concluído]

Use a bolha azul de progresso na parte superior do [!UICONTROL Resumo] para atualizar a porcentagem concluída da tarefa ou problema selecionado. Insira um número ou arraste a bolha para a porcentagem correta.

Quando você arrasta e solta a bolha no painel Resumo, a Porcentagem concluída é atualizada em um ponto. Não é possível inserir um número decimal.

![Porcentagem concluída no painel Resumo](assets/summary-overview-percent-complete.png)

## [!UICONTROL Atualizações]

Use a seção [!UICONTROL Atualizações] do [!UICONTROL Resumo] para exibir atualizações recentes e fazer atualizações sobre a tarefa ou problema selecionado. Clique em **[!UICONTROL Ver tudo]** para ir diretamente para a guia [!UICONTROL Atualizações] na tarefa.

![Atualiza a seção no painel Resumo](assets/summary-updates-section.png)

## [!UICONTROL Documentos]

Use a seção [!UICONTROL Documentos] do [!UICONTROL Resumo] para ver documentos anexados à tarefa ou problema selecionado. Clique na miniatura para abrir uma visualização de documento. Para ir diretamente para a guia [!UICONTROL Documentos] na tarefa ou problema, clique no título **[!UICONTROL Documentos]**.

![Seção Documentos no painel Resumo](assets/summary-documents-section.png)

## [!UICONTROL Detalhes]

Use a seção [!UICONTROL Detalhes] do [!UICONTROL Resumo] para exibir detalhes de item de trabalho de alto nível, fazer atribuições ou adicionar datas de início. Clique em **[!UICONTROL Ver tudo]** para ir diretamente para a guia [!UICONTROL Detalhes] na tarefa ou problema.



![Seção de detalhes no painel Resumo](assets/summary-details-section.png)

## [!UICONTROL Subtarefas]

Esta seção só está disponível para tarefas. Use a seção [!UICONTROL Subtarefas] do [!UICONTROL Resumo] para exibir as subtarefas [!UICONTROL Novas], [!UICONTROL Em Andamento] e [!UICONTROL Fechadas] na tarefa selecionada. Clique no menu suspenso **[!UICONTROL Status]** para alternar entre os status. Para ir diretamente para a guia [!UICONTROL Subtarefas] na tarefa, clique no &#x200B; **[!UICONTROL Subtarefas]**.

Se você não tiver adicionado subtarefas à tarefa, clique em **[!UICONTROL Adicionar uma aqui]** para ir diretamente para a guia [!UICONTROL Subtarefas] da tarefa.

![Seção de subtarefas no painel Resumo](assets/summary-subtasks-section.png)

## [!UICONTROL Horas]

Use a seção [!UICONTROL Horas] do [!UICONTROL Resumo] para registrar horas na tarefa ou problema selecionado. Clique em **[!UICONTROL Registrar Tempo]** e insira suas horas. Para ir diretamente para a guia Horas na tarefa ou problema, clique no título **[!UICONTROL Horas]**.

A contagem de horas no [!UICONTROL Resumo] exibe as horas que você registra. Outros usuários terão diferentes totais de horas no [!UICONTROL Resumo], dependendo do tempo que fizerem logon na tarefa.

Se não houver [!UICONTROL horas] planejadas na tarefa ou problema e você tiver feito o logon, a barra de horas aparecerá em vermelho.

![Seção de horas no painel Resumo](assets/summary-hours-section.png)

## Aprovações

Use a seção [!UICONTROL Aprovações] do [!UICONTROL Resumo] para exibir aprovações anexadas à tarefa ou problema selecionado. Se você não tiver adicionado nenhuma aprovação, selecione uma aprovação existente do menu suspenso ou clique em **[!UICONTROL Criar processo de aprovação de uso único]** para ir diretamente para a guia [!UICONTROL Aprovações] na tarefa ou problema.

Para ir diretamente para a guia [!UICONTROL Aprovações] na tarefa ou problema, clique no título **[!UICONTROL Aprovações]**.

![Seção Aprovações no painel Resumo](assets/summary-approvals-section.png)
