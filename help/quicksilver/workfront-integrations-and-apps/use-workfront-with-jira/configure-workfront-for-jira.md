---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurar [!DNL Adobe Workfront for Jira]
description: Você pode usar [!DNL Adobe Workfront for Jira] para integrar o [!DNL Jira] e [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '2420'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->

Você pode usar [!DNL Adobe Workfront for Jira] para integrar o [!DNL Jira] e [!DNL Workfront] sistemas.

Após instalar o complemento, é possível definir workflows que criam [!DNL Jira] problemas automaticamente quando [!DNL Workfront] itens de trabalho são criados. Os itens em ambos os aplicativos se tornam vinculados e algumas de suas informações são atualizadas automaticamente em ambos os sistemas.

Todos os usuários em [!DNL Workfront] e [!DNL Jira] podem se beneficiar dessa integração. Eles só precisam de uma licença para o sistema em que trabalham mais, e não para ambos os sistemas.

Esse complemento está disponível para o [!UICONTROL Servidor] e [!UICONTROL OnDemand] (ou [!UICONTROL Nuvem]) versões de [!DNL Jira] Software.

Para obter uma lista de [!DNL Jira] versões que [!DNL Workfront for Jira] atualmente compatíveis, consulte [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&amp;tab=overview) no [!DNL Atlassian Marketplace].

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL [!DNL Adobe Workfront] plano]*</td> 
   <td><p>Novo: Qualquer um</p>
       <p>ou</p>
       <p>Atual: [!UICONTROL Pro] ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td><p>Novo: [!UICONTROL Padrão] </p>
       <p>ou</p> 
       <p>Atual: [!UICONTROL Plano] </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no [!DNL Jira] e [!DNL Workfront] para se dedicar a essa integração, em vez de usar as existentes que podem ser anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> <p>Observação: se você ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

## Pré-requisitos

Antes de configurar [!DNL Workfront for Jira], você deve:

* Instalar [!DNL Workfront for Jira].
Para obter instruções sobre como instalar o [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurar [!DNL Workfront for Jira]

Ao configurar [!DNL Workfront for Jira], você pode:

* Definir acionadores que criarão [!DNL Jira] itens quando [!DNL Workfront] itens são criados.
* Especificar quais campos devem ser sincronizados entre itens vinculados entre [!DNL Jira] e [!DNL Workfront].

>[!NOTE]
>
>* Após configurar [!DNL Workfront for Jira] no seu [!DNL Jira] ambiente, tudo [!DNL Jira] os usuários veem um [!DNL Workfront] painel direito em todos [!DNL Jira] itens. O painel contém informações sobre os itens que podem ser vinculados do [!DNL Workfront] ou especifica que não [!DNL Workfront] itens estão vinculados a [!DNL Jira] itens.
>* Ao usar o [!DNL Jira Server] instalação, somente os problemas associados aos projetos identificados como acionadores da integração do Workfront exibirão o painel Workfront. Para obter mais informações sobre a configuração de acionadores para o [!DNL Workfront to Jira] fluxo de trabalho, consulte [Configurar acionadores para vincular automaticamente itens entre [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Para configurar [!DNL Workfront for Jira]:

1. Efetue logon no [!DNL Jira] as a [!DNL Jira] administrador.
1. Clique em **[!UICONTROL Configurações]** no principal [!DNL Jira] menu.
1. Clique em **[!UICONTROL Complementos]** e, em seguida, clique em **[!UICONTROL Gerenciar complementos]**.

1. Expanda a **[!DNL Workfront]** complementar.
1. Clique em **[!UICONTROL Configurar]**.
1. Siga as instruções para fazer logon no [!DNL Workfront].

   >[!NOTE]
   >
   >O usuário deve ter um `apiKey` in [!UICONTROL Workfront] para criar uma conexão bem-sucedida.

   Você deve fazer logon no [!DNL Workfront] as a [!DNL Workfront] administrador para continuar a configuração.

   >[!NOTE]
   >
   >* [!UICONTROL Workfront] conecta-se a [!DNL Jira] usando o OAuth 2.0, um padrão usado pela maioria das integrações baseadas na web para a autenticação e autorização dos usuários.
   >* Quando for solicitado que você insira o domínio de seu [!DNL Workfront] digite-a usando este formato: *yourCompany&#39;sDomain.my.workfront.com*. O domínio da sua empresa geralmente é o nome da sua empresa.
   >* A Autenticação aprimorada não estará disponível até que um [!DNL Workfront] o administrador o habilita nessa integração.

1. No Jira, selecione a variável **[!UICONTROL Triggers]** para configurar a criação automática de [!DNL Jira] itens como novos [!DNL Workfront] itens são criados.

   Para obter mais informações sobre a configuração de acionadores para o Workfront para [!DNL Jira] fluxo de trabalho, consulte [Configurar acionadores para vincular automaticamente itens entre [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Selecione o **[!UICONTROL Configuração]** para configurar a sincronização de campos entre campos vinculados [!DNL Jira] e [!DNL Workfront] itens.

   Para obter mais informações sobre como configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront], consulte [Configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront] Itens](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Após definir os acionadores e a sincronização de campos entre as duas aplicações, qualquer [!DNL Workfront] usuário que pode criar tarefas ou problemas pode potencialmente acionar a criação de um item no [!DNL Jira]. O usuário pode criar um item se os critérios no item que ele criar corresponderem aos acionadores em [!DNL Jira], mesmo que o usuário não tenha um [!DNL Jira] licença. Além disso, qualquer [!DNL Jira] o usuário pode começar a trabalhar imediatamente no [!DNL Jira] e suas atualizações estarão visíveis no [!DNL Workfront], sem que tenham um [!DNL Workfront] licença. Todas as atualizações em [!DNL Workfront] também são visíveis no [!DNL Jira] itens.

1. (Opcional) Selecione a **[!UICONTROL Log de atividades]** para revisar quaisquer erros que possam ter ocorrido durante a integração.

   Para obter mais informações sobre o [!UICONTROL Log de atividades], consulte [Exibir o [!DNL Jira] [!UICONTROL Log de atividades]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurar acionadores para vincular automaticamente itens entre [!DNL Jira] e [!DNL Workfront]

Como a variável [!DNL Jira] administrador do sistema, você pode definir acionadores que criariam problemas automaticamente em [!DNL Jira] quando um item estiver em [!DNL Workfront] satisfaz determinados critérios.

>[!NOTE]
>
>Pode levar até 10 minutos para que a integração crie novos problemas no [!DNL Jira].

Considere o seguinte ao configurar o acionamento da criação de [!DNL Jira] itens como [!DNL Workfront] itens são criados:

* A integração é unidirecional: você só pode acionar itens criados no [!DNL Workfront] para ser criado automaticamente em [!DNL Jira]. Não é possível acionar itens criados no [!DNL Jira] para ser criado automaticamente em [!DNL Workfront].
* Não há limite para o número de acionadores que você pode ter.
* Se um item que você criar no [!DNL Workfront] corresponde a mais de um acionador, somente um item é criado no [!DNL Jira]. O item é criado em [!DNL Jira] de acordo com o primeiro acionador (na ordem em que foram definidos em [!DNL Jira]). Todos os outros acionadores são ignorados.
* Somente um item em [!DNL Workfront] pode ser vinculado a um item no Jira. Você nunca pode vincular um [!DNL Workfront] item para vários [!DNL Jira] problemas ou um [!DNL Jira] problema em vários [!DNL Workfront] itens.

Para configurar acionadores para criar itens automaticamente no [!DNL Jira]:

1. Efetue logon no [!DNL Jira] como administrador do sistema.
1. Clique em **[!UICONTROL Configurações]** no principal [!DNL Jira] menu.
1. Clique em **[!UICONTROL Complementos]**, depois **[!UICONTROL Gerenciar complementos]**.
1. Expanda a **[!DNL Workfront]** complementar.
1. Clique em **[!UICONTROL Configurar]**.
1. Efetue logon no [!DNL Workfront] como administrador do sistema.

   A variável **[!UICONTROL Triggers]** é selecionada por padrão no Jira.

1. Clique em **[!UICONTROL Adicionar acionador]** para adicionar um novo acionador.
1. No **[!UICONTROL Equipe/usuário/função do Workfront]** especifique o nome de um [!DNL Workfront] equipe, usuário ou função de trabalho, em seguida, clique para selecioná-la quando ela for exibida na lista.

   >[!NOTE]
   >
   >Você não pode ter vários acionadores para a mesma equipe, usuário ou função.

   Quando alguém cria uma tarefa ou um problema e o atribui a uma dessas entidades, um problema é automaticamente criado no [!DNL [!DNL Jira]].

1. No **[!UICONTROL [!DNL Jira]projeto]** , comece digitando o nome de um [!DNL Jira] projeto e, em seguida, clique em para selecioná-lo quando ele for exibido na lista.

   Quando a variável [!DNL Jira] problema for criada, ela será colocada no projeto escolhido aqui.

1. Selecione um **I[!UICONTROL tipo de problema]** no menu suspenso.

   Isso indica o tipo de ocorrência criado no [!DNL Jira] quando as condições deste acionador forem atendidas, com base nas configurações desse projeto específico no [!DNL Jira].

1. Clique em **[!UICONTROL Salvar]**.

   Com essa configuração, sempre que um [!DNL Workfront] usuário cria um item que corresponde aos acionadores especificados, um novo problema é criado no [!DNL Jira].

## Configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront] Itens

Como a variável [!DNL Jira] administrador, você pode definir quais campos devem ser sincronizados automaticamente nos itens vinculados entre [!DNL Workfront] e Jira. Determinados campos podem ser sincronizados do [!DNL Workfront] para o [!DNL Jira] e outros são sincronizados do Jira para o Workfront.

Para definir quais campos devem ser sincronizados automaticamente em itens vinculados entre os dois aplicativos:

1. Efetue logon no [!DNL Jira] como administrador Jira.
1. Clique em **[!UICONTROL Configurações]** no principal [!DNL Jira] menu.
1. Clique em **[!UICONTROL Complementos]**, depois **[!UICONTROL Gerenciar complementos]**.
1. Expanda a **[!DNL Workfront]** complementar.
1. Clique em **[!UICONTROL Configurar]**.
1. Efetue logon no [!DNL Workfront] como administrador do Workfront.
1. No Jira, clique no link **[!UICONTROL Configuração]** guia.
1. No **[!UICONTROL Sincronizar do Workfront para o Jira]** selecione os campos que deseja atualizar na seção [!DNL Jira] quando são atualizados no Workfront.

   1. Selecione qualquer uma das seguintes frequências com as quais os campos são sincronizados:

      <table style="table-layout:auto">
         <tr>
              <td>[!UICONTROL Na Criação]</td>
              <td>Os campos especificados são sincronizados entre o Workfront vinculado e [!DNL Jira] itens quando o item é criado no Workfront.</td>
          </tr>
          <tr>
              <td>[!UICONTROL Sempre]</td>
              <td>Os campos especificados são sincronizados entre o Workfront vinculado e [!DNL Jira] itens quando os campos são atualizados no Workfront. </td>
          </tr>
          <tr>
              <td>[!UICONTROL Nunca]</td>
              <td>Os campos especificados nunca são sincronizados entre os campos vinculados [!DNL Workfront] e [!DNL Jira] itens. Não há nenhuma indicação no [!DNL Jira] que o campo foi atualizado em [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Selecione uma das opções a seguir para sincronizar os campos do [!DNL Workfront] para [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Nome]</td>
         <td><p>O nome de uma tarefa ou um problema no [!DNL Workfront] torna-se o nome da ocorrência à qual está vinculada [!DNL Jira].</p><p>Observação: quando novos itens são criados no [!DNL Jira] automaticamente, a variável [!DNL Workfront] O nome sempre é atualizado no [!DNL Jira] item, independentemente de esse campo estar ativado aqui ou não. Quando um [!DNL Jira] o item é vinculado manualmente a um [!DNL Workfront] item, o Nome do [!DNL Workfront] O item só é atualizado em [!DNL Jira] ao selecionar para <strong>Sempre</strong> sincronizar este campo. Para obter mais informações sobre vinculação manual ou automática de itens, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descrição]</td>
         <td>A descrição de uma tarefa ou um problema no [!DNL Workfront] torna-se a descrição do problema ao qual está vinculado [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documentos</td>
         <td><p>Documentos anexados a uma tarefa ou um problema no [!DNL Workfront] também são anexados ao problema ao qual está vinculado no Jira. Novas versões de documentos de [!DNL Workfront] são adicionados como documentos separados ao Jira e são anexados com <i>_v&lt;version number=""&gt;</i> para indicar a versão numerada no Workfront. </p><p>Por exemplo, se o nome de um documento em [!DNL Workfront] é <strong>Anúncio principal</strong>e você adicionar uma nova versão a ela em [!DNL Workfront], a nova versão será transferida para [!DNL Jira] como um novo documento com o nome <strong>Ad_v2 principal</strong>.</p><p>Importante: <p>Considere o seguinte ao sincronizar documentos:</p>
           <ul>
            <li><p>Documentos maiores que 5 MB não são sincronizados. Se a sincronização de um documento falhar porque o documento é muito grande, um erro será registrado no registro de atividades. </p><p>Para obter mais informações sobre o registro de atividades, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Exibir o log de atividades do Jira</a>.</p></li>
            <li><p>Documentos vinculados a tarefas e problemas de servidores externos não são transferidos para o [!DNL Jira] itens. Somente documentos carregados diretamente na tarefa ou no problema no [!DNL Workfront] são transferidos para o problema vinculado no [!DNL Jira].</p></li>
            <li><p>Para criar uma prova a partir de um documento, você deve gerar a prova no [!DNL Workfront]. </p><p>Para obter mais informações sobre como gerar uma prova, consulte <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Criar uma prova para um documento existente </a>in <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Criar uma prova para um documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Data de Término Planejada]</td>
         <td><p>A [!UICONTROL Data de conclusão planejada] de uma tarefa ou um problema em [!DNL Workfront] torna-se a [!UICONTROL Data de vencimento] da ocorrência à qual está vinculado [!DNL Jira].</p><p>Observação: certifique-se de exibir <strong>[!UICONTROL Data de Conclusão]</strong> em [!DNL Jira] problemas, para que esse valor seja sincronizado.</p></td>
        </tr>
       </tbody>
      </table>

1. No **[!UICONTROL Sincronizar a partir de [!DNL Jira] para[!DNL Workfront]]** selecione os campos que deseja atualizar na seção [!DNL Workfront] quando são atualizados em [!DNL Jira].

   1. Selecione qualquer uma das seguintes frequências com as quais os campos são sincronizados:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Sempre]</td>
         <td>Os campos especificados são sempre sincronizados entre os campos [!DNL Workfront] e [!DNL Jira] itens quando os campos forem atualizados no [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nunca]</td>
         <td><p>Os campos especificados nunca são sincronizados entre os campos vinculados [!DNL Workfront] e [!DNL Jira] itens. Não há nenhuma indicação no [!DNL Workfront] que o campo foi atualizado em [!DNL Jira]. </p><p>Observação: ao selecionar Nunca, [!DNL Workfront] os campos ainda podem ser atualizados manualmente a partir de [!DNL Jira] à esquerda [!DNL Workfront] painel da [!DNL Jira] problema. Essas atualizações aparecem somente em [!DNL Workfront] itens em [!DNL Jira] e [!DNL Workfront] e não em [!DNL Jira] itens.</p></td>
        </tr>
       </tbody>
      </table>

   1. Selecione para sincronizar qualquer um dos campos a seguir em [!DNL Jira] para [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>O [!UICONTROL Status] de um problema no [!DNL Jira] torna-se o [!UICONTROL Status] da tarefa ou problema ao qual está vinculado [!DNL Workfront].<br>Para obter mais informações sobre [!DNL Workfront] status, consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Atribuído]</td>
         <td><p>O [!UICONTROL Destinatário] de um problema no [!DNL Jira] torna-se o [!UICONTROL Destinatário] da tarefa ou problema ao qual está vinculado [!DNL Workfront].</p><p>Importante: Quando você atribui um item no [!DNL Jira] para um usuário que não tenha uma [!DNL Workfront] conta, a integração cria um novo usuário ativo no [!DNL Workfront] somente quando <strong>Criar automaticamente um usuário no [!DNL Workfront] se a variável [!DNL Jira] o usuário não tem um [!DNL Workfront] account</strong> está definida como <strong>[!UICONTROL Sempre]</strong>. Este usuário não ocupa um [!DNL Workfront] licença. Usuários ativos podem ser atribuídos a itens de trabalho no [!DNL Workfront], mas não pode ser incluído em atualizações. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Anexos]</td>
         <td>Anexos de um problema no [!DNL Jira] também são anexados à tarefa ou problema ao qual está vinculado em [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comentários]</td>
         <td><p>Um comentário em um [!DNL Jira] problema também é postada no link [!DNL Workfront] item na área [!UICONTROL Atualizações]. Por outro lado, um comentário publicado na área [!UICONTROL Atualizações] para um [!DNL Workfront] sincronizações de tarefa ou problema para [!DNL Jira]Fluxo de comentários nativo do para o problema vinculado. </p><p>Isso é definido como <strong>[!UICONTROL Sempre]</strong> por padrão. Se você selecionar <strong>[!UICONTROL Nunca]</strong> aqui, você ainda pode postar comentários manualmente em um item vinculado no [!DNL Workfront] ou em [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. No **[!UICONTROL OUTRO]** selecione quais campos adicionais devem ser atualizados entre os itens vinculados.

   1. Selecione uma opção para determinar se os campos especificados **[!UICONTROL Sempre]** ou **[!UICONTROL Nunca]** atualizar em [!DNL Jira] ou [!DNL Workfront] quando são modificados.

   1. Selecione entre os seguintes campos e atualizações:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar [!DNL Workfront] Dados personalizados no painel direito no [!DNL Jira]]</td>
         <td><p>Exibe o [!DNL Workfront] Dados personalizados de um item na [!DNL Workfront] painel direito.</p><p>Observação: as seções de Formulário personalizado são exibidas na [!DNL Workfront] painel direito com o nível de acesso do [!DNL Workfront] Administrador do sistema.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar [!DNL Workfront] Prioridade no painel direito do [!DNL Jira]]</td>
         <td>Exibe o [!DNL Workfront] Prioridade de um item na [!DNL Workfront] painel direito.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Adicionar uma atualização no [!DNL Workfront] Guia Atualizações sobre alterações da Data de vencimento no [!DNL Jira]]</td>
         <td>Adiciona um comentário na guia [!UICONTROL Atualizar] do [!DNL Workfront] item quando a [!UICONTROL Data de Conclusão] for alterada em [!DNL Jira] item.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Criar usuário automaticamente em [!DNL Workfront] se a variável [!DNL Jira] o usuário não tem um [!DNL Workfront] account]</td>
         <td><p>Existem os seguintes cenários:</p>
          <ul>
           <li>Ao selecionar <strong>[!UICONTROL Sempre]</strong>, você habilita a integração para criar um novo usuário do Workfront sempre que um [!DNL Jira] usuário sem um [!DNL Workfront] A conta do executa as seguintes ações em um link [!DNL Jira] problema:
            <ul>
             <li>É atribuído a um [!DNL Jira] problema</li>
             <li><p>Registra o tempo em um [!DNL Jira] problema</p><p>Este novo usuário não ocupa um [!DNL Workfront] licença. A configuração padrão é Sempre. O usuário criou desta forma no [!DNL Workfront] possui "[!UICONTROL Jira]" adicionado ao seu nome.</p></li>
            </ul></li>
           <li>Ao selecionar <strong>[!UICONTROL Nunca]</strong>, as seguintes coisas acontecem:
            <ul>
             <li>Você não pode ver nenhum [!DNL Jira] atribuições no [!DNL Workfront] itens. Nesse caso, apenas as [!DNL Workfront] exibir no [!DNL Workfront] itens.</li>
             <li>O tempo registrado em um link [!DNL Jira] problema por um usuário sem um [!DNL Workfront] A conta do não é transferida automaticamente para a [!DNL Workfront] item. Você ainda pode registrar horas na variável [!DNL Workfront] no painel direito do [!DNL Jira] problema.</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Clique em **[!UICONTROL Salvar]**.

   Agora, sempre que um usuário atualizar qualquer um dos campos especificados nessa configuração em um item do [!DNL Jira] ou [!DNL Workfront], o item vinculado no outro aplicativo também é atualizado.

## Solução de problemas

### Os itens não podem ser criados no [!DNL Jira] devido aos campos de acionador marcados como &quot;[!UICONTROL Não foi possível encontrar]&quot;

#### Problema

Quando ocorrer um erro com a variável [!DNL Workfront for Jira] aplicativo, [!DNL Workfront] O desativa os acionadores para evitar mais complicações. Quando esses acionadores estão desativados, eles são exibidos como &quot;[!UICONTROL Não foi possível encontrar].&quot;

#### Solução

Localize o erro que desativou os acionadores. Você pode encontrar o erro no [!DNL Workfront for Jira] [!UICONTROL Log de atividades].

A causa mais comum desse comportamento é o erro &quot;[!UICONTROL O campo &#39;duedate&#39; não pode ser definido. Não está na tela apropriada ou é desconhecido.]&quot;

Esse erro significa que você está tentando sincronizar o &quot;[!UICONTROL Data de Término Planejada]&quot; de [!DNL Workfront] para [!DNL Jira]. Para fazer isso, você deve garantir que suas [!DNL Jira] objetos têm um campo chamado &quot;[!UICONTROL Prazo].&quot; Se eles não tiverem esse campo, [!DNL Workfront] não pode sincronizar a data de conclusão planejada de [!DNL Workfront] e desativa os acionadores.

Para resolver esse erro, tente uma das seguintes opções:

* Pergunte ao seu [!DNL Jira] administrador para atualizar o afetado [!DNL Jira] objetos para garantir que eles tenham um campo de data de vencimento.
* Desativar a sincronização de [!DNL Workfront]Data de conclusão planejada do na Workfront [!UICONTROL Configuração] página.
