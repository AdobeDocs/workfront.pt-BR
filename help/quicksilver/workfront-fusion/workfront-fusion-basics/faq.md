---
content-type: faq
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: workfront-fusion-basics
title: Perguntas frequentes sobre o Adobe Workfront Fusion
description: Este artigo aborda questões comuns relacionadas a [!DNL Adobe Workfront Fusion], incluindo informações sobre o objeto comumente usado em workflows de fusão
author: Becky
feature: Workfront Fusion
exl-id: e2ecc190-ec26-46f0-a4f2-7b283639a1eb
source-git-commit: aa58a64ea6b09192f93fa89a42a4bf6731052d10
workflow-type: tm+mt
source-wordcount: '620'
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
   <td role="rowheader">Licença da [!UICONTROL Adobe Workfront Fusion]**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> <p>[!UICONTROL [!DNL Workfront Fusion] para Automação de Trabalho]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Qual é o cenário?

### Resposta

Um cenário define uma sequência de etapas a serem executadas por [!DNL Adobe Workfront Fusion]. Para cada cenário, você especifica a fonte de dados, como os dados devem ser processados e quais dados devem ser usados e o que deve ser ignorado. [!DNL Workfront Fusion] permite criar cenários tão complexos quanto você precisa; até os cenários mais sofisticados são possíveis.

Para obter mais informações, consulte [Crie um cenário de integração de prática em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/get-started/create-a-practice-scenario.md).

## Posso usar mais de um módulo em um cenário? Ou apenas um gatilho e uma ação?

### Resposta

Você pode usar quantos módulos desejar em um cenário. Você pode criar rotas independentes e especificar quais dados devem fluir por elas. Também é possível usar os resultados retornados por ações individuais e passá-los para a próxima ação.

## Can [!DNL Workfront Fusion] trabalhar com arquivos?

### Resposta

Sim. Usando [!DNL Workfront Fusion], os arquivos podem ser recebidos, salvos, transformados, convertidos, criptografados e assim por diante. Além disso, [!DNL Workfront Fusion] O oferece uma ampla variedade de recursos integrados criados para permitir que os usuários trabalhem de forma eficaz e criativa com os dados contidos nos arquivos.

Para obter mais informações, consulte [Sobre o mapeamento de arquivos no [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md).

## O que acontece se eu deixar [!DNL Workfront Fusion] processar um email contendo mais de um anexo?

### Resposta

Se você usar a variável [!UICONTROL Email] módulo [!UICONTROL Recuperar anexos], cada anexo é enviado individualmente por meio do restante dos módulos no cenário. Módulos semelhantes também estão disponíveis em outros aplicativos que recebem vários arquivos de uma só vez.

Para obter mais informações, consulte [[!UICONTROL Email] módulos](../../workfront-fusion/apps-and-their-modules/email-modules.md).

## Alguns acionadores permitem que cenários sejam executados instantaneamente. O que significa &quot;instantaneamente&quot;?

### Resposta

Cenários comuns são executados em intervalos de acordo com o agendamento especificado (por exemplo, a cada hora, a cada 5 minutos, uma vez por mês e assim por diante). Há acionadores especiais, chamados de acionadores instantâneos (webhooks), que podem iniciar o cenário imediatamente após receber dados de um determinado serviço. Os acionadores instantâneos podem ser extremamente úteis. Recomendamos usá-los sempre que possível. Eles ajudam a reduzir o número de operações. Os dados recebidos são processados imediatamente sem esperar a próxima execução agendada. Por exemplo, a variável [!DNL Google Sheets] módulo [!UICONTROL Monitoramento de alterações] inicia um cenário imediatamente após a atualização de uma célula.

## O que são agregadores?

### Resposta

Um [!UICONTROL Agregador] mescla dados em uma única coleção. Um exemplo disso são arquivos compactados em um arquivo zip e enviados como um anexo de email.

Para obter mais informações, consulte [[!UICONTROL Agregador] módulo em [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## O que é uma operação?

### Resposta

Uma operação é qualquer tarefa executada por um módulo. Uma operação ocorre, por exemplo, sempre que um acionador é executado e sempre que uma ação executa uma tarefa.

## O que é transferência de dados?

### Resposta

A transferência de dados se refere à quantidade de dados transferida por meio do seu cenário. Por exemplo, suponha que você tenha um cenário que recupera uma imagem de 100 KB do FTP e reduz seu tamanho para 50 KB e salva ambas as imagens no [!DNL Dropbox]. A quantidade de dados usada neste cenário é de 150 KB.

## O que é uma conexão?

### Resposta

Uma conexão é o link entre as [!DNL Workfront Fusion] e o serviço de terceiros que deseja usar. A conexão pode ser facilmente criada ao editar um cenário. Para adicionar uma conexão, clique no botão **[!UICONTROL Adicionar]** na configuração do módulo e siga as instruções passo a passo.

Para obter mais informações, consulte [Sobre a conexão [!DNL Adobe Workfront Fusion] para um aplicativo ou serviço](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).
