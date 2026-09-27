---
content-type: reference
navigation-topic: announcements
title: Alteração exigida para adicionar provas à lista de permissões
description: O domínio de comprovação está sendo alterado de proofhq.com para workfront.com.
author: Luke
feature: Product Announcements
exl-id: 05a1fd37-224b-4a0b-abef-4d9a015de524
TQID: 'https://experienceleague.adobe.com/uDxTQpAiB9jDDVfaGnKBvBb-vIfOQOEOEPTS6aEsA88'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 13%
---
# Alteração exigida para adicionar provas à lista de permissões

O domínio de comprovação está alterando from proofhq.com para workfront.com.

Se o firewall ou servidor de email estiver configurado para permitir acesso somente a fornecedores específicos, você deverá adicionar o seguinte URL adicional ao incluo na lista de permissões para garantir que os usuários em sua organização possam exibir provas no Adobe Workfront tanto no visualizador de provas de navegador quanto no visualizador de provas de desktop:

&#42;.workfront.com

A URL &#42;proofhq.com também é necessária.

Para obter mais informações sobre como atualizar o incluo na lista de permissões, consulte [Configurar o incluo na lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

>[!NOTE]
>
>Essa atualização se aplica somente à revisão no Workfront; não se aplica ao usar o aplicativo independente do Workfront Proof.
