---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Criar uma prova avançada com um fluxo de trabalho básico
description: Com um fluxo de trabalho básico, é possível incluir vários revisores em uma prova, mas eles não são organizados em estágios. Todos os revisores adicionados podem acessar a prova imediatamente após criá-la.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f5d0c0e-e070-4f32-89c4-3b511a3b7fdc
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '1853'
ht-degree: 1%

---

# Criar uma prova avançada com um fluxo de trabalho básico

<!-- Audited: 1/2024 -->

Com um fluxo de trabalho básico, é possível incluir vários revisores em uma prova, mas eles não são organizados em estágios. Todos os revisores adicionados podem acessar a prova imediatamente após criá-la.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>
   <p>Novo: Qualquer um</p>
    <p>Plano atual: Pro ou Superior</p>
   <p>Plano herdado: Select ou Higher</p> <p>Para obter mais informações sobre acesso de prova com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
    <p>Atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou perfil de permissão de prova você tem, entre em contato com o administrador do Workfront ou do Workfront Proof.

+++

## Criar uma prova avançada com um fluxo de trabalho básico

1. Vá para o projeto, tarefa ou problema em que deseja a prova e clique no link **Documentos** guia.
1. Clique em **Adicionar novo** > Revise, faça upload do conteúdo e trabalhe nas seções listadas abaixo.

   ou

   Passe o mouse sobre um documento existente, em seguida clique no **Criar prova** > **Prova avançada** e trabalhe nas seções listadas abaixo.

## Configurar o fluxo de trabalho e adicionar revisores

1. Na seção Tipo de fluxo de trabalho, escolha **Básico**.
1. Especifique os usuários que deseja adicionar e escolha uma função de Prova.

   ![](assets/new-proof---roles-350x213.png)

1. A tabela a seguir lista cada função e os direitos associados a ela.

   <table border="1" cellspacing="15" cellpadding="1"> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p> </p> </th> 
      <th> <p><strong>Exibir uma prova</strong> </p> </th> 
      <th> <p><strong>Adicionar marcações</strong> </p> </th> 
      <th> <p><strong>Adicionar comentários</strong> </p> </th> 
      <th> <p><strong>Editar comentários próprios se não houver respostas</strong> </p> </th> 
      <th> <p><strong>Tomar uma decisão</strong> </p> </th> 
      <th> <p><strong>Excluir comentários feitos por outros</strong> </p> </th> 
      <th>Resolver comentários</th> 
      <th>Aplicar ações a comentários</th> 
      <th> <p><strong>Editar a prova</strong> </p> </th> 
      <th>Compartilhar a prova com outras pessoas</th> 
      <th>Criar nova versão</th> 
      <th> <p><strong>Exibir solicitações de aprovação na área Página inicial</strong> </p> </th> 
      <th>Adicionar novos revisores</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p><strong>Somente leitura</strong> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓ µ</td> 
      <td> <p> </p> </td> 
      <td>✓ µ</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Oliveira</strong> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓ µ</td> 
      <td> <p> </p> </td> 
      <td>✓ µ</td> 
      <td> </td> 
      <td> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Aprovador</strong> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓ µ</td> 
      <td> <p> </p> </td> 
      <td>✓ µ</td> 
      <td> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Revisor e Aprovador</strong> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p> </p> </td> 
      <td> </td> 
      <td>✓ µ</td> 
      <td> <p> </p> </td> 
      <td>✓ µ</td> 
      <td> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> </td> 
     </tr> 
     <tr> 
      <td> <p><strong>Autor</strong> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p> </p> </td> 
      <td>✓ µ</td> 
      <td>✓ µ</td> 
      <td> <p>✓ µ</p> </td> 
      <td>✓ µ</td> 
      <td>✓ µ</td> 
      <td> </td> 
      <td>✓ µ</td> 
     </tr> 
     <tr> 
      <td> <p><strong>Moderador</strong> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p><strong>✓ µ</strong> </p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> </td> 
      <td> <p>✓ µ</p> <p> </p> </td> 
      <td>✓ µ</td> 
      <td>✓ µ</td> 
      <td> <p>✓ µ</p> </td> 
      <td>✓ µ</td> 
      <td>✓ µ</td> 
      <td>✓ µ</td> 
      <td>✓ µ</td> 
     </tr> 
    </tbody> 
   </table>

1. Os usuários nos novos planos do Workfront podem conceder funções de autor ou moderador a qualquer usuário no sistema. Os usuários em planos herdados podem conceder funções de autor ou moderador a qualquer usuário com uma licença de prova no sistema.
1. (Opcional) Com o menu suspenso ainda aberto, selecione as permissões adicionais disponíveis na parte inferior do menu:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Resolver comentários e aplicar ações </td> 
      <td> <p>Permite que o usuário do Workfront faça o seguinte:</p> 
       <ul> 
        <li>Resolva um comentário depois que ele for abordado, conforme explicado em <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/resolve-proof-comments.md" class="MCXref xref">Resolver comentários de prova</a>.</li> 
        <li>Aplique ações a comentários, conforme explicado em <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md" class="MCXref xref">Usar ações em comentários de prova</a>. </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar prova por meio de etiqueta</td> 
      <td> <p>Permite que o revisor adicione qualquer usuário do Workfront à prova, conforme explicado em <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/tag-users-to-share-proof.md" class="MCXref xref">Adicione tags aos usuários para compartilhar uma prova</a>.</p> <p>Nota:  <p>Se essas duas opções não estiverem disponíveis (esmaecidas), o usuário já terá um perfil de permissão que permite resolver comentários, aplicar ações a comentários e marcar qualquer usuário. </p> <p>Se as opções não forem exibidas, a pessoa adicionada não será um titular de licença da Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Repita as etapas 1 a 3 para qualquer outro usuário adicionado à prova.
1. Para cada usuário com o qual você está compartilhando, na **Alertas de email** selecione o tipo de alertas de email que esse usuário recebe quando as pessoas fazem comentários e tomam decisões sobre a prova:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Todas as atividades</td> 
      <td>O Workfront envia um email para o revisor sempre que há uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de prova, pois permite que ela veja a atividade enquanto ela acontece. </p><p>Os usuários não recebem um alerta por email sobre suas próprias atividades.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Respostas aos meus comentários</td> 
      <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui as próprias respostas nos comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para os clientes na prova, para que não sejam notificados de nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta por email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador da prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder a comentários de prova</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisões</td> 
      <td>O Workfront envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que está gerenciando o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não é notificado sobre sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Decisão final</td> 
      <td>O Workfront envia um email quando o último aprovador na prova toma sua decisão.<p>Esse alerta é usado com frequência pelo designer, que geralmente não precisa participar da discussão de revisão real. Quando a decisão final é tomada, o designer é notificado e pode então tomar medidas em relação a quaisquer alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precise ser notificado somente quando o processo de revisão for concluído.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumo por Hora</td> 
      <td>O Workfront envia um email ao revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando a atividade além da sua ocorre na última hora. </p><p>Este alerta é uma boa maneira de ter uma visão geral do projeto.</p><p>Um exemplo de caso de uso para este resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resumo Diário</td> 
      <td>O Workfront envia um email com todos os comentários, respostas e decisões listados somente em dias quando houver atividade além da sua.<p>Este alerta é uma boa maneira de ver um resumo do projeto sem precisar de várias atualizações ao longo do dia.</p><p>Um exemplo de caso de uso para este resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários e decisões de prova</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nenhum email</td> 
      <td>O Workfront não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de qualquer alteração.<p>O padrão do sistema é Resumo diário (também visto como Não definido). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Continuar com [Definir configurações de email para a prova](#configure-email-settings-for-the-proof) abaixo.

## Definir configurações de email para a prova {#configure-email-settings-for-the-proof}

1. No **Notificação por e-mail** selecione se deseja enviar notificações por email e uma mensagem personalizada para os usuários selecionados no [Criar uma prova avançada com um fluxo de trabalho básico](#workflow) anteriormente neste artigo:

   <table>
   <tbody>
   <tr>
   <td>Notificar recipients sobre esta prova</td>
   <td>Selecione esta opção para enviar uma notificação por e-mail aos usuários. Quando <strong>Compartilhamento básico</strong> está selecionado no <strong>Fluxo de trabalho</strong> , uma notificação por email é enviada quando a prova é criada. Quando <strong>Fluxo de trabalho automático</strong> está selecionado no <strong>Fluxo de trabalho</strong> , uma notificação por email é enviada quando a prova entra no estágio do Fluxo de trabalho automatizado ao qual o usuário está associado.</td>
   </tr>
   <tr>
   <td>Adicionar mensagem personalizada</td>
   <td>Selecione essa opção para incluir uma mensagem personalizada na notificação. Você pode especificar um assunto e um corpo de mensagem. O corpo da mensagem pode incluir formatação de rich text, como negrito, marcadores e hiperlinks.</td>
   </tr>
   </tbody>
   </table>


1. Continuar com [Definir configurações de prova](#configure-proof-settings) abaixo.

## Definir configurações de prova {#configure-proof-settings}

1. No **Configurações de prova** selecione uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exigir logon - a prova só pode ser compartilhada com outros usuários</td> 
      <td>Quando essa opção está desativada (padrão), qualquer pessoa com o URL pode exibir a prova. <br>Quando esta opção é selecionada:
       <ul>
        <li>Somente usuários do Workfront Proof podem exibir a prova.</li>
        <li>Os usuários não podem fazer logon na prova a menos que tenham sido adicionados à prova.</li>
        <li>Não é possível habilitar assinaturas.</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">É necessária somente uma decisão para essa prova</td> 
      <td>Quando essa opção é selecionada, a revisão é concluída após um dos tomadores de decisão tomar sua decisão.<br>Essa opção está desativada por padrão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente</td> 
      <td>Os usuários são solicitados a especificar seu nome de usuário e senha no momento em que tomam uma decisão sobre uma prova.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prova quando todas as decisões necessárias forem tomadas</td> 
      <td>Quando essa configuração estiver ativada, o estado da prova será bloqueado depois que todas as decisões forem tomadas. O estado é alterado automaticamente de desbloqueado para bloqueado quando o aprovador final toma sua decisão.<br>Essa opção está desativada por padrão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Baixar arquivo original</td> 
      <td>Quando essa opção é selecionada, os revisores podem baixar o arquivo original do qual a prova foi criada.<br>Quando essa opção é desmarcada, o ícone Download não fica mais visível.<br>Essa opção está ativada por padrão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar prova por meio de URL público ou código de inserção</td> 
      <td>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código integrado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inscrever-se para obter prova por meio de URL público ou código incorporado</td> 
      <td>Quando essa opção é selecionada, as pessoas que não foram adicionadas explicitamente à prova podem assinar a prova. A pessoa que se inscreve na prova recebe a função e o email definidos nas seguintes configurações:
       <ul>
        <li><strong>Função do assinante:</strong> A função de prova padrão atribuída a todos os revisores que assinam a prova. </li>
        <li><strong>Configurações de alerta de email para assinantes:</strong> O alerta de email padrão atribuído a todos os revisores que assinam a prova.</li>
       </ul><p>
        <ul>
         <li><strong>É necessário acessar a prova por link de email para:</strong> Configure se o assinante receberá um email com um link para a prova. É possível selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova. A finalidade dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</li>
        </ul><p>Observação: se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para os Proprietários da prova, para que eles possam decidir em qual estágio a pessoa deve ser adicionada.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Criar prova**.

   O Workfront começa a gerar uma prova dos documentos ou sites selecionados. Dependendo do tamanho e do tipo do arquivo, o tempo de atraso no upload de um documento pode variar. Seja paciente, pois arquivos maiores demoram mais para serem gerados. Você pode sair da página e o Workfront continua a gerar seu arquivo. O tamanho máximo do upload de arquivo é 4 GB.

1. Após gerar a prova, clique em **Abrir prova** para iniciar o revisor de provas.

   ![](assets/open-proof-350x132.png)

   Os usuários que não têm a prova ativada em suas contas ainda podem exibir o documento e fazer comentários na prova.