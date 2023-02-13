---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Termos básicos no Adobe Workfront Fusion
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Termos básicos em [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] exige um [!DNL Adobe Workfront Fusion] além de um [!UICONTROL Adobe Workfront] licença.


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Ação</p> </td> 
   <td>Um módulo que permite ler ou gravar pacotes de ou para um aplicativo ou serviço selecionado.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>Um tipo de módulo que une vários pacotes (vários arrays de dados) em um único pacote. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">Módulo [!UICONTROL Aggregator] no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Chave de API</td> 
   <td>Um código exclusivo que identifica o usuário, desenvolvedor ou programa que está chamando a API de um software, usado para autenticação. Since [!DNL Adobe Workfront Fusion] módulos funcionam conectando APIs, chaves de API às vezes são necessárias. As chaves da API são distribuídas pelo aplicativo que requer elas. Por exemplo, se você precisar de uma chave de API para [!DNL ActiveCampaign], você solicitaria por meio de [!DNL ActiveCampaign] conta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aplicativo ou serviço</td> 
   <td> <p>Um aplicativo de software, mais comumente.</p> <p>Um aplicativo também pode ser uma função especial que manipula dados, como um iterador ou um agregador. </p> <p>Um serviço é uma fonte de pacotes que pode incluir uma API da Web, página da Web, diferentes tipos de servidores (FTP, SMTP, IMAP) e assim por diante. </p> <p> <img src="assets/apps-350x420.jpg" style="width: 350;height: 420;"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conector do aplicativo</td> 
   <td>Um aplicativo que se conecta a outro sistema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Pacote</p> </td> 
   <td> <p>Um pacote é uma unidade básica retornada ou recebida por módulos. Um pacote consiste em itens.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Ao adicionar um aplicativo ou serviço a um cenário, provavelmente será necessário primeiro criar uma conexão entre [!DNL Workfront Fusion] e o aplicativo ou serviço para recuperar ou enviar os dados selecionados. Para obter mais informações, consulte <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Sobre a conexão [!DNL Adobe Workfront Fusion] para um aplicativo ou serviço</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ciclo</p> </td> 
   <td> <p>Um ciclo se refere a duas fases da execução do cenário: operação e confirmação. O cenário pode consistir em um ou mais ciclos. Para obter informações mais detalhadas, consulte <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Execução do cenário, ciclos e fases em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Armazenamento de dados</p> </td> 
   <td> <p>Uma ferramenta que armazena dados de cenários ou permite transferir dados entre cenários individuais ou execuções de cenários. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Armazenamento de dados no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transferência de dados</p> </td> 
   <td> <p>A quantidade de dados transferidos por meio do seu cenário. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Detalhes do cenário no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filtro</p> </td> 
   <td> <p>Recursos adicionais que podem ser aplicados entre dois módulos. Um filtro permite que você trabalhe somente com pacotes que se encaixam em determinados critérios. Você pode aplicar vários filtros diferentes. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adicionar um filtro a um cenário no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>Um nome usado para identificar exclusivamente um pacote. Normalmente, uma ID é usada para diferenciar um pacote que deve ser atualizado ou excluído de um determinado serviço.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Itens</p> </td> 
   <td> <p>Uma parte de um pacote. Os pacotes podem consistir em vários itens. Existem vários tipos diferentes de itens: texto, número, booleano (sim/não), data, hora, buffer (dados binários), coleções, menu de seleção, matriz e validação.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>Um tipo de módulo que permite pegar um pacote de dados (uma matriz de dados) e dividir em pacotes separados. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Módulo [!UICONTROL Iterator] em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Módulo</p> </td> 
   <td> <p>Uma única etapa em um cenário que executa uma função, como criar um registro, no aplicativo ou serviço associado.</p> <p>Cada aplicativo ou serviço tem vários módulos que definem a forma como ele responde a uma solicitação.</p> <p>Há quatro tipos de módulos: ações, acionadores, iteradores e agregadores.</p> <p> <img src="assets/module.jpg"> </p> <p>Para obter mais informações, consulte <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Operação</p> </td> 
   <td> <p>Uma tarefa executada por um módulo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Chaves públicas/privadas</td> 
   <td>Chaves públicas e privadas são usadas para criptografar e descriptografar dados. A chave pública pode ser distribuída e qualquer pessoa com a chave pública pode criptografar dados, mas somente a chave privada pode descriptografá-los. Da mesma forma, um usuário com uma chave privada pode criptografar dados que qualquer pessoa com a chave pública pode descriptografar. A criptografia de chave privada garante que os dados sejam provenientes do proprietário da chave privada e sirvam como validação da fonte de dados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>Permite duplicar dados ou adicionar novas rotas a um cenário, para rotear novamente os dados e lidar com diferentes grupos de dados separadamente. Para obter mais informações, consulte <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">Módulo [!UICONTROL Router] em [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Cenário</p> </td> 
   <td> <p>Uma série de etapas automatizadas criadas pelo usuário, cada uma representada e executada por um módulo. A finalidade de um cenário é mover e manipular dados.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Criar um cenário no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transações</p> </td> 
   <td> <p>[!DNL Workfront Fusion] O usa o processamento transacional para capturar o ciclo de vida do cenário. Uma transação consiste em várias fases durante as quais os dados são transformados de um estado consistente em outro estado consistente. Há 4 fases: inicialização, operação (leitura ou gravação), confirmação/reversão e finalização.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Acionador</p> </td> 
   <td> <p>Um módulo que permite capturar pacotes que foram adicionados ou atualizados desde a última execução de um cenário. Há dois tipos de acionadores: polling e instantâneo (webhooks). Para obter mais informações, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Acionadores instantâneos (webhooks) em [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>Um tipo especial de acionador que permite executar um cenário imediatamente depois que um novo pacote estiver disponível. Para obter mais informações, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Acionadores instantâneos (webhooks) no [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
