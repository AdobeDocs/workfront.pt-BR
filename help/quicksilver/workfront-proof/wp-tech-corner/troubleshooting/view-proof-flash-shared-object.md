---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: Problemas Ao Exibir Provas - Objetos Compartilhados Do Flash Explicados
description: '"Nota: As informações neste artigo se referem a funcionalidade que está obsoleta no momento e será removida de [!DNL Workfront] em 2018. Recomendamos que você use o novo Visualizador de Provas da Web (conforme descrito em Revisar Provas no Visualizador de Provas da Web) ou o Visualizador de Provas de Desktop (conforme descrito em Revisar Provas no Visualizador de Provas de Desktop).'''
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: f1f3561e-8660-4c1e-b48f-446eb0eaac06
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '461'
ht-degree: 0%

---

# Problemas ao exibir provas - [!DNL Flash] Objetos compartilhados explicados

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

>[!NOTE]
>
>As informações neste artigo se referem a funcionalidade que está obsoleta no momento e será removida de [!DNL Workfront] em 2018. Recomendamos que você use o novo Visualizador de Provas da Web (conforme descrito em [Revisar Provas no Visualizador de Provas da Web](https://support.workfront.com/hc/en-us/sections/115000275214-Reviewing-Proofs-in-the-Web-Proofing-Viewer)) ou o visualizador de prova de Desktop (conforme descrito em [Revisar provas no visualizador de prova de Desktop](https://support.workfront.com/hc/en-us/sections/360000686434-Reviewing-Proofs-in-the-Desktop-Proofing-Viewer)).

## [!DNL Flash] Objetos compartilhados

Um objeto compartilhado local, às vezes chamado de &quot;[!DNL Flash] cookie&quot; é um arquivo de dados que pode ser criado em seu computador pelos sites que você visitar. Os objetos compartilhados são usados com mais frequência para aprimorar a experiência de navegação na Web. A [!DNL Flash] cookie é uma mensagem usada em [!DNL Adobe Flash] que é enviado de um servidor da Web para um navegador da Web e, em seguida, é armazenado como um arquivo de dados no navegador.

Como a variável [!DNL Workfront Proof] O visualizador é baseado em [!DNL Flash], valeria a pena verificar para que armazenamento é permitido [!DNL Flash] no seu computador.

## [!DNL Flash] Objetos compartilhados - problemas conhecidos

Se a variável [!DNL Flash] o armazenamento está definido como 0 KB ou tem outra configuração que bloqueia [!DNL Flash] Os aplicativos do podem salvar os dados localmente, isso pode causar alguns problemas conhecidos no [!DNL Workfront Proof] Visualizador:

* O pop-up de tour &quot;Introdução&quot; continua aparecendo, embora a opção de não exibi-lo novamente tenha sido escolhida
* [!DNL Workfront Proof] O desempenho do visualizador fica lento devido ao número crescente de comentários adicionados às provas
* As provas não estão sendo carregadas e você obtém a &#39;tela cinza&#39; em vez de uma imagem real

## Permitir [!DNL Flash] Objetos compartilhados

Certifique-se de que o armazenamento [!DNL Flash] Objetos compartilhados é permitido no computador e o limite de armazenamento não é 0.

Para verificar se os Objetos compartilhados são permitidos:

1. Clique com o botão direito do mouse no [!DNL Workfront Proof] Visualizador.
1. Selecionar **[!UICONTROL Configurações globais]** no menu de contexto.
1. Vá para o **[!UICONTROL Armazenamento]** guia .
1. Certifique-se de que **[!UICONTROL Permitir que sites guardem informações neste computador]** está selecionada (1).
1. ![2017-06-09_1929.png](assets/2017-06-09-1929-350x267.png)

## Aumento [!DNL Flash] armazenamento

Por padrão [!DNL Flash] os aplicativos podem armazenar até 100 KB de dados na unidade do usuário, mas isso pode ser facilmente modificado pelos usuários. A solução para muitos [!DNL Flash] problemas relacionados são aumentar a [!DNL Flash] armazenamento. Isso pode ser feito diretamente do [!DNL Workfront Proof] Visualizador:

1. Abra uma prova.
1. Abra o menu do botão direito na prova.
1. Clique em **[!UICONTROL Configurações]** para abrir o [!DNL Flash] pop-up de configurações.
1. Vá para o **[!UICONTROL Local]** guia armazenamento.
1. Aumente o armazenamento até, por exemplo, 100 KB (1).
1. Feche o pop-up de configurações e abra novamente a prova .

![2017-06-09_1926.png](assets/2017-06-09-1926-350x274.png)
