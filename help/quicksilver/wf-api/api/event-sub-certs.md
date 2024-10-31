---
content-type: api
navigation-topic: api-navigation-topic
title: Certificados de inscrição em eventos
description: Certificados de inscrição em eventos
author: Becky
feature: Workfront API
role: Developer
exl-id: 3606b6c3-b373-47ea-9cb5-813bd3af8da7
source-git-commit: 7b67358ec1d665fe2012d2c0156db3b928c48ae5
workflow-type: tm+mt
source-wordcount: '284'
ht-degree: 2%

---

# Configurar o TLS do cliente para a assinatura de eventos

<!--Configuring Client TLS for Event Subscription
Steps to Verify Workfront's Client Certificate
Examples for Server configuration
NGINX
Apache
Certificate to Environment Mapping
Certificates
Production
Preview
Sandbox 1
Sandbox 2
-->

O TLS do cliente permite verificar se a mensagem de inscrição de evento recebida realmente veio do Adobe Workfront. Para habilitar essa funcionalidade, o servidor deve estar configurado para solicitar e validar o certificado x509 da Workfront.


## Verificar o certificado de cliente do Workfront

Este procedimento pressupõe que o servidor esteja configurado para aceitar conexões TLS. O Workfront não oferece suporte a certificados autoassinados.

Em geral, estas são as etapas necessárias para ativar a autenticação de cliente para o servidor:

1. Baixe a versão PEM do certificado CA raiz global da DigiCert.
1. Ativar verificação de certificado de cliente.

   Especifique o certificado CA da etapa 1 como confiável.

1. Defina a profundidade de verificação como 2, pois nosso certificado é assinado pela CA de servidor seguro DigiCert SHA2, que é uma CA intermediária na CA de raiz global DigiCert.
1. Verifique se o certificado do cliente é realmente da Workfront, inspecionando o Nome do domínio do assunto.

## Exemplos de configuração do servidor

### NGINX

```
server {

    listen 443 ssl default_server;
    # ... existing SSL configuration for server authentication ...

    ssl_verify_client on;
    ssl_client_certificate /path/to/DigiCert_Global_Root_CA.pem;
    ssl_verify_depth 2;

        # ... existing location configuration ...
    }
}
```

Para obter mais informações, consulte a [documentação do NGiNX para ngx_http_ssl_module](https://nginx.org/en/docs/http/ngx_http_ssl_module.html).

### Apache

```
Listen 443
<VirtualHost *:443>
    # ... existing SSL configuration for server authentication ...

    SSLVerifyClient require
    SSLCACertificateFile "/path/to/DigiCert_Global_Root_CA.pem"
    SSLVerifyDepth 2
</VirtualHost>

<Directory /var/www/>
    Require expr "%{SSL_CLIENT_S_DN_CN} == <>"

    # ... existing directory configuration ...
</Directory>
```

Para obter mais informações, consulte

* [Controle de Acesso e Autenticação do Cliente](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Módulo Apache mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Certificado para mapeamento de ambiente

| Ambiente WF | Nome comum do certificado | Assunto do certificado (DN) |
| -- | -- | -- |
| Produção | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com |
| Visualização | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com |
| Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |
| Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Baixar certificados

Clique nos links a seguir para baixar os certificados de cliente.

* [Certificado do cliente - Ambiente de produção](assets/event_subscription_nov_2023_production.crt)
* [Certificado do cliente - Ambiente de visualização](assets/event_subscription_nov_2023_preview.crt)
* [Certificado do cliente - Ambiente de sandbox](assets/event_subscription_nov_2023_sandboxes.crt)

>[!NOTE]
>
>Você pode usar o mesmo certificado de cliente para ambos os ambientes de sandbox.
