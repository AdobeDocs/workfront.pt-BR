---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Testar conexões do Webhook
description: Testar conexões do Webhook
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---


# Testar conexões do Webhook

Para verificar se a implementação do webhook do seu documento funciona corretamente, execute os testes manuais nesta seção. Essas etapas passam pela interface da Web do Adobe Workfront e atingem indiretamente os endpoints da implementação do webhook.

## Pré-requisitos

Os seguintes pré-requisitos são necessários para executar os testes:

* Uma conta do Workfront com o Gerenciamento avançado de documentos (ADM) habilitado

* Um usuário do Workfront para esta conta com direitos de administrador do sistema

* Uma instância do Webhook de documentos com pontos de extremidade HTTP acessíveis para o Workfront

Esses testes também pressupõem que a instância do Webhook do documento está registrada. (Você pode registrar sua instância no Workfront em Configuração > Documentos > Integrações personalizadas.)

**Teste 1: provisionar o serviço Webhook de documentos para um usuário**

Testa o URL de autenticação e o URL do ponto de extremidade do token para provedores de Webhook baseados em OAuth.

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Clique na lista suspensa Adicionar documentos e selecione o serviço Webhook de documentos em Adicionar serviço.
1. (Somente serviços OAuth) Depois de concluir a etapa anterior, você verá o carregamento da página de autenticação OAuth2 do seu serviço em uma janela pop-up. (Observação: você pode ser solicitado a fazer logon no serviço primeiro.) Na página de autenticação, conceda acesso à conta do usuário pelo Workfront clicando no botão Confiar ou Permitir.
1. Verifique se o serviço foi adicionado à lista suspensa Adicionar documentos. Caso não o veja inicialmente, tente atualizar o navegador.

**Teste 2: Vincular um documento no Workfront Testa os seguintes pontos de extremidade: /files, /metadata**

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Selecione o serviço Webhook de documentos em Adicionar documentos.
1. Na modal, navegue pela estrutura de pastas.
1. Verifique se você pode navegar pela estrutura de pastas.
1. Selecionar e vincular um documento ao Workfront

**Teste 3: Navegar até um documento no sistema de gerenciamento de conteúdo**

Testa os seguintes pontos de extremidade: /metadata (especificamente o viewLink)

1. Vincular um documento ao Workfront
1. Selecione o documento e clique no link Abrir.
1. Verifique se o documento abre em uma nova guia.

**Teste 4: Navegar até um documento no sistema de gerenciamento de conteúdo (com logon)**

Testa os seguintes pontos de extremidade: /metadata (especificamente o viewLink)

1. Verifique se você está desconectado do sistema de gerenciamento de conteúdo.
1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Abrir.
1. Verifique se a tela de logon do sistema de gerenciamento de conteúdo é carregada em uma nova guia.
1. Faça logon e verifique se você está direcionado ao documento

**Teste 5: Baixar o documento do sistema de gerenciamento de conteúdo**

Testa os seguintes pontos de extremidade (especificamente o link de download): /metadata 

1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Download.
1. Verifique se o download foi iniciado.

**Teste 6: Pesquisar por conteúdo**

Testa os seguintes pontos de extremidade: /search

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Selecione o serviço Webhook de documentos em Adicionar documentos.
1. No modal, execute uma pesquisa.
1. Verifique se os resultados da pesquisa estão corretos.

**Teste 7: Enviar documento do Workfront para o sistema de gerenciamento de conteúdo**

Testa os seguintes pontos de extremidade: /files, /uploadInit, /upload

1. No Workfront, vá para a página principal Documentos clicando no link Documentos na barra de navegação superior.
1. Fazer upload de um documento para o Workfront no seu computador
1. Ir para a página de detalhes do documento
1. Na lista suspensa Ações do documento, selecione o serviço Webhook do documento em Enviar para...
1. Vá para a pasta de destino desejada e clique no botão Save.
1. Verifique se o documento foi carregado no local correto no sistema de gerenciamento de conteúdo.

**Teste 8: Exibir Miniaturas no Workfront**

Testa os seguintes pontos de extremidade: /thumbnail

1. Vincule um documento ao Workfront.
1. Selecione o documento na lista.
1. Verifique se a miniatura aparece no painel direito.

**Teste 9: obter os bytes de conteúdo**

Testa os seguintes pontos de extremidade: /download

1. Vincule um documento ao Workfront.
1. Vá para a página de detalhes do documento.
1. Envie o documento para o Workfront selecionando Ações do documento > Enviar para... > Workfront. Isso criará uma nova versão do documento no Workfront.
1. Baixe o documento do Workfront clicando no link Download.

**Teste 10: atualizar token de acesso (somente provedores de Webhook OAuth2)**

Testa os seguintes endpoints: URL do endpoint do token

1. Provisionar um serviço Webhook de documento para um usuário
1. Invalidar o token de acesso do usuário 1 (aguardando o tempo limite) ou 2) invalidando-o manualmente no sistema externo.
1. Atualize o token de acesso no Workfront. Você pode fazer isso, por exemplo, vinculando um documento ao Workfront. Você saberá que o token de acesso foi atualizado com êxito se conseguir navegar e vincular um documento.

>[!NOTE]
>
>Atualmente, Enviar para... não está disponível para documentos vinculados. Isso será adicionado pelo Workfront. Você pode testar o terminal /download acessando o terminal manualmente usando um cliente REST, como o Postman. Como alternativa, o endpoint /download pode ser testado gerando uma prova digital. Para ativar a prova digital, entre em contato com a Workfront.
