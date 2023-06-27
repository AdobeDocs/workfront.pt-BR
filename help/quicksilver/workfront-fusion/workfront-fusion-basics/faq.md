---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Perguntas frequentes sobre o Adobe Workfront Fusion
description: Este artigo aborda perguntas comuns relacionadas ao [!DNL Adobe Workfront Fusion], incluindo informações sobre objetos comumente usados em workflows do Fusion
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: f2d67401782abc7e7714d9e14c495a4a6ba2fcc7
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 0%

---

# Perguntas frequentes sobre o Adobe Workfront Fusion

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
   <p>Requisito de licença atual: Não [!DNL Workfront Fusion] requisito de licença.</p>
   <p>Ou</p>
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para automação de trabalho]</p>
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

## O que é um cenário?

### Resposta

Um cenário define uma sequência de etapas a serem executadas pelo [!DNL Adobe Workfront Fusion]. Para cada cenário, especifique a fonte de dados, como os dados devem ser processados, quais dados devem ser usados e o que deve ser ignorado. [!DNL Workfront Fusion] O permite criar os cenários mais complexos que você precisar; até mesmo os cenários mais sofisticados são possíveis.

Para obter mais informações, consulte [Criar um cenário de integração de prática no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Posso usar mais de um módulo em um cenário? Ou apenas um gatilho e ação?

### Resposta

Você pode usar quantos módulos desejar em um cenário. Você pode criar rotas independentes e especificar quais dados devem fluir através delas. Você também pode usar os resultados retornados por ações individuais e passá-los para a próxima ação.

## Pode [!DNL Workfront Fusion] trabalhar com arquivos?

### Resposta

Sim. Usar [!DNL Workfront Fusion], os arquivos podem ser recebidos, salvos, transformados, convertidos, criptografados e assim por diante. Além disso, [!DNL Workfront Fusion] O fornece uma grande variedade de recursos incorporados criados para permitir que os usuários trabalhem de maneira eficaz e criativa com os dados contidos nos arquivos.

Para obter mais informações, consulte [Sobre o mapeamento de arquivos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## O que acontece se eu deixar [!DNL Workfront Fusion] processar um email contendo mais de um anexo?

### Resposta

Se você usar o [!UICONTROL E-mail] módulo [!UICONTROL Recuperar anexos], cada anexo é enviado individualmente por meio do restante dos módulos no cenário. Módulos semelhantes também estão disponíveis em outros aplicativos que recebem vários arquivos de uma só vez.

Para obter mais informações, consulte [[!UICONTROL E-mail] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Alguns acionadores permitem que os cenários sejam executados instantaneamente. O que significa &quot;instantaneamente&quot;?

### Resposta

Cenários comuns são executados em intervalos de acordo com o agendamento especificado (por exemplo, a cada hora, a cada 5 minutos, uma vez por mês e assim por diante). Há acionadores especiais, chamados de acionadores instantâneos (webhooks), que podem iniciar seu cenário imediatamente após receberem dados de um determinado serviço. Os acionadores instantâneos podem ser extremamente úteis. Recomendamos usá-los sempre que possível. Eles ajudam a reduzir o número de operações. Os dados recebidos são processados imediatamente sem esperar a próxima execução programada. Por exemplo, a variável [!DNL Google Sheets] módulo [!UICONTROL Observar alterações] inicia um cenário imediatamente após a atualização de uma célula.

## O que são agregadores?

### Resposta

Um [!UICONTROL Agregador] mescla dados em uma única coleção. Um exemplo disso são arquivos compactados em um arquivo zip e enviados como um anexo de email.

Para obter mais informações, consulte [[!UICONTROL Agregador] módulo no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## O que é uma operação?

### Resposta

Uma operação é qualquer tarefa executada por um módulo. Uma operação ocorre, por exemplo, toda vez que um acionador é executado e toda vez que uma ação executa uma tarefa.

## O que é transferência de dados?

### Resposta

Transferência de dados refere-se à quantidade de dados transferidos pelo seu cenário. Por exemplo, suponha que você tenha um cenário que recupere uma imagem de 100 KB do FTP e reduza seu tamanho para 50 KB, além de salvar as duas imagens em [!DNL Dropbox]. A quantidade de dados usada nesse cenário é de 250 KB.

## O que é uma conexão?

### Resposta

Uma conexão é o link entre seu [!DNL Workfront Fusion] e o serviço de terceiros que deseja usar. A conexão pode ser facilmente criada ao editar um cenário. Para adicionar uma conexão, clique no link **[!UICONTROL Adicionar]** na configuração do módulo e siga as instruções passo a passo.

Para obter mais informações, consulte [Sobre a conexão [!DNL Adobe Workfront Fusion] para um aplicativo ou serviço](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
