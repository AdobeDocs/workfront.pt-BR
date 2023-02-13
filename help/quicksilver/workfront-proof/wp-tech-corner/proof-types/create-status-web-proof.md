---
product-previous: workfront-proof
product-area: documents
navigation-topic: proof-types
title: Criar uma prova de site estático usando [!DNL Workfront Proof]
description: Você pode criar provas estáticas nas suas páginas da Web. Além disso, você pode simular vários dispositivos definindo a resolução da tela das capturas.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: b93ed288-1bf2-4268-96c3-6263ab6be633
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Criar uma prova de site estático usando [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Você pode criar provas estáticas nas suas páginas da Web. Além disso, você pode simular vários dispositivos definindo a resolução da tela das capturas.

## Criação de uma prova de site estático

1. Abra o [!UICONTROL Nova prova] conforme descrito em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).
1. Cole ou digite o URL na **www.shareyourlink.com** caixa.
1. Você pode repetir essa etapa para adicionar vários URLs.
1. Logo abaixo desta caixa, clique na resolução (o padrão é 1366x768), em seguida, selecione as resoluções desejadas no **[!UICONTROL Resolução de tela]** caixa.
Selecione uma resolução menor se quiser provar designs para dispositivos móveis. Geralmente, os designs são carregados de acordo com a resolução da tela/janela do navegador.

1. Clique em **[!UICONTROL Procurar subpáginas]** se desejar incluir páginas conectadas que estão no mesmo domínio/subdomínio que o URL inserido.
   [!DNL Workfront Proof] faz a varredura das páginas conectadas e as lista abaixo da variável **[!UICONTROL Procurar subpáginas]** opção. Você pode selecionar as páginas que deseja incluir.

1. Com o [!UICONTROL Combinar provas] você pode enviar todas as páginas da Web como uma única prova de várias páginas.
1. Clique em **[!UICONTROL Concluído]**, em seguida, conclua a configuração da prova, como explicado em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

## Sobre páginas e páginas protegidas por senha que exigem autorização

[!DNL Workfront Proof] O não pode capturar um site protegido por senha como prova estática.

Para criar provas de páginas que exigem autorização, sua equipe de TI deve adicionar um dos seguintes URLs à  de Lista de permissões da empresa pela qual a ferramenta de captura da Web se conecta:

**Clusters AWS nos EUA**: webcapture.proofhq.com

**GCP nos EUA**: webcapture.gcp.proofhq.com

**Grupos EMEA**: webcapture.proofhq.eu

>[!NOTE]
>
>Recomendamos provas interativas em vez de provas estáticas para páginas internas que exigem autorização e sites protegidos por senha. Para obter mais informações, consulte [Visão geral das provas de conteúdo interativo](../../../review-and-approve-work/proofing/proofing-overview/interactive-content-proofs.md).

## Sobre o processamento de provas estáticas do site

* Animações, vídeos incorporados, scripts e interações não podem ser incluídos em provas estáticas de site. Se quiser provar um conteúdo interativo, consulte [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md) em [Gerar provas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/generate-proofs.md).

* Geralmente, as páginas de prova são preparadas com uma taxa de cerca de 20 segundos por página. No entanto, o tempo geral de preparação também depende dos servidores onde as páginas estão hospedadas. A ferramenta aguarda 60 segundos para que cada URL enviado seja carregado. Se esse tempo de espera for excedido, a prova falhará.
* Para provas combinadas, se qualquer um dos URLs não estiver respondendo à ferramenta de captura, a prova falhará.
* [!DNL Workfront Proof] captura páginas da Web até 195 polegadas após a rasterização. Se a página da Web for maior que isso, a prova falhará.
* A extração de texto está disponível em todos os elementos de texto, mas o texto colocado como imagens não é extraído.
* Os hiperlinks de texto são clicáveis nas provas e as páginas vinculadas são abertas nas novas guias do navegador.
* Os hiperlinks nas imagens não são clicáveis se os elementos style=&quot;display:block&quot; forem usados dentro do `<a>` tags. Recomendamos ajustar essas partes do design da página.
* Para obter melhores resultados, recomendamos criar as páginas usando as práticas recomendadas de codificação e os padrões reconhecidos.
