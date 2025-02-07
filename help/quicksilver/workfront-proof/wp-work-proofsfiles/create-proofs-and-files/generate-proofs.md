---
product-previous: workfront-proof
product-area: documents
navigation-topic: create-proofs-and-files
title: Gerar provas em  [!DNL Workfront Proof]
description: O Workfront Proof permite criar provas a partir de documentos ou sites e compartilhá-las com outras pessoas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 49657851-2948-4d3b-b2ce-c8359eeb315b
source-git-commit: ddaee5b339982c826c14b67775d81f3a2bd7bc37
workflow-type: tm+mt
source-wordcount: '2259'
ht-degree: 0%

---

# Gerar provas em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

O [!DNL Workfront Proof] permite que você crie provas a partir de documentos ou sites e compartilhe essas provas com outras pessoas. As etapas a seguir descrevem as várias opções de configuração disponíveis:

## Gerar uma prova para um documento

1. Siga qualquer um destes procedimentos para começar a criar uma nova prova e exibir a página [!UICONTROL Nova prova]:

   * Clique no botão verde **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * Na área **[!UICONTROL Painel]**, na guia **[!UICONTROL Visão geral]**, clique no link **[!UICONTROL Nova prova]**.

   * Enviar via Dropzone (recurso Enterprise).
   * A página **[!UICONTROL Nova prova]** é exibida.

1. Para revisar um ou mais documentos, adicione os documentos a serem revisados de uma das seguintes maneiras (repita esse processo para adicionar vários documentos a serem revisados):

   * Arraste um documento do seu sistema de arquivos para a área de arrastar e soltar na área **[!UICONTROL Adicionar arquivos]**.
   * Clique na área de arrastar e soltar na área **[!UICONTROL Adicionar arquivos]** e procure e selecione o documento que deseja carregar do sistema de arquivos da sua estação de trabalho.

     ![prova_documento_upload.png](assets/proof-document-upload-350x64.png)

1. Para revisar um ou mais sites, especifique a URL do site que deseja revisar na área **[!UICONTROL Adicionar Arquivos]** e pressione **[!UICONTROL Enter]**.

1. (Opcional) Repita esse processo para adicionar vários sites à prova.

   Para obter mais detalhes sobre sites de comprovação, consulte [Gerar uma prova para uma URL](#generate-a-proof-for-a-url).

   ![Site de prova](assets/proof-website-350x65.png)

1. (Opcional) Modifique os nomes dos arquivos carregados:

   1. Passe o mouse sobre o nome do documento que você deseja modificar na lista de documentos da área **[!UICONTROL Adicionar arquivos]** e clique no ícone **[!UICONTROL Editar]**.

      ![proof_edit.png](assets/proof-edit-350x53.png)

   1. No campo **[!UICONTROL Nome da prova]**, especifique um novo nome e clique em **[!UICONTROL Concluído]**.

   1. (Opcional) Para impedir que qualquer arquivo seja carregado, passe com o mouse sobre o documento que deseja excluir na lista de documentos na área **[!UICONTROL Adicionar arquivos]** e clique no ícone **[!UICONTROL Excluir]**.

      ![prova_exclusão.png](assets/proof-delete-350x53.png)

   1. (Opcional) Habilite a opção **[!UICONTROL Combinar todos os arquivos compatíveis em uma única prova]**.

      **Quando esta opção está habilitada:** todos os arquivos e sites estáticos estão disponíveis em uma única prova, e você pode carregar até 50 arquivos em um determinado momento.

      >[!NOTE]
      >
      >Arquivos interativos, incluindo vídeos e sites interativos, não podem ser combinados em uma única prova.

      **Quando esta opção está desabilitada:** todos os documentos e sites são gerados como provas individuais e você pode carregar até 20 arquivos em um determinado momento.

      Para combinar todos os arquivos e sites carregados em uma única prova:

      1. Habilite a opção **[!UICONTROL Combinar todos os arquivos compatíveis em uma única prova]**.
      1. No campo **[!UICONTROL Nome da prova]**, especifique um novo nome para a prova combinada.
      1. Na área **[!UICONTROL Adicionar arquivos]**, reordene os arquivos incluídos arrastando um arquivo para a ordem desejada. A ordem dos arquivos é a ordem de página da prova combinada. Para obter mais informações sobre como criar provas combinadas, consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

1. (Opcional) Se quiser usar um fluxo de trabalho automatizado que inclua vários estágios, na seção **[!UICONTROL Fluxo de trabalho]**, selecione uma das seguintes opções:

   * **Básico:** selecione essa opção para designar usuários aos quais você deseja ter acesso à prova imediatamente após sua criação. Você pode compartilhar a prova com vários usuários.

     Para obter mais informações sobre como compartilhar uma prova, consulte &quot;Adicionando usuários a uma prova&quot; em [Compartilhar uma prova no [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).

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
      <td role="rowheader">Exigir logon - a prova só pode ser compartilhada com outros usuários</td> 
      <td> <p><strong>Exigir logon - a prova só pode ser compartilhada com outros usuários:</strong> Quando esta opção é selecionada, somente [!DNL Workfront Proof] usuários podem exibir a prova.</p> <p>Essa opção está desativada por padrão; qualquer pessoa com o URL pode exibir a prova.</p> <p>Quando esta opção é selecionada:</p> 
       <ul> 
        <li>Os usuários não podem fazer logon na prova a menos que tenham sido adicionados à prova.</li> 
        <li>Não é possível habilitar assinaturas.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">É necessária somente uma decisão para essa prova</td> 
      <td> <p>Quando essa opção é selecionada, a revisão é concluída após um dos tomadores de decisão tomar sua decisão.</p> <p>Essa opção está desabilitada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente</td> 
      <td>Os usuários são solicitados a especificar seu nome de usuário e senha no momento em que tomam uma decisão sobre uma prova.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear prova quando todas as decisões necessárias forem tomadas</td> 
      <td> <p><strong></strong> Quando essa configuração estiver ativada, o estado da prova será bloqueado depois que todas as decisões forem tomadas. O estado é alterado automaticamente de desbloqueado para bloqueado quando o aprovador final toma sua decisão.</p> <p>Essa opção está desabilitada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Baixar arquivo original</td> 
      <td> <p><strong></strong> Quando essa opção é selecionada, os revisores podem baixar o arquivo original do qual a prova foi criada.</p> <p>Quando essa opção é desmarcada, o ícone Download não fica mais visível.<br>Esta opção está habilitada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Compartilhar prova por meio de um URL público ou código integrado</td> 
      <td>Quando essa opção é selecionada, a prova pode ser compartilhada por meio de um URL público ou código integrado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inscrever-se para obter prova por meio de um URL público ou código de inserção</td> 
      <td> <p>Quando essa opção é selecionada, as pessoas que não foram adicionadas explicitamente à prova podem assinar a prova. A pessoa que se inscreve na prova recebe a função e o email definidos nas seguintes configurações:</p> 
       <ul> 
        <li><strong>Função do assinante</strong>: a função de prova padrão que é atribuída a todos os revisores que assinam a prova.</li> 
        <li><strong>Configurações de alerta por email para assinantes</strong>: o alerta por email padrão atribuído a todos os revisores que assinam a prova.</li> 
        <li> <p><strong>Acesso de prova via link de email necessário para</strong>: configure se o assinante recebe um email com um link para a prova. Você pode selecionar <strong>Nenhum email</strong> (o link do email não é necessário para acessar a prova), <strong>Somente email de notificação de prova</strong> (o assinante recebe um link para a prova por email sem qualquer verificação) ou <strong>Emails de notificação de validação e prova</strong> (o assinante recebe um link para a prova por email e deve clicar no link para acessar uma prova; o objetivo dessa opção é garantir que a pessoa tenha inserido um endereço de email correto ao qual tem acesso).</p> <p>Observação: se as provas tiverem o Fluxo de trabalho automatizado anexado, todas as assinaturas gerarão emails de confirmação para o Proprietário da prova, para que ele possa decidir em qual estágio a pessoa deve ser adicionada.</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **[!UICONTROL Criar prova]**.

   O Workfront começa a gerar uma prova dos documentos ou sites selecionados. Dependendo do tamanho e do tipo do arquivo, o tempo de atraso no upload de um documento varia. Seja paciente, pois arquivos maiores demoram mais para serem gerados. Você pode sair da página e o Workfront continua a gerar seu arquivo. O tamanho máximo do upload de arquivo é 4 GB.

   Depois que a prova for gerada, clique em **[!UICONTROL Ir para prova]** para iniciar a ferramenta de prova.

   ![Captura_de_tela_2018-05-16_08-59-34.png](assets/screenshot-2018-05-16-08-59-34-350x134.png)

   O documento é exibido na ferramenta de prova.

   Os usuários que não têm a prova ativada em suas contas ainda podem exibir o documento e fazer comentários na prova.

## Gerar uma prova para um URL {#generate-a-proof-for-a-url}

Você pode gerar uma prova para um URL pela primeira vez. Ou você pode gerar uma nova versão de uma prova de URL em que uma prova foi gerada anteriormente.

>[!NOTE]
>
>Você só poderá gerar uma prova interativa para uma URL se o ambiente do [!DNL Workfront] estiver integrado a uma conta do [!DNL Workfront Proof] Premium. Se você não puder usar provas como discutido nesta seção, entre em contato com o administrador do sistema.

Para gerar uma prova para um URL:

1. Siga qualquer um destes procedimentos para começar a criar uma nova prova e exibir a página [!UICONTROL Nova prova]:

   * Clique no botão verde **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * Na área **[!UICONTROL Painel]**, na guia **[!UICONTROL Visão geral]**, clique no link **[!UICONTROL Nova prova]**.

   * Enviar via Dropzone (recurso Enterprise).

1. (Condicional) Na página **[!UICONTROL Nova prova]** exibida, para criar uma nova versão de uma prova existente:

   1. Selecione a prova de URL em que deseja adicionar uma nova versão.
   1. Clique no botão **[!UICONTROL Nova versão]** na parte superior da página.

      ![Captura_de_tela_2018-05-15_10-59-56.png](assets/screenshot-2018-05-15-10-59-56-350x80.png)

1. Na página Nova versão de prova que é exibida, especifique a URL do site que deseja revisar na área **[!UICONTROL Adicionar arquivos]** e pressione **[!UICONTROL Enter]**.

1. (Opcional) Repita esse processo para adicionar vários sites à prova.

   ![proof_website.png](assets/proof-website-350x65.png)

1. Clique no site na lista de documentos na área **[!UICONTROL Adicionar arquivos]**.

   ![proof_upload_website_modify.png](assets/proof-upload-website-modify-350x185.png)

1. Especifique um **[!UICONTROL Nome da prova]** para a prova.

   Por padrão, o nome da prova é igual ao URL do site.

1. Selecione as opções **[!UICONTROL Lidar com o conteúdo do site]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Capturar captura de tela</td> 
      <td>Cria uma prova de uma imagem estática da página frontal do URL.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Interativo</td> 
      <td> <p>Cria uma prova que permite aos revisores navegar no site, visualizar imagens HTML5, elementos de Flash e assim por diante.</p> <p>Para criar uma prova interativa, o site deve ser hospedado com um protocolo seguro (https). Além disso, os sites que não podem ser incorporados a um iframe não podem ser gerados como uma prova interativa (as restrições de incorporação do iframe são controladas pelo site que você está tentando incorporar).</p> <p>Depois que a prova inicial é criada, essa configuração não pode ser alterada ao criar versões subsequentes.</p> <p>Para obter mais informações sobre provas interativas, consulte <a href="#generate-a-proof-for-interactive-content" class="MCXref xref">Gerar uma prova para conteúdo interativo</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Resolução da captura de tela</td> 
      <td> <p>(Essa opção não está disponível para provas interativas.) É possível ajustar a resolução em que o conteúdo é exibido ou selecionar várias resoluções.</p> <p>Isso permite que os usuários revisem a prova para ver como o conteúdo será exibido em diferentes dispositivos, como telefones, tablets e monitores de vários tamanhos.</p> <p>Se você selecionar várias resoluções, uma prova separada será criada para cada resolução selecionada.</p> <p>Quando os usuários comentam a prova, a resolução de tela atual é exibida automaticamente no comentário para garantir que outros usuários estejam cientes da resolução à qual o comentário está associado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Procurar subpáginas</td> 
      <td>(Essa opção não está disponível para provas interativas.) Selecione esta opção para navegar pelas páginas do site. Você pode expandir o site até dois níveis a partir da página principal. Passe o mouse sobre uma página para visualizar o URL da página. Selecione somente as páginas que deseja revisar. Cada página selecionada é criada como uma prova individual por padrão; ou habilite a opção <strong>Combinar em uma única prova</strong> para combinar todas as páginas selecionadas em uma única prova.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Configure as opções de prova avançada, como compartilhar a prova, adicionar um Fluxo de trabalho automatizado ou definir as configurações de acesso e subscrição. Para obter mais detalhes sobre essas opções, consulte os seguintes artigos:

   * [Compartilhar uma prova no  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * [Configurar uma prova com um Fluxo de Trabalho Automatizado no  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/automated-workflow/set-up-proof-auto-workflow.md)
   * [Definir configurações de acesso e subscrição para uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clique em **[!UICONTROL Concluído]**.

   Se você estiver adicionando uma nova versão a uma prova de URL existente, todas as opções configuradas na prova original ou na versão anterior serão mantidas nesta versão. Se você estiver adicionando uma nova versão a uma prova de URL existente, todas as opções configuradas na prova original ou na versão anterior serão mantidas nesta versão.

1. Clique em **[!UICONTROL Criar prova]**.

## Gerar uma prova para conteúdo interativo {#generate-a-proof-for-interactive-content}

É necessário um Plano Pro Workfront ou superior para usar este recurso. Para obter mais informações sobre os vários planos disponíveis, consulte [Planos do Workfront](https://www.workfront.com/plans).

Para obter mais informações sobre Conteúdo interativo, consulte [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

* [Adicionar conteúdo interativo como um URL](#add-interactive-content-as-a-url)
* [Adicionar conteúdo interativo como um arquivo ZIP](#add-interactive-content-as-a-zip-file)

### Adicionar conteúdo interativo como um URL {#add-interactive-content-as-a-url}

Para obter informações sobre como adicionar uma prova de URL interativa, consulte [Gerar uma prova para uma URL](#generate-a-proof-for-a-url).

### Adicionar conteúdo interativo como um arquivo ZIP {#add-interactive-content-as-a-zip-file}

1. Prepare o conteúdo criando um arquivo .zip agrupado.

   Para obter informações sobre especificações de arquivos .zip agrupados, consulte [Sobre a preparação de conteúdo interativo em um arquivo ZIP para revisão](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md#howtoprepareaninteractiveziparchive) no artigo [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

1. Siga qualquer um destes procedimentos para começar a criar uma nova prova e exibir a página [!UICONTROL Nova prova]:

   * Clique no botão verde **[!UICONTROL Nova prova]** no canto superior esquerdo de qualquer página.
   * Na área **[!UICONTROL Painel]**, na guia **[!UICONTROL Visão geral]**, clique no link **[!UICONTROL Nova prova]**.

   * Enviar via Dropzone (recurso Enterprise).

1. Na página **[!UICONTROL Nova prova]** exibida, arraste e solte seu pacote .zip interativo na área **[!UICONTROL Adicionar arquivos]**.

1. (Opcional) Configure todas as opções de prova avançada, como compartilhar a prova, adicionar um fluxo de trabalho automatizado ou definir as configurações de acesso e subscrição. Para obter mais detalhes sobre essas opções, consulte os seguintes artigos:

   * [Compartilhar uma prova no  [!DNL Adobe Workfront]](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)
   * no artigo
   * [Definir configurações de acesso e subscrição para uma prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/configure-access-subscription-settings-proof.md)

1. Clique em **[!UICONTROL Criar prova]**.

   O Workfront começa a gerar uma prova do pacote .zip. Dependendo do tamanho do pacote, o tempo de atraso no upload de um documento varia. Arquivos maiores demoram mais para serem gerados. Você pode sair da página e o Workfront continua a gerar seu arquivo. O tamanho máximo do upload de arquivo é 4 GB.

   Depois que a prova for gerada, você pode clicar no botão **[!UICONTROL Ir para prova]** que aparece para abrir a prova.
