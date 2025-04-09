---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Gerar provas em  [!DNL Workfront Proof]
description: O Workfront Proof permite criar provas a partir de documentos ou sites e compartilhá-las com outras pessoas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: 1443551b605dac6e53531c5d445b89517384fe11
workflow-type: tm+mt
source-wordcount: '1889'
ht-degree: 2%

---

# Gerar provas em [!DNL Workfront Proof]

<!-- Audited: 4/2025 -->

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

O [!DNL Workfront Proof] permite que você crie provas a partir de documentos ou sites e compartilhe essas provas com outras pessoas. As etapas a seguir descrevem as várias opções de configuração disponíveis:

## Gerar uma prova a partir de um documento

1. Siga um destes procedimentos para abrir a página **[!UICONTROL Nova prova]**:

   * Clique no botão **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * Enviar via Dropzone (recurso Enterprise).

1. Para revisar um ou mais documentos, adicione os documentos a serem revisados de uma das seguintes maneiras (repita esse processo para adicionar vários documentos):

   * Arraste um documento do seu sistema de arquivos para a área de arrastar e soltar na área **[!UICONTROL Adicionar arquivos]**.
   * Na área **[!UICONTROL Adicionar Arquivos]**, clique no link **procurar** para localizar e selecionar o documento que deseja carregar do sistema de arquivos da sua estação de trabalho.

     ![prova_documento_upload.png](assets/proof-document-upload-350x64.png)

1. Para revisar um site, digite a URL na área **[!UICONTROL Adicionar arquivos]** e pressione **[!UICONTROL Enter]**. Repita esta etapa para adicionar vários sites à prova.

   Para obter mais detalhes sobre sites de comprovação, consulte [Gerar uma prova para uma URL](#generate-a-proof-for-a-url).

   ![Site de prova](assets/proof-website-350x65.png)

1. (Opcional) Modifique os nomes dos arquivos carregados:

   1. Na lista de documentos, passe o mouse sobre o nome do documento que você deseja modificar e clique no ícone **[!UICONTROL Editar]**.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. No campo **[!UICONTROL Nome da prova]**, especifique um novo nome e clique em **[!UICONTROL Concluído]**.

   1. (Opcional) Para excluir qualquer arquivo do upload, passe o mouse sobre a documento que deseja excluir na documento lista e clique no ícone Excluir ****.

      ![prova_delete.png](assets/proof-delete-350x53.png)

   1. (Opcional) Habilite a opção **[!UICONTROL Combinar todos os arquivos compatíveis em uma única prova]**.

      **Quando esta opção está habilitada:** todos os arquivos e sites estáticos estão disponíveis em uma única prova, e você pode carregar até 50 arquivos em um determinado momento.

      >[!NOTE]
      >
      >Arquivos interativos, incluindo vídeos e sites interativos, não podem ser combinados em uma única prova.

      **Quando essa opção é desativada:** todas as documentos e sites são gerados como provas individuais e você pode upload até 20 arquivos em um determinado momento.

      Para combinar todos os arquivos e sites carregados em uma única prova:

      1. Ative a opção **[!UICONTROL Combinar todos os arquivos compatíveis em uma única opção de prova]** .
      1. No campo Nome ]**da**[!UICONTROL  prova, insira um novo nome para o prova combinado.
      1. **[!UICONTROL Na área Adicionar arquivos]**, reordene os arquivos incluídos arrastando um arquivo para a solicitar desejada. A solicitar dos arquivos é a página solicitar do prova combinado. Para obter mais informações sobre como criar provas combinadas, consulte [Criar um prova multi-página](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Opcional) Se quiser usar um fluxo de trabalho automatizado que inclua vários estágios, selecione uma das seguintes opções na seção **[!UICONTROL Fluxo de trabalho]**:

   * **Básico:** selecione essa opção para designar usuários aos quais você deseja ter acesso à prova imediatamente após sua criação. Você pode compartilhar a prova com vários usuários.

     Para obter mais informações sobre como compartilhar uma prova, consulte [Compartilhar uma prova no [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

   * **Automatizado:** selecione essa opção para gerenciar a revisão e a aprovação do conteúdo quando tiver processos de revisão complexos ou se enviar conteúdo para revisão aos mesmos grupos de pessoas regularmente. Com um fluxo de trabalho automatizado, a prova é transferida de estágio para estágio até a aprovação final. Os usuários relevantes são notificados a qualquer momento de que precisam fazer uma aprovação.

     Para obter mais informações sobre como criar um Fluxo de Trabalho Automatizado, consulte [Configurar uma prova com um Fluxo de Trabalho Automatizado em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md#create2).

1. Selecione se deseja enviar notificações por email e uma mensagem personalizada para os usuários selecionados na etapa anterior:

   * **Notificar recipients sobre esta prova:** Selecione esta opção para enviar uma notificação por email aos usuários. Quando o **[!UICONTROL Compartilhamento básico]** é selecionado na seção **[!UICONTROL Fluxo de trabalho]**, uma notificação é enviada por email quando a prova é criada. Quando o **[!UICONTROL Fluxo de trabalho automatizado]** é selecionado na seção **[!UICONTROL Fluxo de trabalho]**, uma notificação por email é enviada quando a prova entra no estágio do fluxo de trabalho automatizado ao qual o usuário está associado.

   * **Adicionar mensagem personalizada:** Selecione esta opção para incluir uma mensagem personalizada na notificação. Você pode especificar um assunto e um corpo de mensagem. O corpo da mensagem pode incluir formatação de rich text, como negrito, marcadores e hiperlinks.

1. Selecione qualquer uma das seguintes configurações de prova:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exigir logon. Esta prova não pode ser compartilhada com outros usuários</td> 
      <td> <p>Quando esta opção é selecionada:</p> 
       <ul> 
        <li>Os usuários não podem fazer logon na prova para visualizá-la, a menos que tenham sido adicionados a ela.</li> 
        <li>Não é possível habilitar assinaturas.</li> 
       </ul> 
       <p>Essa opção está desabilitada por padrão.</p> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente</td> 
      <td><p>Quando essa opção é selecionada, os usuários precisam especificar seu nome de usuário e senha no momento em que tomam uma decisão sobre uma prova.</p>
      <p>Essa opção está desabilitada por padrão.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prova quando todas as decisões necessárias forem tomadas</td> 
      <td> <p>Quando essa configuração estiver ativada, o estado da prova será bloqueado depois que todas as decisões forem tomadas. O estado é alterado automaticamente de desbloqueado para bloqueado quando o aprovador final toma sua decisão.</p> 
      <p>Essa opção está desabilitada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir o download do arquivo original</td> 
      <td> <p><strong></strong> Quando essa opção é selecionada, os revisores podem baixar o arquivo original do qual a prova foi criada.</p> <p>Quando essa opção é desmarcada, o ícone Download não fica mais visível.</p>
      <p>Essa opção está ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir o compartilhamento da prova por meio de URL público ou código de inserção</td> 
      <td><p>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código integrado.</p>
       <p>Essa opção está ativada por padrão.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir assinatura da prova por meio de um URL público ou código de inserção</td> 
      <td> <p>Quando essa opção é selecionada, as pessoas que não foram adicionadas à prova podem assinar a prova. A pessoa que se inscreve na prova recebe a função e o email definidos nas seguintes configurações:</p> 
       <ul> 
        <li><strong>Função do assinante</strong>: a função de prova padrão que é atribuída a todos os revisores que assinam a prova.</li> 
        <li><strong>Configurações de alerta por email para assinantes</strong>: o alerta por email padrão atribuído a todos os revisores que assinam a prova.</li> 
        <li> <p><strong>Acesso de prova via link de email necessário para</strong>: configure se o assinante recebe um email com um link para a prova. Você pode selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova. O objetivo dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</p> <p>Observação: se as provas tiverem um Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para o Proprietário da prova, para que ele possa decidir em qual estágio a pessoa deve ser adicionada.</p> </li> 
       </ul> 
        <p>Essa opção está desabilitada por padrão.</p>
       </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar prova]**. O Workfront gera uma prova dos documentos ou sites selecionados.

   O tempo de atraso no upload de um documento varia de acordo com o tamanho e o tipo do arquivo. Arquivos maiores levarão mais tempo para serem gerados. Você pode sair da página enquanto o Workfront continua a gerar o arquivo. O tamanho máximo do upload de arquivo é 4 GB.

## Gerar uma prova estática com um URL {#generate-a-proof-for-a-url}

Você pode gerar uma prova estática usando o URL de um site.

>[!NOTE]
>
>Você só poderá gerar uma prova interativa para uma URL se o ambiente do [!DNL Workfront] estiver integrado a uma conta do [!DNL Workfront Proof] Premium. Se você não puder usar provas conforme discutido nesta seção, entre em contato com o administrador do Workfront.

1. Siga um destes procedimentos para abrir a página **[!UICONTROL Nova prova]**:

   * Clique no botão **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * Enviar via Dropzone (recurso Enterprise).

1. **Na Novo prova** página, insira a URL do site a partir da qual você deseja criar uma prova na **[!UICONTROL área Adicionar arquivos]** e pressione **[!UICONTROL Enter]** ou **[!UICONTROL Return]** no teclado.

1. (Opcional) Repita esse processo para adicionar vários sites à prova.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Na área **[!UICONTROL Adicionar arquivos]**, clique no ícone **Editar** à direita da URL para abrir os detalhes de prova do site.

   ![prova_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Insira um nome ]**de**[!UICONTROL  prova. Por padrão, o nome da prova é o mesmo que o URL do site.

1. Selecione qualquer uma das seguintes **[!UICONTROL opções de Manipulação de conteúdo do]** site:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">captura de tela de Capture</td> 
      <td>Cria uma prova de uma imagem estática da página frontal do URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interativo</td> 
      <td> <p>Cria uma prova que permite que os revisores naveguem pelo site, visualizem imagens HTML5, elementos Flash e assim por diante.</p> <p>Para criar uma prova interativa, o site deve ser hospedado com um protocolo seguro (https). Além disso, os sites que não podem ser incorporados em um iframe não podem ser gerados como uma prova interativa (as restrições de incorporação do iframe são controladas pelo site que você está tentando incorporar).</p> <p>Depois que a prova inicial é criada, essa configuração não pode ser alterada ao criar versões subsequentes.</p> <p>Para obter mais informações sobre provas interativas, consulte <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Gerar uma prova para conteúdo interativo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolução da captura de tela</td> 
      <td> <p>(Essa opção não está disponível para provas interativas.) É possível ajustar a resolução em que o conteúdo é exibido ou selecionar várias resoluções.</p> <p>Isso permite que os usuários revisem a prova para ver como o conteúdo será exibido em diferentes dispositivos, como telefones, tablets e monitores de vários tamanhos.</p> <p>Se você selecionar várias resoluções, uma prova separada será criada para cada resolução selecionada.</p> <p>Quando os usuários comentam a prova, a resolução de tela atual é exibida automaticamente no comentário para garantir que outros usuários estejam cientes da resolução à qual o comentário está associado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procurar subpáginas</td> 
      <td>(Esta opção não está disponível para provas interativas.) Selecione essa opção para navegar pelas páginas do site. Você pode expandir o site em até 2 níveis a partir das página principais. Passe o mouse sobre uma página para visualização a URL do página e selecione apenas as páginas que deseja prova. Cada página que você selecionar é criada como uma prova individual por padrão. Como alternativa, você pode ativar o <strong>Combine todos os arquivos compatíveis em uma única opção de prova</strong> .</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Configure quaisquer opções de prova avançadas, como compartilhar a prova, adicionar um fluxo de trabalho automatizado ou configurar configurações de acesso e assinatura. Para obter mais detalhes sobre essas opções, consulte os seguintes artigos:

   * [Compartilhe um prova no [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurar uma prova com um Fluxo de Trabalho Automatizado no  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Definir configurações de acesso e subscrição para uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clique em **[!UICONTROL Concluído]**.

1. Clique em **[!UICONTROL Criar prova]**.

## Gerar uma prova para conteúdo interativo {#generate-a-proof-for-interactive-content}

<!--A Pro Workfront Plan or higher is required to use this feature. For more information about the various plans available, see [Workfront Plans](https://www.workfront.com/plans).-->

Para obter mais informações sobre Conteúdo interativo, consulte [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Adicionar conteúdo interativo como um URL](#add-interactive-content-as-a-url)
* [Adicionar conteúdo interativo como um arquivo ZIP](#add-interactive-content-as-a-zip-file)

### Adicionar conteúdo interativo como um URL {#add-interactive-content-as-a-url}

Para obter informações sobre como adicionar uma prova de URL interativa, consulte [Gerar uma prova para uma URL](#generate-a-proof-for-a-url).

### Adicionar conteúdo interativo como um arquivo ZIP {#add-interactive-content-as-a-zip-file}

1. Prepare o conteúdo criando um arquivo .zip agrupado.

   Para obter informações sobre especificações de arquivos .zip agrupados, consulte [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Siga um destes procedimentos para abrir a página **[!UICONTROL Nova prova]**:

   * Clique no botão **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * Enviar via Dropzone (recurso Enterprise).

1. Na página **[!UICONTROL Nova prova]**, arraste e solte seu pacote .zip interativo na área **[!UICONTROL Adicionar arquivos]**.

1. (Opcional) Configure todas as opções de prova avançada, como compartilhar a prova, adicionar um fluxo de trabalho automatizado ou definir as configurações de acesso e subscrição. Para obter mais detalhes sobre essas opções, consulte os seguintes artigos:

   * [Compartilhar uma prova no  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Definir configurações de acesso e subscrição para uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clique em **[!UICONTROL Criar prova]**. O Workfront gera uma prova do arquivo zip.

   O tempo de atraso no upload de um documento varia dependendo do tamanho do arquivo zip. Você pode sair da página enquanto o Workfront continua a gerar o arquivo. O tamanho máximo do upload de arquivo é 4 GB.
