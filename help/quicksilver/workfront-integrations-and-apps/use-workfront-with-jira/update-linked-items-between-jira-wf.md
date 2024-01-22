---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Atualizar itens vinculados entre [!DNL Jira] e [!DNL Adobe Workfront]
description: Ao vincular [!DNL Jira] problemas para [!DNL Adobe Workfront] tarefas ou problemas, os usuários podem atualizar itens em um aplicativo e a contrapartida desse item também é atualizada para os usuários que trabalham no segundo aplicativo.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: e01f5eaf3133fa1bdaedf4dad56e9a8175b70667
workflow-type: tm+mt
source-wordcount: '1570'
ht-degree: 0%

---

# Atualizar itens vinculados entre [!DNL Jira] e [!DNL Adobe Workfront]

Ao vincular [!DNL Jira] problemas para [!DNL Adobe Workfront] tarefas ou problemas, os usuários podem atualizar itens em um aplicativo e a contrapartida desse item também é atualizada para os usuários que trabalham no segundo aplicativo.

Para obter mais informações sobre como vincular itens entre [!DNL Workfront] e [!DNL Jira], consulte [Vincular itens entre o Adobe Workfront e o Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Como você está configurando [!DNL Workfront] para [!DNL Jira], como [!DNL Jira] administrador do sistema, você pode configurar determinados campos de um aplicativo para sincronizar com campos de itens vinculados no outro aplicativo.

Para obter mais informações sobre como sincronizar campos entre [!DNL Jira] e [!DNL Workfront] itens, consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

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
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no [!DNL Jira] e [!DNL Workfront] para se dedicar a essa integração, em vez de usar as existentes que podem ser anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador.</p> </td> 
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

## Atualizar itens vinculados no [!DNL Workfront]

Se você trabalha principalmente no [!DNL Workfront], você pode atualizar seus itens de trabalho no [!DNL Workfront] e os seus homólogos em [!DNL Jira] também atualizar. Essa atualização ocorre por meio da integração do [!DNL Workfront] para [!DNL Jira] que não exige um [!DNL Jira] licença.

Contanto que seu [!DNL Workfront] administrador configurou [!DNL Workfront for Jira] para sincronizar os campos entre itens vinculados, determinados campos que você atualiza em [!DNL Workfront] também atualizar para o vinculado [!DNL Jira] problema. Para obter mais informações sobre a atualização de itens em [!DNL Workfront], consulte [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md) e [Editar tarefas](../../manage-work/tasks/manage-tasks/edit-tasks.md).

A lista a seguir mostra quais [!DNL Workfront] campos sincronizar com [!DNL Jira] campos em itens vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Atualizado [!DNL Workfront] campo</strong> </th> 
   <th><strong>Sincronizado [!DNL Jira] campo/ atualização</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Nome da Tarefa ou Problema]</td> 
   <td> <p>[!UICONTROL Nome do problema]</p> <p>Um comentário sobre a Alteração de nome é adicionado à guia <strong>[!DNL Workfront]</strong> guia do [!DNL Jira] problema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Descrição de Problema ou Tarefa]</td> 
   <td> <p> [!UICONTROL Descrição do Problema]</p> <p>Um comentário sobre a Descrição atualizada é adicionado à <strong>[!DNL Workfront]</strong> guia do [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Carregou Documentos]</p> <p>Observação: Documentos vinculados ao [!DNL Workfront] os itens de um servidor externo não são transferidos para [!DNL Jira] problemas. Somente documentos carregados diretamente no [!DNL Workfront] Os itens também são atualizados para a variável [!DNL Jira] problemas. </p> </td> 
   <td> <p>[!UICONTROL Anexos]</p> <p>Um comentário sobre os anexos carregados é adicionado à <strong>[!DNL Workfront]</strong> guia do [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Término Planejada]</td> 
   <td> <p>[!UICONTROL Data de Conclusão]</p> <p>Um comentário sobre a alteração da [!UICONTROL Data de vencimento] é adicionado à [!DNL Workfront] guia do [!DNL Jira] problema. </p> <p>Observação: você deve ativar <strong>[!UICONTROL Data de Conclusão]</strong> para seu [!DNL Jira] problemas para ver esse campo atualizado na [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado e campos personalizados</td> 
   <td> <p> Exibir no [!DNL Workfront] painel direito do [!DNL Jira] problema. <br>Somente os Campos personalizados com um valor real são exibidos no painel.<br></p> <p>Observação: as seções de Formulário personalizado são exibidas com o nível de acesso do [!DNL Workfront] administrador. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema ou Prioridade de Tarefa]</td> 
   <td>Exibições no [!DNL Workfront] painel direito do [!DNL Jira] problema. <br>Isso não atualiza o problema <strong>[!UICONTROL Prioridade]</strong> campo em [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tempo de Log] </td> 
   <td> <p>Um comentário sobre o tempo reportado é adicionado na variável <strong>[!DNL Workfront]</strong> guia do [!DNL Jira] problema. Isso inclui o nome do usuário que registra o horário, bem como o usuário para quem o horário está registrado, caso sejam diferentes. Não há tempo registrado no <strong>[!UICONTROL Log de trabalho]</strong> guia em [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentários]</td> 
   <td> <p>O comentário é adicionado à guia <strong>[!DNL Workfront]</strong> guia do [!DNL Jira] problema. Não é adicionado à variável <strong>[!UICONTROL Comentários]</strong> guia do [!DNL Jira] problema</p> <p>Observação: ao vincular dois itens existentes manualmente, os comentários que foram adicionados ao [!DNL Workfront] item antes de vinculá-lo a [!DNL Jira] não sincronize com o [!DNL Jira] problema. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizar itens vinculados no [!DNL Jira]

Se você trabalha principalmente no [!DNL Jira], você pode atualizar seus itens de trabalho no [!DNL Jira] e os seus homólogos em [!DNL Workfront] também atualizar. Você não precisa ter um [!DNL Workfront] licença para o [!DNL Workfront] itens vinculados ao seu [!DNL Jira] problemas para receber as atualizações que você está fazendo em [!DNL Jira].

Na condição de que o seu [!DNL Workfront] administrador configurou [!DNL Workfront] para [!DNL Jira] para sincronizar os campos entre itens vinculados, determinados campos que você atualiza em [!DNL Jira] também atualizar para o vinculado [!DNL Workfront] item.

A lista a seguir mostra quais [!DNL Jira] campos sincronizar com [!DNL Workfront] campos em itens vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Atualizado [!DNL Jira] Campo</strong> </th> 
   <th><strong>Sincronizado [!DNL Workfront] Campo/ atualização</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Status de Problema]</td> 
   <td> <p> [!UICONTROL Status de Problema ou Tarefa]</p> <p>Status do problema no [!DNL Jira] sincroniza com os seguintes status, ou status que correspondem aos seguintes status, no Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Novo] ([!UICONTROL NOVO])</p> </li> 
     <li> <p>[!UICONTROL Em Andamento] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Fechado]/[!UICONTROL Concluído] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Observação: a variável [!DNL Jira] o status é sincronizado com o primeiro [!DNL Workfront] Status que equivale ao status apropriado.</p> <p>Para obter mais informações sobre os status dos itens em [!DNL Workfront], consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</p> </td> 
  </tr>
  <tr> 
   <td>[!UICONTROL Anexos de Problemas]</td> 
   <td> [!UICONTROL Documentos de Problemas ou de Tarefas]<br>Um comentário sobre o upload de um novo documento no [!DNL Jira] é adicionado à guia [!UICONTROL Atualizações] do [!DNL Workfront] problema ou tarefa.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de Conclusão]</td> 
   <td> <p> Um comentário sobre a alteração da [!UICONTROL Data de Conclusão] em [!DNL Jira] é adicionado à guia [!UICONTROL Atualizações] do [!DNL Workfront] problema ou tarefa. </p> <p>Observação: nenhuma data é alterada no [!DNL Workfront] problema ou tarefa. </p> </td> 
  </tr> 
  <tr> 
   <td> Registrar o tempo no [!DNL Workfront] painel direito ou no menu [!UICONTROL Mais] no painel [!DNL Jira] problema<br></td> 
   <td> <p>Horas<br>Além de adicionar as horas conectadas no Jira ao vinculado [!DNL Workfront] item, um comentário sobre o tempo de registro em log é adicionado à guia [!UICONTROL Atualizações] do [!DNL Workfront] item.</p> <p>Para obter mais informações sobre o tempo de registro em [!DNL Jira] problemas, incluindo a atualização do [!DNL Jira] usuário que está registrando o horário em [!DNL Workfront], consulte <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Registrar o tempo de vinculação [!DNL Jira] e [!DNL Workfront] itens</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comentários <br><br></td> 
   <td> <p>Comentários são adicionados à guia [!UICONTROL Atualizações] do [!DNL Workfront] problema ou tarefa se a variável <strong>[!UICONTROL Comentários]</strong> na seção [!UICONTROL SYNCHRONIZE FROM JIRA TO WORKFRONT] da guia [!UICONTROL Setup] para <strong>[!UICONTROL Sempre]</strong>.</p> <p>Para obter informações sobre como definir as configurações do Workfront em [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuração [!DNL Workfront for Jira]</a>.</p> <p>Para obter informações sobre comentários em itens de [!DNL Jira] problemas, consulte <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comentário de um vinculado [!DNL Jira] problema</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Registrar o tempo a partir de vinculado [!DNL Jira] problemas

O tempo que você grava para um [!DNL Jira] item em [!DNL Jira] também serão transferidas para o [!DNL Workfront] item, independentemente de onde em [!DNL Jira] você registra o horário.\
Quando você registra horas em Jira no [!DNL Workfront] , a hora é registrada somente em [!DNL Workfront].\
A hora em que você grava em [!DNL Workfront] não afeta a hora do problema vinculado no [!DNL Jira].

>[!NOTE]
>
>Se o horário for adicionado a um [!DNL Jira] item vinculado a um [!DNL Workfront] tarefa, a variável [!UICONTROL Tipo de Hora] para o tempo em [!DNL Workfront] é [!UICONTROL Tempo em Tarefa]. Se o horário for adicionado a um [!DNL Jira] item vinculado a um [!DNL Workfront] problema, a variável [!UICONTROL Tipo de Hora] para o tempo em [!DNL Workfront] é [!UICONTROL Hora do Problema].

Um comentário é adicionado à **[!DNL Workfront]** guia em [!DNL Jira] e para o **[!UICONTROL Atualizações]** guia do item em [!DNL Workfront] para registrar o registro de tempo.\
A hora também é exibida no campo **[!UICONTROL Horas]** guia do [!DNL Workfront] item.

* [Registrar o tempo de vinculação [!DNL Jira] e [!DNL Workfront] itens](#log-time-for-linked-jira-and-workfront-items)
* [Registrar o tempo desde [!DNL Jira] para um [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Registrar o tempo de vinculação [!DNL Jira] e [!DNL Workfront] itens

Você pode registrar o tempo de um [!DNL Jira] problema vinculada a um [!DNL Workfront] item, e a hora é registrada tanto no [!DNL Jira] problema, bem como a [!DNL Workfront] item.

>[!IMPORTANT]
>
>Se o usuário fizer logon na [!DNL Jira] não existe no [!DNL Workfront], a integração cria um novo usuário ativo no Workfront se a variável **[!UICONTROL Criar automaticamente um usuário no [!DNL Workfront]&#x200B;se a variável [!DNL Jira] o usuário não tem um *[!DNL Workfront]&#x200B;account]** está definido como**[!UICONTROL  Sempre ]**. Este usuário não ocupa um [!DNL Workfront] licença. Você pode atribuir usuários ativos a itens de trabalho no [!DNL Workfront], mas não é possível incluí-los em atualizações. Para obter informações sobre como configurar a criação automática de [!DNL Workfront] usuários de [!DNL Jira], consulte [Configuração [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Para registrar o tempo de um item em [!DNL Jira] e registre-o em [!DNL Jira] e [!DNL Workfront]:

1. Efetue logon no [!DNL Jira].
1. Vá para a [!DNL Jira] problema vinculada à variável [!DNL Workfront] item.
1. Expanda a **[!UICONTROL Mais]** e clique em **[!UICONTROL Registrar trabalho]**.

1. No **[!UICONTROL Tempo gasto]** especifique o tempo gasto trabalhando nesta ocorrência. Você deve especificar a hora usando os seguintes períodos:

   * [!UICONTROL Semanas] w)
   * [!UICONTROL Dias] d)
   * [!UICONTROL Horas] h)

1. Continue adicionando informações à sua entrada de tempo, incluindo uma **[!UICONTROL Descrição do trabalho]** e, em seguida, clique em **[!UICONTROL Log]**.\
   A hora é adicionada à variável **[!UICONTROL Log de trabalho]** guia do [!DNL Jira] item, bem como à [!DNL Workfront] item vinculado a ele.\
   A descrição de trabalho da entrada de tempo é registrada como uma nota na entrada de hora em [!DNL Workfront].

### Registrar o tempo desde [!DNL Jira] para um [!DNL Workfront] item

Você pode registrar horas apenas no link vinculado [!DNL Workfront] item do [!DNL Jira] problema sem gravar este horário na [!DNL Jira] problema.

1. Efetue logon no [!DNL Jira].
1. Navegue até um [!DNL Jira] problema que está vinculada a um [!DNL Workfront] item.

   Os detalhes do [!DNL Workfront] o item deve ser exibido no [!DNL Workfront] painel direito do problema.

1. Clique em **[!UICONTROL Registro de tempo]** ícone.

1. Especificar a quantidade de **[!UICONTROL Horas]** e **[!UICONTROL Minutes]** registre o problema.

1. Clique em **[!UICONTROL Registro de tempo]**.

   A hora é adicionada à variável [!DNL Workfront] item.

   Este horário não é adicionado ao [!UICONTROL Log de trabalho] guia do [!DNL Jira] problema.

## Comentário de um vinculado [!DNL Jira] problema {#comment-from-a-linked-jira-issue}

Quando você comenta em um [!DNL Jira] item do [!DNL Workfront] painel direito no [!DNL Jira], o comentário também é adicionado à [!UICONTROL Atualizações] do item vinculado no Workfront.

Para comentar de [!DNL Jira] para um [!DNL Workfront] item:

1. Efetue logon no [!DNL Jira].
1. Navegue até um [!DNL Jira] problema que está vinculada a um [!DNL Workfront] item.

   Os detalhes do [!DNL Workfront] o item deve ser exibido no [!DNL Workfront] painel direito do problema.

1. Clique em **[!UICONTROL Comentários]** ícone no [!DNL Workfront] ou no painel **[!UICONTROL Comentários]** guia.

1. Comece a digitar um comentário e clique em **[!UICONTROL Enviar]**.

   O comentário é adicionado ao seguinte:

   * A variável **[!DNL Workfront]** guia do [!DNL Jira] problema.
   * A variável **[!UICONTROL Comentários]** guia do [!DNL Jira] problema.
   * A variável **[!UICONTROL Atualizações]** do item vinculado no Workfront.
