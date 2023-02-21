---
product-area: workfront-integrations
navigation-topic: workfront-for-jira
title: Atualizar itens vinculados entre [!DNL Jira] e [!DNL Adobe Workfront]
description: Ao vincular [!DNL Jira] problemas para [!DNL Adobe Workfront] tarefas ou problemas, os usuários podem atualizar itens em um aplicativo e a contrapartida desse item também é atualizada para os usuários que trabalham no segundo aplicativo.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 79ac6ff1-2f7d-4abc-8735-398f6aac5191
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 0%

---

# Atualizar itens vinculados entre [!DNL Jira] e [!DNL Adobe Workfront]

Ao vincular [!DNL Jira] problemas para [!DNL Adobe Workfront] tarefas ou problemas, os usuários podem atualizar itens em um aplicativo e a contrapartida desse item também é atualizada para os usuários que trabalham no segundo aplicativo.

Para obter mais informações sobre a vinculação de itens entre [!DNL Workfront] e [!DNL Jira], consulte [Vincular itens entre a Adobe Workfront e a Jira](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

Como você está configurando [!DNL Workfront] para [!DNL Jira], como um [!DNL Jira] administrador do sistema, você pode configurar determinados campos de um aplicativo para sincronizar com os campos de itens vinculados em outro aplicativo.

Para obter mais informações sobre a sincronização de campos entre campos vinculados [!DNL Jira] e [!DNL Workfront] itens, consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plano</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] visão geral das licenças</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso do administrador do sistema</p> <p>Importante: Recomendamos que você crie contas de administrador de sistema separadas em [!DNL Jira] e [!DNL Workfront] dedicar-se a essa integração, em vez de usar as existentes que podem ser vinculadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Antes de vincular itens entre [!DNL Workfront] e [!DNL Jira], você deve

* Instalar [!DNL Workfront for Jira].

   Para obter instruções sobre como instalar [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

* Configurar [!DNL Workfront for Jira].

   Para obter instruções sobre como configurar [!DNL Workfront for Jira], consulte [Configurar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

* Vincular itens entre [!DNL Workfront] e [!DNL Jira].

   Para obter instruções, consulte [Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md).

## Atualizar itens vinculados em [!DNL Workfront]

Se você trabalhar principalmente em [!DNL Workfront], você pode atualizar seus itens de trabalho em [!DNL Workfront] e os seus homólogos [!DNL Jira] também atualize. Essa atualização ocorre por meio da integração de [!DNL Workfront] para [!DNL Jira] que não exige que você tenha uma [!DNL Jira] licença.

Contanto que seu [!DNL Workfront] administrador configurou [!DNL Workfront for Jira] para sincronizar os campos entre itens vinculados, determinados campos que você atualiza em [!DNL Workfront] também atualizar para o link [!DNL Jira] problema. Para obter mais informações sobre como atualizar itens em [!DNL Workfront], consulte [Editar problemas](../../manage-work/issues/manage-issues/edit-issues.md) e [Editar tarefas](../../manage-work/tasks/manage-tasks/edit-tasks.md).

A lista a seguir mostra qual [!DNL Workfront] campos sincronizam com [!DNL Jira] campos em itens vinculados:

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
   <td>[!UICONTROL Problema ou nome da tarefa]</td> 
   <td> <p>[!UICONTROL Nome da ocorrência]</p> <p>Um comentário sobre a alteração de Nome é adicionado ao <strong>[!DNL Workfront]</strong> da guia [!DNL Jira] problema. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema ou Descrição da tarefa]</td> 
   <td> <p> [!UICONTROL Descrição do problema]</p> <p>Um comentário sobre a Descrição atualizada é adicionado ao <strong>[!DNL Workfront]</strong> da guia [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td> <p> [!UICONTROL Upload Documents]</p> <p>Observação: Documentos ligados a [!DNL Workfront] os itens de um servidor externo não são transferidos para [!DNL Jira] problemas. Somente documentos carregados diretamente no [!DNL Workfront] os itens também são atualizados para o [!DNL Jira] problemas. </p> </td> 
   <td> <p>[!UICONTROL Anexos]</p> <p>Um comentário sobre os anexos carregados é adicionado ao <strong>[!DNL Workfront]</strong> da guia [!DNL Jira] problema.<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de conclusão planejada]</td> 
   <td> <p>[!UICONTROL Data de vencimento]</p> <p>Um comentário sobre a [!UICONTROL Data de vencimento] ter sido alterada é adicionado ao [!DNL Workfront] da guia [!DNL Jira] problema. </p> <p>Observação: Você deve ativar <strong>[!UICONTROL Data de vencimento]</strong> para seu [!DNL Jira] problemas para visualizar esse campo atualizado na [!UICONTROL Jira]. </p> </td> 
  </tr> 
  <tr> 
   <td>Forms personalizado e campos personalizados</td> 
   <td> <p> Exibir no [!DNL Workfront] painel direito do [!DNL Jira] problema. <br>Somente os Campos personalizados que têm um valor real são exibidos no painel.<br></p> <p>Observação: As seções de Formulário personalizado são exibidas com o nível de acesso da variável [!DNL Workfront] administrador. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Problema ou Prioridade da tarefa]</td> 
   <td>É exibido na [!DNL Workfront] painel direito do [!DNL Jira] problema. <br>Ele não atualiza o problema <strong>[!UICONTROL Prioridade]</strong> em [!DNL Jira]. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Log time] </td> 
   <td> <p>Um comentário sobre o tempo registrado é adicionado na variável <strong>[!DNL Workfront]</strong> da guia [!DNL Jira] problema. Isso inclui o nome do usuário que registra a hora, bem como o usuário para o qual a hora foi registrada, caso ele seja diferente. Nenhuma hora é registrada no <strong>[!UICONTROL Log de trabalho]</strong> em [!DNL Jira].<br></p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentários]</td> 
   <td> <p>O comentário é adicionado ao <strong>[!DNL Workfront]</strong> da guia [!DNL Jira] problema. Não é adicionado ao <strong>[!UICONTROL Comentários]</strong> da guia [!DNL Jira] problema</p> <p>Observação: Quando você vincula dois itens existentes manualmente, os comentários que foram adicionados à variável [!DNL Workfront] antes de vinculá-lo a [!DNL Jira] não sincronize com o [!DNL Jira] problema. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizar itens vinculados em [!DNL Jira]

Se você trabalhar principalmente em [!DNL Jira], você pode atualizar seus itens de trabalho em [!DNL Jira] e os seus homólogos [!DNL Workfront] também atualize. Você não precisa ter um [!DNL Workfront] licença para [!DNL Workfront] itens vinculados à sua [!DNL Jira] problemas para receber as atualizações que você está fazendo [!DNL Jira].

Na condição de que [!DNL Workfront] administrador configurou [!DNL Workfront] para [!DNL Jira] para sincronizar os campos entre itens vinculados, determinados campos que você atualiza em [!DNL Jira] também atualizar para o link [!DNL Workfront] item.

A lista a seguir mostra qual [!DNL Jira] campos sincronizam com [!DNL Workfront] campos em itens vinculados:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Atualizado [!DNL Jira] Campo</strong> </th> 
   <th><strong>Sincronizado [!DNL Workfront] Campo/atualização</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Status do problema]</td> 
   <td> <p> [!UICONTROL Problema ou Status da Tarefa]</p> <p>Status da ocorrência em [!DNL Jira] sincroniza com os seguintes status ou status que são iguais aos seguintes status, no Workfront:</p> 
    <ul> 
     <li> <p>[!UICONTROL Novo] ([!UICONTROL NOVO])</p> </li> 
     <li> <p>[!UICONTROL Em Andamento] ([!UICONTROL INP])</p> </li> 
     <li> <p>[!UICONTROL Fechado]/[!UICONTROL Concluído] ([!UICONTROL CLS]/[!UICONTROL CPL])</p> </li> 
    </ul> <p>Observação: O [!DNL Jira] o status é sincronizado com o primeiro [!DNL Workfront] status que é igual ao status apropriado.</p> <p>Para obter mais informações sobre os status dos itens em [!DNL Workfront], consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destinatário do problema]</td> 
   <td> <p> [!UICONTROL Problema ou destinatário da tarefa]</p> <p>Importante: Ao atribuir um item em [!DNL Jira] para um usuário que não tenha um [!DNL Workfront] , a integração cria um novo usuário ativo no [!DNL Workfront] somente quando a opção "[!UICONTROL Criar automaticamente um usuário no [!DNL Workfront] se a variável [!DNL Jira] o usuário não tem um [!DNL Workfront] account]" está definida como [!UICONTROL Sempre]. Esse usuário não ocupa um [!DNL Workfront] licença. Usuários ativos podem ser atribuídos a itens de trabalho em [!DNL Workfront], mas não podem ser incluídos em atualizações. Para obter mais informações sobre como configurar a criação automática de [!DNL Workfront] usuários de [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuração [!DNL Workfront for Jira]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Emitir anexos]</td> 
   <td> [!UICONTROL Problemas ou documentos da tarefa]<br>Um comentário sobre o upload de um novo documento em [!DNL Jira] é adicionado à guia [!UICONTROL Atualizações] do [!DNL Workfront] problema ou tarefa.  </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Data de vencimento]</td> 
   <td> <p> Um comentário sobre a alteração da [!UICONTROL Data de vencimento] em [!DNL Jira] é adicionado à guia [!UICONTROL Atualizações] do [!DNL Workfront] problema ou tarefa. </p> <p>Observação: Nenhuma alteração de datas na [!DNL Workfront] problema ou tarefa. </p> </td> 
  </tr> 
  <tr> 
   <td> Tempo de logon na [!DNL Workfront] painel direito ou no menu [!UICONTROL Mais] na seção [!DNL Jira] problema<br></td> 
   <td> <p>Horas<br>Além de adicionar as horas conectadas em Jira ao link [!DNL Workfront] , um comentário sobre o tempo de registro é adicionado à guia [!UICONTROL Atualizações] da [!DNL Workfront] item.</p> <p>Para obter mais informações sobre tempo de logon no link vinculado [!DNL Jira] , incluindo a atualização do [!DNL Jira] usuário que está fazendo logon [!DNL Workfront], consulte <a href="#log-time-for-linked-jira-and-workfront-items" class="MCXref xref">Tempo de registro para Linked [!DNL Jira] e [!DNL Workfront] items</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> Comentários <br><br></td> 
   <td> <p>Os comentários são adicionados à guia [!UICONTROL Atualizações] da [!DNL Workfront] emissão ou tarefa se a variável <strong>[!UICONTROL Comentários]</strong> na seção [!UICONTROL SINCRONIZAR DO JIRA PARA a WORKFRONT] da guia [!UICONTROL Configuração] para <strong>[!UICONTROL Sempre]</strong>.</p> <p>Para obter informações sobre como definir as configurações do Workfront em [!DNL Jira], consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md">Configuração [!DNL Workfront for Jira]</a>.</p> <p>Para obter informações sobre comentários em itens de links [!DNL Jira] problemas, consulte <a href="#comment-from-a-linked-jira-issue" class="MCXref xref">Comentário de um link [!DNL Jira] problema</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tempo de log do vinculado [!DNL Jira] problemas

A hora que você gravou para um [!DNL Jira] item em [!DNL Jira] também será transferido para o [!DNL Workfront] , independentemente de onde [!DNL Jira] você registra a hora.\
Quando você faz login no tempo em Jira no [!DNL Workfront] , o tempo é registrado somente em [!DNL Workfront].\
A hora em que você gravou [!DNL Workfront] não afeta o tempo do problema vinculado em [!DNL Jira].

>[!NOTE]
>
>Se a hora for adicionada a um [!DNL Jira] item vinculado a um [!DNL Workfront] tarefa, a [!UICONTROL Tipo de hora] para o tempo em [!DNL Workfront] é [!UICONTROL Hora da Tarefa]. Se a hora for adicionada a um [!DNL Jira] item vinculado a um [!DNL Workfront] , o [!UICONTROL Tipo de hora] para o tempo em [!DNL Workfront] é [!UICONTROL Hora de emissão].

Um comentário é adicionado ao **[!DNL Workfront]** em [!DNL Jira] e à **[!UICONTROL Atualizações]** da guia do item em [!DNL Workfront] para registrar o registro da hora.\
A hora também é exibida na variável **[!UICONTROL Horas]** da guia [!DNL Workfront] item.

* [Tempo de registro para Linked [!DNL Jira] e [!DNL Workfront] items](#log-time-for-linked-jira-and-workfront-items)
* [Tempo de registro de [!DNL Jira] para [!DNL Workfront] item](#log-time-from-jira-to-a-workfront-item)

### Tempo de registro para Linked [!DNL Jira] e [!DNL Workfront] items

Você pode registrar o tempo de um [!DNL Jira] problema vinculado a um [!DNL Workfront] e a hora é registrada tanto no [!DNL Jira] , bem como [!DNL Workfront] item.

>[!IMPORTANT]
>
>Se o usuário estiver fazendo logon [!DNL Jira] não existe em [!DNL Workfront], a integração cria um novo usuário ativo no Workfront se a variável **[!UICONTROL Criar automaticamente um usuário no [!DNL Workfront]&#x200B; se a variável [!DNL Jira] o usuário não tem um *[!DNL Workfront]conta &#x200B;]** está definido como**[!UICONTROL  Sempre ]**. Esse usuário não ocupa um [!DNL Workfront] licença. Você pode atribuir usuários ativos a itens de trabalho no [!DNL Workfront], mas não é possível incluí-los em atualizações. Para obter informações sobre como configurar a criação automática de [!DNL Workfront] usuários de [!DNL Jira], consulte [Configuração [!DNL Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md).

Para registrar o tempo de um item em [!DNL Jira] e faça com que registre ambos [!DNL Jira] e [!DNL Workfront]:

1. Faça logon [!DNL Jira].
1. Vá para o [!DNL Jira] problema que está vinculado à variável [!DNL Workfront] item.
1. Expanda o **[!UICONTROL Mais]** e clique em **[!UICONTROL Trabalho de registro]**.

1. No **[!UICONTROL Tempo gasto]** , especifique a quantidade de tempo gasto trabalhando nesse problema. Você deve especificar o tempo usando os seguintes períodos:

   * [!UICONTROL Semanas] d)
   * [!UICONTROL Dias] d)
   * [!UICONTROL Horas] h)

1. Continue adicionando informações à sua entrada de tempo, incluindo uma **[!UICONTROL Descrição do Trabalho]**, depois clique em **[!UICONTROL Log]**.\
   O tempo é adicionado ao **[!UICONTROL Log de trabalho]** da guia [!DNL Jira] , bem como o [!DNL Workfront] item vinculado a ele.\
   A descrição de trabalho da entrada de tempo é registrada como uma nota na entrada de hora em [!DNL Workfront].

### Tempo de registro de [!DNL Jira] para [!DNL Workfront] item

Você pode registrar o tempo apenas para o link [!DNL Workfront] do [!DNL Jira] problema sem gravar essa vez no [!DNL Jira] problema.

1. Faça logon [!DNL Jira].
1. Navegue até um [!DNL Jira] problema vinculado a um [!DNL Workfront] item.

   Os detalhes da [!DNL Workfront] deve ser exibido na [!DNL Workfront] painel direito do problema.

1. Clique no botão **[!UICONTROL Hora de registro]** ícone .

1. Especifique a quantidade de **[!UICONTROL Horas]** e **[!UICONTROL Minutes]** você deseja registrar o problema.

1. Clique em **[!UICONTROL Hora de registro]**.

   O tempo é adicionado ao [!DNL Workfront] item.

   Esse tempo não é adicionado ao [!UICONTROL Log de trabalho] da guia [!DNL Jira] problema.

## Comentário de um link [!DNL Jira] problema {#comment-from-a-linked-jira-issue}

Quando você comenta uma [!DNL Jira] do [!DNL Workfront] painel direito em [!DNL Jira], o comentário também é adicionado ao [!UICONTROL Atualizações] guia do item vinculado no Workfront.

Para comentar de [!DNL Jira] para [!DNL Workfront] item:

1. Faça logon [!DNL Jira].
1. Navegue até um [!DNL Jira] problema vinculado a um [!DNL Workfront] item.

   Os detalhes da [!DNL Workfront] deve ser exibido na [!DNL Workfront] painel direito do problema.

1. Clique no botão **[!UICONTROL Comentários]** no ícone na [!DNL Workfront] ou no **[!UICONTROL Comentários]** guia .

1. Comece digitando um comentário e clique em **[!UICONTROL Enviar]**.

   O comentário é adicionado ao seguinte:

   * O **[!DNL Workfront]** da guia [!DNL Jira] problema.
   * O **[!UICONTROL Comentários]** da guia [!DNL Jira] problema.
   * O **[!UICONTROL Atualizações]** guia do item vinculado no Workfront.
