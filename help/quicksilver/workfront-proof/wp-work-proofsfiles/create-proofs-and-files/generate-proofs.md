---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Gerar provas em [!DNL Workfront Proof]
description: O Workfront Proof permite criar provas de documentos ou sites e compartilhá-las com outras pessoas. As etapas a seguir descrevem as várias opções de configuração disponíveis - EDITAR-ME.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '2267'
ht-degree: 0%

---

# Gerar provas em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

[!DNL Workfront Proof] O permite criar provas de documentos ou sites e compartilhá-las com outras pessoas. As etapas a seguir descrevem as várias opções de configuração disponíveis:

## Gerar uma prova para um documento

1. Siga qualquer um destes procedimentos para começar a criar uma nova prova e exibir a variável [!UICONTROL Nova prova] página:

   * Clique na cor verde **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * No **[!UICONTROL Painel]** na **[!UICONTROL Visão geral]** clique no botão **[!UICONTROL Nova prova]** link .

   * Enviar via Dropzone (recurso Enterprise).
   * O **[!UICONTROL Nova prova]** será exibida.

1. Para provar um ou mais documentos, adicione documentos a serem provas de uma das seguintes maneiras (repita esse processo para adicionar vários documentos a serem provas):

   * Arraste um documento do sistema de arquivos para a área de arrastar e soltar na **[!UICONTROL Adicionar arquivos]** área.
   * Clique na área de arrastar e soltar na **[!UICONTROL Adicionar arquivos]** em seguida, procure e selecione o documento que deseja fazer upload do sistema de arquivos na sua estação de trabalho.

      ![proof_document_upload.png](assets/proof-document-upload-350x64.png)

1. Para provar um ou mais sites, especifique o URL do site que deseja testar na **[!UICONTROL Adicionar arquivos]** e pressione **[!UICONTROL Enter]**.

1. (Opcional) Repita esse processo para adicionar vários sites à prova.

   Para obter mais detalhes sobre sites de prova, consulte [Gerar uma prova para um URL](#generate-a-proof-for-a-url).

   ![](assets/proof-website-350x65.png)

1. (Opcional) Modifique os nomes de arquivo de qualquer arquivo carregado:

   1. Passe o mouse sobre o nome do documento que deseja modificar na lista de documentos na **[!UICONTROL Adicionar arquivos]** e clique no botão **[!UICONTROL Editar]** ícone .

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. No **[!UICONTROL Nome da prova]** , especifique um novo nome e clique em **[!UICONTROL Concluído]**.

   1. (Opcional) Para excluir arquivos de serem carregados, passe o mouse sobre o documento que deseja excluir na lista de documentos na **[!UICONTROL Adicionar arquivos]** e clique no botão **[!UICONTROL Excluir]** ícone .

      ![proof_delete.png](assets/proof-delete-350x53.png)

   1. (Opcional) Ative a opção , **[!UICONTROL Combinar todos os arquivos compatíveis em uma única prova]**.

      **Quando esta opção é ativada:** Todos os arquivos estáticos e sites estão disponíveis em uma única prova e você pode fazer upload de até 50 arquivos em um determinado momento.

      >[!NOTE]
      >
      >Os arquivos interativos, incluindo vídeos e sites interativos, não podem ser combinados em uma única prova.

      **Quando esta opção está desativada:** Todos os documentos e sites são gerados como provas individuais e você pode carregar até 20 arquivos em um determinado momento.

      Para combinar todos os arquivos e sites carregados em uma única prova:

      1. Ative a opção , **[!UICONTROL Combinar todos os arquivos compatíveis em uma única prova]**.
      1. No **[!UICONTROL Nome da prova]** , especifique um novo nome para a prova combinada.
      1. No **[!UICONTROL Adicionar arquivos]** , reordene os arquivos incluídos arrastando um arquivo para a ordem desejada. A ordem dos arquivos é a ordem de página da prova combinada. Para obter mais informações sobre como criar provas combinadas, consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Opcional) Se você quiser usar um fluxo de trabalho automatizado que inclua vários estágios, na variável **[!UICONTROL Fluxo de trabalho]** selecione uma das seguintes opções:

   * **Básico:** Selecione essa opção para designar usuários que você deseja que tenham acesso à prova imediatamente após sua criação. Você pode compartilhar a prova com vários usuários.

      Para obter mais informações sobre como compartilhar uma prova, consulte &quot;Adicionar usuários a uma prova&quot; em [Compartilhar uma prova em [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatizado:** Selecione essa opção para gerenciar a revisão e a aprovação do conteúdo quando você tiver processos de revisão complexos ou se enviar o conteúdo para revisão para os mesmos grupos de pessoas regularmente. Com o fluxo de trabalho automatizado, a prova é movida de estágio para estágio até aprovação final. Os usuários relevantes são notificados sempre que forem solicitados a fazer uma aprovação.

      Para obter mais informações sobre como criar um Fluxo de Trabalho Automatizado, consulte [Configure uma prova com um Fluxo de trabalho automatizado no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Selecione se deseja enviar notificações por email e uma mensagem personalizada para os usuários selecionados na etapa anterior:

   * **Notificar destinatários sobre esta prova:** Selecione essa opção para enviar uma notificação por email aos usuários. When **[!UICONTROL Compartilhamento básico]** é selecionado no **[!UICONTROL Fluxo de trabalho]** , uma notificação por email é enviada quando a prova é criada. When **[!UICONTROL Fluxo de trabalho automatizado]** é selecionado no **[!UICONTROL Fluxo de trabalho]** , uma notificação por email é enviada quando a prova entra no estágio do fluxo de trabalho automatizado ao qual o usuário está associado.

   * **Adicionar mensagem personalizada:** Selecione essa opção para incluir uma mensagem personalizada na notificação. Você pode especificar um assunto e o corpo da mensagem. O corpo da mensagem pode incluir a formatação Rich Text, como negrito, marcadores e hiperlinks.

1. Selecione qualquer uma das seguintes configurações de prova:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exigir logon - a prova só pode ser compartilhada com outros usuários</td> 
      <td> <p><strong>Exigir logon - a prova só pode ser compartilhada com outros usuários:</strong> Quando esta opção é selecionada, somente [!DNL Workfront Proof] Os usuários do podem exibir a prova.</p> <p>Essa opção é desativada por padrão; qualquer pessoa com o URL pode exibir a prova.</p> <p>Quando esta opção é selecionada:</p> 
       <ul> 
        <li>Os usuários não podem fazer logon na prova, a menos que tenham sido adicionados à prova.</li> 
        <li>As assinaturas não podem ser ativadas.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Só é necessária uma decisão para esta prova</td> 
      <td> <p>Quando esta opção é selecionada, a revisão é concluída depois de um dos tomadores de decisão tomar a sua decisão.</p> <p>Essa opção é desativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente</td> 
      <td>Os usuários devem especificar seu nome de usuário e senha no momento em que tomarem uma decisão em uma prova.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear a prova quando todas as decisões necessárias forem tomadas</td> 
      <td> <p><strong></strong> Quando essa configuração estiver ativada, o estado da prova será bloqueado depois que todas as decisões forem tomadas. O estado é alterado automaticamente de desbloqueado para bloqueado quando o aprovador final decide.</p> <p>Essa opção é desativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Baixar arquivo original</td> 
      <td> <p><strong></strong> Quando essa opção é selecionada, os revisores podem baixar o arquivo original do qual a prova foi criada.</p> <p>Quando essa opção é desmarcada, o ícone Download não fica mais visível.<br>Essa opção é ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar prova por URL público ou código incorporado</td> 
      <td>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código incorporado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Assinar prova via URL público ou código incorporado</td> 
      <td> <p>Quando essa opção é selecionada, as pessoas que não foram adicionadas explicitamente à prova podem assinar a prova. A pessoa que assinar a prova recebe a função e o email definidos nas seguintes configurações:</p> 
       <ul> 
        <li><strong>Função de assinante</strong>: A função de prova padrão atribuída a todos os revisores que assinam a prova.</li> 
        <li><strong>Configurações de alerta de email para assinantes</strong>: O alerta por email padrão atribuído a todos os revisores que assinam a prova.</li> 
        <li> <p><strong>Prova de acesso via link de email necessária para</strong>: Configure se o assinante recebe um email com um link para a prova. Você pode selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação), ou <strong>Emails de notificação de validação e prova</strong> (O assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova; a finalidade dessa opção é garantir que a pessoa tenha digitado um endereço de email correto para o qual tenha acesso).</p> <p>Observação: Se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para o Proprietário da prova, para que possam decidir em qual estágio a pessoa deve ser adicionada.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar prova]**.

   O Workfront começa a gerar uma prova dos documentos ou sites selecionados. Dependendo do tamanho e do tipo do arquivo, o tempo de atraso em um upload de documento varia. Seja paciente, pois arquivos maiores demoram mais para serem gerados. Você pode sair da página e o Workfront continua a gerar seu arquivo. O tamanho máximo de upload de arquivo é de 4 GB.

   Depois que a prova for gerada, clique em **[!UICONTROL Ir para prova]** para iniciar a ferramenta de prova.

   ![Captura de tela_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   O documento aparece na ferramenta de prova.

   Os usuários que não tiverem a prova ativada em sua conta ainda poderão exibir o documento e fazer comentários na prova.

## Gerar uma prova para um URL {#generate-a-proof-for-a-url}

Você pode gerar uma prova para um URL pela primeira vez. Ou você pode gerar uma nova versão de uma prova de URL, onde uma prova foi gerada anteriormente.

>[!NOTE]
>
>Você pode gerar uma prova interativa para um URL somente se [!DNL Workfront] O ambiente é integrado a um [!DNL Workfront Proof] Conta Premium. Se não puder usar a prova, conforme discutido nesta seção, entre em contato com o administrador do sistema.

Para gerar uma prova para um URL:

1. Siga qualquer um destes procedimentos para começar a criar uma nova prova e exibir a variável [!UICONTROL Nova prova] página:

   * Clique na cor verde **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * No **[!UICONTROL Painel]** na **[!UICONTROL Visão geral]** clique no botão **[!UICONTROL Nova prova]** link .

   * Enviar via Dropzone (recurso Enterprise).

1. (Condicional) Na **[!UICONTROL Nova prova]** para criar uma nova versão de uma prova existente:

   1. Selecione a prova de URL à qual deseja adicionar uma nova versão.
   1. Clique no botão **[!UICONTROL Nova versão]** na parte superior da página.

      ![Captura de tela_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. Na página Nova versão de prova que é exibida, especifique o URL do site que deseja testar na **[!UICONTROL Adicionar arquivos]** e pressione **[!UICONTROL Enter]**.

1. (Opcional) Repita esse processo para adicionar vários sites à prova.

   ![proof_site.png](assets/proof-website-350x65.png)

1. Clique no site na lista de documentos na **[!UICONTROL Adicionar arquivos]** área.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Especifique um **[!UICONTROL Nome da prova]** para a prova.

   Por padrão, o nome da prova é igual ao URL do site.

1. Selecionar **[!UICONTROL Gerenciar o conteúdo do site]** opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Capturar captura de tela</td> 
      <td>Cria uma prova de uma imagem estática da página inicial do URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interativo</td> 
      <td> <p>Cria uma prova que permite aos revisores navegarem no site, exibirem imagens de HTML5, elementos de Flash e assim por diante.</p> <p>Para criar uma prova interativa, o site deve ser hospedado com um protocolo seguro (https). Além disso, os sites que não podem ser incorporados em um iframe não podem ser gerados como uma prova interativa (as restrições de incorporação do iframe são controladas pelo site que você está tentando incorporar).</p> <p>Depois que a prova inicial é criada, essa configuração não pode ser alterada ao criar versões subsequentes.</p> <p>Para obter mais informações sobre a prova interativa, consulte <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Gerar uma prova para conteúdo interativo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolução de captura de tela</td> 
      <td> <p>(Essa opção não está disponível para provas interativas.) Você pode ajustar a resolução em que seu conteúdo é exibido ou pode selecionar várias resoluções.</p> <p>Isso permite que os usuários revisem a prova para ver como o conteúdo será exibido em diferentes dispositivos, como vários tamanhos de telefones, tablets e monitores.</p> <p>Se você selecionar várias resoluções, uma prova separada será criada para cada resolução selecionada.</p> <p>Quando os usuários comentam na prova, a resolução de tela atual é exibida automaticamente no comentário para garantir que outros usuários estejam cientes de qual resolução o comentário está associado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procurar subpáginas</td> 
      <td>(Essa opção não está disponível para provas interativas.) Selecione essa opção para navegar pelas páginas do site. Você pode expandir o site até dois níveis a partir da página principal. Passe o mouse sobre uma página para visualizar o URL da página. Selecione somente as páginas que deseja testar. Cada página selecionada é criada como uma prova individual por padrão; ou ativar a <strong>Combinar em uma única prova</strong> para combinar todas as páginas selecionadas em uma única prova.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Configure quaisquer opções avançadas de prova, como compartilhar a prova, adicionar um Fluxo de trabalho automatizado ou configurar as configurações de acesso e de assinatura. Para obter mais detalhes sobre essas opções, consulte os seguintes artigos:

   * [Compartilhar uma prova em [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configure uma prova com um Fluxo de trabalho automatizado no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Definir configurações de acesso e assinatura para uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clique em **[!UICONTROL Concluído]**.

   Se você estiver adicionando uma nova versão a uma prova de URL existente, todas as opções que foram configuradas na prova original ou na versão anterior serão mantidas nessa versão. Se você estiver adicionando uma nova versão a uma prova de URL existente, todas as opções que foram configuradas na prova original ou na versão anterior serão mantidas nessa versão.

1. Clique em **[!UICONTROL Criar prova]**.

## Gerar uma prova para conteúdo interativo {#generate-a-proof-for-interactive-content}

É necessário um Pro Workfront Plan ou superior para usar esse recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos da Workfront](https://www.workfront.com/plans).

Para obter mais informações sobre conteúdo interativo, consulte [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Adicionar conteúdo interativo como URL](#add-interactive-content-as-a-url)
* [Adicionar conteúdo interativo como arquivo ZIP](#add-interactive-content-as-a-zip-file)

### Adicionar conteúdo interativo como URL {#add-interactive-content-as-a-url}

Para obter informações sobre como adicionar uma prova de URL interativa, consulte  [Gerar uma prova para um URL](#generate-a-proof-for-a-url).

### Adicionar conteúdo interativo como arquivo ZIP {#add-interactive-content-as-a-zip-file}

1. Prepare seu conteúdo criando um arquivo .zip empacotado.

   Para obter informações sobre as especificações do arquivo compactado .zip, consulte [Sobre a preparação de conteúdo interativo em um arquivo ZIP para prova](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) no artigo [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Siga qualquer um destes procedimentos para começar a criar uma nova prova e exibir a variável [!UICONTROL Nova prova] página:

   * Clique na cor verde **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * No **[!UICONTROL Painel]** na **[!UICONTROL Visão geral]** clique no botão **[!UICONTROL Nova prova]** link .

   * Enviar via Dropzone (recurso Enterprise).

1. No **[!UICONTROL Nova prova]** página exibida, arraste e solte o pacote .zip interativo no **[!UICONTROL Adicionar arquivos]** área.

1. (Opcional) Configure quaisquer opções avançadas de prova, como compartilhar a prova, adicionar um fluxo de trabalho automatizado ou configurar as configurações de acesso e assinatura. Para obter mais detalhes sobre essas opções, consulte os seguintes artigos:

   * [Compartilhar uma prova em [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * no artigo
   * [Definir configurações de acesso e assinatura para uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clique em **[!UICONTROL Criar prova]**.

   A Workfront começa a gerar uma prova do pacote .zip. Dependendo do tamanho do pacote, o tempo de atraso em um upload de documento varia. Arquivos maiores levam mais tempo para serem gerados. Você pode sair da página e o Workfront continua a gerar seu arquivo. O tamanho máximo de upload de arquivo é de 4 GB.

   Depois que a prova for gerada, você poderá clicar no botão **[!UICONTROL Ir para prova]** que aparece para abrir a prova.
