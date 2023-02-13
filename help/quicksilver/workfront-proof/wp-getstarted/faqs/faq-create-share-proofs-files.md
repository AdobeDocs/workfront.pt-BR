---
content-type: faq
product-previous: workfront-proof
product-area: documents;system-administration
navigation-topic: faqs-workfront-proof
title: Perguntas frequentes - Criar e compartilhar provas e arquivos
description: Uma prova é um arquivo estático, de áudio ou de vídeo que está disponível para revisão no visualizador de prova. Os revisores adicionados a uma prova têm um conjunto de ferramentas disponíveis para fazer comentários e tomar decisões sobre a prova.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: eb0eb160-4bcf-4bc1-ad13-df19f692bef6
source-git-commit: d5ffd576fcedf9b10dce5e5d5bd9245dd7f67ef8
workflow-type: tm+mt
source-wordcount: '1365'
ht-degree: 0%

---

# Perguntas frequentes - Criar e compartilhar provas e arquivos

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

## O que é prova?

### Resposta

Uma prova é um arquivo estático, de áudio ou de vídeo que está disponível para revisão no visualizador de prova. Os revisores adicionados a uma prova têm um conjunto de ferramentas disponíveis para fazer comentários e tomar decisões sobre a prova.

## Quais tipos de arquivos são compatíveis?

### Resposta

Provas podem ser criadas a partir de arquivos estáticos, de áudio e de vídeo. Não é possível carregar arquivos com mais de 4 GB. [!DNL Workfront] suporta mais de 150 tipos de arquivo (consulte [Visão geral dos tipos de arquivos de prova suportados e limites de tamanho](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md) para obter uma lista completa).

## Qual é a diferença entre uma prova e um arquivo?

### Resposta

Ao fazer upload de um arquivo para [!DNL Workfront Proof], o sistema armazena o arquivo em seu [!DNL Workfront Proof] conta. Quando você o compartilha, [!DNL Workfront Proof] envia por email os destinatários com um link em que eles podem clicar para baixar o arquivo. Você pode compartilhar qualquer tipo de arquivo que desejar.

Ao criar uma prova de um arquivo, você carregou para o [!DNL Workfront Proof], você pode disponibilizar o arquivo para revisão no visualizador de prova. Os revisores recebem um email com um link para a prova. Ao abrir a prova, eles veem a imagem da prova e podem adicionar comentários e tomar decisões sobre ela. Você pode criar provas usando arquivos da lista de tipos de arquivos suportados. Você também pode criar provas usando URLs para sites e outros conteúdos da Web.

Para obter uma lista completa dos tipos de arquivos suportados, consulte [Visão geral dos tipos de arquivos de prova suportados e limites de tamanho](../../../review-and-approve-work/proofing/proofing-overview/supported-proofing-file-types.md).

## Como criar uma prova?

### Resposta

Você pode criar provas de arquivos estáticos, arquivos de áudio, arquivos de vídeo e URLs (consulte ).

Para criar uma prova na conta, você precisa ser um usuário com o perfil de permissão correto (consulte [[!UICONTROL Perfis de permissões de prova] em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md)).

Se você carregar vários arquivos ao mesmo tempo, crie várias provas que podem ser enviadas para o mesmo grupo de revisores usando um email. Se sua organização tiver uma [!UICONTROL Empresa] ou [!UICONTROL Ilimitado] você pode combinar arquivos em uma única prova (consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md)).

## Quais são as funções de prova e alertas de email?

### Resposta

As funções de prova definem quais ações um revisor precisa tomar em uma prova. Há diferentes opções de função que podem ser usadas para revisores ao criar uma prova, dependendo se você deseja que eles possam fazer comentários, tomar decisões e assim por diante. Para obter mais informações, consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md).

Os alertas de email atualizam os revisores em um progresso de prova (são diferentes das notificações de nova prova e de prova tardia). Você pode selecionar opções diferentes para revisores diferentes, dependendo da função de cada revisor na prova. Para obter mais informações, consulte [Criar uma prova avançada com um [!UICONTROL Fluxo de trabalho automatizado]](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Posso criar uma prova a partir de vários arquivos?

### Resposta

Combinar vários arquivos em uma única prova é um recurso disponível em [!UICONTROL Empresa] e [!UICONTROL Ilimitado] planos de edição. Essa opção é possível somente para arquivos estáticos, não para arquivos de vídeo. Para obter mais informações, consulte  [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Posso criar provas de URLs?

### Resposta

Sim, você pode criar provas de sites e de outro conteúdo da Web. Ao adicionar um URL para criar uma prova, você pode especificar se deseja uma prova estática ou uma prova interativa:

* Em uma prova interativa, os revisores podem navegar e interagir normalmente com o site ou outro conteúdo da Web, como anúncios com vídeo ou áudio de transmissão, [!DNL Flash] elementos em um anúncio, animações de HTML e banners interativos. Para obter mais informações, consulte [Criar uma prova para o conteúdo interativo em um arquivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).
* Para uma prova estática, [!DNL Workfront] O usa um conjunto de capturas de tela das páginas e subpáginas especificadas. Os hiperlinks estão ativos na prova, portanto, você pode testar se levam ou não ao destino correto. Para obter mais informações, consulte [Criar uma prova estática para um site ou outro conteúdo da Web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-static-proof-website-other-web-content.md).

Você pode adicionar vários URLs de uma só vez, se separá-los com um espaço. Observe que a combinação só está disponível em [!UICONTROL Empresa] e [!UICONTROL Ilimitado] planos de edição.

## As pessoas que não têm uma prova de logon podem criar provas na minha conta?

### Resposta

Você precisa de credenciais de logon para criar provas diretamente em uma [!DNL Workfront Proof] conta.

## O que significa compartilhar uma prova?

### Resposta

O compartilhamento de uma prova dá aos revisores acesso a ela para que possam adicionar comentários e marcações e tomar decisões sobre ela. Os revisores convidados acessam provas da notificação por email recebida. Revisores com seus próprios [!DNL Workfront Proof] pode acessar provas na [!UICONTROL Painel].

## Como compartilho uma prova?

### Resposta

Ao criar uma prova, você pode adicionar revisores no [!UICONTROL Fluxo de trabalho] da seção [!UICONTROL Nova prova] página. Quando a prova estiver pronta, [!DNL Workfront Proof] envia um email para os revisores que contém um link para a prova.

Se você tiver as permissões necessárias em uma prova, poderá usar o visualizador de prova, sua [!UICONTROL Painel]ou qualquer uma das exibições da lista para adicionar revisores a uma prova existente (consulte [Compartilhar uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof.md) and [Manage Items on the [!UICONTROL Views] Página em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-items-on-views-page.md).

Adicionar revisores é a maneira mais comum de compartilhar provas. Se quiser explorar outras opções disponíveis, consulte:

* [Compartilhar links de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-proof-links.md)
* [Compartilhe o URL público em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/share-public-url.md)
* [Assinar uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/subscribe-to-proof.md)
* [Criar uma Mini prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/create-mini-proof.md)

## Você precisa ser um usuário para revisar uma prova?

### Resposta

não. Revisores convidados (pessoas sem [!DNL Workfront Proof] credenciais de logon) podem acessar uma prova da notificação por email de prova recebida. Você pode compartilhar uma prova com quantos convidados quiser.

É possível restringir o compartilhamento de provas a pessoas com [!DNL Workfront Proof] credenciais de logon. Isso adiciona outra camada de segurança às provas. Para maior segurança, os administradores de sistema de organizações com [!UICONTROL Empresa] e [!UICONTROL Ilimitado] os planos podem configurar esse requisito para todas as provas criadas na organização.

Para obter mais informações sobre como exigir logon, consulte [Segurança de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/proof-security-in-workfront-proof.md).

Se sua organização requer revisores para assinar provas eletronicamente, o que requer fazer logon em [!DNL Workfront Proof], os usuários podem compartilhar provas somente com usuários registrados. Isso está disponível em [!UICONTROL Empresa] e [!UICONTROL Ilimitado] planos de edição. Para obter mais informações, consulte [Noções básicas sobre assinaturas eletrônicas no [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/managing-security/electronic-sigs-in-wp.md).

## Posso definir um prazo para meus revisores?

### Resposta

Você pode definir um prazo para uma nova prova ou uma nova versão de prova ao criar a prova. Você faz isso no [!UICONTROL Fluxo de trabalho] da seção [!UICONTROL Nova prova] página. Se você usar [!UICONTROL Fluxo de trabalho automatizado], é possível definir um prazo diferente para cada etapa da revisão.

Você também pode definir ou atualizar um prazo para uma prova existente usando o [!UICONTROL Detalhes da prova] página. Para obter mais informações, consulte [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).

## Como posso criar uma nova versão da minha prova?

### Resposta

Os revisores muitas vezes solicitam alterações em seus comentários em uma prova e desejam ver uma nova versão da prova. Você pode criar novas versões de uma prova. [!DNL Workfront Proof] lembra das configurações da prova da versão anterior. Você ainda pode editar essas configurações se precisar fazer algo como adicionar ou remover revisores para a prova.

Você deve compartilhar cada versão com os revisores específicos que precisam exibi-la. Por exemplo, se você compartilhar apenas a versão 3 com um revisor, essa pessoa não poderá ver as versões 1 e 2. Supervisores e administradores em sua conta supervisionam todos os projetos na conta, para que possam ver e editar todas as versões da prova.

Para obter mais informações, consulte .

## Posso compartilhar arquivos usando [!DNL Workfront Proof]?

### Resposta

Sim. Se você deseja compartilhar algo com outras pessoas, mas não precisa que elas o exibam como uma prova (ou se é um tipo de arquivo não compatível com [!DNL Workfront Proof]), você pode fazer upload dele como um arquivo para sua [!DNL Workfront Proof] conta. Assim como com provas, você pode organizar seus arquivos em pastas, marcar arquivos e adicionar uma mensagem personalizada ao email de notificação quando compartilhar o arquivo. Para obter mais informações, consulte [Fazer upload de arquivos e conteúdo da Web para [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/upload-files-web-content.md).

Quando os recipients recebem a notificação por email sobre um arquivo que você está compartilhando, eles podem baixar o arquivo clicando no link na notificação.

[!DNL Workfront Proof] os usuários podem converter arquivos em provas depois de salvá-los em suas contas.

<!--Is there a limit-->
