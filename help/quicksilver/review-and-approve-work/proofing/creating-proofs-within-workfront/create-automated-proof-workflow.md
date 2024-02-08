---
product-area: documents;setup
navigation-topic: create-proofs-within-workfront
title: Criar uma prova avançada com um fluxo de trabalho automatizado
description: Um fluxo de trabalho automatizado facilita o gerenciamento do processo de revisão se o processo for complexo ou se você enviar conteúdo para revisão para as mesmas pessoas regularmente. A prova vai de estágio em estágio e o Adobe Workfront notifica cada usuário quando chegar a sua vez de revisá-la. Para obter mais informações sobre fluxos de trabalho automatizados, consulte Visão geral do fluxo de trabalho automatizado.
author: Courtney
feature: Digital Content and Documents
exl-id: 977fe1bc-458f-4301-8056-dc51c61edb6c
source-git-commit: ccfea4cdf7280f992068bc64bab27e63aaab8b74
workflow-type: tm+mt
source-wordcount: '1820'
ht-degree: 0%

---

# Criar uma prova avançada com um fluxo de trabalho automatizado

<!-- Audited: 2/2024 -->

Um fluxo de trabalho automatizado facilita o gerenciamento do processo de revisão se o processo for complexo ou se você enviar conteúdo para revisão para as mesmas pessoas regularmente. A prova vai de estágio em estágio e o Adobe Workfront notifica cada usuário quando chegar a sua vez de revisá-la. Para obter mais informações sobre workflows automatizados, consulte [Visão geral do fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Novo: Qualquer um</p><p>Plano atual: Pro ou Superior</p><p>Plano herdado: Select ou Higher</p> <p>Para obter mais informações sobre acesso de prova com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Padrão</p><p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Criar uma prova avançada com um fluxo de trabalho automatizado

1. Vá para o projeto, tarefa ou problema em que deseja a prova e clique no link **Documentos** guia.
1. Clique em **Adicionar novo** > Revise, faça upload do conteúdo e trabalhe nas seções listadas abaixo.

   ou

   Passe o mouse sobre um documento existente, em seguida clique no **Criar prova** > **Prova avançada** e trabalhe nas seções listadas abaixo.

## Configurar os estágios de prova

1. Na seção Tipo de fluxo de trabalho, escolha **Automatizado**.
1. (Opcional) Se quiser usar um modelo de Fluxo de trabalho automatizado que o administrador do Workfront criou e compartilhou com você, clique em **Adicionar modelo**, selecione o modelo na caixa exibida e clique em **Adicionar modelo**.

   >[!NOTE]
   >
   >Considere o seguinte ao usar um modelo de Fluxo de trabalho automatizado:
   >   
   >* As configurações de um modelo de Fluxo de trabalho automatizado determinam o que você pode fazer com o Fluxo de trabalho automatizado para uma prova. Por exemplo, se o botão Adicionar um estágio estiver desativado no modelo, ele não ficará visível enquanto você trabalhar com as configurações de Fluxo de trabalho automatizado para a prova.
   >* Quando uma pessoa é adicionada a um estágio em um modelo de Fluxo de trabalho automatizado, mas também já está presente como revisor na prova, a aplicação do modelo remove o revisor do estágio. Se você não adicionar outro revisor ao estágio, uma mensagem solicitará que você adicione um.
   >* Sua capacidade de modificar um modelo de Fluxo de trabalho automatizado depende das configurações do modelo definidas pelo administrador do Workfront, conforme descrito em . Se a capacidade de modificar o modelo estiver desativada, somente o proprietário do modelo poderá modificá-lo.

1. Configure o primeiro estágio do fluxo de trabalho automatizado:

   1. (Opcional) Se quiser criar um nome para o primeiro estágio, clique em **Estágio 1** e digite o nome.
   1. No **Destinatários** para o estágio, adicione revisores ao estágio.

      >[!NOTE]
      >
      >Considere o seguinte ao adicionar revisores a um estágio:
      >   
      >* Você pode adicionar usuários externos a um estágio com um endereço de email.
      >* Depois de adicionar um usuário a um estágio, você pode definir as configurações para esse usuário na prova.
      >* Você pode arrastar os usuários diretamente para outro estágio ou arrastar os usuários para um estágio na **Estágios** diagrama. Para selecionar vários usuários, pressione Shift+Ctrl (no Windows) ou Shift+Command (no Mac).
      >* É possível adicionar um revisor a uma prova apenas uma vez, o que significa que não é possível adicionar a mesma pessoa a mais de um estágio na prova.
      >* Os revisores que não são adicionados a um estágio privado não podem ver esse estágio na prova ou nos comentários feitos nesse estágio.
      >* Por padrão, adicionar um usuário a um estágio concede a ele acesso para visualizar a prova a partir do momento em que a prova é criada. O administrador do Workfront pode impedir que os usuários acessem a prova até que o fluxo de trabalho entre no estágio em que o usuário foi adicionado.

   1. Clique em **Configurações de preparo**.
   1. Clique em um **Ativar estágio** opção para indicar como você deseja que o estágio seja ativado.

      Para o primeiro estágio, é possível selecionar apenas **Na criação da prova**, **Em uma data e hora específicas** ou **Manualmente**.

   1. (Condicional) Se você selecionou **Em uma data e hora específicas** na etapa anterior, selecione a data e a hora em que deseja ativar o estágio na variável **Ativar em** que aparece.

   1. Use qualquer uma das opções abaixo para configurar ainda mais o estágio.

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Definir prazo final da fase</td>
         <td><p>Para definir um prazo para o estágio, clique em uma opção na <strong>Opções de prazo final</strong> lista suspensa. Em seguida, em <strong>Prazo</strong>, execute um dos procedimentos a seguir:</p>
          <ul>
           <li>Se você escolher <strong>Definir data específica</strong>: selecione a data e a hora do prazo que deseja.</li>
           <li>Se você escolher <strong>Calcular a partir da data de ativação do estágio</strong>: selecione o número de dias úteis que deseja adicionar à data de ativação do estágio para determinar o prazo.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bloquear estágio</td>
         <td>Especifique quando o estágio pode ser bloqueado. </td>
        </tr>
        <tr>
         <td role="rowheader">Transferir direitos de decisão primários para</td>
         <td><p>Selecione o tomador de decisão principal no estágio (disponível somente depois de adicionar pelo menos uma pessoa ao estágio que tenha uma função de Aprovador ou superior). Se você selecionar um tomador de decisão principal, a variável <strong>É necessária somente uma decisão</strong> está desabilitada neste estágio.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Requer apenas uma decisão para este estágio</td>
         <td>Encerra todo o processo de revisão quando um dos tomadores de decisão toma uma decisão.<p>Essa opção não estará disponível se você tiver designado um usuário na <strong>Tomador de decisão principal</strong>menu suspenso.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Tornar privado este estágio</td>
         <td>Permite que apenas as seguintes pessoas visualizem comentários e decisões tomadas durante esse estágio: Supervisores, administradores do Workfront e administradores do Workfront Proof</td>
        </tr>
       </tbody>
      </table>

1. Para adicionar e configurar outro estágio:

   1. Clique em **Nova etapa**.
   1. (Opcional) Se quiser criar um nome para o primeiro estágio, clique em **Estágio 2** (ou **Estágio 3**, **Estágio 4** e assim por diante), em seguida, digite o nome.

   1. Clique em **Ativar estágio** e selecione uma opção para especificar se o estágio é ativado automática ou manualmente.

      Além das opções **Na criação da prova**, **Em uma data e hora específicas** ou **Manualmente**, você pode selecionar uma opção que depende do que ocorreu na etapa anterior:

      ![](assets/activate-stage-options-for-stage-2-plus-350x177.png)

   1. Se você selecionou uma opção Ativar estágio dependente do que ocorreu na etapa anterior, use as opções exibidas para definir a configuração de ativação.

      Por exemplo, se você selecionou **Quando o status do estágio anterior é alterado**, selecione o **Fase anterior**, em seguida, selecione o status na **Status alterado para** caixa.

1. Repita a etapa anterior conforme necessário para adicionar mais estágios.

   À medida que você adiciona estágios ao Fluxo de Trabalho Automatizado, um diagrama se forma na tela para representá-los:

   ![](assets/stages-diagram-350x213.png)

1. Continuar com [Definir configurações de email para a prova](#configure-email-settings-for-the-proof) abaixo.

## Definir configurações de email para a prova {#configure-email-settings-for-the-proof}

1. No **Notificação por e-mail** selecione se deseja enviar notificações por email e uma mensagem personalizada para os usuários selecionados no [Criar uma prova avançada com um fluxo de trabalho automatizado](#workflow) anteriormente neste artigo:

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
        <li>Somente usuários do Workfront Proof podem visualizar a prova.</li>
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
        <li><strong>Função do assinante:</strong> A função de prova padrão atribuída a todos os revisores que assinam a prova.</li>
        <li><strong>Configurações de alerta de email para assinantes:</strong> O alerta de email padrão atribuído a todos os revisores que assinam a prova.</li>
       </ul><p>
        <ul>
         <li><strong>É necessário acessar a prova por link de email para:</strong> Configure se o assinante receberá um email com um link para a prova. É possível selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova. A finalidade dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</li>
        </ul><p><strong>Nota:</strong> Se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para os Proprietários da prova, para que eles possam decidir em qual estágio a pessoa deve ser adicionada.<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Criar prova**.

   O Workfront começa a gerar uma prova dos documentos ou sites selecionados. Dependendo do tamanho e do tipo do arquivo, o tempo de atraso no upload de um documento pode variar. Seja paciente, pois arquivos maiores demoram mais para serem gerados. Você pode sair da página e o Workfront continua a gerar seu arquivo. O tamanho máximo do upload de arquivo é 4 GB.

1. Após gerar a prova, clique em **Abrir prova** para iniciar o revisor de provas.

   ![](assets/open-proof-350x132.png)

   Os usuários que não têm a prova ativada em suas contas ainda poderão exibir o documento e fazer comentários na prova [.](../../../timesheets/config-timesheet-prefs/config-time-logged-hrs-days.md)
