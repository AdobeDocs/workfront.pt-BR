---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Desinstale o conector herdado
description: texto
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4b3834bf-2e6d-4588-8d77-671e14390115
source-git-commit: 3a1bc4a56cba2fe224a1f0a21c8882c2d9d030de
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 0%

---

# Desinstale o Workfront com o conector herdado do Adobe Experience Manager

Você deve desinstalar o conector herdado do Workfront com Adobe Experience Manager para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.

## Cancelar inscrição no Workfront

1. Abra o Adobe Experience Manager.
1. No Experience Manager, acesse **Ferramentas** > **Cloud Services** > **Configuração de integração do Workfront**.
1. Selecione sua configuração (global-workfront por padrão) e clique em **Propriedades**.
   ![cancelar inscrição na frente de trabalho](assets/unsubscribe-from-workfront.png)
1. Desative Documento, Comentário e Sincronização de Metadados. O rótulo deve ser o dia Desativado.
Isso removerá as assinaturas no Workfront e permitirá que o usuário crie uma nova assinatura usando o mesmo url definido no Day CQ Link Externalizer.

## Excluir a configuração de integração do Workfront

Após remover a assinatura, agora é seguro excluir a Configuração de integração do Workfront.

1. Abra a configuração e selecione **Excluir**.
   ![excluir configuração](assets/delete-wf-configuration.png)

## Remover mapeamento

Em seguida, é necessário excluir o Mapeamento de propriedades do Workfront.

1. No Experience Manager, acesse **Ferramentas** > **Ativos** > **Mapeamento de propriedades do Workfront**.

1. Selecione todos os mapeamentos e clique em **Excluir**.

## Permissões do usuário

Todos os usuários que acessam AEM Dam do Workfront receberam permissões de leitura para `/content/dam`. Se um usuário não precisar mais disso, você poderá remover as permissões fornecidas a esses usuários.

O conector opera usando o serviço front-service do usuário do sistema. Isso é desinstalado ao desinstalar o conector.

>[!NOTE]
>
>Se estiver usando o conector versão 2.0.3 e tiver adicionado o grupo `workfront-aem-connector-group`, isso também precisa ser removido indo **Ferramentas** > **Segurança** > **Grupos**.

## Externalizador de links CQ do dia

Se você não precisar do Day CQ Link Externalizer, poderá reverter para `localhost:4502` ao `/system/console/configMgr` e procurando pelo &#39;Day CQ Link Externalizer&#39;.

>[!NOTE]
>
>Se estiver usando o Adobe Experience Manager as a Cloud Service, você pode alterá-lo pesquisando no seu projeto e localizando o arquivo _com.day.cq.commons.impl.ExternalizerImpl.xml_ inside _ui.apps/src/main/content/jcr_root/apps/mysite/config_.

![Externalizador de links CQ do dia](assets/Day-CQ-Link-Externalizer.png)

## Desinstalar Pacote do Conector

As etapas necessárias para desinstalar o pacote de conectores diferem de acordo com qual versão do Adobe Experience Manager você tem.

### Adobe Experience Manager no local

Se estiver usando o Adobe Experience Manager no local, acesse _crx/packmgr/index.jsp_ e procure o `workfront-aem-connector.all-<version>.zip`, clique em **Mais** e depois **Desinstalar**.

Verifique em `/conf` para verificar se todos os arquivos criados pelo Workfront foram removidos.

### Adobe Experience Manager as a Cloud Service

Para o Adobe Experience Manager as a Cloud Service, você pode remover as dependências do conector dos arquivos pom.do projeto.

## Firewall e Dispatcher

Não se esqueça de remover seus URLs Workfront da lista de permissões se a comunicação não for mais necessária. Além disso, o conector usa os cabeçalhos apiKey e o nome de usuário que foi definido para o dispatcher. Eles também podem ser removidos.
