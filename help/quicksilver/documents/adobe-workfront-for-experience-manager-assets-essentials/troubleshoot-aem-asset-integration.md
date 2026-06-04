---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Solução de problemas de integração do Adobe Experience Manager
description: 'Problema: o Assets não é salvo no Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
TQID: https://experienceleague.adobe.com/VaiQnZXQe39sYlnJOblWoea9UwOaujEU3ME-jh7-0EI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 0%

---

# Solução de problemas de integração do Adobe Experience Manager

## Problema: o Assets não é salvo no Adobe Experience Manager

Quando um usuário seleciona um ativo ou pasta para exportar para o Experience Manager Assets e clica em Selecionar, a janela do seletor é fechada, mas os ativos não são salvos no Experience Manager Assets. Não há nenhuma indicação no Workfront de que os ativos não foram salvos na Experience Manager Assets.

### Causa

Isso pode ocorrer devido ao incluo na lista de permissões no Adobe Cloud Manager. Se o incluo na lista de permissões Cloud Manager do Adobe de uma organização estiver vazio, os endereços IP não serão limitados e o Workfront poderá acessar as pastas e os ativos da organização no Adobe Experience Manager. No entanto, mesmo que um único endereço IP seja adicionado ao incluo na lista de permissões do Cloud Manager, o incluo na lista de permissões presume que qualquer endereço IP que não esteja na lista não é permitido. Portanto, se o incluo na lista de permissões do Cloud Manager incluir qualquer endereço IP, os endereços IP do Workfront também deverão ser adicionados ao incluo na lista de permissões para permitir que o Workfront envie ativos para o Experience Manager Assets.

### Solução:

Adicione os endereços IP da Workfront ao incluo na lista de permissões Adobe Cloud Manager.

* Para obter instruções sobre como adicionar endereços IP ao Adobe Cloud Manager, consulte [Introdução ao IP Lista de permissões](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) na documentação do Adobe Experience Manager.
* Para obter uma lista de endereços IP da Workfront a serem adicionados ao incluo na lista de permissões, consulte [Configurar firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
