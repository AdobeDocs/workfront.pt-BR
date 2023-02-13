---
product-area: documents
navigation-topic: proofing-overview
title: Visão geral das provas de conteúdo interativo
description: O conteúdo interativo fornece vários métodos de envolvimento de visualizadores. As agências podem medir o sucesso de suas campanhas usando análises coletadas das respostas a este conteúdo.
author: Courtney
feature: Digital Content and Documents
exl-id: fdcad9c6-5508-476a-bfb8-2fe3bfbb007b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Visão geral das provas de conteúdo interativo

O conteúdo interativo fornece vários métodos de envolvimento de visualizadores. As agências podem medir o sucesso de suas campanhas usando análises coletadas das respostas a este conteúdo.

Exemplos de conteúdo interativo incluem:

* Sites
* Vídeos integrados ou de transmissão
* Banners interativos
* animações do HTML5
* Microsites
* Emails interativos

Este artigo fornece o seguinte sobre revisão de conteúdo interativo:

## Sobre a criação de provas para conteúdo interativo

Você pode criar uma prova para conteúdo interativo de uma das seguintes maneiras:

* Crie uma prova de um arquivo ZIP contendo o conteúdo interativo.

   O Adobe Workfront descompacta o conteúdo do arquivo ZIP e o armazena em um servidor Workfront. Como é armazenado dessa forma, você pode confiar no conteúdo que permanece o mesmo durante todo o ciclo de revisão de prova.

* Especifique o URL do conteúdo.

   Essa é a maneira mais simples de criar uma prova para conteúdo interativo. Essa também é a única maneira de revisar seu conteúdo interativamente, já que os usuários o experimentam na Internet.

   Com essa abordagem, um servidor externo desconhecido da Workfront armazena e hospeda o conteúdo.

   Recomendamos esse método para sites grandes porque é difícil coletar todos os arquivos que compõem um site grande. No entanto, como o conteúdo da prova é armazenado externamente, o Workfront não pode protegê-lo de alterações feitas pelos desenvolvedores que trabalham nele, portanto, talvez você não possa depender do conteúdo permanecer o mesmo durante todo o ciclo de revisão de prova.

## Sobre a preparação de conteúdo interativo em um arquivo ZIP para prova

Ao agrupar o conteúdo interativo em um arquivo ZIP para prova, verifique se ele inclui as seguintes especificações:

* Todos os ativos, como CSS, JavaScript, vídeos, sons e imagens devem ser incluídos no arquivo de pacote.
* O conteúdo interativo deve incluir o arquivo principal (index.html, index.htm). Se esse arquivo não for colocado no local raiz, a ferramenta pesquisará automaticamente a pasta para encontrá-lo. O arquivo principal não precisa ser chamado de index.html/index.htm, no entanto, só pode haver um arquivo .html/.htm no local principal.
* O arquivo deve conter pelo menos uma página Web de arquivo estático.
* O tamanho máximo do pacote é de 500 MB.
* No caso de arquivos .zip criados no iOS, a ferramenta identifica automaticamente a pasta onde o conteúdo está localizado
* Os projetos interativos são suportados somente como arquivos .zip. Os envios padrão de arquivos .zip falharão.
* O site deve ser seguro (HTTPS).

   Esse não é um requisito ao usar o Desktop Proofing Viewer.

   Para obter mais informações, consulte [Entender o visualizador de prova de desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

* O site deve ter permissão para ser visualizado em um iframe.

   Esse não é um requisito ao usar o Desktop Proofing Viewer.

   Para obter mais informações, consulte [Entender o visualizador de prova de desktop](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md).

## Sobre a criação de uma prova interativa

Depois de preparar o arquivo de pacote ZIP, crie uma prova interativa.

Para obter mais informações, consulte [Criar uma prova para o conteúdo interativo em um arquivo ZIP](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-proof-interactive-content-.md).

Ou, se estiver usando o Workfront Proof, consulte a seção [Gerar uma prova para conteúdo interativo](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md#generati) no artigo [Gerar provas na prova do Workfront](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Sobre a revisão de provas interativas

Recomendamos que você use o Desktop Proofing Viewer independente como visualizador padrão para provas interativas. No entanto, se as políticas de sua organização não permitirem o uso do aplicativo Desktop Proofing Viewer, o administrador do Workfront poderá configurar o sistema para que você possa revisar o conteúdo interativo, empacotado em um arquivo ZIP, no Web Proofing Viewer. Para obter informações comparativas sobre o Visualizador de Verificação de Verificação Linguística para Desktop e o Visualizador de Verificação Linguística para Web, consulte [Diferenças entre o Visualizador de Provas da Web e a visão geral do Visualizador de Provas de Desktop](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).
