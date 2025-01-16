---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-2-0
title: Metadados de conexão no Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: af260c63-3385-4d5c-abc2-d5c23175be40
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Metadados de conexão no Adobe Workfront Fusion

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Metadados de conexão](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/connections/connection-metadata.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requer uma licença [!DNL Adobe Workfront Fusion] além de uma licença [!DNL Adobe Workfront].

Nem todas as conexões são iguais. Entender as diferenças entre conexões é muito importante para conhecer o contexto comercial. O Fusion usa metadados para identificar atributos importantes de uma conexão.

Os metadados de conexão podem ser definidos ao criar uma nova conexão. Esses atributos estão na mesma caixa de diálogo usada para configurar uma conexão:

![Metadados de conexão](assets/connection-metadata-setup.png)

Os usuários do Fusion podem exibir e editar conexões na área Conexões.

![Metadados de conexão na área Conexões](assets/connections-area-metadata.png)

## Tipo de ambiente

As conexões de fusão podem ser usadas por sistemas de produção e não produção. Saber a diferença é muito importante para proteger ambientes de produção. Observe que o tipo de ambiente, assim como outros metadados de conexão, é usado apenas para fins informativos. Os usuários ainda são responsáveis por definir com precisão esse atributo.

## Tipo de autenticação

As conexões de fusão podem ser usadas para contas de serviço e contas pessoais. Contas de serviço são usadas para autenticação quando um cenário é automatizado como Fusion. Contas pessoais são autenticações baseadas em uma pessoa específica. O tipo de autenticação usado depende dos requisitos do cenário. Contas pessoais devem ser usadas para ações automatizadas do usuário. Por exemplo, se um cenário do Fusion automatiza a aprovação por uma pessoa específica, o tipo de autenticação deve ser para essa pessoa. Caso contrário, o Fusion estará agindo como o Fusion e o tipo deverá ser &quot;Conta de Serviço&quot;.

Observe que esse tipo, assim como outros metadados de conexão, é usado apenas para fins informativos. Os usuários ainda são responsáveis por definir com precisão esse atributo manualmente.

Para obter mais informações sobre tipos de autenticação, consulte [Autenticação](https://developer.adobe.com/developer-console/docs/guides/authentication/) no guia de Autenticação do Adobe.
