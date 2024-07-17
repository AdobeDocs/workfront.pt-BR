---
content-type: reference
product-previous: workfront-proof
product-area: documents
navigation-topic: organize-your-work-workfront-proof
title: Compreender as Permissões de Pasta em  [!DNL Workfront Proof]
description: Se uma pessoa tiver permissão para ver um item em uma pasta, ela também poderá ver a própria pasta. No entanto, eles podem ver apenas os itens na pasta que foram compartilhados explicitamente com eles.
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 96162fe8-eef9-40f4-bc94-02911b970f02
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 15%

---

# Entender as Permissões de Pasta em [!DNL Workfront Proof]

>[!IMPORTANT]
>
>Este artigo se refere à funcionalidade no produto independente [!DNL Workfront Proof]. Para obter informações sobre provas dentro de [!DNL Adobe Workfront], consulte [Prova](../../../review-and-approve-work/proofing/proofing.md).

Se uma pessoa tiver permissão para ver um item em uma pasta, ela também poderá ver a própria pasta. No entanto, eles podem ver apenas os itens na pasta que foram compartilhados explicitamente com eles.

## Pastas Públicas

Se uma pasta for pública, os usuários na conta (excluindo Observadores e usuários Light) poderão ver o nome da pasta na barra lateral esquerda.

Seu perfil de permissão também afeta os direitos que você tem sobre pastas públicas:

| **Perfil/ Ação** | **Ver todos os itens na pasta** | **Ver itens compartilhados explicitamente com eles** | **Adicionar itens** | **Excluir itens** | **Adicionar subpastas** | **Excluir subpastas** | **Editar detalhes da pasta** |
|---|---|---|---|---|---|---|---|
| **Criador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador de Cobrança** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Supervisor** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Gerente** | Não | Sim | Sim | Não | Sim | Não | Sim |
| **Observador** | Não | Sim | Não | Não | Não | Não | Não |

{style="table-layout:auto"}

Se a pasta pública pertencer a um gerente, ele poderá excluir a pasta raiz e quaisquer subpastas.

Para obter mais informações, consulte [Perfis de permissões de prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md).

## Pastas privadas

Se uma pasta for privada, outros usuários na mesma conta não poderão ver o nome da pasta na barra lateral esquerda, a menos que a pasta ou os itens na pasta tenham sido compartilhados explicitamente com eles ou tenham um perfil de Supervisor, Administrador ou Administrador de Faturamento:

| **Perfil/ Ação** | **Ver todos os itens na pasta** | **Ver itens compartilhados explicitamente com eles** | **Adicionar itens** | **Excluir itens** | **Adicionar subpastas** | **Excluir subpastas** | **Editar detalhes da pasta** |
|---|---|---|---|---|---|---|---|
| **Criador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador de Cobrança** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Administrador** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Supervisor** | Sim | Sim | Sim | Sim | Sim | Sim | Sim |
| **Gerente** | Não | Sim | Não | Não | Não | Não | Não |
| **Observador** | Não | Sim | Não | Não | Não | Não | Não |

{style="table-layout:auto"}

Se, por exemplo, você quiser que o Gerente de projetos e suas equipes vejam apenas pastas específicas, o Gerente de projetos pode configurar uma pasta privada e, em seguida, compartilhar a pasta com usuários específicos.

Ao compartilhar uma pasta privada, você pode decidir se deseja que os gerentes possam criar, editar e excluir itens da pasta.

Você pode definir isso para cada pessoa individualmente na página Nova pasta e alterá-lo na seção [!UICONTROL Compartilhado com] da página Detalhes da pasta. Para obter mais informações, consulte [Criar Pastas [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/create-folders.md) e [Gerenciar Pastas e seus Conteúdos [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/manage-folders-and-contents.md).

Se uma Pasta privada for compartilhada com um Observador ou, ele terá acesso Somente leitura a todos os itens na pasta. Para obter mais informações, consulte [Perfis de Permissões de Prova em [!DNL Workfront Proof]](../../../workfront-proof/wp-acct-admin/account-settings/proof-perm-profiles-in-wp.md) e [Compartilhar Pastas em [!DNL Workfront Proof]](../../../workfront-proof/wp-work-proofsfiles/organize-your-work/share-folders.md).

>[!NOTE]
>
>* Se uma pasta pai for privada, todas as subpastas também serão privadas. Não é possível ter uma subpasta pública em uma pasta primária privada. No entanto, você pode ter uma subpasta privada em uma pasta principal pública.
>* O criador e o proprietário da pasta sempre terão acesso a ela e não serão removíveis.
>* Somente o Criador e o Proprietário da pasta privada podem excluir a pasta.

