---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Tipos de dados de item em  [!DNL Adobe Workfront Fusion]
description: Seus  [!DNL Adobe Workfront Fusion] cenários podem conter os tipos de itens listados abaixo em um pacote.
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 0%

---

# Tipos de dados de item em [!DNL Adobe Workfront Fusion]

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plano*</td> 
   <td> <p>[!DNL Pro] ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licença*</td> 
   <td> <p>[!UICONTROL Plano], [!UICONTROL Trabalho]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td>
   <p>Requisito de licença atual: nenhum requisito de licença [!DNL Workfront Fusion].</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] do [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Tipos de dados de item

Você pode conter os tipos de itens listados abaixo em um pacote.

Para obter informações sobre quais tipos de itens [!DNL Workfront Fusion] permitem a conversão entre si, consulte [Coerção de tipo em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Texto</p> </td> 
   <td> <p>O tipo de item mais comum. Para alguns itens de texto, o [!DNL Adobe Workfront Fusion] verifica se o comprimento máximo ou mínimo permitido foi atingido ou se o item executa a validação de formato (email, URL ou nome de arquivo).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Número</p> </td> 
   <td> <p>Para alguns itens numéricos, [!DNL Workfront Fusion] pode validar a entrada para um intervalo especificado (o valor mínimo ou máximo permitido).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Booleano (Sim/Não)</p> </td> 
   <td> <p>Esse tipo é usado para itens com apenas dois valores possíveis: verdadeiro ou falso. </p> <p>Ao definir módulos, o tipo Booleano pode aparecer de duas formas diferentes:</p> 
    <ul> 
     <li> <p>A caixa de seleção obrigatória é exibida caso o campo seja obrigatório e deva ser preenchido.</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>Campos opcionais que podem ser deixados em branco são exibidos como uma caixa de seleção, permitindo a seleção entre três valores: <code>Yes</code>, <code>No</code> e <code>Not defined</code> (padrão).</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>Você pode clicar em <strong>[!UICONTROL Mapa]</strong> se precisar mapear o valor para um item de outro módulo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Data</p> </td> 
   <td> <p>As datas são inseridas no formato de data ISO 8601, por exemplo, <code>2015-09-18T11:58Z</code>. Você pode alterar o fuso horário nas configurações do seu perfil, conforme explicado em <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">Alterar configurações do perfil em [!DNL Adobe Workfront Fusion]</a>. </p> <p>Se você clicar em um campo que requer uma data, um calendário pop-up será exibido nas configurações do módulo. O tempo não é necessário para alguns itens.</p> <p>Os valores dos itens de Data são formatados usando o fuso horário local e da Web selecionado no seu perfil. É possível exibir a versão ISO 8601 do valor de um item de data, passando o mouse sobre o item.</p> <p>Observação: se o valor ISO não for exibido, o item provavelmente é um texto, não uma data.</p> <p>A hora é inserida no formato <code>hours:minutes:seconds</code>, por exemplo, <code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Buffer (dados binários)</p> </td> 
   <td> <p>O conteúdo do arquivo geralmente é enviado como conteúdo do tipo Buffer (conteúdo de imagem, arquivo de vídeo e outros). Em alguns casos, dados de texto são incluídos nesse tipo (por exemplo, um arquivo de texto). O [!DNL Workfront Fusion] pode converter automaticamente dados de texto em código binário em texto e texto em dados de texto em código binário. Para obter mais informações, consulte <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">Sobre o mapeamento de arquivos no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Coleção</p> </td> 
   <td> <p>Uma coleção é um item que consiste em vários subitens. O item Remetente em uma mensagem de email é um exemplo de uma coleção: ele contém o nome do remetente (tipo de texto) e o endereço de email do remetente (tipo de texto).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Selecionar (menu)</p> </td> 
   <td> <p>Ao definir as configurações do módulo conforme descrito em <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">Definir as configurações de um módulo no [!DNL Adobe Workfront Fusion]</a>, você pode selecionar entre vários itens do mesmo tipo. Um exemplo é o menu de seleção de pasta nas configurações dos módulos [!DNL Dropbox]. </p> <p>Ao configurar módulos, o menu de seleção pode aparecer de duas formas:</p> <p> <p>Se for possível fazer várias seleções, vários itens com caixas de seleção serão exibidos.</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>Se apenas uma opção for possível, um menu suspenso será exibido.</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>Se você precisar mapear um item de outro módulo, use o botão <strong>Mapear</strong>. Esse botão abre um campo de texto em vez do menu de seleção. Para obter mais informações, consulte <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">Mapear informações de um módulo para outro em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Matriz</p> </td> 
   <td> <p>Você pode usar o tipo de matriz para trabalhar com vários valores do mesmo tipo, incluindo coleções. Um exemplo são os módulos [!UICONTROL Email]: eles retornam uma matriz de anexos e cada anexo contém nome, conteúdo, tamanho e assim por diante. Para obter mais informações, consulte <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">Mapear uma matriz em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Validação</p> </td> 
   <td> <p>[!DNL Workfront Fusion] executar a validação em cada tipo de item. Se um item não passar na validação, o módulo parará de ser processado devido a um erro de dados. Para obter mais informações, consulte <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">Processamento de erros em [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
