---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Entender as permissões da pasta em [!DNL Workfront Proof]
description: Se uma pessoa tiver permissão para ver um item em uma pasta, ela também poderá ver a própria pasta. No entanto, eles podem ver apenas os itens na pasta que foram explicitamente compartilhados com eles.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 17%

---

# Entender as permissões da pasta em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre prova dentro de [!DNL Adobe Workfront], consulte [Tofing](../../../review-and-approve-work/proofing/proofing.md).

Se uma pessoa tiver permissão para ver um item em uma pasta, ela também poderá ver a própria pasta. No entanto, eles podem ver apenas os itens na pasta que foram explicitamente compartilhados com eles.

## Pastas públicas

Se uma pasta for pública, os usuários na conta (excluindo Observadores e usuários leves) poderão visualizar o nome da pasta na barra lateral esquerda.

O perfil de permissão também afeta os direitos que você tem sobre pastas públicas:

| **Perfil/ Ação** | **Ver todos os itens na pasta** | **Veja os itens compartilhados explicitamente com eles** | **Adicionar itens** | **Excluir itens** | **Adicionar subpastas** | **Excluir subpastas** | **Editar detalhes da pasta** |
|---|---|---|---|---|---|---|---|
| **Criador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador de Faturamento** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Supervisor** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Gerente** | não | Sim | Sim | não | Sim | não | Sim |
| **Observador** | não | Sim | não | não | não | não | não |

{style=&quot;table-layout:auto&quot;}

Se a pasta pública for de propriedade de um gerente, ele poderá excluir a pasta raiz e qualquer subpasta.

Para obter mais informações, consulte [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Pastas privadas

Se uma pasta for privada, outros usuários na mesma conta não poderão visualizar o nome da pasta na barra lateral esquerda, a menos que a pasta ou os itens na pasta tenham sido compartilhados explicitamente com eles ou tenham um perfil de Supervisor, Administrador ou Administrador de Faturamento:

| **Perfil/ Ação** | **Ver todos os itens na pasta** | **Veja os itens compartilhados explicitamente com eles** | **Adicionar itens** | **Excluir itens** | **Adicionar subpastas** | **Excluir subpastas** | **Editar detalhes da pasta** |
|---|---|---|---|---|---|---|---|
| **Criador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador de Faturamento** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Supervisor** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Gerente** | não | Sim | não | não | não | não | não |
| **Observador** | não | Sim | não | não | não | não | não |

{style=&quot;table-layout:auto&quot;}

Por exemplo, se você quiser que seu Gerenciador de projetos e suas equipes vejam apenas pastas específicas, ele poderá configurar uma pasta privada e compartilhar a pasta com usuários específicos.

Ao compartilhar uma pasta privada, você pode decidir se deseja que os Gerentes possam criar, editar e excluir itens de pasta.

Você pode definir isso para cada pessoa individualmente na página Nova pasta e alterá-lo no [!UICONTROL Compartilhado com] da página Detalhes da pasta . Para obter mais informações, consulte [Criar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) e [Gerenciar pastas e seu conteúdo em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Se uma pasta Privada for compartilhada com um ou Observador, ele terá acesso Somente leitura a todos os itens na pasta. Para obter mais informações, consulte [Perfis de prova de permissões em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Compartilhar pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Se uma pasta pai for privada, todas as subpastas também serão privadas. Não é possível ter uma subpasta pública em uma pasta pai privada. No entanto, você pode ter uma subpasta privada em uma pasta pai pública.
>* O Criador e o Proprietário da pasta sempre terão acesso a ela e não serão removíveis.
>* Somente o Criador e o Proprietário da pasta privada podem excluir a pasta.


