---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Desinstale o conector herdado
description: texto
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
TQID: https://experienceleague.adobe.com/vA8FflK8mA9a002-Mf8WKzECsEhOaIlvnd0kG958ySE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 397
ht-degree: 3%

---

# Desinstalar o Workfront com o conector legado do Adobe Experience Manager

Você deve desinstalar o conector herdado do Workfront com Adobe Experience Manager para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.

## Cancelar assinatura no Workfront

1. Abra o Adobe Experience Manager.
1. No Experience Manager, vá para **Ferramentas** > **Serviços de Nuvem** > **Configuração de Integração do Workfront**.
1. Selecione sua configuração (global-workfront por padrão) e clique em **Propriedades**.

   ![cancelar assinatura do workfront](assets/unsubscribe-from-workfront.png)

1. Desative a sincronização de documentos, comentários e metadados. O rótulo deve ser dia Desativado.
Isso removerá as assinaturas no Workfront e permitirá que o usuário crie uma nova assinatura usando o mesmo url definido no Day CQ Link Externalizer.

## Excluir a configuração de integração do Workfront

Após remover a assinatura, agora é seguro excluir a Configuração de integração do Workfront.

1. Abra a configuração e selecione **Excluir**.

   ![excluir configuração](assets/delete-wf-configuration.png)

## Remover mapeamento

Em seguida, é necessário excluir o Mapeamento de propriedades do Workfront.

1. No Experience Manager, vá para **Ferramentas** > **Assets** > **Mapeamento de Propriedades do Workfront**.

1. Selecione todos os mapeamentos e clique em **Excluir**.

## Permissões de usuário

Todos os usuários que acessam o AEM Dam pelo Workfront receberam permissões de leitura para `/content/dam`. Se um usuário não precisar mais disso, você poderá remover as permissões concedidas a esses usuários.

O conector opera usando o serviço workfront do usuário do sistema. Isso é desinstalado ao desinstalar o conector.

>[!NOTE]
>
>Se você estiver usando a versão 2.0.3 do conector e tiver adicionado o grupo `workfront-aem-connector-group`, isso também precisará ser removido, acessando **Ferramentas** > **Segurança** > **Grupos**.

## Day CQ Link Externalizer

Se você não precisar do Day CQ Link Externalizer, poderá reverter isso para `localhost:4502` acessando `/system/console/configMgr` e procurando pelo &quot;Day CQ Link Externalizer&quot;.

>[!NOTE]
>
>Se você estiver usando o Adobe Experience Manager as a Cloud Service, altere isso verificando seu projeto e localizando o arquivo _com.day.cq.commons.impl.ExternalizerImpl.xml_ dentro de _ui.apps/src/main/content/jcr_ root/apps/mysite/config_.

![Externalizador de links CQ de dias](assets/Day-CQ-Link-Externalizer.png)

## Desinstalar pacote do conector

As etapas necessárias para desinstalar o pacote do conector diferem de acordo com a versão do Adobe Experience Manager que você tem.

### Adobe Experience Manager no local

Se você estiver usando o Adobe Experience Manager no local, vá para _crx/packmgr/index.jsp_ e procure por `workfront-aem-connector.all-<version>.zip`, clique em **Mais** e depois em **Desinstalar**.

Verifique em `/conf` para ter certeza que todos os arquivos criados pela Workfront foram removidos.

### Adobe Experience Manager as a Cloud Service

Para o Adobe Experience Manager as a Cloud Service, você pode remover as dependências do conector dos arquivos pom.mbox do projeto.

## Firewall e Dispatcher

Não se esqueça de remover seus URLs do Workfront na lista de permissões se a comunicação não for mais necessária. Além disso, o conector usa a apiKey e o nome de usuário dos cabeçalhos definidos para o dispatcher. Eles também podem ser removidos.
