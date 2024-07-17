---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: 'Perguntas frequentes: criar e compartilhar provas e arquivos'
description: Uma prova é um arquivo estático, de áudio ou vídeo que está disponível para revisão no visualizador de provas. Os revisores adicionados a uma prova têm um conjunto de ferramentas disponíveis para fazer comentários e tomar decisões sobre a prova.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '1369'
ht-degree: 1%

---

# Perguntas frequentes: criar e compartilhar provas e arquivos

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

## O que é uma prova?

### Responder

Uma prova é um arquivo estático, de áudio ou vídeo que está disponível para revisão no visualizador de provas. Os revisores adicionados a uma prova têm um conjunto de ferramentas disponíveis para fazer comentários e tomar decisões sobre a prova.

## Que tipos de arquivos são aceitos?

### Responder

É possível criar provas de arquivos estáticos, de áudio e de vídeo. Não é possível carregar arquivos com mais de 4 GB. [!DNL Workfront] oferece suporte a mais de 150 tipos de arquivos (consulte a [Visão geral de tipos de arquivos de comprovação e limites de tamanho com suporte](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) para obter uma lista completa).

## Qual é a diferença entre uma prova e um arquivo?

### Responder

Ao carregar um arquivo para [!DNL Workfront Proof], o sistema armazena o arquivo na sua conta [!DNL Workfront Proof]. Quando você o compartilha, [!DNL Workfront Proof] envia por email aos seus destinatários um link no qual eles podem clicar para baixar o arquivo. Você pode compartilhar qualquer tipo de arquivo desejado.

Ao criar uma prova a partir de um arquivo que você carregou para [!DNL Workfront Proof], você pode tornar o arquivo disponível para revisão no visualizador de provas. Os revisores recebem um email com um link para a prova. Ao abrir a prova, ele vê a imagem da prova e pode adicionar comentários e tomar decisões sobre ela. Você pode criar provas usando arquivos da lista de tipos de arquivos compatíveis. Você também pode criar provas usando URLs para sites e outro conteúdo da Web.

Para obter uma lista completa de tipos de arquivos com suporte, consulte [Visão geral de tipos de arquivos com suporte e limites de tamanho](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## Como criar uma prova?

### Responder

Você pode criar provas a partir de arquivos estáticos, arquivos de áudio, arquivos de vídeo e URLs (consulte ).

Para criar uma prova na conta, você precisa ser um usuário com o perfil de permissão correto (consulte [[!UICONTROL Perfis de Permissões de Prova] em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Se você fizer upload de vários arquivos ao mesmo tempo, criará várias provas que poderá enviar para o mesmo grupo de revisores usando um email. Se sua organização tiver uma conta da [!UICONTROL Empresa] ou [!UICONTROL Ilimitada], você poderá combinar arquivos em uma única prova (consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)).

## Quais são as funções de prova e os alertas de email?

### Responder

As funções de prova definem quais ações um revisor precisa realizar em uma prova. Há diferentes opções de função que podem ser usadas para revisores ao criar uma prova, dependendo se você deseja que eles possam fazer comentários, tomar decisões etc. Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

Os alertas de email atualizam os revisores sobre o progresso de uma prova (eles são diferentes das notificações de nova prova e prova atrasada). É possível selecionar opções diferentes para revisores diferentes, dependendo da função de cada revisor na prova. Para obter mais informações, consulte [Criar uma prova avançada com um [!UICONTROL Fluxo de trabalho automatizado]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Posso criar uma prova a partir de vários arquivos?

### Responder

Combinar vários arquivos em uma única prova é um recurso disponível nos planos de edição [!UICONTROL Empresa] e [!UICONTROL Ilimitado]. Essa opção é possível somente para arquivos estáticos, não para arquivos de vídeo. Para obter mais informações, consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Posso criar provas com base em URLs?

### Responder

Sim, você pode criar provas de sites e outros conteúdos da Web. Ao adicionar um URL para criar uma prova, você pode especificar se deseja uma prova estática ou uma prova interativa:

* Em uma prova interativa, os revisores podem navegar e interagir normalmente com o site ou outro conteúdo da Web, como anúncios com vídeo ou áudio em fluxo contínuo, elementos [!DNL Flash] em um anúncio, animações HTML e banners interativos. Para obter mais informações, consulte [Criar uma prova para conteúdo interativo em um arquivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).
* Para uma prova estática, o [!DNL Workfront] captura um conjunto de capturas de tela das páginas e subpáginas que você especificar. Os hiperlinks estão ativos na prova, para que você possa testar se eles levam ou não ao destino correto. Para obter mais informações, consulte [Criar uma prova estática para um site ou outro conteúdo da Web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

Você pode adicionar vários URLs de uma só vez se separá-los com um espaço. Observe que a combinação só está disponível nos planos de edição [!UICONTROL Empresa] e [!UICONTROL Ilimitado].

## As pessoas que não possuem um login podem criar provas em minha conta?

### Responder

Você precisa de credenciais de logon para criar provas diretamente em uma conta do [!DNL Workfront Proof].

## O que significa compartilhar uma prova?

### Responder

Compartilhar uma prova dá aos revisores acesso a ela para que possam adicionar comentários e marcações e tomar decisões sobre ela. Os revisores convidados acessam as provas a partir da notificação por email que recebem. Revisores com sua própria conta [!DNL Workfront Proof] podem acessar provas no [!UICONTROL Painel].

## Como faço para compartilhar uma prova?

### Responder

Ao criar uma prova, você pode adicionar revisores na seção [!UICONTROL Fluxo de trabalho] da página [!UICONTROL Nova prova]. Quando a prova estiver pronta, [!DNL Workfront Proof] envia um email aos revisores contendo um link para a prova.

Se você tiver direitos suficientes em uma prova, poderá usar o visualizador de provas, o [!UICONTROL Painel] ou qualquer um dos modos de exibição de lista para adicionar revisores a uma prova existente (consulte [Compartilhar uma Prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] Página em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

Adicionar revisores é a maneira mais comum de compartilhar provas. Se quiser explorar outras opções disponíveis, consulte:

* [Compartilhar links de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [Compartilhar a URL Pública em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [Assinar uma Prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Criar uma Mini prova no  [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## Você precisa ser um usuário do para revisar uma prova?

### Responder

Não. Os revisores convidados (pessoas sem [!DNL Workfront Proof] credenciais de logon) podem acessar uma prova na notificação por email de prova que recebem. Você pode compartilhar uma prova com quantos convidados desejar.

É possível restringir o compartilhamento de provas a pessoas com [!DNL Workfront Proof] credenciais de logon. Isso adiciona outra camada de segurança às provas. Para maior segurança, os administradores de sistema de organizações com planos da [!UICONTROL Empresa] e [!UICONTROL Ilimitados] podem configurar este requisito para todas as provas criadas na organização.

Para obter mais informações sobre a exigência de logon, consulte [Prova de segurança em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Se sua organização exigir que os revisores assinem provas eletronicamente, o que exige logon no [!DNL Workfront Proof], os usuários poderão compartilhar provas somente com usuários registrados. Isto está disponível nos planos de edição [!UICONTROL Empresa] e [!UICONTROL Ilimitado]. Para obter mais informações, consulte [Noções básicas sobre assinaturas eletrônicas [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## Posso definir um prazo final para meus revisores?

### Responder

É possível definir um prazo para uma nova prova ou versão de prova ao criar a prova. Faça isso na seção [!UICONTROL Fluxo de trabalho] da página [!UICONTROL Nova prova]. Se você usa o [!UICONTROL Fluxo de Trabalho Automatizado], é possível definir um prazo diferente para cada estágio da sua revisão.

Você também pode definir ou atualizar um prazo para uma prova existente usando a página [!UICONTROL Detalhes da prova]. Para obter mais informações, consulte [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Como posso criar uma nova versão da minha prova?

### Responder

Os revisores frequentemente solicitam alterações em seus comentários em uma prova e desejam ver uma nova versão da prova. Você pode criar novas versões de uma prova. [!DNL Workfront Proof] lembra das configurações da prova da versão anterior. Você ainda poderá editar essas configurações se precisar fazer algo como adicionar ou remover revisores para a prova.

Você deve compartilhar cada versão com os revisores específicos que precisam visualizá-la. Por exemplo, se você compartilhar somente a versão 3 com um revisor, essa pessoa não poderá ver as versões 1 e 2. Os supervisores e administradores na sua conta supervisionam todos os projetos na conta para que possam visualizar e editar todas as versões da prova.

Para obter mais informações, consulte.

## Posso compartilhar arquivos usando o [!DNL Workfront Proof]?

### Responder

Sim. Se você quiser compartilhar algo com outras pessoas, mas não precisar que elas o vejam como uma prova (ou se for um tipo de arquivo para o qual o [!DNL Workfront Proof] não oferece suporte), você poderá carregá-lo como um arquivo para sua conta do [!DNL Workfront Proof]. Assim como ocorre com as provas, você pode organizar os arquivos em pastas, marcar arquivos e adicionar uma mensagem personalizada ao email de notificação quando compartilha o arquivo. Para obter mais informações, consulte [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

Quando os destinatários recebem a notificação por email sobre um arquivo que você está compartilhando, eles podem baixar o arquivo clicando no link na notificação.

[!DNL Workfront Proof] usuários podem converter arquivos em provas depois de salvá-los em suas contas.

<!--Is there a limit-->
