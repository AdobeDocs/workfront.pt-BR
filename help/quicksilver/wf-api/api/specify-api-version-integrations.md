---
content-type: api
navigation-topic: api-navigation-topic
title: Especificar uma versão da API em suas integrações
description: Especificar uma versão da API em suas integrações
author: Becky
feature: Workfront API
role: Developer
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
TQID: https://experienceleague.adobe.com/GWA77t-kaVNG7tfSsg5Fe5kLtR3Ibo0YbW7Gp7wBQ0U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 438
ht-degree: 3%

---

# Especifique uma versão da API em suas integrações

Todos os URIs do Adobe Workfront devem fazer referência a uma versão específica da API após a parte &quot;attask/api&quot; do URI. O exemplo a seguir chama a Versão 15.0:

`attask/api/v15.0/<objectName>/<objectId>`

Verifique se todas as suas integrações chamam as APIs do Workfront compatíveis no momento.

## Programação de lançamento e descontinuação de APIs do Workfront

Novas versões da API são lançadas regularmente, geralmente duas vezes por ano. Cada versão é compatível por três anos após sua data de lançamento, com um ano adicional em um estado obsoleto, em que a versão está disponível, mas não é compatível.

Para obter mais informações sobre a cadência de lançamento e a programação de descontinuação das APIs do Workfront, consulte [Controle de versão da API e programação de suporte](../../wf-api/api/api-version-support-schedule.md).

>[!IMPORTANT]
>
>* A versão padrão da API é definida como a versão mais recente. Qualquer chamada de API sem a versão especificada usará a versão padrão. Cada vez que o Workfront lança uma nova versão da API, a versão padrão será atualizada para a versão mais recente. **Portanto, depois que uma nova versão da API do Workfront for lançada, todas as chamadas de API que usam a versão padrão deverão ser verificadas para garantir que a funcionalidade ainda tenha suporte.**
>
>* Se sua organização estiver usando a API padrão no momento, o administrador do Workfront receberá uma mensagem do Centro de notificações com mais instruções sobre a API padrão.
>
>Para ver a versão mais recente da API, consulte [Controle de versão da API e agendamento de suporte](../../wf-api/api/api-version-support-schedule.md).


## Determinar a versão da API que você está usando

Você pode determinar a versão da API que está usando verificando o URI de uma solicitação HTTP enviada para a API do Workfront. O exemplo a seguir mostra um URI de solicitação Workfront que especifica a Versão 15 da API:

`https://<domainname>.my.workfront.com/attask/api/v15.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Se um URI não especificar uma versão, ele estará usando a Versão padrão da API, conforme mostrado no exemplo a seguir:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrações que não especificam uma versão da API no URI são automaticamente roteadas para a Versão padrão da API.

## Atualização de integrações para usar versões de API compatíveis

À medida que você cria ou mantém integrações do Workfront, deve incluir um método para atualizar dinamicamente a versão da API e outras propriedades sujeitas a alterações (como sua chave de API).

Para tornar a atualização das integrações mais eficiente, considere as seguintes sugestões para registrar valores de integração:

* Armazenar valores sujeitos a alterações futuras em um arquivo de propriedades que você mantém atualizado
* Criar um serviço Web para gerenciar propriedades em tempo real
* Armazenar valores de propriedade em um armazenamento de dados que seu aplicativo pode ler

Projetar as integrações do Workfront tendo isso em mente alivia a necessidade de um trabalho extenso de desenvolvimento quando esses valores inevitavelmente mudam.
