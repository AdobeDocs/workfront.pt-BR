---
content-type: api
navigation-topic: api-navigation-topic
title: Especificar uma versão da API em suas integrações
description: Especificar uma versão da API em suas integrações
author: Becky
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '496'
ht-degree: 0%

---

# Especificar uma versão da API em suas integrações

<span class="preview">As informações destacadas nesta página se referem à funcionalidade ainda não disponível no geral. Ela está disponível somente no ambiente Preview Sandbox .</span>

Todos os URIs do Adobe Workfront devem referenciar uma versão específica da API após a parte &quot;attask/api&quot; do URI. O exemplo a seguir chama a Versão 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

Certifique-se de que todas as suas integrações chamam as APIs do Workfront compatíveis no momento.

## Lançamento e agendamento de desativação das APIs do Workfront

Novas versões da API são lançadas regularmente, geralmente duas vezes por ano. Cada versão é compatível por três anos após a data de lançamento, com um ano adicional em um estado obsoleto, onde a versão está disponível, mas não é compatível.

Para obter mais informações sobre a cadência da versão e o agendamento de descontinuação das APIs do Workfront, consulte [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* Após a versão 23.2, a versão padrão da API será definida como a versão mais recente. Qualquer chamada de API sem a versão especificada usará a versão padrão. Sempre que o Workfront lançar uma nova versão da API, a versão padrão será atualizada para a versão mais recente. Portanto, depois que uma nova versão da API do Workfront for lançada, todas as chamadas de API que usam a versão padrão deverão ser verificadas para garantir que a funcionalidade ainda seja suportada.
>
>* Se sua organização estiver usando atualmente a API padrão, o administrador do Workfront recebeu uma mensagem da Central de anúncios com mais instruções relacionadas à API padrão.
>
>* <span class="preview">A API padrão no ambiente de Visualização é definida como a versão mais recente. A API padrão no ambiente de produção será definida como a versão mais recente após a versão 23.2 (abril de 2023)</span>.
>
>Para ver a versão mais recente da API, consulte [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).


## Determinar a versão da API que você está usando

Você pode determinar a versão da API que está usando, verificando o URI de uma solicitação HTTP enviada para a API do Workfront. O exemplo a seguir mostra um URI de solicitação do Workfront que especifica a Versão 15 da API:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Se um URI não especificar uma versão, ele estará usando a Versão padrão da API, como mostrado no exemplo a seguir:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrações que não especificam uma versão da API no URI são encaminhadas automaticamente para a versão padrão da API.

## Atualização das integrações para usar as versões de API suportadas

À medida que você cria ou mantém integrações do Workfront, deve incluir um método para atualizar dinamicamente a versão da API e outras propriedades sujeitas a alterações (como sua chave de API).

Para tornar a atualização das integrações mais eficiente, considere as seguintes sugestões para registrar os valores de integração:

* Armazenar valores sujeitos a alterações futuras em um arquivo de propriedades que você mantém atualizado
* Criar um serviço da Web para gerenciar propriedades em tempo real
* Armazenar valores de propriedade em um armazenamento de dados que seu aplicativo pode ler

Projetar as integrações do Workfront pensando nisso reduz a necessidade de um trabalho de desenvolvimento abrangente quando esses valores inevitavelmente mudam.
