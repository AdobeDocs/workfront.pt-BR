---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Desinstale o conector aprimorado do Workfront para Adobe Experience Manager
description: Você deve desinstalar o conector aprimorado do Workfront com Adobe Experience Manager para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: c6203c71-a4c4-41ee-ac4e-57137661e5b3
source-git-commit: 9673009f12509b5e7051ee91e142d311f333f215
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 0%

---

# Desinstale o conector aprimorado do Workfront com Adobe Experience Manager

Você deve desinstalar o conector aprimorado do Workfront com Adobe Experience Manager para a integração nativa mais recente que conecta o Workfront e o Adobe Experience Manager Assets as a Cloud Service.

## Pré-requisitos

* (Opcional) Se necessário, reverta quaisquer alterações feitas nas configurações do Workfront firewall e do AEM dispatcher.

## Desinstale o conector aprimorado

1. Acesse e clone seu repositório do AEM as a Cloud Service no Cloud Manager.

1. Abra o repositório Git clonado no IDE de sua escolha.

1. Confira a ramificação onde o conector aprimorado está instalado.

1. Navegue até o seguinte caminho e remova o arquivo zip do conector aprimorado:

   `Path: /ui.apps/src/main/resources/<zip file will be here>`

1. Remova a seguinte dependência do arquivo pom.xml da raiz do projeto.

   ```
   <!-- Workfront Tools -->
    <dependency>
        <groupId>digital.hoodoo</groupId>
        <artifactId>workfront-tools.ui.apps</artifactId>
        <type>zip</type>
        <version>1.8.0</version>
        <scope>system</scope>
        <systemPath>${project.basedir}/ui.apps/src/main/resources/workfront-tools.ui.apps.zip</systemPath>
    </dependency>
   ```

   >[!NOTE]
   >
   >Verifique se a versão referenciada no bloco de código acima, ou seja, a 1.8.0, reflete a versão que está sendo desinstalada do código.

1. Remova a seguinte dependência do arquivo pom.xml do submódulo do projeto denominado **all**.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. Remova o seguinte incorporado do arquivo pom.xml do submódulo do projeto chamado all.

   ```
   <!-- Workfront Tools -->
   <embedded>
       <groupId>digital.hoodoo</groupId>
       <artifactId>workfront-tools.ui.apps</artifactId>
       <type>zip</type>
       <target>/apps/<path-to-project-install-folder>/install</target>
   </embedded>
   ```

1. (Condicional) Remova a configuração do repositório do arquivo pom.xml da raiz do projeto.


   ```
   <repository>
       <id>hoodoo-maven</id>
       <name>Hoodoo Repository</name>
       <url>https://gitlab.com/api/v4/projects/12715200/packages/maven</url>
   </repository>
   ```

1. (Condicional) Remova a configuração do servidor do settings.xml, presente no seguinte caminho ./cloudmanager/maven/settings.xml na raiz do projeto.&#39;

   ```
           <server>
           <id>hoodoo-maven</id>
           <configuration>
               <httpHeaders>
                   <property>
                       <name>Deploy-Token</name>
                       <value>*********************</value>
                   </property>
               </httpHeaders>
           </configuration>
       </server>
   ```

1. Confirme as alterações e envie o código para o repositório do Cloud Manager

1. Execute o pipeline do Cloud Manager para implantar as alterações na instância do Cloud Service
