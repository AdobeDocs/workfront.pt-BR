---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Definir configurações de notificação por email no [!DNL Workfront Proof]
description: As notificações por email geradas pelo Workfront Proof informam os colaboradores sobre a atividade recente de provas, como comentários, respostas ou decisões.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: e80a3ede9ccf6ccf9ea7777aab35cc859f13a6ac
workflow-type: tm+mt
source-wordcount: '2058'
ht-degree: 0%

---

# Definir configurações de notificação por email no [!DNL Workfront Proof]

<!--Audited: 01/2024-->

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro do [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

As notificações por email informam os colaboradores sobre atividades recentes em provas, como comentários, respostas ou decisões.

É possível definir notificações por email para revisores nas seguintes áreas:

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
<tr> 
   <td role="rowheader">Produto</td> 
   <td>Workfront Proof Standalone</td> 
  </tr> 
</table>

As notificações por email para revisores podem ser definidas na página Nova prova, [!UICONTROL Nova versão] e gerenciado na [!UICONTROL Fluxo de trabalho] seção do [!UICONTROL Detalhes da prova] página. Para obter mais informações, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* A página Nova prova
* A variável [!UICONTROL Nova versão] página
* A variável [!UICONTROL Fluxo de trabalho] seção do [!UICONTROL Detalhes da prova] página.

Para obter mais informações, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)


* [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Gerenciar detalhes da prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).


Cada usuário também pode definir suas próprias configurações de alerta por email, que são aplicadas automaticamente quando uma prova é compartilhada com ele se os colaboradores tiverem suas preferências ou os administradores de conta tiverem suas recomendações sobre a frequência de alertas. Isso pode ser definido como um padrão de prova nas páginas de detalhes do usuário.

Cada usuário também pode definir suas próprias configurações de alerta de email, que serão aplicadas automaticamente quando uma prova for compartilhada com ele. <!--If the collaborators have their preferences, or account administrators have their recommendation on alerts frequency. This can be set as a proof default on the users details pages.-->

>[!NOTE]
>
>Essas configurações são sugeridas quando os usuários estão criando as provas e adicionando esses colaboradores. No entanto, essas são apenas sugestões, para que possam ser ajustadas a qualquer momento durante o processo de revisão e as alterações se apliquem a todas as atividades feitas após a alteração. As configurações padrão de prova são substituídas pelas configurações no nível da prova.

Usuários com [!UICONTROL Administrador] ou [!UICONTROL Administrador de Cobrança] Os perfis também podem definir os padrões de prova para outros usuários em sua conta nas configurações da Conta.

Para obter informações sobre perfis, consulte [Perfis de permissões de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Configurar padrões de prova em configurações pessoais ([!DNL Workfront Proof] somente usuários)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [Alterar alertas de email de um destinatário](#change-email-alerts-for-a-recipient)
* [Configurar padrões de prova para um usuário](#configure-proof-defaults-for-a-user)

## Configurar padrões de prova em configurações pessoais ([!DNL Workfront Proof] somente usuários)

É possível definir configurações de prova para provas criadas por você.

<!--For information about proof settings the [!DNL Workfront] administrator or [!DNL Workfront Proof] administrator can configure, see .-->

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações pessoais]**.

1. Clique em **[!UICONTROL Padrões de provas]** guia.
1. Clique em **[!UICONTROL Configurações padrão de notificação por email]** para expandi-la.
1. Na lista suspensa à direita das duas configurações a seguir, selecione uma das opções explicadas na tabela abaixo.

   * **[!UICONTROL Alerta de email padrão]**: afeta todas as provas compartilhadas com você. Essa configuração pode ser substituída no nível da prova.
   * **[!UICONTROL Alerta de email padrão para novos revisores convidados]**: afeta revisores que não existiam anteriormente como contatos em sua conta.

   >[!NOTE]
   >
   >Se você não escolher uma das opções a seguir, [!DNL Workfront Proof] O envia um resumo diário sobre a atividade em suas provas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Toda a atividade]</td> 
      <td>A [!UICONTROL Workfront] envia um email para o revisor sempre que há alguma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de prova, pois permite que ela veja a atividade enquanto ela acontece. </p><p>Os usuários não recebem um alerta por email sobre suas próprias atividades.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Respostas aos meus comentários]</td> 
      <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui as próprias respostas nos comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para os clientes na prova, para que não sejam notificados de nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta por email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador da prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder a comentários de prova</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisões]</td> 
      <td>[!DNL Workfront] O envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que está gerenciando o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não é notificado sobre sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisão final]</td> 
      <td>[!DNL Workfront] envia um email quando o último aprovador na prova toma sua decisão.<p>Esse alerta é usado com frequência pelo designer, que geralmente não precisa participar da discussão de revisão real. Quando a decisão final é tomada, o designer é notificado e pode então tomar medidas em relação a quaisquer alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precise ser notificado somente quando o processo de revisão for concluído.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumo por Hora]</td> 
      <td>[!DNL Workfront] envia um email ao revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando a atividade além da sua ocorre na última hora. </p><p>Este alerta é uma boa maneira de ter uma visão geral do projeto.</p><p>Um exemplo de caso de uso para este resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumo Diário]</td> 
      <td>[!DNL Workfront] O envia um email com todos os comentários, respostas e decisões listados somente nos dias em que houver atividade além da sua.<p>Este alerta é uma boa maneira de ver um resumo do projeto sem precisar de várias atualizações ao longo do dia.</p><p>Um exemplo de caso de uso para este resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários e decisões de prova</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Sem email]</td> 
      <td>[!DNL Workfront] O não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de qualquer alteração.<p>O padrão do sistema é [!UICONTROL Resumo diário] (também visto como [!UICONTROL Não definido]). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Altere qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmação de email quando as provas estiverem prontas]</td> 
      <td>Especifique se deseja receber um email [!UICONTROL Proof made] ao criar uma prova. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">O email [!UICONTROL Proof Made]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Formato dos emails enviados para mim] </td> 
      <td> <p>Escolha entre emails com estilo HTML e emails de texto sem formatação. </p> <p><b>Nota</b></p>
      <p>As configurações padrão de prova são substituídas pelas configurações no nível da prova. No entanto, se as notificações por email de prova estiverem desabilitadas para toda a conta nas configurações da [!UICONTROL Conta], nenhum alerta por email será enviado aos colaboradores, mesmo que o [!UICONTROL Alerta de email Desabilitado] não esteja selecionado nas provas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Em **[!UICONTROL Configurações de mensagem]**, altere qualquer uma das seguintes opções:

   | Modelo de prova | Descrição |
   |---|---|
   | **[!UICONTROL Modelo de assunto da prova]** | É exibido nas páginas Nova prova, Nova versão, Mensagem e Lembrar. Pode ser editado antes de ser enviado. |
   | **[!UICONTROL Modelo de mensagem de prova]** | É exibido na página Nova prova, Nova versão, Mensagem e Lembrar. Pode ser editado antes de ser enviado. |

## Alterar alertas de email de um destinatário

Você pode alterar alertas de email para um determinado recipient em uma ação em lote.

1. Clique em **[!UICONTROL Contatos]** no painel de navegação esquerdo.
1. Clique em **[!UICONTROL Mais]** menu ![](assets/more-button-small.png) para o recipient e clique em **[!UICONTROL Exibir detalhes do membro]** no menu suspenso.

1. Abra o **[!UICONTROL Itens compartilhados]** seção.
1. Marque a caixa de seleção à esquerda de cada item para o qual deseja alterar o alerta de email.
1. Clique em **[!UICONTROL Mais]** acima da lista de itens compartilhados, clique em **[!UICONTROL Alterar alerta de email]** no menu suspenso.

1. Altere o alerta de email e clique em **[!UICONTROL Enviar]**.

## Configurar padrões de prova para um usuário

Se você é um [!DNL Workfront Proof] administrador, você pode definir padrões de prova para os usuários em sua conta.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**.

1. Abra o **[!UICONTROL Usuários]** guia.
1. Abra o **[!UICONTROL Mais]** menu ![Mais_botão_pequeno.png](assets/more-button-small.png) à direita do nome do usuário.

1. Clique em **[!UICONTROL Exibir detalhes de usuários]** no menu suspenso.
1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Configurações padrão de alerta por email]** para expandi-la.

1. Na lista suspensa à direita das duas configurações a seguir, selecione uma das opções explicadas na tabela abaixo:

   * **[!UICONTROL Alerta de email padrão]**: afeta todas as provas compartilhadas com você. Essa configuração pode ser substituída no nível da prova.
   * **[!UICONTROL Alerta de email padrão para novos revisores convidados]**: afeta revisores que não existiam anteriormente como contatos em sua conta.

   >[!NOTE]
   >
   >Se você não escolher uma das seguintes opções para um usuário, [!DNL Workfront Proof] O envia aos usuários um resumo diário sobre a atividade em suas provas.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Toda a atividade]</td>
      <td>[!DNL Workfront] O envia um email para o revisor sempre que há uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de prova, pois permite que ela veja a atividade enquanto ela acontece. </p><p>Os usuários não recebem um alerta por email sobre suas próprias atividades.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Respostas aos meus comentários]</td>
      <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui as próprias respostas nos comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para os clientes na prova, para que não sejam notificados de nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta por email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador da prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder a comentários de prova</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisões]</td>
      <td>[!DNL Workfront] O envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que está gerenciando o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não é notificado sobre sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisão final]</td>
      <td>[!DNL Workfront] envia um email quando o último aprovador na prova toma sua decisão.<p>Esse alerta é usado com frequência pelo designer, que geralmente não precisa participar da discussão de revisão real. Quando a decisão final é tomada, o designer é notificado e pode então tomar medidas em relação a quaisquer alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precise ser notificado somente quando o processo de revisão for concluído.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumo por Hora]</td>
      <td>[!DNL Workfront] envia um email ao revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando a atividade além da sua ocorre na última hora. </p><p>Este alerta é uma boa maneira de ter uma visão geral do projeto.</p><p>Um exemplo de caso de uso para este resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumo Diário]</td>
      <td>[!DNL Workfront] O envia um email com todos os comentários, respostas e decisões listados somente nos dias em que houver atividade além da sua.<p>Este alerta é uma boa maneira de ver um resumo do projeto sem precisar de várias atualizações ao longo do dia.</p><p>Um exemplo de caso de uso para este resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários e decisões de prova</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Sem email]</td>
      <td>[!DNL Workfront] O não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de qualquer alteração.<p>O padrão do sistema é [!UICONTROL Resumo diário] (também visto como [!UICONTROL Não definido]). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td>
     </tr>
    </tbody>
   </table>

1. No restante **[!UICONTROL Configurações padrão de alerta por email]**, altere qualquer uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmação de email quando as provas estiverem prontas]</td> 
      <td>Especifique se deseja receber um email [!UICONTROL Proof made] ao criar uma prova. Para obter mais informações, consulte <a href="https://support.workfront.com/hc/en-us/article">Email [!UICONTROL Proof Made].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Formato dos emails enviados para mim] </td> 
      <td> <p>Escolha entre emails com estilo HTML e emails de texto sem formatação. </p> <p><b>Nota</b></p> <p>As configurações padrão de prova são substituídas pelas configurações no nível da prova. No entanto, se as notificações por email de prova estiverem desabilitadas para toda a conta nas configurações da [!UICONTROL Conta], nenhum alerta por email será enviado aos colaboradores, mesmo que o [!UICONTROL Alerta de email Desabilitado] não esteja selecionado nas provas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
