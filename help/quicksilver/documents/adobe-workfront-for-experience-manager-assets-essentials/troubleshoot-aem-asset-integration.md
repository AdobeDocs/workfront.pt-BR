---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Solução de problemas de integração do Adobe Experience Manager
description: 'Problema: o Assets não é salvo no Adobe Experience Manager'
author: Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: f7e31e20-01e3-462d-9020-005e155f0259
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---

# Solução de problemas de integração do Adobe Experience Manager

## Problema: o Assets não é salvo no Adobe Experience Manager

Quando um usuário seleciona um ativo ou pasta para exportar para o Experience Manager Assets e clica em Selecionar, a janela do seletor é fechada, mas os ativos não são salvos no Experience Manager Assets. Não há nenhuma indicação no Workfront de que os ativos não foram salvos na Experience Manager Assets.

### Causa

Isso pode ocorrer devido à inclui na lista de permissões no Adobe Cloud Manager. Se a Adobe do incluir na lista de permissões Cloud Manager para uma organização estiver vazia, os endereços IP não serão limitados e o Workfront poderá acessar as pastas e os ativos da organização no Adobe Experience Manager. No entanto, se até mesmo um único endereço IP for adicionado à Cloud Manager do incluir na lista de permissões, o incluo na lista de permissões presumirá que qualquer endereço IP que não esteja na lista não é permitido. Portanto, se a Cloud Manager do incluir na lista de permissões modificar incluir qualquer endereço IP, o endereço IP do Workfront também deverá ser adicionado ao incluo na lista de permissões para permitir que o Workfront envie ativos para o Experience Manager Assets.

### Solução:

Adicione os endereços IP da Workfront ao arquivo de inclui na lista de permissões do Adobe Cloud Manager.

* Para obter instruções sobre como adicionar endereços IP ao Adobe Cloud Manager, consulte [Introdução ao IP Lista de permissões](https://experienceleague.adobe.com/pt-br/docs/experience-manager-cloud-service/content/implementing/using-cloud-manager/ip-allow-lists/introduction) na documentação do Adobe Experience Manager.
* Para obter uma lista de endereços IP da Workfront a serem adicionados ao arquivo de inclui na lista de permissões, consulte [Configurar firewall](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
