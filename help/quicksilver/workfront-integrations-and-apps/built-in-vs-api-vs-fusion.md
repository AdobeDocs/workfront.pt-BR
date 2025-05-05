---
content-type: reference
product-area: workfront-integrations
keywords: nativo,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Métodos de integração do Adobe Workfront
description: Você pode integrar o [!DNL Adobe Workfront] com aplicativos de terceiros. Essas integrações podem estender a utilidade do  [!DNL Workfront]  e adaptá-lo às necessidades da sua organização. É possível usar qualquer uma ou todas essas integrações, dependendo do que for mais útil para uma determinada tarefa.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Métodos de integração do Adobe Workfront

Você pode integrar o [!DNL Adobe Workfront] a aplicativos de terceiros, bem como outros produtos do [!DNL Adobe]. Essas integrações podem estender a utilidade do [!DNL Workfront] e personalizá-lo de acordo com as necessidades da sua organização. É possível usar qualquer uma ou todas essas integrações, dependendo do que for mais útil para uma determinada tarefa.

## Integrações integradas

O Workfront fornece várias integrações que você pode configurar diretamente do Workfront ou de outro aplicativo instalando o suplemento do Workfront para esse aplicativo. Essas integrações integradas abordam muitos cenários de casos de uso comuns e se concentram na extensão e conexão das experiências do usuário para usuários finais.

As integrações integradas do Workfront se concentram principalmente na produtividade e colaboração pessoais. Essas integrações reduzem as interrupções no fluxo de trabalho de um usuário individual, permitindo que ele receba notificações do Workfront, acesse informações e atue em itens de trabalho do Workfront sem sair do aplicativo integrado.

As vantagens das integrações integradas podem incluir o seguinte:

* Muitas dessas integrações integradas estão disponíveis sem custo adicional. (Outros exigem uma compra adicional.)
* As integrações internas abrangem muitos dos aplicativos mais comuns usados por empresas, como os produtos [!DNL Slack], [!DNL Google Drive] ou [!DNL Adobe], como o Assets [!DNL Adobe Creative Cloud] ou [!DNL Adobe Experience Manager]. Se sua empresa já usa esses aplicativos, a integração transita sem problemas para o fluxo de trabalho existente dos usuários.
* Integrar o [!DNL Workfront] com um aplicativo usado com frequência pode aumentar a adoção entre os usuários.

>[!INFO]
>
>**Exemplo:**
>
>Com o [!DNL Workfront for Microsoft Teams integration], você pode receber notificações em [!DNL Microsoft Teams] sobre seus itens de trabalho [!DNL Workfront]. Sem sair de [!DNL Microsoft Teams], você pode executar ações como aprovar, comentar ou alterar o status de itens de trabalho. Quaisquer alterações feitas em itens de trabalho de [!DNL Microsoft Teams] também serão refletidas em [!DNL Workfront].

Para obter mais informações sobre integrações internas, incluindo uma lista das integrações internas disponíveis no momento, consulte [[!DNL Adobe Workfront] visão geral das integrações internas](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Aplicativos OAuth2 personalizados

Os administradores do Adobe [!DNL Workfront] podem criar aplicativos OAuth2 para a sua instância do [!DNL Workfront], que permitem que outros aplicativos acessem o [!DNL Workfront]. Seus usuários podem conceder permissão a esses outros aplicativos para acessar os dados do [!DNL Workfront]. Dessa forma, você pode integrar o Workfront com os aplicativos de sua escolha, incluindo seus próprios aplicativos internos.

>[!NOTE]
>
>No contexto do OAuth2, &quot;criação de um aplicativo&quot; refere-se ao processo de criação desse tipo de link de acesso entre um aplicativo e um servidor, como o Workfront.

As vantagens de criar um aplicativo [!UICONTROL OAuth2] podem incluir o seguinte:

* Os usuários podem usar essas integrações diretamente no [!DNL Workfront], de modo semelhante às integrações integradas.
* Configurar ou usar um aplicativo [!UICONTROL OAuth2] não requer conhecimento técnico adicional, como familiaridade com a API [!DNL Workfront].
* Sua organização pode usar um software que não é oferecido como um aplicativo interno do [!DNL Workfront]. Você ainda pode integrar este software com o [!DNL Workfront] usando um aplicativo do [!UICONTROL OAuth2], mesmo que o software seja proprietário da sua organização.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## API [!DNL Workfront]

O [!DNL Workfront] oferece uma API pública (interface de programação de aplicativos) que permite estender e aprimorar sua experiência com o Workfront. O objetivo da API [!DNL Workfront] é simplificar a criação de suas próprias integrações com o [!DNL Workfront], introduzindo uma arquitetura REST-ful que opera via HTTP. A API [!DNL Workfront] exige conhecimento técnico, mas é uma ferramenta muito poderosa para recuperar, criar e modificar dados. Você pode personalizar chamadas de API para executar funções muito específicas.

Além disso, o [!DNL Workfront] oferece uma API de Assinatura de Evento. Quando ocorrer uma ação em um objeto [!DNL Workfront] com suporte em assinaturas de evento, você poderá configurar o [!DNL Workfront] para enviar uma resposta ao ponto de extremidade desejado. Isso significa que aplicativos de terceiros podem receber atualizações das interações [!DNL Workfront] por meio da API [!DNL Workfront] logo após ocorrerem.

As vantagens de usar a API [!DNL Workfront] podem incluir o seguinte:

* Você pode usar a API [!DNL Workfront] para se conectar a quase qualquer outro serviço ou aplicativo da Web que ofereça uma API pública. Portanto, é possível integrar o [!DNL Workfront] a quase qualquer serviço ou aplicativo da Web que você deseje usar.
* A flexibilidade da API [!DNL Workfront] também se estende ao software proprietário da sua empresa. Você pode usar e modificar os dados do [!DNL Workfront] de dentro do seu próprio software.
* Como as APIs são muito comuns ao software, os desenvolvedores internos provavelmente estão familiarizados com elas. O [!DNL Workfront] usa uma API REST-ful, o tipo mais comum de API, tornando ainda mais fácil para os seus desenvolvedores atualizarem rapidamente.

>[!INFO]
>
>**Exemplo:**
>
>A chamada de API a seguir coloca um comentário no fluxo de atualização da tarefa com a ID especificada.
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Para obter mais informações sobre a API [!DNL Workfront], consulte [noções básicas da API](../wf-api/general/api-basics.md).

Para obter mais informações sobre assinaturas de evento, consulte [API de Assinatura de Evento](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] permite automatizar fluxos de trabalho. Com a licença do [!DNL Workfront Fusion for Work Automation and Integration], você pode criar essas automações em vários aplicativos e serviços Web, criando cenários em que os aplicativos trabalham juntos para executar uma tarefa. Um cenário é uma representação visual da tarefa ou do fluxo de trabalho criado por meio de módulos, que são tarefas distintas, como &quot;Baixar um documento&quot; ou &quot;Criar um projeto&quot;. Os módulos são encadeados para definir o fluxo de trabalho, que é executado automaticamente quando uma condição de acionador é atendida.

As vantagens do [!DNL Workfront Fusion] podem incluir:

* [!DNL Workfront Fusion] não requer tanto conhecimento técnico quanto a API porque a interface visual auxilia na compreensão e configuração do fluxo de trabalho. Isso significa que ele pode ser usado por indivíduos fora de uma equipe de desenvolvimento, o que pode economizar tempo e dinheiro da organização.
* Como o [!DNL Workfront Fusion] funciona por meio da API, ele pode acessar a maioria dos aplicativos e serviços Web. Muitos aplicativos têm módulos para fazer chamadas de API ou você pode usar os módulos HTTP, SOAP ou JSON para interagir com serviços Web que não têm um conector [!DNL Workfront Fusion] dedicado.

>[!INFO]
>
>**Exemplo:**
>
>O seguinte módulo [!DNL Workfront] em [!DNL Workfront Fusion] está configurado para adicionar um comentário ao projeto selecionado. Depois que o módulo é executado, o comentário fica visível no fluxo de atualização do projeto no Workfront.
>
>![Exemplo: Adicionando um comentário no Fusion](assets/fusion-example-comment-350x416.png)

Para obter mais informações sobre [!DNL Workfront Fusion], consulte [[!DNL Adobe Workfront Fusion]](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/home).
