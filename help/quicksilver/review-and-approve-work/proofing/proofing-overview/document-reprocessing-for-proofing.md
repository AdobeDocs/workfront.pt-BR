---
product-area: documents
navigation-topic: proofing-overview
title: Visão geral do reprocessamento de documentos para revisão
description: Quando você envia um documento (DOCX, PDF, XLSX, AI) para revisão de texto, o Adobe Workfront o reprocessa para que ele possa ser exibido no revisor de provas sem o aplicativo de software usado para criá-lo.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '680'
ht-degree: 0%

---

# Visão geral do reprocessamento de documentos para revisão

Quando você envia um documento (DOCX, PDF, XLSX, AI) para revisão de texto, o Adobe Workfront o reprocessa para que ele possa ser exibido no revisor de provas sem o aplicativo de software usado para criá-lo. 

Cada página do documento aparece no visualizador de provas como uma imagem em miniatura. Ao clicar em uma miniatura, é possível aplicar o zoom em uma versão de bitmap dessa página em 100%, 200% e 400%. Para provas que excedam 800 mm em altura ou largura, o nível máximo de zoom é de 200%.

As cores do documento são exibidas em sRGB com conversão de cores da biblioteca Adobe mais recente. O visualizador de provas é compatível com qualquer perfil ICC (Consórcio Internacional de Cores) incorporado no documento.

Todo o texto da fonte é extraído em sua camada, desde que você inclua a extensão de arquivo correta ao fazer upload do documento no sistema. O texto incluído como imagens ou curvas não é exibido.

>[!NOTE]
>
>O Workfront atualmente suporta documentos que contêm até 2.000 páginas. Isso inclui provas combinadas. Para obter mais informações, consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Dicas gerais

* Como os arquivos PDF são os mais padronizados e confiáveis, recomendamos converter os documentos para esse formato antes de carregá-los.
* Use a versão mais recente possível do software para criar os documentos originais.
* Se não tiver certeza sobre quais configurações usar ao salvar ou exportar seus documentos no aplicativo em que você os criou, use as configurações padrão. 
* Certifique-se de incorporar todas as fontes usadas em um documento dentro dele. Se você usar fontes personalizadas, o documento exibirá essas fontes somente nos computadores em que elas estiverem instaladas. No entanto, como as fontes personalizadas não estão incluídas no sistema de prova, ele não pode usar fontes personalizadas ao gerar o arquivo, mesmo quando incorporado.
* Se possível, coloque todos os elementos de texto nas camadas superiores do design. Isso deve garantir que o texto seja extraído e selecionável na ferramenta de anotação de texto.
* Coloque todas as imagens e os elementos do documento dentro dele. Se você os vincular a partir de fontes externas, como outro arquivo no computador, eles não serão exibidos na prova criada.
* Crie o documento usando os padrões recomendados para o tipo e otimize-o antes de carregá-lo. Isso garantirá que o documento será aberto com êxito no visualizador de provas, bem como em todos os outros aplicativos e plataformas.
* No software de design, tente executar as opções de &quot;comprovação&quot; para ver se o documento gera avisos. Essas opções estão disponíveis na maioria dos aplicativos como pré-visualização de saída, produção de impressão e assim por diante. Consulte a documentação do aplicativo para obter mais informações.
* Verifique se as configurações de cor são consistentes em todo o documento.
* Se o seu documento estiver protegido contra ações como copiar arquivos, a ferramenta de extração de prova talvez não consiga acessar seu conteúdo.

## Tempos do processo

Normalmente, o processamento leva alguns segundos por página. Entretanto, vários fatores podem prolongar isso, como tráfego/largura de banda de rede, velocidades de conexão local e velocidades de conexão internacional (para usuários fora dos EUA). Os seguintes itens também podem afetar o tempo de processamento:

* Para documentos e imagens estáticos: contagem de páginas, dimensões de página, volume de texto, imagem e complexidade de objetos (elementos como vários elementos de vetor, camadas, transparências).
* Para vídeos: durações longas, dimensões grandes e codecs usados.
* Para capturas da Web: tempos de carregamento da página da Web e dimensões da página.

## Etapas do processo

Os arquivos enviados passam por algumas ou todas as seguintes etapas:

1. **Envio**. Ao fazer upload de um documento no sistema, você faz isso usando a página Nova prova ou usando uma interface de programação de aplicativo (API). 
1. **Fila**. Durante períodos de tráfego intenso, a Workfront pode precisar colocar os envios em fila para evitar sobrecarga do sistema. A maioria das provas passa apenas alguns segundos em uma fila. 
1. **Processando.** Os arquivos chegam às máquinas de processamento de acordo com o tipo de conteúdo. Usamos diferentes ferramentas para processar provas de vídeo, capturas da Web, imagens estáticas e documentos. Os envios de Rich Media containers (ZIP) e captura interativa na Web não exigem processamento.
