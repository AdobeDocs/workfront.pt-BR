---
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: email-alerts-workfront-proof
title: Defina as configurações de notificação de email em [!DNL Workfront Proof]
description: As notificações por email informam os colaboradores sobre atividades recentes em provas, como comentários, respostas, decisões.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb82c075-e275-46b7-ac2c-ed50367f53a7
source-git-commit: 088570f516bbea2e6fd81b1f711151d8941ca71e
workflow-type: tm+mt
source-wordcount: '1998'
ht-degree: 0%

---

# Defina as configurações de notificação de email em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

As notificações por email informam os colaboradores sobre atividades recentes em provas, como comentários, respostas, decisões.

As notificações por email para revisores podem ser definidas na página Nova prova , [!UICONTROL Nova versão] e gerenciada na [!UICONTROL Fluxo de trabalho] da seção [!UICONTROL Detalhes da prova] página. Para obter mais informações, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md)

* [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

Cada usuário também pode definir suas próprias configurações de alerta de email que serão aplicadas automaticamente quando uma prova for compartilhada com ele. Se os colaboradores tiverem suas preferências ou se os administradores de conta tiverem suas recomendações sobre a frequência dos alertas. Isso pode ser definido como um padrão de prova nas páginas de detalhes do usuário.

>[!NOTE]
>
>Essas configurações são sugeridas quando os usuários estão criando as provas e adicionando esses colaboradores. No entanto, essas são apenas sugestões, portanto, podem ser ajustadas a qualquer momento durante o processo de revisão e as alterações se aplicam a todas as atividades feitas após a alteração. As configurações padrão da prova são substituídas pelas configurações no nível da prova.

Usuários com [!UICONTROL Administrador] ou [!UICONTROL Administrador de Faturamento] perfis também podem definir os padrões de prova para outros usuários em suas contas nas configurações da conta.

Para obter informações sobre perfis, consulte [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

* [Defina padrões de prova em configurações pessoais ([!DNL Workfront Proof] somente usuários)](#configure-proof-defaults-in-personal-settings-workfront-proof-users-only)
* [Alterar alertas de email de um recipient](#change-email-alerts-for-a-recipient)
* [Configurar padrões de prova para um usuário](#configure-proof-defaults-for-a-user)

## Defina padrões de prova em configurações pessoais ([!DNL Workfront Proof] somente usuários)

Você pode definir configurações de prova para provas criadas.

Para obter informações sobre configurações de prova, consulte [!DNL Workfront] administrador ou [!DNL Workfront Proof] administrador pode configurar, consulte .

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações pessoais]**.

1. Clique no botão **[!UICONTROL Padrões de prova]** guia .
1. Clique em **[!UICONTROL Configurações padrão de notificação de email]** para expandi-lo.
1. Na lista suspensa à direita das duas configurações a seguir, selecione uma das opções explicadas na tabela abaixo.

   * **[!UICONTROL Alerta de email padrão]**: Afeta todas as provas que são compartilhadas com você. Essa configuração pode ser substituída no nível da prova.
   * **[!UICONTROL Alerta por email padrão para novos revisores convidados]**: Afeta os revisores que não existiam anteriormente como contatos na sua conta.

   >[!NOTE]
   >
   >Se você não escolher uma das opções a seguir, [!DNL Workfront Proof] envia um resumo diário sobre a atividade em suas provas.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Todas as atividades]</td> 
      <td>O [!UICONTROL Workfront] envia um email para o revisor sempre que houver uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de verificação porque permite que ela veja a atividade como ela acontece. </p><p>Os usuários não recebem um alerta por email sobre sua própria atividade.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Respostas aos meus comentários]</td> 
      <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui suas próprias respostas em seus próprios comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para seus clientes na prova, de modo que eles não sejam notificados sobre nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta de email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador de prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder comentários de prova</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisões]</td> 
      <td>[!DNL Workfront] envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que gerencia o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não será notificado de sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Decisão final]</td> 
      <td>[!DNL Workfront] envia um email quando o último aprovador na prova tiver tomado a decisão.<p>Esse alerta é frequentemente usado pelo designer, que geralmente não precisa participar da discussão da revisão real. Quando a decisão final é tomada, o criador é notificado e pode tomar medidas relativamente às alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precisa ser notificado somente quando o processo de revisão for concluído.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumo por hora]</td> 
      <td>[!DNL Workfront] envia um email para o revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando uma atividade além da sua ocorrer na última hora. </p><p>Esse alerta é uma boa maneira de ver uma visão geral do projeto.</p><p>Um exemplo de uso desse resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Resumo diário]</td> 
      <td>[!DNL Workfront] envia um email com todos os comentários, respostas e decisões listados somente em dias em que há atividade além da sua.<p>Esse alerta é uma boa maneira de ver um resumo do projeto sem ficar sobrecarregado com várias atualizações ao longo do dia.</p><p>Um exemplo de uso deste resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários e decisões de prova</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">[!UICONTROL Sem email]</td> 
      <td>[!DNL Workfront] não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de quaisquer alterações.<p>O padrão do sistema é [!UICONTROL Daily summary] (também visto como [!UICONTROL Not Set]). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Altere qualquer um dos itens a seguir:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmação de email quando as provas estiverem prontas]</td> 
      <td>Especifique se deseja receber um email [!UICONTROL Proof made] ao criar uma prova. Para obter mais informações, consulte <a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">O email [!UICONTROL Proof Fade]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Formato dos emails enviados para mim]</strong> </td> 
      <td> <p>Escolha entre emails com HTML e texto sem formatação. </p> <p>Observação:  As configurações padrão da prova são substituídas pelas configurações no nível da prova. No entanto, se notificações por email de prova estiverem desativadas para toda a conta nas configurações da [!UICONTROL Conta], nenhum alerta por email será enviado aos colaboradores mesmo se o [!UICONTROL Disabled email alert] não estiver selecionado nas provas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Em **[!UICONTROL Configurações de mensagem]**, altere qualquer um dos seguintes itens:

   | **[!UICONTROL Modelo de assunto da prova]** | Exibe na página Nova prova, na página Nova versão, na página Mensagem e na página Lembrar. Pode ser editado antes de ser enviado. |
   |---|---|
   | **[!UICONTROL Modelo de mensagem de prova]** | Exibe na página Nova prova, na página Nova versão, na página Mensagem e na página Lembrar. Pode ser editado antes de ser enviado. |

   {style=&quot;table-layout:auto&quot;}

## Alterar alertas de email de um recipient

Você pode alterar alertas de email de um determinado recipient em uma ação em lote.

1. Clique em **[!UICONTROL Contatos]** no painel de navegação esquerdo.
1. Clique no botão **[!UICONTROL Mais]** (três pontos) para o recipient e, em seguida, clique em **[!UICONTROL Exibir detalhes do membro]** no menu suspenso.

1. Abra o **[!UICONTROL Itens compartilhados]** seção.
1. Marque a caixa de seleção à esquerda de cada item para o qual deseja alterar o alerta de email.
1. Clique em **[!UICONTROL Mais]** acima da lista de itens compartilhados, em seguida, clique em **[!UICONTROL Alterar alerta de email]** no menu suspenso.

1. Altere o alerta do email e clique em **[!UICONTROL Enviar]**.

## Configurar padrões de prova para um usuário

Se você for um [!DNL Workfront Proof] administrador, você pode definir padrões de prova para usuários em sua conta.

1. Clique em **[!UICONTROL Configurações]** > **[!UICONTROL Configurações da conta]**.

1. Abra o **[!UICONTROL Usuários]** guia .
1. Abra o **[!UICONTROL Mais]** à direita do nome do usuário. ![Mais_button_small.png](assets/more-button-small.png)

1. Clique em **[!UICONTROL Exibir detalhes dos usuários]** no menu suspenso.
1. Em **[!UICONTROL Configurações]**, clique em **[!UICONTROL Configurações padrão de alerta de email]** para expandi-lo.

1. Na lista suspensa à direita das duas configurações a seguir, selecione uma das opções explicadas na tabela abaixo:

   * **[!UICONTROL Alerta de email padrão]**: Afeta todas as provas que são compartilhadas com você. Essa configuração pode ser substituída no nível da prova.
   * **[!UICONTROL Alerta por email padrão para novos revisores convidados]**: Afeta os revisores que não existiam anteriormente como contatos na sua conta.

   >[!NOTE]
   >
   >Se você não escolher uma das opções a seguir para um usuário, [!DNL Workfront Proof] envia aos usuários um resumo diário sobre a atividade em suas provas.

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">[!UICONTROL Todas as atividades]</td>
      <td>[!DNL Workfront] envia um email para o revisor sempre que houver uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de verificação porque permite que ela veja a atividade como ela acontece. </p><p>Os usuários não recebem um alerta por email sobre sua própria atividade.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Respostas aos meus comentários]</td>
      <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui suas próprias respostas em seus próprios comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para seus clientes na prova, de modo que eles não sejam notificados sobre nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta de email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador de prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder comentários de prova</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisões]</td>
      <td>[!DNL Workfront] envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que gerencia o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não será notificado de sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Decisão final]</td>
      <td>[!DNL Workfront] envia um email quando o último aprovador na prova tiver tomado a decisão.<p>Esse alerta é frequentemente usado pelo designer, que geralmente não precisa participar da discussão da revisão real. Quando a decisão final é tomada, o criador é notificado e pode tomar medidas relativamente às alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precisa ser notificado somente quando o processo de revisão for concluído.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumo por hora]</td>
      <td>[!DNL Workfront] envia um email para o revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando uma atividade além da sua ocorrer na última hora. </p><p>Esse alerta é uma boa maneira de ver uma visão geral do projeto.</p><p>Um exemplo de uso desse resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td>
     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Resumo diário]</td>
      <td>[!DNL Workfront] envia um email com todos os comentários, respostas e decisões listados somente em dias em que há atividade além da sua.<p>Esse alerta é uma boa maneira de ver um resumo do projeto sem ficar sobrecarregado com várias atualizações ao longo do dia.</p><p>Um exemplo de uso deste resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários e decisões de prova</a>.</p></td>
     </tr>
     <tr data-mc-conditions="">
      <td role="rowheader">[!UICONTROL Sem email]</td>
      <td>[!DNL Workfront] não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de quaisquer alterações.<p>O padrão do sistema é [!UICONTROL Daily summary] (também visto como [!UICONTROL Not Set]). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td>
     </tr>
    </tbody>
   </table>

1. No restante **[!UICONTROL Configurações padrão de alerta de email]**, altere qualquer um dos seguintes itens:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Confirmação de email quando as provas estiverem prontas]</td> 
      <td>Especifique se deseja receber um email [!UICONTROL Proof made] ao criar uma prova. Para obter mais informações, consulte <a href="https://support.workfront.com/hc/en-us/article">O Email Da [!UICONTROL Proof Feed].</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Formato dos emails enviados para mim]</strong> </td> 
      <td> <p>Escolha entre emails com HTML e texto sem formatação. </p> <p>Observação:  As configurações padrão da prova são substituídas pelas configurações no nível da prova. No entanto, se notificações por email de prova estiverem desativadas para toda a conta nas configurações da [!UICONTROL Conta], nenhum alerta por email será enviado aos colaboradores mesmo se o [!UICONTROL Disabled email alert] não estiver selecionado nas provas.<br></p> </td> 
     </tr> 
    </tbody> 
   </table>
