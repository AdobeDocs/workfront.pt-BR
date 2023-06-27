---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: conector
navigation-topic: apps-and-their-modules
title: Módulos de tradução gerenciados por SDL
description: Em um [!DNL Adobe Workfront Fusion] cenário, você pode conectar sua conta do SDL Managed Translation a vários aplicativos e serviços de terceiros.
author: Becky
feature: Workfront Fusion
exl-id: e1ef114f-8ce4-4210-b176-727dc4f5e561
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '529'
ht-degree: 1%

---

# [!DNL SDL Managed Translation] módulos

Em um [!DNL Adobe Workfront Fusion] cenário, você pode conectar seu [!DNL SDL Managed Translation] conta para vários aplicativos e serviços de terceiros.

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
   <td>
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e integração do trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o [!UICONTROL Select] ou o [!UICONTROL Prime] [!DNL Adobe Workfront] Planejar, sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no [!UICONTROL Ultimate] [!DNL Workfront] plano.</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir que plano, tipo de licença ou acesso você tem, entre em contato com o [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!DNL SDL Managed Translation] Módulos

>[!NOTE]
>
>O tempo limite da operação para chamadas a [!DNL SDL Managed Translation] é **120 segundos**.

### Arquivos

#### [!UICONTROL Baixar arquivo traduzido]

Este módulo recupera o conteúdo de um único arquivo traduzido, contido no projeto especificado. Se o arquivo solicitado ainda não estiver no status Downland, talvez o conteúdo do arquivo ainda não tenha sido totalmente traduzido. Se o arquivo estiver no status Download e você o tiver recuperado com êxito, certifique-se de marcar o arquivo como concluído usando o `Cancel or Complete File` método.

#### [!UICONTROL Carregar um arquivo]

Esse módulo permite uploads de arquivos para tradução ou para inclusão em um projeto de tradução como material de referência. Os carregamentos devem ser enviados usando várias partes/dados de formulário e podem conter mais de um arquivo. Você especifica a `ProjectOptionId` que deve ser usado para avaliar os arquivos carregados. Isso determina se cada arquivo carregado é um possível candidato para tradução ou deve ser tratado como material de referência. No caso dos arquivos (`zip `, `rar`, `7z`, `tar` arquivos) o aplicativo examina o conteúdo do arquivamento e indica se o arquivamento como um todo pode ser traduzido ou se contém uma mistura de arquivos traduzíveis e não traduzíveis.

>[!NOTE]
>
>O upload de mais de um arquivo por vez não é recomendado, pois pode aumentar o impacto de qualquer falha.

#### [!UICONTROL Adicionar um arquivo de referência]

Este módulo adiciona um arquivo de referência.

### Projetos

#### [!UICONTROL Criar um Projeto]

Este módulo cria o projeto especificado.

#### Cancelar ou concluir um projeto

Este módulo cancela ou conclui o projeto especificado. Se o projeto estiver aguardando o download, ele passará por todas as etapas finais do fluxo de trabalho e, eventualmente, será movido para a conclusão. Se o projeto estiver aguardando aprovação ou a seleção do fornecedor for cancelada. Se o projeto estiver em qualquer outro status, a solicitação falhará.

#### [!UICONTROL Baixar o zip do projeto]

Este módulo obtém o `zip` arquivo de arquivos traduzidos para o projeto especificado.

#### [!UICONTROL Ler um projeto]

Este módulo obtém o projeto especificado.

#### [!UICONTROL Obter Projetos com Status]

Este módulo obtém todos os projetos disponíveis no status especificado. Esse método permite que os resultados sejam paginados, especificando `$top`, `$skip`, e `$orderby` parâmetros de consulta.

#### [!UICONTROL Obter lista de projetos]

Obtém uma lista simples de todos os projetos, fornecendo informações gerais sobre cada projeto. Esse método permite que os resultados sejam páginas, especificando `$top`, `$skip`, e `$orderby` parâmetros de consulta.

#### [!UICONTROL Pesquisar opções de criação de projeto]

Este módulo obtém Opções de Criação de Projeto.

### Outro

#### [!UICONTROL Fazer uma chamada de API]

Esse módulo executa uma chamada de API autorizada arbitrária.
