---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: O Tableau Desktop não pode estabelecer uma conexão
description: Quando você tenta conectar o Tableau Desktop ao Data Connect, ocorre um erro.
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---


# O Tableau Desktop não pode estabelecer uma conexão

## Problema

Ao tentar conectar o Tableau Desktop ao Data Connect, você vê o seguinte erro:

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## Causa

Esse erro é causado por uma configuração de proxy no computador local que impede que os dados sejam carregados da Conexão de dados.

O Data Connect é fornecido por meio de serviços em nuvem de terceiros da Snowflake. O Tableau requer uma rede aberta para se comunicar com a Snowflake.

## Solução

Você pode tentar o seguinte para resolver esse problema:

* **Solucione problemas desabilitando a ferramenta de segurança**: desative a ferramenta de segurança, como Zscaler ou Cisco, para ver se ela resolve o problema de conectividade. Se isso resolver o problema de conexão, certifique-se de que sua ferramenta de segurança está atualizada para a versão mais recente, adicione o endereço IP da conexão de dados (Snowflake) ao VPN inclua na lista de permissões com sua equipe interna de rede.

* **Adicionar Endereços IP à Inclui na lista de permissões**: verifique se as configurações do firewall permitem os endereços IP usados pela Conexão de Dados. Incluir na lista de permissões Use o comando `SYSTEM$ALLOWLIST()` para obter o endereço IP, que você poderá então modificar na VPN.

* **Verificar configurações de firewall e proxy**: verifique se há configurações de firewall ou proxy na rede bloqueando o acesso aos pontos de extremidade da Snowflake. Talvez seja necessário entrar em contato com o administrador da rede para adicionar as portas e os endereços IP Snowflake necessários à inclui na lista de permissões da sua empresa.

* **Opção alternativa**: criar uma extração de uma tela de planilha em vez do painel Data Source no Tableau. A conexão não é perdida e o processo de extração é concluído.

