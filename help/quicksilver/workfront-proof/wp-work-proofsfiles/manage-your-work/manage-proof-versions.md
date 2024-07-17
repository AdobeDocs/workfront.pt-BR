---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Gerenciando Versões de Prova em  [!DNL Workfront Proof]
description: Gerenciar feedback em várias versões ou revisões de um trabalho pode ser um enorme desafio.O  [!DNL Workfront Proof] simplifica esse processo permitindo que você crie e compare várias versões de uma prova.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '768'
ht-degree: 0%

---

# Gerenciando versões de prova em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Gerenciar feedback em várias versões ou revisões de um trabalho pode ser um enorme desafio. O [!DNL Workfront Proof] simplifica esse processo ao permitir que você crie e compare várias versões de uma prova.

Não há limite para o número de versões de uma prova que você pode criar. Portanto, se você precisar passar por muitas revisões com um cliente para obter uma aprovação final, todas as versões criadas poderão ser visualizadas e gerenciadas facilmente no [!DNL Workfront Proof].

As permissões são específicas a uma versão, portanto, é possível conceder permissão a uma pessoa para ver uma versão, mas não outra. Por outro lado, se você compartilhar uma versão posterior com uma pessoa, ela não poderá ver as versões anteriores, a menos que você retorne e adicione-as explicitamente a essas versões anteriores também.

Para criar uma nova versão de uma prova, você deve ter direitos de edição na prova.

Consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) para obter mais informações sobre quem tem direitos de edição em uma prova. Consulte para saber mais sobre criação de versões.

## Exibição de versões de prova no visualizador de provas

O nome completo da versão que você está visualizando é exibido na parte superior esquerda do visualizador de provas. Qualquer outra versão da prova será exibida somente como números de versão.

1. Abra uma prova no visualizador de provas, conforme descrito em [Abrindo uma Prova no [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. No visualizador de provas, clique no número da versão à direita do nome da prova.
1. Para exibir a outra versão, clique no nome no menu que aparece ao clicar no número da versão.
1. Para comparar duas versões, clique no ícone **[!UICONTROL Comparar provas]**.\
   ![Comparar_Provas_button.png](assets/compare-proofs-button.png)\
   Se houver várias versões da prova, você poderá selecionar quais duas versões deseja comparar clicando no número da versão relevante em cada lado da tela dividida do modo de comparação.

Para obter informações sobre como revisar provas em um visualizador de provas, consulte [Revisar uma prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Acesso a versões de prova por meio da página Detalhes da prova

É possível acessar todas as versões de uma prova na página Detalhes da prova.

1. Abra a página de detalhes da prova para obter uma prova, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Clique na guia das guias de versão na parte superior da página e clique em **[!UICONTROL Ir para prova]** para abrir a versão desejada no visualizador de provas.\
   ![Guias_de_Versão_na_Prova_Detalhes_página.png](assets/version-tabs-on-proof-details-page-350x205.png)

## Vincular versões de prova

Se a prova tiver várias versões, a versão anterior da prova será comumente conhecida como prova principal.

Se você quiser alterar a prova principal (versão anterior) para outra prova na sua conta ou conectar uma única prova a outra prova na sua conta (como uma nova versão da outra prova), siga estas etapas:

1. Abra a página de detalhes da prova para obter uma prova, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Alterar versão anterior]**.

1. Na caixa **[!UICONTROL Alterar versão anterior]** exibida, selecione a prova que deseja definir como a prova pai (versão anterior).\
   Se precisar de ajuda para encontrar a prova na lista, você pode classificar as colunas clicando no cabeçalho da coluna.

1. Clique em **[!UICONTROL Alterar versão anterior]** na parte inferior da caixa para conectar versões.

>[!NOTE]
>
>Quando você conecta uma prova a outra prova em sua conta (como uma nova versão), o [!DNL Workfront Proof] bloqueia a prova de que está agora na versão anterior.

## Desvinculação de versões de prova

Você pode desvincular a prova que está visualizando no momento da prova principal (versão anterior) sem vinculá-la a outra prova na sua conta do:

1. Abra a página de detalhes da prova para obter uma prova, conforme descrito em [Gerenciar detalhes da prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Remover link para a versão anterior]**.

   * Somente a última versão pode ser desvinculada (desconectada) de todo o conjunto de versões. Assim, ele se tornará uma única prova.
   * Se for necessário inserir uma versão entre duas versões existentes, desvincule todas as versões da mesma prova e vincule-as novamente na ordem correta.

## Sobre conjuntos de versões e limites de prova

Cada conjunto de cinco versões contará como uma prova em relação ao limite total de prova.

Por exemplo, se você fizer upload de cinco versões de um design (incluindo a versão original), isso contará como uma prova. Se você fizer upload de seis versões de um design, contará como duas provas. Onze versões contariam como três provas e assim por diante.

Para arquivos audiovisuais, cada nova versão conta como uma nova prova.
