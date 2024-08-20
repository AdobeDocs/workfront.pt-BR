---
title: Visão Geral dos Tipos de Registro Conectados
description: Uma maneira de indicar como os tipos de registro individuais se relacionam entre si é conectá-los. Além disso, é possível conectar tipos de registro do Adobe Workfront Planning a tipos de objeto de outros aplicativos para aprimorar a experiência dos usuários e manter o foco em um aplicativo.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ded6db27fa3fba9195e2133134f60bcadb0f897a
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Visão geral dos tipos de registro conectados

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

Você pode indicar que os tipos de registro individuais se relacionam entre si ou com objetos de outros aplicativos, conectando-os.

Este artigo é uma visão geral das conexões de tipo de registro e descreve os tipos de conexões que você pode estabelecer entre tipos de registro e de objeto.

Para obter informações sobre como conectar tipos de registro, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

## Considerações sobre a conexão de tipos de registro

Há duas etapas para conexões no Workfront Planning:

1. Primeiro, você deve estabelecer uma conexão entre dois tipos de registro ou um tipo de registro e um tipo de objeto de outro aplicativo. Para obter informações sobre como você pode conectar tipos de registro, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).
1. Em segundo lugar, você pode conectar registros individuais de um tipo com registros de outro tipo depois que os dois tipos de registros estiverem conectados. Para obter informações sobre como conectar registros, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

Considere o seguinte sobre a conexão de tipos de registro:

* Você pode conectar as seguintes entidades no Adobe Workfront Planning:

   * Dois tipos de registro.

     Por padrão, você pode conectar dois tipos de registro do mesmo espaço de trabalho. Você também pode configurar tipos de registro para se conectar com tipos de registro de outros espaços de trabalho. Para obter informações, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).
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
     >Todos os usuários com permissões de Exibição ou superiores para o espaço de trabalho podem exibir as informações nos campos de pesquisa, independentemente de suas permissões ou nível de acesso na aplicação dos tipos de objeto vinculados ou suas permissões em outros espaços de trabalho.

     Os campos de registro vinculados são precedidos por um ícone de relação ![](assets/relationship-field-icon.png).

     Os campos vinculados são precedidos por um ícone que identifica o tipo de campo. Por exemplo, campos vinculados (ou de pesquisa) são precedidos por ícones que indicam que um campo é um número, um parágrafo ou uma data.

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and AEM assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you select the many-to-many connection type between record types, you can later connect many records with multiple records you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can connect several campaigns with multiple projects. You can also connect the same projects you are connecting to the campaigns to more than one campaign. 

A real-life example of a many-to-many relationship type is the relationship between customers and products: customers can purchase multiple products; and those products can also be purchased by many other customers. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)

When you select the one-to-many connection type between record types, you can later connect one record with multiple records you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with multiple projects. But one of the projects you're connecting to the campaigns can be connected only to one campaign at a time. 

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 
 
### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)

When you select the many-to-one connection type between record types, you can later connect many records with only one record you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you select the one-to-one connection type between record types, you can later connect one record with one other record that you're connecting to. 

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



