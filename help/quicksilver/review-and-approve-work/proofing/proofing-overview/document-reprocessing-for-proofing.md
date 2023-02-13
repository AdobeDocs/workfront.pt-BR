---
product-area: documents
navigation-topic: proofing-overview
title: Reprocessamento de documentos para visão geral de revisão
description: Ao enviar um documento (DOCX, PDF, XLSX, AI) para prova, a Adobe Workfront o reprocessa para que possa ser exibido no visualizador de prova sem o aplicativo de software usado para criá-lo.
author: Courtney
feature: Digital Content and Documents
exl-id: e577fa71-4828-4fc2-93a2-0eddbb5ad2ad
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '649'
ht-degree: 0%

---

# Reprocessamento de documentos para visão geral de revisão

Ao enviar um documento (DOCX, PDF, XLSX, AI) para prova, a Adobe Workfront o reprocessa para que possa ser exibido no visualizador de prova sem o aplicativo de software usado para criá-lo. 

Cada página do seu documento aparece no visualizador de prova como uma imagem em miniatura. Ao clicar em uma miniatura, é possível ampliar a versão de bitmap dessa página em 100%, 200% e 400%. Para provas de altura ou largura superiores a 800 mm, o nível máximo de zoom é de 200%.

As cores em seu documento são exibidas em sRGB com conversão de cores da biblioteca de Adobe mais recente. O visualizador de prova suporta qualquer perfil ICC (International Color Consortium) incorporado no documento.

Todo o texto da fonte é extraído em sua camada, desde que você inclua a extensão de arquivo correta ao fazer upload do documento para o sistema. O texto incluído como imagens ou curvas não é exibido.

>[!NOTE]
>
>Atualmente, o Workfront suporta documentos contendo até 2000 páginas. Isso inclui provas combinadas. Para obter mais informações, consulte [Criar uma prova de várias páginas](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-multi-page-proof.md).

## Dicas gerais

* Como os arquivos PDF são os mais padronizados e confiáveis, recomendamos converter documentos nesse formato antes de carregá-los.
* Use a versão mais recente possível do seu software para criar seus documentos originais.
* Se não tiver certeza de quais configurações usar ao salvar ou exportar seus documentos no aplicativo em que você os criou, use as configurações padrão. 
* Certifique-se de incorporar todas as fontes usadas em um documento dentro dele. Se você usar fontes personalizadas, seu documento exibirá essas fontes somente em máquinas onde elas estiverem instaladas.
* Se possível, coloque todos os elementos de texto nas camadas superiores do design. Isso deve garantir que o texto seja extraído e selecionável na ferramenta de anotação de texto.
* Coloque todas as imagens e elementos do seu documento dentro dele. Se você os vincular de fontes externas, como outro arquivo em seu computador, eles não serão exibidos na prova criada.
* Crie seu documento usando os padrões recomendados para seu tipo e otimize-o antes de carregá-lo. Isso garantirá que o documento seja aberto com êxito no visualizador de prova, bem como em todos os outros aplicativos e plataformas.
* No software de design, tente executar opções de &quot;comprovação&quot; para ver se o documento gera algum aviso. Essas opções estão disponíveis na maioria dos aplicativos como visualização de saída, produção de impressão e assim por diante. Consulte a documentação do aplicativo para obter mais informações.
* Certifique-se de que as configurações de cores sejam consistentes em todo o documento.
* Se o documento estiver protegido contra ações como a cópia de arquivos, a ferramenta de extração de prova poderá não conseguir acessar seu conteúdo.

## Tempos do processo

Normalmente, o processamento leva alguns segundos por página. No entanto, vários fatores podem prolongar isso, como tráfego/largura de banda da rede, velocidades de conexão locais e velocidades de conexão internacionais (para usuários fora dos EUA). O tempo de processamento pode também ser afetado:

* Para documentos e imagens estáticas: contagem de página, dimensões de página, volume de texto, imagem e complexidade de objetos (elementos como vários elementos vetoriais, camadas, transparências).
* Para vídeos: durações longas, dimensões grandes e codecs usados.
* Para capturas da Web: tempos de carregamento de página da Web e dimensões de página.

## Etapas do processo

Os arquivos enviados passam por algumas ou todas as etapas a seguir:

1. **Submissão**. Ao fazer upload de um documento para o sistema, você faz isso usando a página New proof ou usando uma API (Application Programing Interface). 
1. **Fila**. Durante longos períodos de tráfego, a Workfront pode precisar colocar em fila envios para evitar sobrecarga do sistema. A maioria das provas gasta apenas alguns segundos em uma fila. 
1. **Processando.** Os arquivos chegam às máquinas de processamento de acordo com o tipo de conteúdo. Usamos ferramentas diferentes para processar provas de vídeo, capturas da Web, imagens estáticas e documentos. Os envios de captura da Web interativa e contêineres de mídia avançada (ZIP) não exigem processamento.
