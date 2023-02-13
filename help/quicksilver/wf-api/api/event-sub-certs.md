---
content-type: api
navigation-topic: api-navigation-topic
title: Certificados de assinatura de evento
description: Certificados de assinatura de evento
author: Becky
feature: Workfront API
source-git-commit: 53ef8f4fda22c912c274841d07ad865aa04141c8
workflow-type: tm+mt
source-wordcount: '330'
ht-degree: 0%

---

# Configurar o TLS do cliente para assinatura de evento

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

O TLS do cliente permite verificar se a mensagem de assinatura do evento recebida realmente veio do Adobe Workfront. Para ativar essa funcionalidade, seu servidor deve ser configurado para solicitar e validar o certificado x509 do Workfront.


## Verificar certificado de cliente Workfront

Esse procedimento pressupõe que seu servidor esteja configurado para aceitar conexões TLS. A Workfront não oferece suporte a certificados autoassinados.

Em geral, essas são as etapas necessárias para ativar a autenticação de cliente para seu servidor:

1. Baixe a versão PEM do certificado da autoridade de certificação raiz global DigiCert.
1. Ative a verificação de certificado de cliente.

   Especifique o certificado CA da etapa 1 como confiável.

1. Defina a profundidade de verificação como 2, pois nosso certificado é realmente assinado pela CA do Servidor Seguro DigiCert SHA2, que é uma CA intermediária na CA raiz global DigiCert.
1. Verifique se o certificado do cliente é realmente da Workfront inspecionando o Nome do domínio do assunto.

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

Para obter mais informações, consulte o [Documentação do NGiNX para ngx_http_ssl_module](http://nginx.org/en/docs/http/ngx_http_ssl_module.html).

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

* [Autenticação de Cliente e Controle de Acesso](https://httpd.apache.org/docs/2.4/ssl/ssl_howto.html#accesscontrol)
* [Apache Module mod_ssl](https://httpd.apache.org/docs/2.4/mod/mod_ssl.html)
 

## Mapeamento de certificado para ambiente

| Ambiente WF | Nome comum do certificado | Titular do certificado (DN) | | — | — | — | | Produção | *.prod.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.prod.eventsubscriptions.workfront.com| | Pré-visualização | *.preview.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.preview.eventsubscriptions.workfront.com | | Sandbox 1 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com | | Sandbox 2 | *.sandbox.eventsubscriptions.workfront.com | subject= /C=US/ST=Utah/L=Lehi/O=Workfront, Inc./CN=*.sandbox.eventsubscriptions.workfront.com |

## Fazer download de certificados

Clique nos links a seguir para baixar os certificados do cliente.

* [Certificado do cliente - Ambiente de produção](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_production.crt)
* [Certificado do cliente - Ambiente de visualização](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_preview.crt)
* [Certificado do cliente - Ambiente de sandbox](https://cdn.experience.workfront.com/Documentation/Event+Subscriptions/event_subscription_dec_2022_sandboxes.crt)

>[!NOTE]
>
>Você pode usar o mesmo certificado de cliente para ambos os ambientes do Sandbox.

