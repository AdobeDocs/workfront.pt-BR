---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Solução de problemas de integração do Adobe Experience Manager
description: "Problema: os ativos não são salvos no Adobe Experience Manager"
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: a73ebfe8c735eb9e103b01a201a8f71d6ab7bda2
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 0%

---

# Solução de problemas de integração do Adobe Experience Manager

## Problema: os ativos não são salvos no Adobe Experience Manager

Quando um usuário seleciona um ativo ou pasta para exportar para o Experience Manager Assets e clica em Selecionar, a janela do seletor é fechada, mas os ativos não são salvos no Experience Manager Assets. Não há nenhuma indicação no Workfront de que os ativos não foram salvos na Experience Manager Assets.

### Causa

Isso pode ocorrer devido à inclui na lista de permissões no Adobe Cloud Manager. Se a Adobe do incluir na lista de permissões Cloud Manager para uma organização estiver vazia, os endereços IP não serão limitados e a Workfront poderá acessar as pastas e os ativos da organização no Adobe Experience Manager. No entanto, se até mesmo um único endereço IP for adicionado ao incluo na lista de permissões do Cloud Manager, a inclui na lista de permissões presumirá que qualquer endereço IP que não esteja na lista não é permitido. Portanto, se a inclui na lista de permissões do Cloud Manager incluir qualquer endereço IP, o endereço IP do Workfront incluir na lista de permissões também deverá ser adicionado ao arquivo para permitir que o Workfront envie ativos para o Experience Manager Assets.

### Solução:

Adicione os endereços IP da Workfront ao Adobe incluo na lista de permissões do Cloud Manager.

* Para obter instruções sobre como adicionar endereços IP ao Adobe Cloud Manager, consulte [Introdução a Listas de permissões de IP](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction.html?lang=en) na documentação do Adobe Experience Manager.
* Para obter uma lista de endereços IP da Workfront incluir na lista de permissões que serão adicionados ao arquivo, consulte [Configurar o firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).


