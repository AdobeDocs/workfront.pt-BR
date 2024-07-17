---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Criar uma Prova Estática de Site usando  [!DNL Workfront Proof]
description: É possível criar provas estáticas nas páginas da Web. Além disso, é possível simular vários dispositivos definindo a resolução de tela das capturas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Criar uma Prova Estática de Site usando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

É possível criar provas estáticas nas páginas da Web. Além disso, é possível simular vários dispositivos definindo a resolução de tela das capturas.

## Criação de uma prova estática de site

1. Abra a página [!UICONTROL Nova prova], conforme descrito em [Gerar Provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Cole ou digite sua URL na caixa **www.shareyourlink.com**.
1. Você pode repetir essa etapa para adicionar vários URLs.
1. Logo abaixo desta caixa, clique na resolução (o padrão é 1366x768) e selecione qualquer resolução desejada na caixa **[!UICONTROL Resolução da captura de tela]**.
Selecione uma resolução menor se quiser revisar designs para dispositivos móveis. Geralmente, os designs são carregados de acordo com a resolução da janela da tela/navegador.

1. Clique em **[!UICONTROL Procurar subpáginas]** se desejar incluir páginas conectadas que estejam no mesmo domínio/subdomínio que a URL inserida.
   O [!DNL Workfront Proof] verifica as páginas conectadas e as lista abaixo da opção **[!UICONTROL Procurar subpáginas]**. É possível selecionar as páginas que deseja incluir.

1. Com o recurso [!UICONTROL Combinar provas], é possível enviar todas as páginas da Web como uma única prova de várias páginas.
1. Clique em **[!UICONTROL Concluído]** e finalize a configuração da prova conforme explicado em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Sobre Páginas Protegidas por Senha e Páginas que Exigem Autorização

[!DNL Workfront Proof] não pode capturar um site protegido por senha como uma prova estática.

Para criar provas a partir de páginas que exigem autorização, sua equipe de TI deve adicionar um dos seguintes URLs ao Incluo na lista de permissões da sua empresa por meio do qual nossa ferramenta de captura da Web se conecta:

**clusters AWS nos EUA**: webcapture.proofhq.com

**Clusters GCP nos EUA**: webcapture.gcp.proofhq.com

**clusters EMEA**: webcapture.proofhq.eu

>[!NOTE]
>
>Recomendamos provas interativas em vez de provas estáticas para páginas internas que exigem autorização e sites protegidos por senha. Para obter mais informações, consulte [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Sobre o processamento de provas estáticas do site

* Animações, vídeos incorporados, scripts e interações não podem ser incluídos em provas estáticas do site. Para revisar o conteúdo interativo, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* As páginas de prova geralmente são preparadas capturadas na taxa de cerca de 20 segundos por página. No entanto, o tempo de preparação geral também depende dos servidores onde as páginas estão hospedadas. A ferramenta aguarda 60 segundos para que cada URL enviado seja carregado. Se esse tempo de espera for excedido, a prova falhará.
* Para provas combinadas, se qualquer um dos URLs não estiver respondendo à ferramenta de captura, a prova falhará.
* O [!DNL Workfront Proof] captura páginas da Web de até 195 polegadas de comprimento após a rasterização. Se a página da Web for maior que isso, a prova falhará.
* A extração de texto está disponível em todos os elementos de texto, mas o texto inserido como imagens não é extraído.
* Hiperlinks de texto são clicáveis nas provas e as páginas vinculadas abrem nas novas guias do navegador.
* Os hiperlinks nas imagens não podem ser clicados se os elementos style=&quot;display:block&quot; forem usados dentro das tags `<a>`. Recomendamos ajustar essas partes do design da página.
* Para obter melhores resultados, recomendamos criar as páginas usando as melhores práticas de codificação e padrões reconhecidos.
