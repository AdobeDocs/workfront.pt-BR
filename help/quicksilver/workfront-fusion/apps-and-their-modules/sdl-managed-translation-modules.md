---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de tradução gerenciados SDL
description: Em um [!DNL Adobe Workfront Fusion] Você pode conectar sua conta de Tradução gerenciada pelo SDL a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '481'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] módulos

Em um [!DNL Adobe Workfront Fusion] você pode conectar seu [!DNL SDL Managed Translation] para vários aplicativos e serviços de terceiros.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano*</td>
  <td> <p>[!UICONTROL Pro] ou superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td>
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licença**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Módulos

>[!NOTE]
>
>O tempo limite da operação para chamadas para [!DNL SDL Managed Translation] é **120 segundos**.

### Arquivos

#### [!UICONTROL Baixar arquivo traduzido]

Esse módulo recupera o conteúdo de um único arquivo traduzido, contido no projeto especificado. Se o arquivo solicitado ainda não estiver no status de Downland, o conteúdo do arquivo pode não ser totalmente traduzido. Se o arquivo estiver em status de Download e você o tiver recuperado com êxito, certifique-se de marcar o arquivo como concluído usando o `Cancel or Complete File` método .

#### [!UICONTROL Fazer upload de um arquivo]

Esse módulo permite uploads de arquivos para tradução ou para inclusão em um projeto de tradução como material de referência. Os uploads devem ser enviados usando multipart/form-data e podem conter mais de um arquivo. Especifique a `ProjectOptionId` que deve ser usada para avaliar os arquivos carregados. Isso determina se cada arquivo carregado é um possível candidato para tradução ou deve ser tratado como material de referência. No caso dos arquivos (`zip `, `rar`, `7z`, `tar` arquivos) o aplicativo examina o conteúdo do arquivo e indica se o arquivo como um todo pode ser traduzido ou se ele contém uma mistura de arquivos traduzíveis e não traduzíveis.

>[!NOTE]
>
>Não é recomendado fazer upload de mais de um arquivo de cada vez, pois pode aumentar o impacto de qualquer falha.

#### [!UICONTROL Adicionar um arquivo de referência]

Esse módulo adiciona um arquivo de referência.

### Projetos

#### [!UICONTROL Criar um Projeto]

Esse módulo cria o projeto especificado.

#### Cancelar ou concluir um projeto

Esse módulo cancela ou conclui o projeto especificado. Se o projeto estiver aguardando download, o projeto será transferido por meio de quaisquer etapas finais no fluxo de trabalho e, eventualmente, será movido para conclusão. Se o projeto estiver aguardando aprovação ou a seleção do fornecedor for cancelada. Se o projeto estiver em qualquer outro status, a solicitação falhará.

#### [!UICONTROL Baixar o Zip do projeto]

Esse módulo obtém o `zip` arquivo de arquivos traduzidos para o projeto especificado.

#### [!UICONTROL Ler um projeto]

Esse módulo obtém o projeto especificado.

#### [!UICONTROL Obter projetos no status]

Esse módulo obtém todos os projetos disponíveis no status especificado. Esse método permite paginar os resultados especificando: `$top`, `$skip`e `$orderby` parâmetros de consulta.

#### [!UICONTROL Obter lista de projetos]

Obtém uma lista simples de todos os projetos, fornecendo informações gerais sobre cada projeto. Esse método permite que os resultados sejam páginas, especificando `$top`, `$skip`e `$orderby` parâmetros de consulta.

#### [!UICONTROL Opções de criação de projeto de pesquisa]

Esse módulo obtém as Opções de criação do projeto.

### Outro

#### [!UICONTROL Faça uma chamada de API]

Esse módulo executa uma chamada de API autorizada arbitrária.
