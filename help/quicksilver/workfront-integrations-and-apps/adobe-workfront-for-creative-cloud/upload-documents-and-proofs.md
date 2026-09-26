---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Carregar documentos e provas de [!DNL Adobe Workfront plugin] para [!DNL Creative Cloud]
description: Carregar documentos e provas de [!DNL Adobe Workfront plugin] para [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
TQID: 'https://experienceleague.adobe.com/bZsOnrrwZ7ksCaoM3jfIyeTO00XqG1hDTEmG5VmWOcA'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: a1f87682-0525-5459-aa06-3560bb4c3b2a
    internal-label: Workfront Integrations and Apps
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%
---
# Carregar documentos e provas de [!DNL Adobe Workfront plugin] para [!DNL Creative Cloud]

Você pode carregar seus projetos como documentos para revisão e aprovação rápidas ou simplesmente armazená-los em [!DNL Adobe Workfront].

>[!NOTE]
>
>Atualmente, o upload de documentos e provas não é suportado no Premiere Pro e no After Effects.


## Limitações do documento

Esta seção descreve as limitações conhecidas do documento no [!DNL Workfront for Adobe Creative Cloud plugins].

### Novas versões de documentos aceitam apenas um arquivo para upload

Como [!DNL Workfront] documentos não podem conter vários arquivos, algumas configurações devem ser desabilitadas para carregar novas versões de documentos para o Workfront.

>[!NOTE]
>
>Se precisar gerar vários arquivos, crie uma prova. A nova prova não será associada ao documento original.



Para alterar sua alternância de volta para um único arquivo em [!DNL InDesign]:

1. Abra a caixa de diálogo **Definir Configurações do Arquivo de Exportação**.

   ![Configurações de exportação de arquivo](assets/file-export-settings.png)

1. Encontre o tipo de ativo que deseja exportar e ajuste as configurações conforme descrito abaixo:

   <table>
    <tr>
    <td><strong>PDF e PDF-PRINT</strong>
    </td>
    <td>Desmarque <strong>Criar Arquivos PDF Separados</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Selecione <strong>Intervalos</strong> e digite um único número de página. 
    <p>
    <strong>Observação</strong>: se quiser carregar o documento completo, você deve criar uma prova. 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB e EPUB-FIXED</strong>
    </td>
    <td>Não são necessários ajustes.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>Não são necessários ajustes.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>Selecione <strong>Intervalos</strong> e digite um único número de página. 
    <p>
    <strong>Observação</strong>: se quiser carregar o documento completo, você deve criar uma prova. 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>Selecione <strong>Intervalos</strong> e digite um único número de página. 
    <p>
    <strong>Observação</strong>: se quiser carregar o documento completo, você deve criar uma prova. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Não são necessários ajustes. 
    </td>
    </tr>
    </table>
