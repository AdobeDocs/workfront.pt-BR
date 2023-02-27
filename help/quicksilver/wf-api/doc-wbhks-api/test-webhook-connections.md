---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Testar conexões do Webhook
description: Testar conexões do Webhook
author: Becky
feature: Workfront API
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 0%

---


# Testar conexões do Webhook

Para verificar se a implementação do webhook do documento funciona corretamente, execute os testes manuais nesta seção. Essas etapas passam pela interface da Web do Adobe Workfront e acessam indiretamente os endpoints da implementação do webhook.

## Pré-requisitos

Os seguintes pré-requisitos são necessários para executar os testes:

* Uma conta Workfront com o Gerenciamento Avançado de Documentos (ADM) ativado

* Um usuário do Workfront para esta conta com direitos de administrador do sistema

* Uma instância do Webhook de documento com endpoints HTTP que são acessíveis ao Workfront

Esses testes também presumem que a instância do Webhook do documento está registrada. (Você pode registrar sua instância no Workfront em Configuração > Documentos > Integrações personalizadas.)

**Teste 1: Provisionar o serviço do Webhook de documentos para um usuário**

Testa o URL de autenticação e o URL do ponto de extremidade do token para provedores do Webhook baseados em OAuth.

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Clique no menu suspenso Adicionar documentos e selecione o serviço Webhook de documentos em Adicionar serviço.
1. (Somente serviços OAuth) Após concluir a etapa anterior, você verá a página de autenticação OAuth2 do seu serviço carregada em uma janela pop-up. (Observação: você pode ser solicitado a fazer logon em seu serviço primeiro.) Na página de autenticação, conceda à Workfront acesso à conta do usuário clicando no botão Confiar ou Permitir .
1. Verifique se o serviço foi adicionado ao menu suspenso Adicionar documentos . Se não o vir inicialmente, tente atualizar seu navegador.

**Teste 2: Vincule um documento aos Testes do Workfront aos seguintes endpoints: /files, /metadata**

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Selecione o serviço Webhook do documento em Adicionar documentos.
1. No modal , navegue pela estrutura de pastas.
1. Verifique se é possível navegar pela estrutura de pastas.
1. Selecionar e vincular um documento ao Workfront

**Teste 3: Navegue até um documento no sistema de gerenciamento de conteúdo**

Testa os seguintes endpoints: /metadata (especificamente o viewLink)

1. Vincular um documento ao Workfront
1. Selecione o documento e clique no link Open .
1. Verifique se o documento abre em uma nova guia.

**Teste 4: Navegue até um documento no sistema de gerenciamento de conteúdo (com logon)**

Testa os seguintes endpoints: /metadata (especificamente o viewLink)

1. Verifique se você está desconectado do sistema de gerenciamento de conteúdo.
1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Open .
1. Verifique se a tela de logon do sistema de gerenciamento de conteúdo é carregada em uma nova guia.
1. Faça logon e verifique se você foi levado para o documento

**Teste 5: Baixe o documento do sistema de gerenciamento de conteúdo**

Testa os seguintes endpoints (especificamente o link de download): /metadados 

1. Vincule um documento ao Workfront.
1. Selecione o documento e clique no link Download .
1. Verifique se o download começa.

**Teste 6: Pesquisar conteúdo**

Testa os seguintes endpoints: /search

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Selecione o serviço Webhook do documento em Adicionar documentos.
1. No modal , faça uma pesquisa.
1. Verifique se os resultados da pesquisa estão corretos.

**Teste 7: Enviar documento do Workfront para o sistema de gerenciamento de conteúdo**

Testa os seguintes endpoints: /files, /uploadInit, /upload

1. No Workfront, vá para a página principal de Documentos clicando no link Documents na barra de navegação superior.
1. Carregar um documento no Workfront a partir do seu computador
1. Vá para a página de detalhes do documento
1. Na lista suspensa Ações do documento , selecione o serviço Webhook do documento em Enviar para...
1. Vá para a pasta de destino desejada e clique no botão Save .
1. Verifique se o documento foi carregado no local correto no sistema de gerenciamento de conteúdo.

**Teste 8: Exibir miniaturas no Workfront**

Testa os seguintes endpoints: /miniatura

1. Vincule um documento ao Workfront.
1. Selecione o documento na lista.
1. Verifique se a miniatura aparece no painel direito.

**Teste 9: Obter os bytes de conteúdo**

Testa os seguintes endpoints: /download

1. Vincule um documento ao Workfront.
1. Vá para a página de detalhes do documento.
1. Envie o documento para o Workfront selecionando Ações do documento > Enviar para... > Workfront. Isso criará uma nova versão de documento no Workfront.
1. Baixe o documento do Workfront clicando no link Download .

**Teste 10: Atualizar token de acesso (somente provedores do Webhook OAuth2)**

Testa os seguintes endpoints: URL do ponto de extremidade do token

1. Provisionar o serviço do Webhook de documentos para um usuário
1. Invalidar o token de acesso do usuário ao aguardar o tempo limite de 1 ou 2) invalidá-lo manualmente no sistema externo.
1. Atualize o token de acesso no Workfront. Você pode fazer isso, por exemplo, vinculando um documento ao Workfront. Você saberá que o token de acesso foi atualizado com êxito se conseguir navegar e vincular um documento.

>[!NOTE]
>
>Atualmente, o Enviar para... não está disponível para documentos vinculados. Isso será adicionado pelo Workfront. Você pode testar o endpoint /download acessando o endpoint manualmente usando um cliente REST, como o Postman. Como alternativa, o endpoint /download pode ser testado gerando uma prova digital. Para ativar a prova digital, entre em contato com a Workfront.
