---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurar [!DNL Adobe Workfront for Jira]
description: Você pode usar [!DNL Adobe Workfront for Jira] para integrar [!DNL Jira] e [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: f22a67cd3235a3111f7b874637ec05f8299de271
workflow-type: tm+mt
source-wordcount: '2400'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Jira]

Você pode usar [!DNL Adobe Workfront for Jira] para integrar [!DNL Jira] e [!DNL Workfront] sistemas.

Depois de instalar o complemento, você pode definir workflows que criam [!DNL Jira] emite automaticamente quando [!DNL Workfront] itens de trabalho são criados. Os itens em ambos os aplicativos são vinculados, e algumas de suas informações são automaticamente atualizadas em ambos os sistemas.

Todos os usuários em [!DNL Workfront] e [!DNL Jira] pode se beneficiar dessa integração. Eles só precisam de uma licença para o sistema em que trabalham mais, e não para ambos os sistemas.

Esse complemento está disponível para a variável [!UICONTROL Servidor] e [!UICONTROL OnDemand] ou [!UICONTROL Cloud]) versões de [!DNL Jira] Software.

Para uma lista de [!DNL Jira] versões que [!DNL Workfront for Jira] atualmente compatível, consulte [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) no [!DNL Atlassian Marketplace].

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] plano]</a>*</td> 
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

Antes de configurar [!DNL Workfront for Jira], você deve

* Instalar [!DNL Workfront for Jira]\
   Para obter instruções sobre como instalar [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurar [!DNL Workfront for Jira]

Ao configurar [!DNL Workfront for Jira] é possível:

* Definir acionadores que criarão [!DNL Jira] itens quando [!DNL Workfront] são criados.
* Especificar quais campos devem sincronizar entre itens vinculados entre [!DNL Jira] e [!DNL Workfront].

>[!NOTE]
>
>* Depois de configurar [!DNL Workfront for Jira] em seu [!DNL Jira] ambiente, tudo [!DNL Jira] os usuários veem um [!DNL Workfront] painel direito em todos [!DNL Jira] itens. O painel contém informações sobre os itens que podem ser vinculados [!DNL Workfront] ou especifica que [!DNL Workfront] os itens estão vinculados a [!DNL Jira] itens.
>* Ao usar a variável [!DNL Jira Server] instalação, somente os problemas associados aos projetos identificados como acionadores da integração do Workfront são exibidos no painel Workfront . Para obter mais informações sobre como configurar acionadores para a variável [!DNL Workfront to Jira] para obter mais informações, consulte [Configurar acionadores para vinculação automática de itens entre [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>




Para configurar [!DNL Workfront for Jira]:

1. Faça logon [!DNL Jira] como [!DNL Jira] administrador.
1. Clique em **[!UICONTROL Configurações]** no principal [!DNL Jira] menu.
1. Clique em **[!UICONTROL Complementos]**, depois clique em **[!UICONTROL Gerenciar complementos]**.

1. Expanda o **[!DNL Workfront]** complemento.
1. Clique em **[!UICONTROL Configurar]**.
1. Siga as instruções para fazer logon no [!DNL Workfront].

   >[!NOTE]
   >
   >[!UICONTROL Workfront] conecta-se a [!DNL Jira] usando o OAuth 2.0, um padrão usado pela maioria das integrações baseadas na Web para a autenticação e a autorização dos usuários.

   Você deve fazer logon no [!DNL Workfront] como [!DNL Workfront] para continuar a configuração.

   >[!NOTE]
   >
   >* Quando for solicitado a inserir o domínio de [!DNL Workfront] digite-a usando este formato: *sua empresa&#39;sDomain.my.workfront.com*. O domínio de sua empresa geralmente é o nome de sua empresa.
   >* A Autenticação aprimorada não está disponível até que um [!DNL Workfront] O administrador o habilita para essa integração.



1. Selecione o **[!UICONTROL Triggers]** para configurar a criação automática de [!DNL Jira] itens como novos [!DNL Workfront] são criados.

   Para obter mais informações sobre como configurar acionadores para o Workfront para [!DNL Jira] para obter mais informações, consulte [Configurar acionadores para vinculação automática de itens entre [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Selecione o **[!UICONTROL Configuração]** para configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront] itens.

   Para obter mais informações sobre como configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront], consulte [Configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront] Itens](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Após definir os acionadores e a sincronização dos campos entre os dois aplicativos, qualquer [!DNL Workfront] usuário que pode criar tarefas ou problemas pode possivelmente acionar a criação de um item em [!DNL Jira]. O usuário pode criar um item se os critérios no item criado corresponderem aos acionadores em [!DNL Jira], mesmo que o usuário não tenha um [!DNL Jira] licença. Além disso, qualquer [!DNL Jira] o usuário pode começar imediatamente a trabalhar no [!DNL Jira] e suas atualizações estão visíveis em [!DNL Workfront], sem que tenham uma [!DNL Workfront] licença. Qualquer atualização em [!DNL Workfront] também estão visíveis no [!DNL Jira] itens.

1. (Opcional) Selecione o **[!UICONTROL Log de atividades]** para revisar qualquer erro que possa ter ocorrido durante a integração.

   Para obter mais informações sobre o [!UICONTROL Log de atividades], consulte [Visualize o [!DNL Jira] [!UICONTROL Log de atividades]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurar acionadores para vinculação automática de itens entre [!DNL Jira] e [!DNL Workfront]

Como [!DNL Jira] administrador do sistema, você pode definir acionadores que criariam problemas automaticamente no [!DNL Jira] quando um item em [!DNL Workfront] satisfaz determinados critérios.

>[!NOTE]
>
>Pode levar até 10 minutos para a integração criar novos problemas no [!DNL Jira].

Considere o seguinte ao configurar o acionamento da criação de [!DNL Jira] itens como [!DNL Workfront] Os itens são criados:

* A integração é unidirecional: Só é possível acionar itens criados no [!DNL Workfront] para ser criado automaticamente em [!DNL Jira]. Não é possível acionar itens criados no [!DNL Jira] para ser criado automaticamente em [!DNL Workfront].
* Não há limite para quantos acionadores você pode ter.
* Se um item criado em [!DNL Workfront] corresponde a mais de um dos acionadores, somente um item é criado em [!DNL Jira]. O item é criado em [!DNL Jira] de acordo com o primeiro acionador (na ordem em que foram definidos em [!DNL Jira]). Todos os outros acionadores são ignorados.
* Somente um item em [!DNL Workfront] pode ser vinculado a um item em Jira. Você nunca pode vincular um [!DNL Workfront] item para múltiplo [!DNL Jira] problemas ou um [!DNL Jira] problema para vários [!DNL Workfront] itens.

Para configurar acionadores para criar itens automaticamente no [!DNL Jira]:

1. Faça logon [!DNL Jira] como administrador do sistema.
1. Clique em **[!UICONTROL Configurações]** no principal [!DNL Jira] menu.
1. Clique em **[!UICONTROL Complementos]**, em seguida **[!UICONTROL Gerenciar complementos]**.

1. Expanda o **[!DNL Workfront]** complemento.
1. Clique em **[!UICONTROL Configurar]**.
1. Faça logon em [!DNL Workfront] como administrador do sistema.

   O **[!UICONTROL Triggers]** é selecionada por padrão.

1. Clique em **[!UICONTROL Adicionar acionador]** para adicionar um novo acionador.
1. No **[!UICONTROL Equipe/usuário/função do Workfront]** , especifique o nome de um [!DNL Workfront] equipe, usuário ou função de trabalho, em seguida, clique para selecioná-lo quando for exibido na lista.

   >[!NOTE]
   >
   >Não é possível ter vários acionadores para a mesma equipe, usuário ou função.

   Quando alguém cria uma tarefa ou um problema e a atribui a uma dessas entidades, um problema é criado automaticamente no [!DNL [!DNL Jira]].

1. No **[!UICONTROL [!DNL Jira]projeto]** , comece a digitar o nome de um [!DNL Jira] projeto, clique em para selecioná-lo quando for exibido na lista.

   Quando a variável [!DNL Jira] for criado, ele será colocado no projeto especificado aqui.

1. Selecione um **I[!UICONTROL tipo de problema]** no menu suspenso.

   Isso indica o tipo de problema criado em [!DNL Jira] quando as condições desse acionador forem atendidas, com base nas configurações para esse projeto específico em [!DNL Jira].

1. Clique em **[!UICONTROL Salvar]**.

   Com essa configuração, sempre que uma [!DNL Workfront] o usuário cria um item que corresponde aos acionadores especificados, um novo problema é criado em [!DNL Jira].

## Configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront] Itens

Como [!DNL Jira] administrador, você pode definir quais campos devem sincronizar automaticamente nos itens vinculados entre [!DNL Workfront] e Jira. Certos campos podem sincronizar a partir do [!DNL Workfront] para [!DNL Jira] e outros sincronizam de Jira para Workfront.

Para definir quais campos devem ser sincronizados automaticamente em itens vinculados entre os dois aplicativos:

1. Faça logon [!DNL Jira] como administrador Jira.
1. Clique em **[!UICONTROL Configurações]** no principal [!DNL Jira] menu.
1. Clique em **[!UICONTROL Complementos]**, em seguida **[!UICONTROL Gerenciar complementos]**.

1. Expanda o **[!DNL Workfront]** complemento.
1. Clique em **[!UICONTROL Configurar]**.
1. Faça logon em [!DNL Workfront] como administrador do Workfront.
1. Clique no botão **[!UICONTROL Configuração]** guia .

1. No **[!UICONTROL Sincronizar do Jira para o Workfront]** selecione os campos que deseja atualizar em [!DNL Jira] quando são atualizados no Workfront.

   1. Selecione qualquer uma das seguintes frequências com as quais os campos são sincronizados:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Na Criação]</td>
              <td>Os campos especificados são sincronizados entre a Workfront vinculada e [!DNL Jira] itens quando o item é criado no Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Sempre]</td>
              <td>Os campos especificados são sincronizados entre a Workfront vinculada e [!DNL Jira] quando os campos são atualizados no Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Nunca]</td>
              <td>Os campos especificados nunca são sincronizados entre os [!DNL Workfront] e [!DNL Jira] itens. Não existe indicação em [!DNL Jira] que o campo foi atualizado em [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Selecione para sincronizar qualquer um dos seguintes campos de [!DNL Workfront] para [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Name]</td>
         <td><p>O nome de uma tarefa ou um problema em [!DNL Workfront] torna-se o nome do problema ao qual está vinculado [!DNL Jira].</p><p>Observação: Quando novos itens são criados em [!DNL Jira] automaticamente, a variável [!DNL Workfront] O nome sempre é atualizado no [!DNL Jira] , independentemente de este campo estar ou não ativado aqui. Quando uma [!DNL Jira] estiver vinculado manualmente a um item [!DNL Workfront] , o Nome da [!DNL Workfront] atualizações somente de item em [!DNL Jira] ao selecionar <strong>Sempre</strong> sincronize este campo. Para obter mais informações sobre vinculação manual ou automática de itens, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descrição]</td>
         <td>A descrição de uma tarefa ou de um problema em [!DNL Workfront] torna-se a descrição do problema ao qual está vinculado [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documentos</td>
         <td><p>Documentos anexados a uma tarefa ou a um problema em [!DNL Workfront] também estão anexadas ao problema ao qual está vinculado em Jira. Novas versões de documento de [!DNL Workfront] são adicionados como documentos separados ao Jira e são anexados com <i>_v&lt;version number=""&gt;</i> para indicar a versão numerada no Workfront. </p><p>Por exemplo, se o nome de um documento em [!DNL Workfront] é <strong>Anúncio principal</strong>e você adiciona uma nova versão a ele em [!DNL Workfront], a nova versão é transferida para o [!DNL Jira] como um novo documento com o nome <strong>Anúncio principal_v2</strong>.</p><p>Importante: <p>Considere o seguinte ao sincronizar documentos:</p>
           <ul>
            <li><p>Documentos com mais de 5 MB não são sincronizados. Se uma sincronização de documento falhar porque o documento é muito grande, um erro é registrado no registro de atividades, </p><p>Para obter mais informações sobre o log de atividades, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Exibir o registro de atividades do Jira</a>.</p></li>
            <li><p>Os documentos vinculados a tarefas e problemas de servidores externos não são transferidos para a [!DNL Jira] itens. Somente documentos carregados diretamente na tarefa ou no problema em [!DNL Workfront] são transferidos para o problema vinculado em [!DNL Jira].</p></li>
            <li><p>Para criar uma prova a partir de um documento, você deve gerar a prova em [!DNL Workfront]. </p><p>Para obter mais informações sobre a geração de uma prova, consulte <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create" class="MCXref xref">Criar uma prova para um documento existente </a>em <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Criar uma prova para um documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Data de conclusão planejada]</td>
         <td><p>A [!UICONTROL Data de conclusão planejada] de uma tarefa ou um problema em [!DNL Workfront] torna-se a [!UICONTROL Data de vencimento] do problema ao qual está vinculado [!DNL Jira].</p><p>Observação: Certifique-se de exibir <strong>[!UICONTROL Data de vencimento]</strong> on [!DNL Jira] problemas, para que esse valor seja sincronizado.</p></td>
        </tr>
       </tbody>
      </table>

1. No **[!UICONTROL Sincronizar de [!DNL Jira] para[!DNL Workfront]]** selecione os campos que deseja atualizar em [!DNL Workfront] quando são atualizados em [!DNL Jira].

   1. Selecione qualquer uma das seguintes frequências com as quais os campos são sincronizados:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Sempre]</td>
         <td>Os campos especificados são sempre sincronizados entre os [!DNL Workfront] e [!DNL Jira] quando os campos forem atualizados em [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nunca]</td>
         <td><p>Os campos especificados nunca são sincronizados entre os [!DNL Workfront] e [!DNL Jira] itens. Não existe indicação em [!DNL Workfront] que o campo foi atualizado em [!DNL Jira]. </p><p>Observação: Ao selecionar Nunca, [!DNL Workfront] os campos ainda podem ser atualizados manualmente de [!DNL Jira] à esquerda [!DNL Workfront] painel do [!DNL Jira] problema. Essas atualizações aparecem somente no [!DNL Workfront] itens em [!DNL Jira] e [!DNL Workfront] e não em [!DNL Jira] itens.</p></td>
        </tr>
       </tbody>
      </table>

   1. Selecione para sincronizar qualquer um dos seguintes campos de [!DNL Jira] para [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>O [!UICONTROL Status] de um problema em [!DNL Jira] se torna o [!UICONTROL Status] da tarefa ou problema à qual está vinculado [!DNL Workfront].<br>Para obter mais informações sobre [!DNL Workfront] status, consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Destinatário]</td>
         <td><p>O [!UICONTROL Destinatário] de um problema em [!DNL Jira] se torna o [!UICONTROL Destinatário] da tarefa ou problema à qual está vinculado [!DNL Workfront].</p><p>Importante: Ao atribuir um item em [!DNL Jira] para um usuário que não tenha um [!DNL Workfront] , a integração cria um novo usuário ativo no [!DNL Workfront] somente quando a variável <strong>Criar automaticamente um usuário no [!DNL Workfront] se a variável [!DNL Jira] o usuário não tem um [!DNL Workfront] account</strong> está definida como <strong>[!UICONTROL Sempre]</strong>. Esse usuário não ocupa um [!DNL Workfront] licença. Usuários ativos podem ser atribuídos a itens de trabalho em [!DNL Workfront], mas não podem ser incluídos em atualizações. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Anexos]</td>
         <td>Anexos de um problema em [!DNL Jira] também estão anexadas à tarefa ou problema ao qual está vinculada [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comentários]</td>
         <td><p>Um comentário em um [!DNL Jira] o problema também é publicado no link [!DNL Workfront] na área [!UICONTROL Atualizações]. Por outro lado, um comentário publicado na área [!UICONTROL Atualizações] para um [!DNL Workfront] sincronizações de tarefas ou problemas para [!DNL Jira]O fluxo de comentários nativos do para o problema vinculado. </p><p>Isso é definido como <strong>[!UICONTROL Sempre]</strong> por padrão. Se você selecionar <strong>[!UICONTROL Nunca]</strong> aqui, você ainda pode postar comentários manualmente em um item vinculado em [!DNL Workfront] ou [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. No **[!UICONTROL OUTRAS]** selecione quais campos adicionais devem ser atualizados entre os itens vinculados.

   1. Selecione uma opção para determinar se os campos foram especificados **[!UICONTROL Sempre]** ou **[!UICONTROL Nunca]** atualização em [!DNL Jira] ou [!DNL Workfront] quando forem modificadas.

   1. Selecione um dos seguintes campos e atualizações:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar [!DNL Workfront] Dados personalizados no painel direito em [!DNL Jira]]</td>
         <td><p>Exibe a [!DNL Workfront] Dados personalizados de um item na [!DNL Workfront] painel direito.</p><p>Observação: As seções de Formulário personalizado são exibidas na seção [!DNL Workfront] painel direito com o nível de acesso da [!DNL Workfront] Administrador do sistema.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar [!DNL Workfront] Prioridade no painel direito em [!DNL Jira]]</td>
         <td>Exibe a [!DNL Workfront] Prioridade de um item na [!DNL Workfront] painel direito.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Adicionar uma atualização no [!DNL Workfront] Guia Atualizações sobre as alterações de Data de Vencimento em [!DNL Jira]]</td>
         <td>Adiciona um comentário na guia [!UICONTROL Update] da [!DNL Workfront] quando a [!UICONTROL Data de Vencimento] for alterada no link [!DNL Jira] item.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Criar um usuário automaticamente em [!DNL Workfront] se a variável [!DNL Jira] o usuário não tem um [!DNL Workfront] account]</td>
         <td><p>Os seguintes cenários existem:</p>
          <ul>
           <li>Ao selecionar <strong>[!UICONTROL Sempre]</strong> habilite a integração para criar um novo usuário do Workfront sempre que uma [!DNL Jira] usuário sem um [!DNL Workfront] A conta executa as seguintes ações em um [!DNL Jira] problema:
            <ul>
             <li>É atribuído a um [!DNL Jira] problema</li>
             <li><p>Registra a hora em um [!DNL Jira] problema</p><p>Esse novo usuário não ocupa um [!DNL Workfront] licença. A configuração padrão é Sempre. O usuário criou dessa forma em [!DNL Workfront] tem "[!UICONTROL Jira]" adicionado ao nome.</p></li>
            </ul></li>
           <li>Ao selecionar <strong>[!UICONTROL Nunca]</strong>, as seguintes coisas acontecem:
            <ul>
             <li>Você não pode ver nenhum [!DNL Jira] atribuições no [!DNL Workfront] itens. Nesse caso, somente as atribuições feitas em [!DNL Workfront] exibir no [!DNL Workfront] itens.</li>
             <li>A hora de logon em um link [!DNL Jira] problema por um usuário sem um [!DNL Workfront] A conta não é transferida automaticamente para o [!DNL Workfront] item. Você ainda pode registrar o tempo no [!DNL Workfront] no painel direito do [!DNL Jira] problema.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Clique em **[!UICONTROL Salvar]**.

   Agora, sempre que um usuário atualiza qualquer um dos campos especificados nessa configuração em um item em [!DNL Jira] ou [!DNL Workfront], o item vinculado em outro aplicativo também é atualizado.

## Solução de problemas

### Os itens não podem ser criados em [!DNL Jira] devido a campos de acionamento marcados como &quot;[!UICONTROL Não foi possível localizar]&quot;

#### Problema

Quando ocorrer um erro com a [!DNL Workfront for Jira] pedido, [!DNL Workfront] desativa os acionadores para evitar mais complicações. Quando esses acionadores estiverem desativados, serão exibidos como &quot;[!UICONTROL Não foi possível localizar]&quot;.

#### Solução

Localize o erro que desabilitou os acionadores. Você pode encontrar o erro na variável [!DNL Workfront for Jira] &quot;[!UICONTROL Log de atividades]&quot;.

A causa mais comum desse comportamento é o erro &quot;[!UICONTROL O campo &#39;duedate&#39; não pode ser definido. Não está na tela apropriada ou é desconhecida.]&quot;

Este erro significa que você está tentando sincronizar o &quot;[!UICONTROL Data de Conclusão Planejada]&quot; de [!DNL Workfront] para [!DNL Jira]. Para fazer isso, você deve garantir que o [!DNL Jira] objetos têm um campo chamado &quot;[!UICONTROL Data de vencimento]&quot;. Se não tiverem esse campo, [!DNL Workfront] não consegue sincronizar a data de conclusão planejada a partir de [!DNL Workfront] e desativa os acionadores.

Para resolver esse erro, tente uma das seguintes opções:

* Pergunte ao seu [!DNL Jira] administrador para atualizar o [!DNL Jira] para garantir que eles tenham um campo de data de vencimento.
* Desativar a sincronização de [!DNL Workfront]Data de conclusão planejada da Workfront &quot;[!UICONTROL Configuração]&quot; página
