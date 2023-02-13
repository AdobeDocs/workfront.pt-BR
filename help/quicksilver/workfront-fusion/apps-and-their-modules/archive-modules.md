---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Arquivar módulos
description: Em um [!DNL Adobe Workfront Fusion] você pode conectar um arquivo, como um arquivo zipado, a vários aplicativos e serviços de terceiros. Por exemplo, você pode configurar um cenário que
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL Arquivar] módulos

Em um [!DNL Adobe Workfront Fusion] no seu cenário, é possível usar um arquivo, como um arquivo zipado, para usá-lo em suas automações ou integrações.

Se precisar de instruções para criar um cenário, consulte [Crie um cenário em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Para obter informações sobre módulos, consulte [Módulos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Arquivar] módulos e seus campos

Ao configurar [!UICONTROL Arquivar] módulos, [!DNL Workfront Fusion] exibe os campos listados abaixo. Junto com esses, [!UICONTROL Arquivar] podem ser exibidos, dependendo de fatores como seu nível de acesso no aplicativo ou serviço. Um título em negrito em um módulo indica um campo obrigatório.

Se o botão de mapa for exibido acima de um campo ou função, é possível usá-lo para definir variáveis e funções para esse campo. Para obter mais informações, consulte [Mapear informações de um módulo para outro no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extrair um arquivo]](#extract-an-archive)
* [[!UICONTROL Criar um arquivo]](#create-an-archive)
* [[!UICONTROL Inflar]](#inflate)
* [[!UICONTROL Defender]](#deflate)

## [!UICONTROL Extrair um arquivo]

Esse módulo de ação extrai um arquivo identificado a partir de um arquivo.

O módulo retorna a ID do arquivo e quaisquer campos associados, juntamente com quaisquer campos e valores personalizados que a conexão acessa. Você pode mapear essas informações em módulos subsequentes do cenário.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td> <p> Selecione o arquivo que deseja extrair. Esse arquivo pode ser mapeado de um módulo anterior (como o [!DNL Workfront] &gt; [!UICONTROL Baixar um documento] módulo).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** Obtenha o arquivo ZIP do [!DNL Dropbox] pasta (por exemplo, Arquivos), extraia-a usando o [!UICONTROL Arquivar] e enviar arquivos extraídos para o endereço de email desejado como anexos com o [!UICONTROL Email] ou [!DNL Gmail] módulo.
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Criar um arquivo]

Esse módulo agregador adiciona os arquivos desejados a um [!UICONTROL ZIP] ou [!UICONTROL TAR] arquivo.

Ao configurar esse módulo, os seguintes campos são exibidos.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Módulo de origem]</td> 
   <td> <p> Selecione o módulo do qual deseja recuperar os arquivos.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tipo] </td> 
   <td> <p>Selecione se deseja adicionar arquivos a um arquivo [!UICONTROL ZIP] ou a um arquivo [!UICONTROL TAR].</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comentário]</td> 
   <td>Insira um comentário que deseja adicionar ao arquivo.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Agrupar por]</td> 
   <td> <p>Defina uma expressão pela qual deseja agrupar a saída agregada. Essa expressão pode conter um ou mais itens mapeados. Os dados agregados serão então separados em grupos usando o valor dessa expressão. Cada grupo é gerado como um pacote separado com uma chave (a expressão avaliada) e um valor (o texto agregado). Você pode usar a chave como filtro em módulos subsequentes.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parar o processamento após uma agregação vazia]</td> 
   <td>Selecione essa opção para interromper o cenário quando não houver resultados.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Nome do arquivo]</td> 
   <td> <p> Insira um nome para o arquivo criado. Não adicione uma extensão.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Arquivo de origem]</td> 
   <td> <p>Selecione um arquivo de origem de um módulo anterior ou mapeie o nome e os dados do arquivo de origem.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exemplo:** Assista aos emails recebidos usando o [!DNL Gmail] >[!UICONTROL Assistir a emails] módulo. Se um email for recebido, seus anexos serão iterados em pacotes individuais e arquivados no [!DNL ZIP] e salvas na pasta Dropbox definida.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflar]

Esse módulo transformador descompacta dados binários usando um algoritmo de inflação.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dados] </td> 
   <td> <p>Insira ou mapeie os dados que deseja descompactar usando a função inflar.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Defender]

Esse módulo transformador compacta dados binários usando um algoritmo de deflação.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Dados] </td> 
   <td> <p>Insira ou mapeie os dados que deseja compactar usando a função deflate .</p> </td> 
  </tr> 
 </tbody> 
</table>
