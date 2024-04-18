---
product-area: documents
navigation-topic: approvals
title: AppBuilder nos Detalhes do documento do Workfront
description: Você pode instalar o AppBuilder nos Detalhes do documento
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
source-git-commit: 0d9212f0719535f191e61d27a73b8f5b2ef5fb30
workflow-type: tm+mt
source-wordcount: '1186'
ht-degree: 0%

---


# AppBuilder nos Detalhes do documento do Workfront

Você pode instalar o AppBuilder em Detalhes do documento.

## Pré-requisitos

Você deve ter o seguinte:

* Uma conta do Workfront habilitada para IMS
* Uma máquina dev com nó v18 e npm

## Adicionar desenvolvedores ao Admin Console

>[!IMPORTANT]
>
>Verifique se você selecionou a organização IMS correta para todas as etapas a seguir. Se você pertencer a várias organizações, é possível selecionar a errada. Verifique se você está agindo na organização correta, que geralmente está listada no canto superior direito.


1. Navegue até uma das seguintes opções:

* Estágio: [https://stage.adminconsole.adobe.com/](https://stage.adminconsole.adobe.com/)
* Produção: [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/)

1. Na seção Usuários, clique em **Desenvolvedores** > **Adicionar desenvolvedores**.

   ![](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >Se não vir uma opção para gerenciar desenvolvedores, você não tem um produto que permita o acesso de desenvolvimento. A Workfront não fornece acesso de desenvolvedor, mas o AEM oferece. Se você não vir isso, precisaremos descobrir como incluir o Workfront na lista de aplicativos que permite desenvolvedores.

1. Adicione o email do usuário. Ele deve pesquisar usuários existentes que já foram adicionados no Admin Console.

1. Adicione os produtos necessários ao perfil do desenvolvedor e clique em **Salvar**.

![](assets/add-developer.png)

## Obter acesso ao AppBuilder

As organizações precisam trabalhar com os gerentes de conta para comprar o AppBuilder. O processo exato para isso não é compreendido porque não precisamos fazer isso para a POC.

Se quiser testar a integração do AppBuilder, solicite uma avaliação gratuita para sua organização IMS aqui:
[https://developer.adobe.com/app-builder/trial/#](https://developer.adobe.com/app-builder/trial/#)

Tenho a impressão de que, embora seja um julgamento gratuito de 30 dias, eles não desativarão o julgamento depois desse período.

Se o AppBuilder estiver configurado corretamente, você deverá ver &quot;Criar projeto a partir do modelo&quot; como parte da criação de um novo projeto (que é abordado na próxima seção).

## Criar um novo projeto no Dev Console

1. Clique em **Criar projeto a partir de modelo**.

   >[!IMPORTANT]
   >
   >Se não vir essa opção, você está configurado incorretamente no Admin Console e não tem acesso ao catálogo do App Builder. Essa opção é exibida somente quando você tem acesso ao AppBuilder.

   ![](assets/create-from-template.png)

1. Selecionar **Construtor de aplicativos**.

1. Insira um **Título do projeto** e **Nome do aplicativo**. Ambos têm padrões, mas será mais fácil identificar o Projeto que você deseja mais tarde, se você personalizar o valor.

   >[!NOTE]
   >
   >Há uma opção para adicionar espaços de trabalho adicionais nesta etapa. Foi sugerido que criássemos um espaço de trabalho para cada desenvolvedor. Isso mantém os segredos e as implantações separadas umas das outras à medida que os devs funcionam. Você deve nomear o espaço de trabalho com o nome do desenvolvedor que o utiliza. A interface AIO tem opções para alternar o espaço de trabalho, que abordaremos mais tarde.


1. Sair **Incluir tempo de execução** selecionado. Eu não sei porque, realmente, mas não mude!

1. Clique em **Salvar**.

## CLI do Adobe IO (aio)

O Adobe fornece uma CLI de código aberto que pode ser usada para ajudar a criar os aplicativos do App Builder. A documentação pode ser encontrada aqui: [https://github.com/adobe/aio-cli](https://github.com/adobe/aio-cli) e também Instruções do Construtor de aplicativos Adobe [https://developer.adobe.com/app-builder/docs/getting_started/first_app/](https://developer.adobe.com/app-builder/docs/getting_started/first_app/).

1. Instalação
   1. Para instalar a ferramenta (verifique se você está no nó v18 primeiro), execute: `npm install -g @adobe/aio-cli `.

1. Autenticar no Terminal
   1. Inicie o terminal e faça logon na AIO com o comando: `aio login`.

1. Inicializar seu aplicativo
   1. Comece a configurar seu aplicativo executando: `aio app init example-app`.

1. Seleção da configuração
   1. Continue para selecionar sua Organização e Projeto a partir das opções fornecidas.\
      ![](assets/select-org.png)
      ![](assets/select-project.png)

1. Seleção e configuração de modelo
   1. Procure todos os modelos disponíveis e escolha a **@adobe/aem-cf-editor-ui-ext-tpl** para o seu projeto.
      ![](assets/search-template.png)
      ![](assets/select-template.png)

1. Definir A Extensão
   1. Nomeie sua extensão.
   1. Forneça um resumo descritivo da funcionalidade da sua extensão.
   1. Selecione um número de versão inicial para começar.
   1. Confirme a conclusão selecionando **Terminei**.
      ![](assets/define-extension.png)

1. Navegue até a pasta do projeto
   1. Acessar a pasta src
   1. Renomear a pasta `aem-cf-editor-1` para `workfront-doc-details-1`.

1. Modificar arquivos de configuração
   1. Abrir app.config.yaml
   1. Atualizar a linha de `aem/cf-editor/1` para `workfront/doc-details/1`.
   1. Ajustar o caminho de inclusão de `src/aem-cf-editor-1/ext.config.yaml` para `src/workfront-doc-details-1/ext.config.yaml`.

1. Editar o componente de registro de extensão
   1. Abertura `src/workfront-doc-details-1/web-src/src/components/ExtensionRegistration.js`.
   1. Na seção de métodos, adicione uma função `secondaryNav` que contém uma função assíncrona `getButtons`.
   1. `getButtons` O deve receber um objeto com a seguinte estrutura:

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Essa função retorna uma matriz de objetos de botão que aparecerão na navegação:

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Configurar Roteamento de Aplicativo
   1. Abra o arquivo App.js e configure as rotas para incluir as funcionalidades recém-desenvolvidas. Será necessário configurar rotas para a exibição padrão e quaisquer exibições adicionais, como a página de revisão. Veja como você pode definir essas rotas:

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Detalhes do documento de acesso
   1. Implementar a função fornecida `document.getDocumentDetails` no aplicativo para buscar informações essenciais do documento. Esta função recupera um objeto que contém `docId` e `docvId`, juntamente com um `sharedContext` objeto com `hostname`, `protocol`e detalhes de autenticação. Certifique-se de que o aplicativo manipule esses dados adequadamente.

1. Integre a busca de dados em seus componentes
   1. Adicione um novo componente à pasta de componentes do aplicativo. Nesse componente, estabeleça uma conexão com o Workfront para recuperar informações de documentos e dados de autenticação usando a conexão estabelecida com o aplicativo host. Este é um exemplo de como você pode estruturar seu componente para lidar com isso:

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Configuração de projetos AIO existentes

1. Atualizar arquivos de configuração
   1. Abertura `app.config.yaml`.
   1. Modifique a configuração atualizando a referência de `aem/cf-editor/1` para `workfront/doc-details/1`. Esse ajuste alinha os caminhos do arquivo com a estrutura do projeto atual.

1. Revise o componente de Registro de extensão
   1. Localize e abra o arquivo chamado `ExtensionRegistration.js`.
   1. Na seção de métodos, adicione uma função `secondaryNav` que contém uma função assíncrona `getButtons`.
   1. `getButtons` O deve receber um objeto com a seguinte estrutura:

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. Essa função retorna uma matriz de objetos de botão que aparecerão na navegação:

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. Configurar Roteamento de Aplicativo
   1. Abra o `App.js`arquive e configure as rotas para incluir as funcionalidades recém-desenvolvidas. Será necessário configurar rotas para a exibição padrão e quaisquer exibições adicionais, como a página de revisão. Veja como você pode definir essas rotas:

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. Detalhes do documento de acesso
   1. Implementar a função fornecida `document.getDocumentDetails` no aplicativo para buscar informações essenciais do documento. Esta função recupera um objeto que contém `docId` e `docvId`, juntamente com um `sharedContext` objeto com `hostname`, `protocol`e detalhes de autenticação. Certifique-se de que o aplicativo manipule esses dados adequadamente.

1. Integre a busca de dados em seus componentes
   1. Adicione um novo componente à pasta de componentes do aplicativo. Nesse componente, estabeleça uma conexão com o Workfront para recuperar informações de documentos e dados de autenticação usando a conexão estabelecida com o aplicativo host. Este é um exemplo de como você pode estruturar seu componente para lidar com isso:

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## Publicar aplicativos

>[!IMPORTANT]
>
>Verifique se você selecionou a Organização IMS correta para cada uma das etapas a seguir.

Para ter um aplicativo convidado carregado no Workfront, o aplicativo precisa ser enviado para o espaço de trabalho Produção e enviado para aprovação.

1. Implante o aplicativo no espaço de trabalho de produção
   1. `aio app use -w Production `
   1. `aio app deploy `

1. Navegue até [https://developer-stage.adobe.com/](https://developer-stage.adobe.com/) ou [https://developer.adobe.com/](https://developer.adobe.com/).
   1. Clique em **Console** no canto superior direito.

1. Localize o projeto usado para criar o aplicativo AppBuilder.

1. Selecione o Espaço de trabalho de produção.
   ![](assets/find-application.png)

1. Envie a solicitação para revisão privada (você receberá avisos de que não estamos publicando no aplicativo exchange marketplace, o que é normal).

1. Preencha o formulário (título, descrição, ícone e nota ao revisor).
   ![](assets/submission-details.png)

>[!IMPORTANT]
>
>Depois de enviado, um administrador do sistema da organização precisará aprovar o envio.

## Aprovar o envio

1. Como administrador do sistema, navegue até [https://stage.exchange.adobe.com/](https://stage.exchange.adobe.com/) ou [https://exchange.adobe.com/](https://exchange.adobe.com/).

1. Clique em **Gerenciar** > **Aplicativos Experience Cloud**. Você deve ver os aplicativos enviados com opções para aprovar/rejeitar.
Depois de aprovadas, as extensões de aplicativos publicadas devem ser carregadas automaticamente em seu ambiente do Workfront.

   ![](assets/approve-submission.png)

## Ajuda adicional

O Adobe tem excelente documentação sobre como começar a criar aplicativos para o AppBuilder e implantá-los.

Estes são alguns links úteis:

* [https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli)

* [https://developer.adobe.com/uix/docs/guides/publication/](https://developer.adobe.com/uix/docs/guides/publication/)

* [https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/](https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/)
