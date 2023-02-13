---
content-type: reference
product-area: workfront-integrations
keywords: nativo,ootb
navigation-topic: workfront-integrations-navigation-topic
title: Métodos de integração do Adobe Workfront
description: É possível integrar [!DNL Adobe Workfront] com aplicativos de terceiros. Essas integrações podem estender o utilitário de [!DNL Workfront] e adequá-lo às necessidades de sua organização. É possível usar qualquer uma ou todas essas integrações, dependendo do que é mais útil para uma determinada tarefa.
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 685186f76cd89e69eac0a07bff9a39e2e28f9429
workflow-type: tm+mt
source-wordcount: '963'
ht-degree: 0%

---

# Métodos de integração do Adobe Workfront

É possível integrar [!DNL Adobe Workfront] com aplicativos de terceiros. Essas integrações podem estender o utilitário de [!DNL Workfront] e adequá-lo às necessidades de sua organização. É possível usar qualquer uma ou todas essas integrações, dependendo do que é mais útil para uma determinada tarefa.

## Integrações integradas

O Workfront fornece várias integrações que você pode configurar diretamente do Workfront ou de outro aplicativo instalando o complemento Workfront para esse aplicativo. Essas integrações integradas abrangem muitos cenários de casos de uso comuns e se concentram na extensão e na conexão de experiências de usuário para usuários finais.

As integrações integradas da Workfront se concentram principalmente na produtividade pessoal e na colaboração. Essas integrações reduzem as interrupções no fluxo de trabalho de um usuário individual, permitindo que ele receba notificações do Workfront, acesse informações e atue nos itens de trabalho do Workfront sem sair do aplicativo integrado.

As vantagens das integrações integradas podem incluir:

* Muitas dessas integrações integradas estão disponíveis sem custo adicional. (Outros exigem uma compra adicional.)
* As integrações integradas abrangem muitos dos aplicativos mais comuns usados por empresas, como o Slack, [!DNL Google Drive]ou produtos de Adobe, como [!DNL Adobe Creative Cloud] ou [!DNL Adobe Experience Manager] Ativos. Se a empresa já usar esses aplicativos, a integração entrará facilmente no fluxo de trabalho existente dos usuários.
* Integração [!DNL Workfront] com um aplicativo usado frequentemente pode aumentar a adoção entre seus usuários.

>[!INFO]
>
>**Exemplo:**
>
>Com o [!DNL Workfront for Microsoft integration], você pode receber notificações no [!DNL Microsoft Teams] sobre o seu [!DNL Workfront] itens de trabalho. Sem sair [!DNL Microsoft Teams], você pode executar ações como aprovar, comentar ou alterar o status dos itens de trabalho. Quaisquer alterações feitas nos itens de trabalho de [!DNL Microsoft] As equipes refletem em [!DNL Workfront] também.

Para obter mais informações sobre integrações integradas, incluindo uma lista de integrações integradas disponíveis no momento, consulte [[!DNL Adobe Workfront] visão geral de integrações integradas](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## Aplicativos OAuth2 personalizados

Adobe [!DNL Workfront] Os administradores podem criar aplicativos OAuth2 para sua instância de [!DNL Workfront], que permitem que outros aplicativos acessem o Workfront. Seus usuários podem conceder permissão a esses outros aplicativos para acessar seus dados do Workfront. Dessa forma, você pode integrar o Workfront com aplicativos de sua escolha, incluindo seus próprios aplicativos internos.

>[!NOTE]
>
>No contexto do OAuth2, &quot;criar um aplicativo&quot; refere-se ao processo de criação desse tipo de link de acesso entre um aplicativo e um servidor, como o Workfront.

Vantagens de criar um [!UICONTROL OAuth2] O pedido pode incluir:

* Os usuários podem usar essas integrações diretamente em [!DNL Workfront], semelhante às integrações integradas.
* Configurar ou usar um [!UICONTROL OAuth2] não exige conhecimentos técnicos adicionais, como a familiaridade com a [!DNL Workfront] API.
* Sua organização pode usar software que não é oferecido como um [!DNL Workfront] aplicativo integrado. Você ainda pode integrar este software com [!DNL Workfront] usando um [!UICONTROL OAuth2] , mesmo que o software seja proprietário de sua organização.

Para obter mais informações, consulte [Criar aplicativos OAuth2 para integrações do Workfront](../administration-and-setup/configure-integrations/create-oauth-application.md).

## API do Workfront

A Workfront oferece uma API pública (interface de programação de aplicativos) que permite estender e aprimorar sua experiência com o Workfront. O objetivo da API do Workfront é simplificar a criação de suas próprias integrações com o Workfront, introduzindo uma arquitetura REST-ful que opera via HTTP. A API do Workfront requer algum conhecimento técnico, mas é uma ferramenta poderosa para recuperar, criar e modificar dados. Você pode personalizar chamadas de API para executar funções muito específicas.

Além disso, [!DNL Workfront] O oferece uma API de assinatura de evento. Quando uma ação ocorre em uma [!DNL Workfront] objeto compatível com assinaturas de eventos, é possível configurar [!DNL Workfront] para enviar uma resposta ao terminal desejado. Isso significa que aplicativos de terceiros podem receber atualizações de [!DNL Workfront] interações por meio do [!DNL Workfront] A API logo após a ocorrência.

Vantagens de usar o [!DNL Workfront] A API pode incluir:

* Você pode usar o [!DNL Workfront] API para se conectar a quase qualquer outro serviço da Web ou aplicativo que ofereça uma API pública. Por conseguinte, é possível integrar [!DNL Workfront] com praticamente qualquer serviço ou aplicativo da Web que você deseja usar.
* O [!DNL Workfront] A flexibilidade da API também se estende ao software proprietário da sua empresa. Você pode usar e modificar [!DNL Workfront] dados de dentro de seu próprio software.
* Como as APIs são tão comuns ao software, seus desenvolvedores internos provavelmente se familiarizarão com elas. [!DNL Workfront] O usa uma API REST-ful, o tipo mais comum de API, tornando ainda mais fácil para seus desenvolvedores se familiarizarem com a velocidade do .

>[!INFO]
>
>**Exemplo:**
>
>A chamada de API a seguir coloca um comentário no fluxo de atualização da tarefa com a ID especificada.
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

Para obter mais informações sobre o [!DNL Workfront] API, consulte [Noções básicas da API](../wf-api/general/api-basics.md).

Para obter mais informações sobre assinaturas de eventos, consulte [API de assinatura de evento](../wf-api/general/event-subs-api.md).

## Adobe Workfront Fusion

O Workfront Fusion permite automatizar workflows. Com o [!DNL Workfront Fusion for Work Automation and Integration] Você pode criar essas automações em vários aplicativos e serviços da Web, criando cenários em que os aplicativos trabalham juntos para executar uma tarefa. Um cenário é uma representação visual da tarefa ou do fluxo de trabalho que é criado usando módulos, que são tarefas discretas como &quot;Baixar um documento&quot; ou &quot;Criar um projeto&quot;. Conecte módulos para definir o workflow e, em seguida, o workflow é executado automaticamente quando uma condição de disparo é atendida.

Vantagens para [!DNL Workfront Fusion] podem incluir:

* O Workfront Fusion não requer tanto conhecimento técnico quanto a API, pois a interface visual auxilia na compreensão e configuração do workflow. Isso significa que ele pode ser usado por indivíduos fora de uma equipe de desenvolvimento, o que pode economizar tempo e dinheiro em sua organização.
* Since [!DNL Workfront Fusion] O funciona por meio da API do , ele pode acessar a maioria dos aplicativos e serviços da Web. Muitos aplicativos têm módulos para fazer chamadas de API, ou você pode usar os módulos HTTP, SOAP ou JSON para interagir com serviços da Web que não têm um [!DNL Workfront Fusion] conector.

>[!INFO]
>
>**Exemplo:**
>
>O seguinte [!DNL Workfront] módulo em [!DNL Workfront Fusion] é configurada para adicionar um comentário ao projeto selecionado. Após a execução do módulo, o comentário é visível no fluxo de atualização do projeto no Workfront.
>
>![](assets/fusion-example-comment-350x416.png)

Para obter mais informações sobre o Workfront Fusion, consulte [Adobe Workfront Fusion](../workfront-fusion/workfront-fusion-2.md).
