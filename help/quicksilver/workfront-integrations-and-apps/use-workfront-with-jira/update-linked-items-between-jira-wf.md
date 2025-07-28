---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Atualizar itens vinculados entre [!DNL Jira] e [!DNL Adobe Workfront]
description: Quando você vincula [!DNL Jira] problemas a [!DNL Adobe Workfront] tarefas ou problemas, seus usuários podem atualizar itens em um aplicativo e a contraparte desse item também é atualizada para os usuários que trabalham no segundo aplicativo.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '1700'
ht-degree: 0%

---

# Atualizar itens vinculados entre [!DNL Jira] e [!DNL Adobe Workfront]

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Jira não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Jira.
>
>Oito modelos de Automação e Integração do Workfront prontos para uso para Jira estarão disponíveis até agosto para ajudar a replicar fluxos de trabalho comuns e acelerar a implementação. Os modelos são totalmente personalizáveis para atender às necessidades específicas dos negócios e podem ser estendidos à medida que os requisitos evoluem.
> 
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Jira, consulte [módulos do Software Jira](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

Quando você vincula [!DNL Jira] problemas a [!DNL Adobe Workfront] tarefas ou problemas, seus usuários podem atualizar itens em um aplicativo e a contrapartida desse item também é atualizada para os usuários que trabalham no segundo aplicativo.

Para obter mais informações sobre como vincular itens entre [!DNL Workfront] e [!DNL Jira], consulte [Vincular itens entre o Adobe Workfront e a Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Como você está configurando o [!DNL Workfront] para [!DNL Jira], como administrador do sistema do [!DNL Jira], é possível configurar determinados campos de um aplicativo para sincronizá-los com campos de itens vinculados no outro aplicativo.

Para obter mais informações sobre como sincronizar campos entre itens [!DNL Jira] e [!DNL Workfront] vinculados, consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td><p>Novo: Qualquer um</p>
       <p>ou</p>
       <p>Atual: [!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td><p>Novo: [!UICONTROL Padrão]</p>
       <p>ou</p>
       <p>Atual: [!UICONTROL Plano]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no [!DNL Jira] e no [!DNL Workfront] para se dedicar a essa integração, em vez de usar as existentes que podem estar anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador [!DNL Workfront].</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Pré-requisitos

Antes de vincular itens entre [!DNL Workfront] e [!DNL Jira], você deve:

* Instalar [!DNL Workfront for Jira].

  Para obter instruções sobre como instalar o [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront for Jira].

  Para obter instruções sobre como configurar o [!DNL Workfront for Jira], consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Vincular itens entre [!DNL Workfront] e [!DNL Jira].

  Para obter instruções, consulte [Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Atualizar itens vinculados em [!DNL Workfront]

Se você trabalhar principalmente no [!DNL Workfront], poderá atualizar seus itens de trabalho no [!DNL Workfront] e os equivalentes no [!DNL Jira] também poderão ser atualizados. Esta atualização acontece por meio da integração do [!DNL Workfront] para [!DNL Jira], que não requer uma licença do [!DNL Jira].

Desde que o administrador do [!DNL Workfront] tenha configurado o [!DNL Workfront for Jira] para sincronizar os campos entre itens vinculados, determinados campos que você atualiza no [!DNL Workfront] também serão atualizados para o problema [!DNL Jira] vinculado. Para obter mais informações sobre como atualizar itens em [!DNL Workfront], consulte [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md) e [Editar tarefas](../../manage-work/tasks/manage-tasks/edit-tasks.md).

A lista a seguir mostra quais campos do [!DNL Workfront] são sincronizados com os campos do [!DNL Jira] em itens vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo [!DNL Workfront] atualizado</strong> </th> 
   <th><strong>Campo/atualização [!DNL Jira] sincronizado</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome da Tarefa ou Problema]</td> 
   <td> <p>[!UICONTROL Nome do problema]</p> <p>Um comentário sobre a Alteração de nome é adicionado à guia <strong>[!DNL Workfront]</strong> do problema [!DNL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Descrição de Problema ou Tarefa]</td> 
   <td> <p> [!UICONTROL Descrição do Problema]</p> <p>Um comentário sobre a Descrição atualizada é adicionado à guia <strong>[!DNL Workfront]</strong> do problema [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Carregou Documentos]</p> <p>Observação: documentos vinculados a [!DNL Workfront] itens de um servidor externo não são transferidos para [!DNL Jira] problemas. Somente documentos carregados diretamente em [!DNL Workfront] itens também são atualizados para os [!DNL Jira] problemas vinculados. </p> </td> 
   <td> <p>[!UICONTROL Anexos]</p> <p>Um comentário sobre os anexos carregados é adicionado à guia <strong>[!DNL Workfront]</strong> do problema [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Término Planejada]</td> 
   <td> <p>[!UICONTROL Data de Conclusão]</p> <p>Um comentário sobre a alteração da [!UICONTROL Data de Conclusão] é adicionado à guia [!DNL Workfront] do problema [!DNL Jira]. </p> <p>Observação: você deve habilitar a <strong>[!UICONTROL Data de Conclusão]</strong> para que seus problemas [!DNL Jira] possam ver esse campo atualizado na [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado e campos personalizados</td> 
   <td> <p> Exibir no painel direito [!DNL Workfront] do problema [!DNL Jira]. <br>Somente os Campos Personalizados que têm um valor real são exibidos no painel.<br></p> <p>Observação: as seções de Formulário personalizado são exibidas com o nível de acesso do administrador [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema ou Prioridade de Tarefa]</td> 
   <td>Exibido no painel direito [!DNL Workfront] do problema [!DNL Jira]. <br>Ele não atualiza o campo <strong>[!UICONTROL Priority]</strong> do problema em [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo de Log] </td> 
   <td> <p>Um comentário sobre o tempo registrado é adicionado na guia <strong>[!DNL Workfront]</strong> do problema [!DNL Jira]. Isso inclui o nome do usuário que registra o horário, bem como o usuário para quem o horário está registrado, caso sejam diferentes. Não há tempo registrado na guia <strong>[!UICONTROL Log de trabalho]</strong> em [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentários]</td> 
   <td> <p>O comentário é adicionado à guia <strong>[!DNL Workfront]</strong> do problema [!DNL Jira]. Não foi adicionado à guia <strong>[!UICONTROL Comentários]</strong> do problema [!DNL Jira]</p> <p>Observação: ao vincular dois itens existentes manualmente, os comentários adicionados ao item [!DNL Workfront] antes de vinculá-lo a [!DNL Jira] não são sincronizados com o problema [!DNL Jira]. </p> <p>Comentários Jira sincronizam com o Workfront.</td> 
  </tr> 
 </tbody> 
</table>

## Atualizar itens vinculados em [!DNL Jira]

Se você trabalhar principalmente no [!DNL Jira], poderá atualizar seus itens de trabalho no [!DNL Jira] e os equivalentes no [!DNL Workfront] também poderão ser atualizados. Você não precisa ter uma licença do [!DNL Workfront] para os itens do [!DNL Workfront] vinculados aos seus problemas do [!DNL Jira] para receber as atualizações que você está fazendo no [!DNL Jira].

Condição de o administrador do [!DNL Workfront] ter configurado o [!DNL Workfront] para [!DNL Jira] sincronizar os campos entre itens vinculados, determinados campos que você atualizar no [!DNL Jira] também serão atualizados para o item [!DNL Workfront] vinculado.

A lista a seguir mostra quais campos do [!DNL Jira] são sincronizados com os campos do [!DNL Workfront] em itens vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Campo [!DNL Jira] Atualizado</strong> </th> 
   <th><strong>Campo/Atualização [!DNL Workfront] Sincronizado</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Status de Problema]</td> 
   <td> <p> [!UICONTROL Status de Problema ou Tarefa]</p> <p>O status de problema em [!DNL Jira] sincroniza com os seguintes status, ou status que correspondem aos seguintes status, no Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Novo] ([!UICONTROL NOVO])</p> </li> 
     <li> <p>[!UICONTROL Em Andamento] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Fechado]/[!UICONTROL Concluído] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Observação: o status [!DNL Jira] sincroniza com o primeiro status [!DNL Workfront] que equivale ao status apropriado.</p> <p>Para obter mais informações sobre os status dos itens em [!DNL Workfront], consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Anexos de Problemas]</td> 
   <td> [!UICONTROL Documentos de Problemas ou de Tarefas]<br>Um comentário sobre o carregamento de um novo documento em [!DNL Jira] foi adicionado à guia [!UICONTROL Atualizações] do problema ou da tarefa [!DNL Workfront].  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Conclusão]</td> 
   <td> <p> Um comentário sobre a alteração da [!UICONTROL Data de Conclusão] em [!DNL Jira] é adicionado à guia [!UICONTROL Atualizações] da tarefa ou problema [!DNL Workfront]. </p> <p>Observação: nenhuma data foi alterada no problema ou na tarefa [!DNL Workfront]. </p> </td> 
  </tr> 
  <tr> 
   <td> Registrar tempo no painel direito [!DNL Workfront] ou no menu [!UICONTROL Mais] sobre o problema [!DNL Jira]<br></td> 
   <td> <p>Horas<br>Além de adicionar as horas registradas no Jira ao item [!DNL Workfront] vinculado, um comentário sobre o tempo de registro é adicionado à guia [!UICONTROL Atualizações] do item [!DNL Workfront].</p> <p>Para obter mais informações sobre o tempo de registro em log de problemas de [!DNL Jira] vinculados, incluindo a atualização do usuário [!DNL Jira] que está registrando o tempo em [!DNL Workfront], consulte <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Tempo de registro para itens [!DNL Jira] e [!DNL Workfront] vinculados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comentários <br><br></td> 
   <td> <p>Comentários são adicionados à guia [!UICONTROL Atualizações] do problema ou tarefa [!DNL Workfront] se a configuração <strong>[!UICONTROL Comentários]</strong> na seção [!UICONTROL SINCRONIZAR DE JIRA PARA WORKFRONT] da guia [!UICONTROL Instalação] para <strong>[!UICONTROL Sempre]</strong>.</p> <p>Para obter informações sobre como definir as configurações do Workfront em [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configurando [!DNL Workfront for Jira]</a>.</p> <p>Para obter informações sobre como comentar em itens de [!DNL Jira] problemas vinculados, consulte <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comentário de um [!DNL Jira] problema vinculado</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Registrar em log o tempo de [!DNL Jira] problemas vinculados

O horário em que você gravar para um item [!DNL Jira] em [!DNL Jira] também será transferido para o item [!DNL Workfront] vinculado, independentemente de onde você registra o horário em [!DNL Jira].\
Ao registrar horas no Jira no painel [!DNL Workfront], as horas são registradas somente em [!DNL Workfront].\
A hora em que você grava em [!DNL Workfront] não afeta a hora do problema vinculado em [!DNL Jira].

>[!NOTE]
>
>Se o horário for adicionado a um item [!DNL Jira] vinculado a uma tarefa [!DNL Workfront], o [!UICONTROL Tipo de Hora] do horário em [!DNL Workfront] será [!UICONTROL Tempo de Tarefa]. Se a hora for adicionada a um item [!DNL Jira] vinculado a um problema [!DNL Workfront], o [!UICONTROL Tipo de Hora] do tempo em [!DNL Workfront] será [!UICONTROL Tempo de Problema].

Um comentário é adicionado à guia **[!DNL Workfront]** em [!DNL Jira] e à guia **[!UICONTROL Atualizações]** do item em [!DNL Workfront] para registrar o registro de tempo.\
O horário também é exibido na guia **[!UICONTROL Horas]** do item [!DNL Workfront].

* [Registrar horas de  [!DNL Jira] e [!DNL Workfront] itens](#log-time-for-linked-jira-and-workfront-items) vinculados
* [Registrar o tempo de [!DNL Jira] a um [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Registrar o tempo para os itens [!DNL Jira] e [!DNL Workfront] vinculados

Você pode registrar o tempo de um problema [!DNL Jira] vinculado a um item [!DNL Workfront], e o tempo é registrado no problema [!DNL Jira] e no item [!DNL Workfront].

>[!IMPORTANT]
>
>Se o usuário que registra o tempo em [!DNL Jira] não existir em [!DNL Workfront], a integração criará um novo usuário ativo no Workfront se o **[!UICONTROL Criar automaticamente um usuário em [!DNL Workfront]&#x200B;se o usuário [!DNL Jira] não tiver uma *[!DNL Workfront] &#x200B;conta]** definida como&#x200B;**[!UICONTROL &#x200B; Sempre &#x200B;]**. Este usuário não ocupa uma licença [!DNL Workfront]. Você pode atribuir usuários ativos a itens de trabalho em [!DNL Workfront], mas não pode incluí-los em atualizações. Para obter informações sobre como configurar a criação automática de [!DNL Workfront] usuários a partir de [!DNL Jira], consulte [Configurando [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Para registrar o tempo de um item em [!DNL Jira] e registrá-lo em [!DNL Jira] e [!DNL Workfront]:

1. Faça logon em [!DNL Jira].
1. Vá para o problema [!DNL Jira] que está vinculado ao item [!DNL Workfront].
1. Expanda o menu **[!UICONTROL Mais]** e clique em **[!UICONTROL Registrar trabalho]**.

1. No campo **[!UICONTROL Tempo gasto]**, especifique a quantidade de tempo gasto trabalhando nesta ocorrência. Você deve especificar a hora usando os seguintes períodos:

   * [!UICONTROL Semanas] (w)
   * [!UICONTROL Dias] (d)
   * [!UICONTROL Horas] (h)

1. Continue adicionando informações à sua entrada de tempo, incluindo uma **[!UICONTROL Descrição do Trabalho]**, e depois clique em **[!UICONTROL Log]**.\
   A hora é adicionada à guia **[!UICONTROL Log de trabalho]** do item [!DNL Jira], bem como ao item [!DNL Workfront] vinculado a ele.\
   A descrição de trabalho da entrada de horas é registrada como uma observação na entrada de horas em [!DNL Workfront].

### Registrar o tempo de [!DNL Jira] em um item [!DNL Workfront]

Você pode registrar horas apenas no item [!DNL Workfront] vinculado a partir do problema [!DNL Jira] sem gravar essa hora no problema [!DNL Jira].

1. Faça logon em [!DNL Jira].
1. Navegue até um problema [!DNL Jira] que esteja vinculado a um item [!DNL Workfront].

   Os detalhes do item [!DNL Workfront] devem ser exibidos no painel direito [!DNL Workfront] do problema.

1. Clique no ícone **[!UICONTROL Log Time]**.

1. Especifique a quantidade de **[!UICONTROL Horas]** e **[!UICONTROL Minutos]** que deseja registrar para a questão.

1. Clique em **[!UICONTROL Log Time]**.

   A hora é adicionada ao item [!DNL Workfront].

   Este horário não é adicionado à guia [!UICONTROL Log de Trabalho] do problema [!DNL Jira].

## Comentário de um problema [!DNL Jira] vinculado {#comment-from-a-linked-jira-issue}

Ao comentar em um item [!DNL Jira] do painel direito [!DNL Workfront] em [!DNL Jira], o comentário também é adicionado à guia [!UICONTROL Atualizações] do item vinculado no Workfront.

Para comentar de [!DNL Jira] para um item [!DNL Workfront]:

1. Faça logon em [!DNL Jira].
1. Navegue até um problema [!DNL Jira] que esteja vinculado a um item [!DNL Workfront].

   Os detalhes do item [!DNL Workfront] devem ser exibidos no painel direito [!DNL Workfront] do problema.

1. Clique no ícone **[!UICONTROL Comentários]** no painel [!DNL Workfront] ou na guia **[!UICONTROL Comentários]**.

1. Comece a digitar um comentário e clique em **[!UICONTROL Enviar]**.

   O comentário é adicionado ao seguinte:

   * A guia **[!DNL Workfront]** do problema [!DNL Jira].
   * A guia **[!UICONTROL Comentários]** do problema [!DNL Jira].
   * A guia **[!UICONTROL Atualizações]** do item vinculado no Workfront.
