---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: O Tableau Desktop não conseguiu estabelecer uma conexão
description: Quando você tenta conectar o Tableau Desktop ao Data Connect, ocorre um erro.
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 5%

---

# O Tableau Desktop não conseguiu estabelecer uma conexão

## Problema

Ao tentar conectar o Tableau Desktop ao Data Connect, você vê o seguinte erro:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Causa

Esse erro é causado por uma configuração de proxy no computador local que impede que os dados sejam carregados da Conexão de dados.

O Data Connect é fornecido por meio de serviços em nuvem de terceiros da Snowflake. O Tableau requer uma rede aberta para se comunicar com a Snowflake.

## Solução

Você pode tentar o seguinte para resolver esse problema:

* **Solucione problemas desabilitando a ferramenta de segurança**: desative a ferramenta de segurança, como Zscaler ou Cisco, para ver se ela resolve o problema de conectividade. Se isso resolver o problema de conexão, certifique-se de que sua ferramenta de segurança está atualizada para a versão mais recente, adicione o endereço IP do Data Connect (Snowflake) ao incluo na lista de permissões VPN com sua equipe interna de rede.

* **Adicionar Endereços IP ao Incluo na lista de permissões**: verifique se as configurações do firewall permitem os endereços IP usados pela Conexão de Dados. Use o comando `SYSTEM$ALLOWLIST()` para obter o endereço IP, que você pode incluir na lista de permissões na VPN.

* **Verificar configurações de firewall e proxy**: verifique se há configurações de firewall ou proxy na rede bloqueando o acesso aos pontos de extremidade da Snowflake. Talvez seja necessário entrar em contato com o administrador de rede para adicionar as portas e os endereços IP Snowflake necessários ao incluo na lista de permissões de sua empresa.

* **Opção alternativa**: criar uma extração de uma tela de planilha em vez do painel Data Source no Tableau. A conexão não é perdida e o processo de extração é concluído.
