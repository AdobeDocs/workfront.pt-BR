---
product-area: documents
navigation-topic: proofing-overview
title: Visão geral das provas de conteúdo interativo
description: O conteúdo interativo fornece vários métodos para envolver visualizadores. As agências podem medir o sucesso de suas campanhas usando análises coletadas de respostas a esse conteúdo.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: f783e3033a67b4702e4e2d80214cbb0c4591b922
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Visão geral das provas de conteúdo interativo

<!-- Audited: 01/2024 -->

O conteúdo interativo fornece vários métodos para envolver visualizadores. As agências podem medir o sucesso de suas campanhas usando análises coletadas de respostas a esse conteúdo.

Exemplos de conteúdo interativo:

* Sites
* Vídeos incorporados ou em fluxo contínuo
* Banners interativos
* animações HTML5
* Microsites
* Emails interativos

## Sobre a criação de provas para conteúdo interativo

Você pode criar uma prova para conteúdo interativo de uma das seguintes maneiras:

* Crie uma prova a partir de um arquivo ZIP contendo o conteúdo interativo.

  O Adobe Workfront descompacta o conteúdo do arquivo ZIP e o armazena em um servidor Workfront. Como é armazenado dessa maneira, você pode confiar que o conteúdo permanecerá o mesmo durante todo o ciclo de revisão de prova.

* Especifique o URL do conteúdo.

  Essa é a maneira mais simples de criar uma prova para conteúdo interativo. Essa também é a única maneira de revisar seu conteúdo interativamente, à medida que os usuários o experimentam na Internet.

  Com essa abordagem, um servidor externo desconhecido da Workfront armazena e hospeda o conteúdo.

  Recomendamos esse método para sites grandes porque é difícil coletar todos os arquivos que compõem um site grande. No entanto, como o conteúdo da prova é armazenado externamente, o Workfront não pode protegê-lo de alterações feitas pelos desenvolvedores que trabalham nele, portanto, talvez você não possa depender de o conteúdo permanecer o mesmo durante o ciclo de revisão da prova.

## Sobre a preparação de conteúdo interativo em um arquivo ZIP para revisão

Ao reunir o conteúdo interativo em um arquivo ZIP para comprovação, certifique-se de que ele inclua as seguintes especificações:

* Todos os ativos, como CSS, JavaScript, vídeos, sons e imagens devem ser incluídos no arquivo de pacote.
* O conteúdo interativo deve incluir o arquivo principal (index.html, index.htm). Se esse arquivo não for colocado no local raiz, a ferramenta pesquisará automaticamente a pasta para encontrá-lo. O arquivo principal não precisa ser chamado de index.html/index.htm, no entanto, só pode haver um arquivo .html/.htm colocado no local principal.
* O arquivo deve conter pelo menos uma página da Web de arquivo estático.
* O tamanho máximo do pacote é 500 MB.
* No caso de arquivos .zip criados no iOS, a ferramenta identifica automaticamente a pasta onde o conteúdo está localizado.
* Os projetos interativos são suportados somente como arquivos .zip. Os envios de arquivos .zip padrão falharão.
* O site deve ser seguro (HTTPS).

  Isso não é um requisito ao usar o Visualizador de provas de desktop.

  Para obter mais informações, consulte [Entender o visualizador de provas de desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* O site deve ter permissão para ser exibido em um iframe.

  Isso não é um requisito ao usar o Visualizador de provas de desktop.

  Para obter mais informações, consulte [Entender o visualizador de provas de desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Sobre a criação de uma prova interativa

Depois de preparar o arquivo de pacote ZIP, crie uma prova interativa.

Para obter mais informações, consulte [Criar uma prova para conteúdo interativo em um arquivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content.md).

Ou, se estiver usando o Workfront Proof, consulte a seção [Gerar uma prova para conteúdo interativo](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generate-a-proof-for-interactive-content) no artigo [Gerar provas no Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Sobre a revisão de provas interativas

Recomendamos que você use o Desktop Proofing Viewer independente como o visualizador padrão para provas interativas. No entanto, se as políticas de sua organização não permitirem o uso do aplicativo Visualizador de provas de desktop, o administrador do Workfront poderá configurar seu sistema para que você possa revisar o conteúdo interativo, incluído em um arquivo ZIP, no Visualizador de provas de web. Para obter informações comparativas sobre o Desktop Proofing Viewer e o Web Proofing Viewer, consulte [Diferenças entre o Visualizador de provas da Web e a visão geral do Visualizador de provas do desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
