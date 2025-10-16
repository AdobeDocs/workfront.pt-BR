---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Configurar [!DNL Adobe Workfront for Jira]
description: Você pode usar o [!DNL Adobe Workfront for Jira] para integrar seus [!DNL Jira] e [!DNL Workfront] sistemas.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 959adc88-5201-4945-96c4-ea890f0bd371
source-git-commit: b1b55b8046aa771abb2cceda333940ccf827356a
workflow-type: tm+mt
source-wordcount: '2454'
ht-degree: 0%

---

# Configurar [!DNL Adobe Workfront for Jira]

<!-- Audited: 12/2023 -->


>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Jira não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Jira.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Jira, consulte [módulos do Software Jira](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules).

<!--

>[!IMPORTANT]
>
>To deliver more stable and scalable integrations, we're shifting to a modern, flexible integration approach using Workfront Automation and Integration (Fusion). As part of this transition process, the Workfront for Jira integration will not be available after **February 28, 2026**. 
>
>We recommend using Workfront Automation and Integration for your organization's integration needs with Jira. 
>
>Eight ready-to-use Workfront Automation and Integration templates for Jira will be available by August to help replicate common workflows and accelerate implementation. Templates are fully customizable to meet specific business needs and can be extended as requirements evolve. 
> 
>For an overview of Workfront Automation and Integration, see [Adobe Workfront Fusion overview](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview). 
>
>For information about the specific capabilities of the Workfront Automation and Integration modules for Jira, see [Jira Software modules](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/jira-software-modules). 

-->

Você pode usar o [!DNL Adobe Workfront for Jira] para integrar seus sistemas [!DNL Jira] e [!DNL Workfront].

Após instalar o complemento, você pode definir fluxos de trabalho que criem [!DNL Jira] problemas automaticamente quando [!DNL Workfront] itens de trabalho forem criados. Os itens em ambos os aplicativos se tornam vinculados e algumas de suas informações são atualizadas automaticamente em ambos os sistemas.

Todos os usuários em [!DNL Workfront] e [!DNL Jira] podem se beneficiar dessa integração. Eles só precisam de uma licença para o sistema em que trabalham mais, e não para ambos os sistemas.

Este complemento está disponível para as versões do Software [!UICONTROL Servidor] e [!UICONTROL OnDemand] (ou [!UICONTROL Nuvem]) do [!DNL Jira].

Para obter uma lista de [!DNL Jira] versões que [!DNL Workfront for Jira] suporta atualmente, consulte [[!DNL Workfront for Jira]](https://marketplace.atlassian.com/apps/1218653/workfront-for-jira?hosting=cloud&tab=overview) no [!DNL Atlassian Marketplace].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard </p>
       <p>Plano </p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Acesso à Jira</td> 
   <td> <p>Acesso de administrador do sistema</p> <p>Importante: recomendamos que você crie contas de administrador do sistema separadas no Jira e no Workfront para se dedicar a essa integração, em vez de usar as existentes que podem ser anexadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de configurar o [!DNL Workfront for Jira], você deve:

* Instalar [!DNL Workfront for Jira].
Para obter instruções sobre como instalar o [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Configurar [!DNL Workfront for Jira]

Ao configurar o [!DNL Workfront for Jira], você pode:

* Defina os acionadores que criarão [!DNL Jira] itens quando [!DNL Workfront] itens forem criados.
* Especifique quais campos devem ser sincronizados entre itens vinculados entre [!DNL Jira] e [!DNL Workfront].

>[!NOTE]
>
>* Após configurar o [!DNL Workfront for Jira] no seu ambiente [!DNL Jira], todos os usuários do [!DNL Jira] verão um painel direito do [!DNL Workfront] em todos os itens do [!DNL Jira]. O painel contém informações sobre os itens que podem ser vinculados de [!DNL Workfront] ou especifica que nenhum item [!DNL Workfront] está vinculado a itens [!DNL Jira].
>* Ao usar a instalação do [!DNL Jira Server], somente os problemas associados aos projetos identificados como acionadores da integração do Workfront exibem o painel do Workfront. Para obter mais informações sobre como configurar acionadores para o fluxo de trabalho [!DNL Workfront to Jira], consulte [Configurar acionadores para vincular automaticamente itens entre [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).
>

Para configurar [!DNL Workfront for Jira]:

1. Faça logon em [!DNL Jira] como administrador [!DNL Jira].
1. Clique em **[!UICONTROL Configurações]** no menu principal [!DNL Jira].
1. Clique em **[!UICONTROL Complementos]** e em **[!UICONTROL Gerenciar complementos]**.

1. Expanda o complemento **[!DNL Workfront]**.
1. Clique em **[!UICONTROL Configurar]**.
1. Siga as instruções para fazer logon no [!DNL Workfront].

   >[!NOTE]
   >
   >O usuário deve ter um `apiKey` válido no [!UICONTROL Workfront] para criar uma conexão bem-sucedida.

   Você deve fazer logon em [!DNL Workfront] como administrador [!DNL Workfront] para continuar a configuração.

   >[!NOTE]
   >
   >* O [!UICONTROL Workfront] se conecta ao [!DNL Jira] usando o OAuth 2.0, um padrão usado pela maioria das integrações baseadas na Web para a autenticação e autorização de usuários.
   >* Quando for solicitado que você insira o domínio da sua conta do [!DNL Workfront], digite-o usando este formato: *yourCompany&#39;sDomain.my.workfront.com*. O domínio da sua empresa geralmente é o nome da sua empresa.
   >* A Autenticação Aprimorada não estará disponível até que um administrador do [!DNL Workfront] a habilite para esta integração.

1. No Jira, selecione a guia **[!UICONTROL Triggers]** para configurar a criação automática de [!DNL Jira] itens à medida que novos [!DNL Workfront] itens forem criados.

   Para obter mais informações sobre como configurar acionadores para o fluxo de trabalho do Workfront para [!DNL Jira], consulte [Configurar acionadores para vincular automaticamente itens entre [!DNL Jira] e [!DNL Workfront]](#configure-triggers-for-automatically-linking-items-between-jira-and-workfront).

1. Selecione a guia **[!UICONTROL Instalação]** para configurar a sincronização de campos entre itens [!DNL Jira] e [!DNL Workfront] vinculados.

   Para obter mais informações sobre como configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront], consulte [Configurar a sincronização de campos entre [!DNL Jira] e [!DNL Workfront] Itens](#configure-field-synchronization-between-jira-and-workfront-items).

   >[!NOTE]
   >
   >Após definir os acionadores e a sincronização de campos entre os dois aplicativos, qualquer usuário do [!DNL Workfront] que possa criar tarefas ou problemas poderá disparar a criação de um item no [!DNL Jira]. O usuário poderá criar um item se os critérios no item que criar corresponderem aos acionadores em [!DNL Jira], mesmo se o usuário não tiver uma licença do [!DNL Jira]. Além disso, qualquer usuário do [!DNL Jira] pode começar imediatamente a trabalhar no item [!DNL Jira], e suas atualizações ficam visíveis no [!DNL Workfront], sem que ele tenha uma licença do [!DNL Workfront]. Todas as atualizações em [!DNL Workfront] também estão visíveis nos itens [!DNL Jira].

1. (Opcional) Selecione a guia **[!UICONTROL Log de atividades]** para examinar todos os erros ocorridos durante a integração.

   Para obter mais informações sobre o [!UICONTROL Log de Atividades], consulte [Exibir o [!DNL Jira] [!UICONTROL Log de Atividades]](../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md).

## Configurar disparadores para vincular automaticamente itens entre [!DNL Jira] e [!DNL Workfront]

Como administrador do sistema [!DNL Jira], você pode definir acionadores que criariam problemas automaticamente em [!DNL Jira] quando um item em [!DNL Workfront] atendesse a determinados critérios.

>[!NOTE]
>
>A integração pode levar até 10 minutos para criar novos problemas no [!DNL Jira].

Considere o seguinte ao configurar o disparo da criação de [!DNL Jira] itens, pois [!DNL Workfront] itens são criados:

* A integração é unidirecional: você só pode acionar itens criados no [!DNL Workfront] para serem criados automaticamente no [!DNL Jira]. Você não pode acionar itens criados em [!DNL Jira] para serem criados automaticamente em [!DNL Workfront].
* Não há limite para o número de acionadores que você pode ter.
* Se um item que você criar em [!DNL Workfront] corresponder a mais de um dos acionadores, apenas um item será criado em [!DNL Jira]. O item é criado em [!DNL Jira] de acordo com o primeiro acionador (na ordem em que foram definidos em [!DNL Jira]). Todos os outros acionadores são ignorados.
* Somente um item em [!DNL Workfront] pode ser vinculado a um item no Jira. Você nunca pode vincular um item [!DNL Workfront] a vários problemas [!DNL Jira], ou um problema [!DNL Jira] a vários itens [!DNL Workfront].

Para configurar acionadores para criar itens automaticamente em [!DNL Jira]:

1. Faça logon em [!DNL Jira] como administrador do sistema.
1. Clique em **[!UICONTROL Configurações]** no menu principal [!DNL Jira].
1. Clique em **[!UICONTROL Complementos]** e depois em **[!UICONTROL Gerenciar complementos]**.
1. Expanda o complemento **[!DNL Workfront]**.
1. Clique em **[!UICONTROL Configurar]**.
1. Faça logon em [!DNL Workfront] como administrador do sistema.

   A guia **[!UICONTROL Triggers]** é selecionada por padrão no Jira.

1. Clique em **[!UICONTROL Adicionar acionador]** para adicionar um novo acionador.
1. No campo **[!UICONTROL Equipe/usuário/função do Workfront]**, especifique o nome de uma equipe, usuário ou função de trabalho [!DNL Workfront] e clique para selecioná-lo quando ele for exibido na lista.

   >[!NOTE]
   >
   >Você não pode ter vários acionadores para a mesma equipe, usuário ou função.

   Quando alguém cria uma tarefa ou um problema e o atribui a uma dessas entidades, um problema é automaticamente criado no [!DNL [!DNL Jira]].

1. No campo **[!UICONTROL [!DNL Jira]projeto]**, comece digitando o nome de um projeto [!DNL Jira] e clique para selecioná-lo quando ele for exibido na lista.

   Quando o problema [!DNL Jira] é criado, ele é colocado no projeto que você escolheu aqui.

1. Selecione um **I[!UICONTROL tipo de problema]** no menu suspenso.

   Isso indica o tipo de problema criado em [!DNL Jira] quando as condições deste gatilho são atendidas, com base nas configurações do projeto específico em [!DNL Jira].

1. Clique em **[!UICONTROL Salvar]**.

   Com essa configuração, toda vez que um usuário [!DNL Workfront] cria um item que corresponde aos acionadores especificados, um novo problema é criado em [!DNL Jira].

## Configurar a sincronização de campo entre [!DNL Jira] e [!DNL Workfront] itens

Como administrador do [!DNL Jira], você pode definir quais campos devem ser sincronizados automaticamente nos itens vinculados entre o [!DNL Workfront] e o Jira. Determinados campos podem ser sincronizados de [!DNL Workfront] para o item [!DNL Jira], e outros são sincronizados de Jira para Workfront.

Para definir quais campos devem ser sincronizados automaticamente em itens vinculados entre os dois aplicativos:

1. Faça logon em [!DNL Jira] como administrador Jira.
1. Clique em **[!UICONTROL Configurações]** no menu principal [!DNL Jira].
1. Clique em **[!UICONTROL Complementos]** e depois em **[!UICONTROL Gerenciar complementos]**.
1. Expanda o complemento **[!DNL Workfront]**.
1. Clique em **[!UICONTROL Configurar]**.
1. Faça logon em [!DNL Workfront] como administrador do Workfront.
1. No Jira, clique na guia **[!UICONTROL Configuração]**.
1. Na seção **[!UICONTROL Sincronizar do Workfront para o Jira]**, selecione os campos que deseja atualizar em [!DNL Jira] quando forem atualizados no Workfront.

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
              <td>Os campos especificados nunca são sincronizados entre os itens [!DNL Workfront] e [!DNL Jira] vinculados. Não há nenhuma indicação em [!DNL Jira] de que o campo foi atualizado em [!DNL Workfront]. </td>
          </tr>
      </table>

   1. Selecione qualquer uma das opções a seguir para sincronizar os campos de [!DNL Workfront] a [!DNL Jira]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Nome]</td>
         <td><p>O nome de uma tarefa ou um problema em [!DNL Workfront] torna-se o nome do problema ao qual ela está vinculada em [!DNL Jira].</p><p>Observação: quando novos itens são criados no [!DNL Jira] automaticamente, o Nome do [!DNL Workfront] sempre é atualizado no item [!DNL Jira], independentemente de esse campo estar ou não habilitado aqui. Quando um item [!DNL Jira] é vinculado manualmente a um item [!DNL Workfront], o Nome do item [!DNL Workfront] só é atualizado em [!DNL Jira] quando você seleciona <strong>Sempre</strong> para sincronizar este campo. Para obter mais informações sobre como vincular itens manual ou automaticamente, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/link-items-between-wf-jira.md" class="MCXref xref">Vincular itens entre [!DNL Adobe Workfront] e [!DNL Jira]</a>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Descrição]</td>
         <td>A descrição de uma tarefa ou um problema em [!DNL Workfront] torna-se a descrição do problema ao qual ela está vinculada em [!DNL Jira].</td>
        </tr>
        <tr>
         <td role="rowheader">Documentos</td>
         <td><p>Documentos anexados a uma tarefa ou um problema em [!DNL Workfront] também são anexados ao problema ao qual ele está vinculado no Jira. Novas versões de documentos de [!DNL Workfront] são adicionadas como documentos separados ao Jira e são anexadas com <i>_v&lt;número de versão&gt;</i> para indicar a versão numerada no Workfront. </p><p>Por exemplo, se o nome de um documento em [!DNL Workfront] for <strong>Anúncio principal</strong> e você adicionar uma nova versão a ele em [!DNL Workfront], a nova versão será transferida para [!DNL Jira] como um novo documento com o nome <strong>Anúncio principal_v2</strong>.</p><p>Importante: <p>Considere o seguinte ao sincronizar documentos:</p>
           <ul>
            <li><p>Documentos maiores que 5 MB não são sincronizados. Se a sincronização de um documento falhar porque o documento é muito grande, um erro será registrado no registro de atividades. </p><p>Para obter mais informações sobre o log de atividades, consulte <a href="../../workfront-integrations-and-apps/use-workfront-with-jira/view-the-jira-activity-log.md" class="MCXref xref">Exibir o Log de Atividades do Jira</a>.</p></li>
            <li><p>Documentos vinculados a tarefas e problemas de servidores externos não são transferidos para os itens [!DNL Jira]. Somente documentos carregados diretamente na tarefa ou no problema em [!DNL Workfront] são transferidos para o problema vinculado em [!DNL Jira].</p></li>
            <li><p>Para criar uma prova de um documento, você deve gerar a prova em [!DNL Workfront]. </p><p>Para obter mais informações sobre como gerar uma prova, consulte <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md#create-a-proof-for-an-existing-document" class="MCXref xref">Criar uma prova para um documento existente </a>em <a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-for-a-document.md" class="MCXref xref">Criar uma prova para um documento</a>.<br></p></li>
           </ul></p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Data de Término Planejada]</td>
         <td><p>A [!UICONTROL Data de Conclusão Planejada] de uma tarefa ou um problema em [!DNL Workfront] torna-se a [!UICONTROL Data de Conclusão] do problema ao qual está vinculado em [!DNL Jira].</p><p>Observação: exiba <strong>[!UICONTROL Data de Vencimento]</strong> em [!DNL Jira] problemas, para que esse valor seja sincronizado.</p></td>
        </tr>
       </tbody>
      </table>

1. Na seção **[!UICONTROL Sincronizar de [!DNL Jira] para[!DNL Workfront]]**, selecione os campos que deseja atualizar em [!DNL Workfront] quando forem atualizados em [!DNL Jira].

   1. Selecione qualquer uma das seguintes frequências com as quais os campos são sincronizados:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Sempre]</td>
         <td>Os campos especificados são sempre sincronizados entre os itens [!DNL Workfront] e [!DNL Jira] vinculados quando os campos são atualizados em [!DNL Jira]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Nunca]</td>
         <td><p>Os campos especificados nunca são sincronizados entre os itens [!DNL Workfront] e [!DNL Jira] vinculados. Não há nenhuma indicação em [!DNL Workfront] de que o campo foi atualizado em [!DNL Jira]. </p><p>Observação: ao selecionar Nunca, os campos [!DNL Workfront] ainda podem ser atualizados manualmente de [!DNL Jira] no painel [!DNL Workfront] esquerdo do problema [!DNL Jira]. Essas atualizações aparecem somente nos itens [!DNL Workfront] em [!DNL Jira] e [!DNL Workfront] e não nos itens [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

   1. Selecione para sincronizar qualquer um dos seguintes campos de [!DNL Jira] a [!DNL Workfront]:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Status]</td>
         <td>O [!UICONTROL Status] de um problema em [!DNL Jira] torna-se o [!UICONTROL Status] da tarefa ou problema ao qual ele está vinculado em [!DNL Workfront].<br>Para obter mais informações sobre [!DNL Workfront] status, consulte <a href="../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Atribuído]</td>
         <td><p>O [!UICONTROL Atribuído] de um problema em [!DNL Jira] torna-se o [!UICONTROL Atribuído] da tarefa ou problema ao qual está vinculado em [!DNL Workfront].</p><p>Importante: quando você atribui um item em [!DNL Jira] a um usuário que não tem uma conta [!DNL Workfront], a integração cria um novo usuário ativo em [!DNL Workfront] somente quando <strong>Cria automaticamente um usuário em [!DNL Workfront] se o usuário [!DNL Jira] não tiver uma conta [!DNL Workfront]</strong> estiver definido como <strong>[!UICONTROL Always]</strong>. Este usuário não ocupa uma licença [!DNL Workfront]. Usuários ativos podem ser atribuídos a itens de trabalho em [!DNL Workfront], mas não podem ser incluídos em atualizações. </p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Anexos]</td>
         <td>Anexos de um problema em [!DNL Jira] também são anexados à tarefa ou problema ao qual ele está vinculado em [!DNL Workfront]. </td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Comentários]</td>
         <td><p>Um comentário sobre um problema [!DNL Jira] também é postado no item [!DNL Workfront] vinculado na área [!UICONTROL Atualizações]. Por outro lado, um comentário postado na área [!UICONTROL Atualizações] para uma tarefa [!DNL Workfront] ou problema sincroniza com o fluxo de comentários nativo de [!DNL Jira] para o problema vinculado. </p><p>Isso é definido como <strong>[!UICONTROL Always]</strong> por padrão. Se você selecionar <strong>[!UICONTROL Nunca]</strong> aqui, ainda poderá postar comentários manualmente em um item vinculado em [!DNL Workfront] ou em [!DNL Jira].</p></td>
        </tr>
       </tbody>
      </table>

1. Na seção **[!UICONTROL OTHER]**, selecione quais campos adicionais devem ser atualizados entre itens vinculados.

   1. Selecione uma opção para determinar se os campos que você especifica **[!UICONTROL Sempre]** ou **[!UICONTROL Nunca]** são atualizados em [!DNL Jira] ou [!DNL Workfront] quando são modificados.

   1. Selecione entre os seguintes campos e atualizações:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar Dados Personalizados [!DNL Workfront] no painel direito em [!DNL Jira]]</td>
         <td><p>Exibe os [!DNL Workfront] Dados Personalizados de um item no painel direito [!DNL Workfront].</p><p>Observação: as seções de Formulário personalizado são exibidas no painel direito do [!DNL Workfront] com o nível de acesso do Administrador do Sistema do [!DNL Workfront].</p></td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Copiar Prioridade [!DNL Workfront] no painel direito em [!DNL Jira]]</td>
         <td>Exibe a Prioridade [!DNL Workfront] de um item no painel direito [!DNL Workfront].</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Adicionar uma atualização na guia Atualizações [!DNL Workfront] sobre alterações da Data de Conclusão em [!DNL Jira]]</td>
         <td>Adiciona um comentário na guia [!UICONTROL Atualizar] do item [!DNL Workfront] quando a [!UICONTROL Data de Conclusão] é alterada no item [!DNL Jira] vinculado.</td>
        </tr>
        <tr>
         <td role="rowheader">[!UICONTROL Criar automaticamente um usuário em [!DNL Workfront] se o usuário [!DNL Jira] não tiver uma conta [!DNL Workfront]]</td>
         <td><p>Existem os seguintes cenários:</p>
          <ul>
           <li>Ao selecionar <strong>[!UICONTROL Always]</strong>, você habilita a integração para criar um novo usuário do Workfront sempre que um usuário do [!DNL Jira] sem uma conta do [!DNL Workfront] executar as seguintes ações em um problema do [!DNL Jira] vinculado:
            <ul>
             <li>Está atribuído a um problema [!DNL Jira]</li>
             <li><p>Registra o tempo em um problema [!DNL Jira]</p><p>Este novo usuário não ocupa uma licença do [!DNL Workfront]. A configuração padrão é Sempre. O usuário criado desta forma em [!DNL Workfront] adicionou "[!UICONTROL Jira]" ao seu nome.</p></li>
            </ul></li>
           <li>Quando você seleciona <strong>[!UICONTROL Nunca]</strong>, as seguintes coisas acontecem:
            <ul>
             <li>Você não pode ver nenhuma atribuição do [!DNL Jira] nos itens [!DNL Workfront]. Nesse caso, somente as atribuições feitas em [!DNL Workfront] são exibidas nos itens [!DNL Workfront].</li>
             <li>O tempo registrado em um problema [!DNL Jira] vinculado por um usuário sem uma conta [!DNL Workfront] não é transferido automaticamente para o item [!DNL Workfront] vinculado. Você ainda pode registrar horas no item [!DNL Workfront] no painel direito do problema [!DNL Jira].</li>
            </ul></li>
          </ul></td>
        </tr>
       </tbody>
      </table>

1. Clique em **[!UICONTROL Salvar]**.

   Agora, sempre que um usuário atualizar qualquer um dos campos especificados nessa configuração em um item no [!DNL Jira] ou [!DNL Workfront], o item vinculado no outro aplicativo também será atualizado.

## Solução de problemas

### Não é possível criar itens em [!DNL Jira] devido a campos de gatilho marcados como &quot;[!UICONTROL Não foi possível encontrar]&quot;

#### Problema

Quando ocorre um erro com o aplicativo [!DNL Workfront for Jira], o [!DNL Workfront] desabilita os disparadores para evitar mais complicações. Quando esses acionadores são desativados, eles são exibidos como &quot;[!UICONTROL Não foi possível encontrá-los]&quot;.

#### Solução

Localize o erro que desativou os acionadores. Você pode encontrar o erro no [!DNL Workfront for Jira] [!UICONTROL Log de atividades].

A causa mais comum desse comportamento é o erro &quot;[!UICONTROL O campo &#39;duedate&#39; não pode ser definido. Não está na tela apropriada, ou é desconhecido.]&quot;

Este erro significa que você está tentando sincronizar a &quot;[!UICONTROL Data de Término Planejada]&quot; de [!DNL Workfront] para [!DNL Jira]. Para fazer isso, você deve garantir que seus objetos [!DNL Jira] tenham um campo chamado &quot;[!UICONTROL Data de vencimento]&quot;. Se eles não tiverem esse campo, [!DNL Workfront] não poderá sincronizar a data de conclusão planejada de [!DNL Workfront] e desabilitará seus gatilhos.

Para resolver esse erro, tente uma das seguintes opções:

* Peça ao administrador do [!DNL Jira] para atualizar os objetos [!DNL Jira] afetados para garantir que eles tenham um campo de data de vencimento.
* Desabilite a sincronização da data de conclusão planejada de [!DNL Workfront] na página [!UICONTROL Instalação] da Workfront.
