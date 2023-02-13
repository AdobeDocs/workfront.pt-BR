---
product-previous: workfront-proof
product-area: documents
navigation-topic: manage-your-work-workfront-proof
title: Gerenciamento de versões de prova em [!DNL Workfront Proof]
description: O gerenciamento de feedback em várias versões ou revisões de um trabalho pode ser um grande desafio. [!DNL Workfront Proof] O simplifica esse processo, permitindo que você crie e compare várias versões de uma prova.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: d1bee64d-c091-40d3-a9c1-847c7f645b96
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 0%

---

# Gerenciamento de versões de prova em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

O gerenciamento de feedback em várias versões ou revisões de um trabalho pode ser um grande desafio. [!DNL Workfront Proof] O simplifica esse processo, permitindo que você crie e compare várias versões de uma prova.

Não há limite para o número de versões de uma prova que você pode criar. Portanto, se você precisar passar por muitas revisões com um cliente para obter uma aprovação final, todas as versões criadas podem ser visualizadas e facilmente gerenciadas dentro do [!DNL Workfront Proof].

As permissões são específicas de uma versão, portanto, você pode conceder a uma pessoa permissão para ver uma versão, mas não outra. Por outro lado, se você compartilhar uma versão posterior com uma pessoa, ela não poderá ver as versões anteriores, a menos que você volte e as adicione explicitamente a essas versões anteriores também.

Para criar uma nova versão de uma prova, você deve ter direitos de edição na prova.

Consulte [Gerenciar funções de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/share-proofs-and-files/manage-proof-roles.md) para obter mais informações sobre quem tem direitos de edição em uma prova. Consulte para saber mais sobre como criar versões.

## Exibição de versões de prova no visualizador de prova

O nome completo da versão que você está visualizando é exibido na parte superior esquerda do visualizador de prova. Qualquer outra versão da prova será exibida somente como números de versão.

1. Abra uma prova no visualizador de prova, conforme descrito em [Abrir uma prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/open-proof.md).
1. No visualizador de prova, clique no número da versão à direita do nome da prova.
1. Para exibir a outra versão, clique no nome no menu exibido ao clicar no número da versão.
1. Para comparar duas versões, clique no botão **[!UICONTROL Comparar provas]** ícone .\
   ![Comparar_provas_button.png](assets/compare-proofs-button.png)\
   Se houver várias versões da prova, você poderá selecionar duas versões que deseja comparar clicando no número da versão relevante em cada lado da tela de divisão do modo de comparação.

Para obter informações sobre como revisar provas em um visualizador de prova, consulte [Revisar uma prova](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-a-proof.md).

## Acessar versões de prova por meio da página Detalhes da prova

Você pode acessar todas as versões de uma prova na página Detalhes da prova .

1. Abra a página Detalhes da prova para obter uma prova, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Clique na guia das guias de versão na parte superior da página e clique em **[!UICONTROL Ir para prova]** para abrir a versão desejada no visualizador de prova.\
   ![Version_tabs_on_Proof_Details_page.png](assets/version-tabs-on-proof-details-page-350x205.png)

## Vincular versões de prova

Se sua prova tiver várias versões, a versão anterior da prova será comumente conhecida como prova principal.

Se você quiser alterar a prova principal (versão anterior) para outra prova em sua conta ou conectar uma única prova a outra prova em sua conta (como uma nova versão da outra prova), poderá fazer isso facilmente seguindo estas etapas:

1. Abra a página Detalhes da prova para obter uma prova, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Alterar versão anterior]**.

1. No **[!UICONTROL Alterar versão anterior]** for exibida, selecione a prova que deseja definir como a prova principal (versão anterior).\
   Se você precisar de ajuda para encontrar a prova na lista, é possível classificar as colunas clicando no cabeçalho da coluna.

1. Clique em **[!UICONTROL Alterar versão anterior]** na parte inferior da caixa para conectar versões.

>[!NOTE]
>
>Ao conectar uma prova a outra prova em sua conta (como uma nova versão), [!DNL Workfront Proof] bloqueia a prova que agora é a versão anterior.

## Desvinculação de versões de prova

Você pode desvincular a prova que está visualizando no momento de sua prova principal (versão anterior) sem vinculá-la a outra prova em sua conta:

1. Abra a página Detalhes da prova para obter uma prova, conforme descrito em [Gerenciar detalhes de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/manage-proof-details.md).
1. Clique em **[!UICONTROL Mais]** > **[!UICONTROL Remover link para a versão anterior]**.

   * Somente a última versão pode ser desvinculada (desconectada) do conjunto inteiro de versões. Depois, tornar-se-á uma prova única.
   * Se você precisar inserir uma versão entre duas versões existentes, poderá desvincular todas as versões da mesma prova e vinculá-las novamente na ordem correta.

## Sobre conjuntos de versões e limites de prova

Cada conjunto de cinco versões contará como uma prova em relação ao limite total de prova.

Por exemplo, se você carregar cinco versões de um design (incluindo a versão original), isso será contado como uma prova. Se você carregar seis versões de um design, isso será contado como duas provas. Onze versões contariam como três provas e assim por diante.

Para arquivos visuais de áudio, cada nova versão conta como uma nova prova.
