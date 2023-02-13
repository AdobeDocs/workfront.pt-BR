---
content-type: api
navigation-topic: api-navigation-topic
title: Especificar uma versão da API em suas integrações
description: Especificar uma versão da API em suas integrações
author: John
feature: Workfront API
exl-id: 2971749d-1d34-42a4-9eda-411aa8c3a2ab
source-git-commit: 183f7b766fd6f02b51625778e380cf00c5ecf61f
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Especificar uma versão da API em suas integrações

Todos os URIs do Adobe Workfront devem referenciar uma versão específica da API após a parte &quot;attask/api&quot; do URI. O exemplo a seguir chama a Versão 7.0:
`attask/api/v7.0/<objectName>/<objectId>` Certifique-se de que todas as suas integrações chamam as APIs do Workfront compatíveis no momento.

## Lançamento e agendamento de desativação das APIs do Workfront

Novas versões da API são lançadas semestralmente — a cada seis a oito meses. Cada versão é compatível por três anos após a data de lançamento, com um ano adicional em um estado obsoleto, onde a versão está disponível, mas não é compatível.

Para obter mais informações sobre a cadência da versão e o agendamento de descontinuação das APIs do Workfront, consulte [Controle de versão da API e cronograma de suporte](../../wf-api/api/api-version-support-schedule.md).

A Workfront substituiu a versão padrão da API desde julho de 2017. Isso significa que o Workfront não designa mais uma versão específica da API como a versão padrão. Todos os URIs de API futuros devem especificar uma versão da API para serem válidos.

>[!IMPORTANT]
>
> Todas as integrações que usam a versão da API padrão devem ser atualizadas para chamar uma versão específica da API compatível até 1º de julho de 2018.

## Determinar a versão da API que você está usando

Você pode determinar a versão da API que está usando, verificando o URI de uma solicitação HTTP enviada para a API do Workfront. O exemplo a seguir mostra um URI de solicitação do Workfront que especifica a Versão 7 da API:

`https://<domainname>.my.workfront.com/attask/api/v7.0/proj/4c7c08b20000002de5ca1ebc19edf2d5`

Se um URI não especificar uma versão, ele estará usando a Versão padrão da API, como mostrado no exemplo a seguir:

`https://<domainname>.my.workfront.com/attask/api/proj/4c7c08b20000002de5ca1ebc19edf2d5`

>[!IMPORTANT]
>
> Integrações que não especificam uma versão da API no URI são encaminhadas automaticamente para a versão padrão da API e não funcionarão após 1 de julho de 2018.

## Atualização das integrações para usar as versões de API suportadas

À medida que você cria ou mantém integrações do Workfront, deve incluir um método para atualizar dinamicamente a versão da API e outras propriedades sujeitas a alterações (como sua chave de API).

Para tornar a atualização das integrações mais eficiente, considere as seguintes sugestões para registrar os valores de integração:

* Armazenar valores sujeitos a alterações futuras em um arquivo de propriedades que você mantém atualizado
* Criar um serviço da Web para gerenciar propriedades em tempo real
* Armazenar valores de propriedade em um armazenamento de dados que seu aplicativo pode ler

Projetar as integrações do Workfront pensando nisso reduz a necessidade de um trabalho de desenvolvimento abrangente quando esses valores inevitavelmente mudam.
