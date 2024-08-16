---
title: Visão Geral dos Tipos de Registro Conectados
description: Uma maneira de indicar como os tipos de registro individuais se relacionam entre si é conectá-los. Além disso, é possível conectar tipos de registro do Adobe Workfront Planning a tipos de objeto de outros aplicativos para aprimorar a experiência dos usuários e manter o foco em um aplicativo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d56a4721353f8b7db856eab5a3ae3b53396bd079
workflow-type: tm+mt
source-wordcount: '1086'
ht-degree: 1%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Visão geral dos tipos de registro conectados

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

Você pode indicar que os tipos de registro individuais se relacionam entre si ou com objetos de outros aplicativos, conectando-os.

Este artigo é uma visão geral das conexões de tipo de registro e descreve os tipos de conexões que você pode estabelecer entre tipos de registro e de objeto.

Para obter informações sobre como conectar tipos de registro, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

## Considerações sobre a conexão de tipos de registro

* Você pode conectar as seguintes entidades no Adobe Workfront Planning:

   * Dois tipos de registro.

     Por padrão, você pode conectar dois tipos de registro do mesmo espaço de trabalho. Você também pode configurar tipos de registro para se conectar com tipos de registro de outros espaços de trabalho.
   * Um tipo de registro e um tipo de objeto de outro aplicativo.

* Você pode conectar tipos de registro do Workfront Planning com os seguintes tipos de objeto dos seguintes aplicativos:

   * Adobe Workfront:

      * Projetos
      * Portfólios
      * Programas
      * Empresas
      * Grupos

   * Adobe Experience Manager Assets:

      * Imagens
      * Pastas

     >[!IMPORTANT]
     >
     >Você deve ter uma licença do Adobe Experience Manager Assets e a instância da Workfront de sua organização deve ser integrada à Plataforma de negócios Adobe ou à Adobe Admin Console para conectar os registros do Workfront Planning à Adobe Experience Manager Assets.
     >
     >Em caso de dúvidas sobre a integração com a Adobe Admin Console, consulte as [Perguntas frequentes sobre a Experiência unificada do Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Depois de criar registros individuais para um tipo de registro, você pode selecionar os registros aos quais se conectar no campo Tipo de registro vinculado. Para obter informações, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Depois de conectar um tipo de registro com outro tipo de registro ou com um tipo de objeto de outro aplicativo, existem os seguintes cenários:

   * **Quando você conecta dois tipos de registro**: um campo de registro vinculado é criado no tipo de registro ao qual você está se conectando. Um campo de registro vinculado semelhante é criado no tipo de registro ao qual você está se conectando.

     Por exemplo, se você conectar o tipo de registro &quot;Campanha&quot; ao tipo de registro &quot;Produto&quot;, um campo de registro vinculado chamado &quot;Produto vinculado&quot; será criado no tipo de registro Campanha. Um tipo de registro vinculado chamado automaticamente de &quot;Campanha&quot; é criado no tipo de registro Produto.

   * **Ao conectar um tipo de registro com um tipo de objeto de outro aplicativo**:

      * Um campo de registro vinculado é criado no tipo de registro ao qual você está se conectando. Nenhum campo de registro vinculado é criado automaticamente no tipo de objeto do outro aplicativo.

      * Os campos de registros de planejamento não podem ser acessados de objetos do Workfront.
      * Os campos de registro do Planning podem ser acessados de ativos do Experience Manager quando o administrador do Workfront configura o mapeamento de metadados por meio da integração entre o Workfront e o Adobe Experience Manager Assets. Para obter mais informações, consulte [Configurar o mapeamento de metadados de ativos entre o Adobe Workfront e o Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

   * **Ao adicionar campos vinculados (ou de pesquisa) a partir do registro ou objeto ao qual você se conecta**: além de criar um campo de registro vinculado, você também pode se conectar a campos do registro ou tipo de objeto conectado que são chamados de campos de pesquisa. Um campo vinculado (ou de pesquisa) com informações do registro ao qual você está se conectando é exibido no registro do qual você está se conectando.

     Você pode conectar campos de outros tipos de registro ou objetos de outro aplicativo ao tipo de registro do Workfront Planning.

     Os campos vinculados são somente leitura e exibem automaticamente informações de registros ou objetos conectados quando você os conecta ou aos objetos.

     Você pode fazer referência a campos de pesquisa de outros tipos de registro ou objeto em fórmulas, filtros ou agrupamentos.

     Por exemplo, se você conectar o tipo de registro &quot;Campanha&quot; com um projeto do Workfront e selecionar trazer o campo Data de conclusão planejada do projeto para o registro do Workfront Planning, um campo vinculado chamado Data de conclusão planejada (do projeto) será criado automaticamente para a campanha. Não é possível editar manualmente esse campo vinculado. O campo Data de conclusão planejada (do projeto) exibe a Data de conclusão planejada dos projetos vinculados.

     >[!IMPORTANT]
     >
     >Todos os usuários com permissões de Exibição ou superiores ao espaço de trabalho podem exibir as informações nos campos de pesquisa, independentemente de suas permissões ou nível de acesso no aplicativo dos tipos de objeto vinculados <!--or their permissions in other workspaces-->.

<!--see the commented out text above for the release of cross-workspace connections-->

* Os campos de registro vinculados são precedidos por um ícone de relação ![](assets/relationship-field-icon.png).

  Os campos vinculados são precedidos por um ícone que identifica o tipo de campo. Por exemplo, campos vinculados (ou de pesquisa) são precedidos por ícones que indicam que um campo é um número, um parágrafo ou uma data.


## Tipos de conexão

Depois de estabelecer uma conexão entre dois tipos de registro ou entre um registro e um tipo de objeto de outro aplicativo, você pode adicionar registros nos campos de registro conectado.

Dependendo de quantos registros você pode adicionar a um campo de registro conectado, os seguintes tipos de conexão que você pode escolher ao conectar tipos de registro:

* [Um para muitos](#one-to-many-connection-type)
* [Um para um](#many-to-one-connection-type)
* [Muitos para um](#many-to-one-connection-type)
* [Muitos para muitos](#many-to-many-connection-type)

>[!WARNING]
>
>Essas opções não estão disponíveis ao conectar o seguinte:
>* Dois registros de espaços de trabalho diferentes
>
>* Um tipo de registro e ativos AEM


<!-- add screen shots for each type of connection below-->

### Tipo de conexão um para muitos

![](assets/one-to-many-connection-picker.png)

Ao selecionar o tipo de conexão um para muitos entre os tipos de registro, você pode conectar um registro com vários registros aos quais está se conectando.

Por exemplo, se você conectar campanhas a projetos, será possível conectar uma campanha a vários projetos. Mas um projeto pode ser conectado somente a uma campanha.

Ao selecionar esse tipo de conexão, você poderá alterá-lo posteriormente somente para um tipo de conexão muitos para muitos.

### Tipo de conexão um para um

![](assets/one-to-one-connection-picker.png)

Ao selecionar o tipo de conexão um para um entre os tipos de registro, você pode conectar um registro a outro registro ao qual está se conectando posteriormente.

Por exemplo, se você conectar campanhas a projetos, será possível conectar uma campanha a um projeto. Um projeto pode ser conectado somente a uma campanha.

Ao selecionar esse tipo de conexão, você pode alterá-lo posteriormente para qualquer outro tipo.

### Tipo de conexão muitos para um

![](assets/many-to-one-connection-picker.png)

Ao selecionar o tipo de conexão muitos para um entre os tipos de registro, você pode conectar muitos registros posteriormente com apenas um registro ao qual está se conectando.

Por exemplo, se você conectar campanhas a projetos, será possível conectar várias campanhas a um único projeto. Um projeto pode ser conectado a várias campanhas.

Ao selecionar esse tipo de conexão, você poderá alterá-lo posteriormente somente para um tipo de conexão muitos para muitos.

### Tipo de conexão muitos para muitos

![](assets/many-to-many-connection-picker.png)

Ao selecionar o tipo de conexão muitos para muitos entre os tipos de registro, você pode conectar muitos registros com vários registros aos quais está se conectando.

Por exemplo, se você conectar campanhas a projetos, será possível conectar várias campanhas a vários projetos. Você também pode conectar vários projetos a várias campanhas.

Ao selecionar esse tipo de conexão, você não pode alterar o tipo de conexão depois de salvá-lo.

