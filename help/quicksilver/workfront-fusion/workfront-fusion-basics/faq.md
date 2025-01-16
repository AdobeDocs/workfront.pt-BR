---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Perguntas frequentes sobre o Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 1%

---

# Perguntas frequentes sobre o Adobe Workfront Fusion

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Perguntas frequentes sobre o planejamento de cenário](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/plan-a-scenario/faq.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

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
   <p>Requisito de licença herdada: [!UICONTROL [!DNL Workfront Fusion] para Automação e Integração do Trabalho], [!UICONTROL [!DNL Workfront Fusion] para Automação do Trabalho]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Requisito atual do produto: se você tiver o Plano [!DNL Adobe Workfront] da [!UICONTROL Select] ou da [!UICONTROL Prime], sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo. [!DNL Workfront Fusion] está incluído no plano [!DNL Workfront] da [!UICONTROL Ultimate].</p>
   <p>Ou</p>
   <p>Requisito de produto herdado: sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para saber que plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## O que é um cenário?

### Responder

Um cenário define uma sequência de etapas a serem executadas por [!DNL Adobe Workfront Fusion]. Para cada cenário, especifique a fonte de dados, como os dados devem ser processados, quais dados devem ser usados e o que deve ser ignorado. O [!DNL Workfront Fusion] permite criar os cenários mais complexos que você precisa; até mesmo os cenários mais sofisticados são possíveis.

Para obter mais informações, consulte [Criar um cenário de integração de prática [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Posso usar mais de um módulo em um cenário? Ou apenas um gatilho e ação?

### Responder

Você pode usar quantos módulos desejar em um cenário. Você pode criar rotas independentes e especificar quais dados devem fluir através delas. Você também pode usar os resultados retornados por ações individuais e passá-los para a próxima ação.

## [!DNL Workfront Fusion] pode trabalhar com arquivos?

### Responder

Sim. Usando o [!DNL Workfront Fusion], os arquivos podem ser recebidos, salvos, transformados, convertidos, criptografados e assim por diante. Além disso, o [!DNL Workfront Fusion] fornece uma ampla variedade de recursos incorporados criados para permitir que os usuários trabalhem de forma eficaz e criativa com os dados contidos nos arquivos.

Para obter mais informações, consulte [Sobre o mapeamento de arquivos em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## O que acontece se eu permitir que o [!DNL Workfront Fusion] processe um email contendo mais de um anexo?

### Responder

Se você usar o módulo [!UICONTROL Email] [!UICONTROL Recuperar anexos], cada anexo será enviado individualmente através do restante dos módulos no cenário. Módulos semelhantes também estão disponíveis em outros aplicativos que recebem vários arquivos de uma só vez.

Para obter mais informações, consulte [[!UICONTROL Email] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Alguns acionadores permitem que os cenários sejam executados instantaneamente. O que significa &quot;instantaneamente&quot;?

### Responder

Cenários comuns são executados em intervalos de acordo com o agendamento especificado (por exemplo, a cada hora, a cada 5 minutos, uma vez por mês e assim por diante). Há acionadores especiais, chamados de acionadores instantâneos (webhooks), que podem iniciar seu cenário imediatamente após receberem dados de um determinado serviço. Os acionadores instantâneos podem ser extremamente úteis. Recomendamos usá-los sempre que possível. Eles ajudam a reduzir o número de operações. Os dados recebidos são processados imediatamente sem esperar a próxima execução programada. Por exemplo, o módulo [!DNL Google Sheets] [!UICONTROL Observar alterações] inicia um cenário imediatamente após a atualização de uma célula.

## O que são agregadores?

### Responder

Um [!UICONTROL Agregador] mescla dados em uma única coleção. Um exemplo disso são arquivos compactados em um arquivo zip e enviados como um anexo de email.

Para obter mais informações, consulte o módulo [[!UICONTROL Agregador] em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## O que é uma operação?

### Responder

Uma operação é qualquer tarefa executada por um módulo. Uma operação ocorre, por exemplo, toda vez que um acionador é executado e toda vez que uma ação executa uma tarefa.

## O que é transferência de dados?

### Responder

Transferência de dados refere-se à quantidade de dados transferidos pelo seu cenário. Por exemplo, suponha que você tenha um cenário que recupere uma imagem de 100 KB do FTP e reduza seu tamanho para 50 KB, além de salvar as duas imagens em [!DNL Dropbox]. A quantidade de dados usada nesse cenário é de 250 KB.

## O que é uma conexão?

### Responder

Uma conexão é o vínculo entre sua conta do [!DNL Workfront Fusion] e o serviço de terceiros que você deseja usar. A conexão pode ser facilmente criada ao editar um cenário. Para adicionar uma conexão, clique no botão **[!UICONTROL Adicionar]** na configuração do módulo e siga as instruções passo a passo.

Para obter mais informações, consulte [Visão geral das conexões](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
