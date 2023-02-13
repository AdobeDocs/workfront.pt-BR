---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Fazer upload de documentos e provas do [!DNL Adobe Workfront plugin] para [!DNL Creative Cloud]
description: Fazer upload de documentos e provas do [!DNL Adobe Workfront plugin] para [!DNL Creative Cloud]
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 67952bf88a782595e13e559bfbc14ce1c622d432
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 0%

---


# Fazer upload de documentos e provas do [!DNL Adobe Workfront plugin] para [!DNL Creative Cloud]

Você pode fazer upload de seus projetos como documentos para uma revisão e aprovação rápidas ou simplesmente armazenar em [!DNL Adobe Workfront].

>[!NOTE]
>
>No momento, o upload de documentos e provas não é suportado no Premiere Pro e no After Effects.


## Limitações do documento

Esta seção descreve as limitações conhecidas de documentos no [!DNL Workfront for Adobe Creative Cloud plugins].

### As novas versões de documento aceitam apenas um arquivo para upload

Porque [!DNL Workfront] documentos não podem conter vários arquivos, determinadas configurações devem ser desativadas para carregar novas versões do documento no Workfront.

>[!NOTE]
>
>Se você precisar gerar vários arquivos, poderá criar uma prova. A nova prova não será associada ao documento original.



Para alterar sua opção de volta para um único arquivo em [!DNL InDesign]:

1. Abra o **Definir configurações do arquivo de exportação** caixa de diálogo.

   ![](assets/file-export-settings.png)

1. Localize o Tipo de ativo que deseja exportar e ajuste as configurações conforme descrito abaixo:

   <table>
    <tr>
    <td><strong>PDF e PDF-PRINT</strong>
    </td>
    <td>Desmarcar <strong>Criar arquivos PDF separados</strong>.
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>Selecionar <strong>Intervalos</strong> e digite um único número de página. 
    <p>
    <strong>Observação</strong>: Para carregar o documento completo, você deve criar uma prova. 
    </td>
    </tr>
    <tr>
    <td><strong>ePub e EPUB FIXO</strong>
    </td>
    <td>Nenhum ajuste necessário.
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>Nenhum ajuste necessário.
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>Selecionar <strong>Intervalos</strong> e digite um único número de página. 
    <p>
    <strong>Observação</strong>: Para carregar o documento completo, você deve criar uma prova. 
    </td>
    </tr>
    <tr>
    <td><strong>Imagem PNG</strong>
    </td>
    <td>Selecionar <strong>Intervalos</strong> e digite um único número de página. 
    <p>
    <strong>Observação</strong>: Para carregar o documento completo, você deve criar uma prova. 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>Nenhum ajuste necessário. 
    </td>
    </tr>
    </table>
