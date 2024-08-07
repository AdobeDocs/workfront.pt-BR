---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Diretivas para manipulação de erros em  [!DNL Adobe Workfront Fusion]
description: Este artigo descreve diretivas que podem ser usadas para manipulação de erros em  [!DNL Adobe Workfront Fusion]  cenários.
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '955'
ht-degree: 12%

---

# Diretivas para manipulação de erros em [!DNL Adobe Workfront Fusion]

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

## Diretivas para tratamento de erros

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Reversão</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>A execução do cenário é interrompida imediatamente e uma fase de <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">Reversão</a> é iniciada em todos os módulos na tentativa de reverter todos para seu estado inicial. Os módulos subsequentes não são processados.</p> <p>Exceto alguns tipos de erro, o cenário é desativado após o número de erros consecutivos especificados em Configurações do cenário. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">Número de erros consecutivos</a>.</p> <p>O status de execução do cenário é marcado como “erro”.</p> <p>Observação: esse é o comportamento padrão se nenhuma rota de manipulador de erros estiver anexada ao módulo e a configuração <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Permitir armazenamento de execuções incompletas]</a> nas [!UICONTROL Configurações de cenário] não estiver marcada.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Confirmar</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>A execução do cenário é interrompida imediatamente e uma fase de confirmação é iniciada em todos os módulos. Os módulos subsequentes não são processados.</p> <p>Todos os pacotes não processados são ignorados.</p> <p>O status de execução do cenário é marcado como "sucesso". Para obter informações sobre fases de confirmação, consulte <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">Confirmar</a> no artigo <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Execução de cenário, ciclos e fases no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Retomar</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>Uma saída substituta é especificada e fornecida ao módulo que encontra um erro.</p> <p>Os módulos subsequentes são processados.</p> <p>O status de execução do cenário é marcado como “sucesso”.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ignorar</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>O erro é ignorado e os módulos subsequentes não são processados.</p> <p>Se houver pacotes não processados, a execução do cenário continuará normalmente.</p> <p>O status de execução do cenário é marcado como “sucesso”.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Interrupção</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>O estado de execução do cenário é armazenado na fila de execuções incompletas, onde o erro pode ser resolvido manualmente. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Exibir e resolver execuções incompletas no Adobe Workfront Fusion</a>. </p> <p>Há, no entanto, algumas exceções. Para obter mais informações, consulte <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">Permitir o armazenamento de execuções incompletas</a> no artigo <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">O painel de configurações de cenário no Adobe Workfront Fusion</a>.</p> <p>Os módulos subsequentes não são processados.</p> <p>Se houver pacotes não processados, a execução do cenário continuará normalmente.</p> <p>O status de execução do cenário é marcado como "aviso" quando a opção [!UICONTROL Concluir execução automaticamente] está desabilitada.</p> <p>Consulte a seção <a href="#break" class="MCXref xref">[!UICONTROL Break]</a> abaixo para obter mais informações.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Tente novamente</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>Em alguns casos, pode ser útil reexecutar um módulo com falha por algumas vezes quando houver uma chance de o motivo da falha passar do tempo.</p> <p>Atualmente, o Workfront Fusion não oferece a diretiva Repetir, embora várias soluções alternativas possam ser empregadas para mimetizar sua funcionalidade. Para obter mais informações, consulte <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Repetir tratamento de erros no Adobe Workfront Fusion</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Atualmente, as diretivas de tratamento de erros não podem ser usadas fora de uma rota de tratamento de erros.
>
>   Para obter mais informações, consulte [Rota do manipulador de erros](../../workfront-fusion/errors/error-handling.md#error) no artigo [Tratamento de erros no Adobe Workfront Fusion](../../workfront-fusion/errors/error-handling.md).
>* No momento, o [!DNL Workfront Fusion] não oferece um módulo Lançar que permitiria gerar erros (lançar) condicionalmente de maneira fácil, embora uma solução alternativa possa ser empregada para mimetizar sua funcionalidade.
>
>   Para obter mais informações, consulte [Solução alternativa para lançamento](../../workfront-fusion/errors/throw.md#workaround-for-throw) no artigo [Manipulação de erros em Adobe Workfront Fusion](../../workfront-fusion/errors/throw.md).

## Interrupção {#break}

Quando um erro é tratado pela diretiva [!DNL Break], um registro é criado na pasta Execuções incompletas. Esse registro armazena o estado da execução do cenário, juntamente com os dados dos módulos anteriores. O registro faz referência ao módulo em que o erro se originou e contém informações sobre quais dados foram recebidos pelo módulo como entrada. Para cada pacote de dados que causa o erro, um registro separado é criado.

Para obter mais informações, consulte [Exibir e resolver execuções incompletas no Adobe Workfront Fusion](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Resolver erros resultantes da diretiva de Interrupção

Você pode resolver o erro manualmente atualizando o cenário (se necessário) e executando-o uma vez.

Você também pode configurar o cenário para processar automaticamente uma execução incompleta reexecutando o cenário. Para configurar o módulo para processar execuções incompletas:

1. No módulo Break, habilite a opção [!UICONTROL **Concluir execução automaticamente**].
1. No campo **Número de tentativas**, insira ou mapeie o número máximo de tentativas que o módulo deverá repetir a execução

   Este número deve estar entre 1 e 100.
1. No campo **Intervalo entre tentativas**, digite ou mapeie o número de minutos entre cada nova tentativa.

Com essa opção habilitada, quando ocorre um erro, a execução incompleta é recuperada (após o tempo especificado no campo [!UICONTROL Intervalo entre tentativas]) e executada com os dados de entrada originais. Isso se repetirá até que a execução do módulo seja concluída sem erros ou até que o Número de tentativas especificado seja atingido.

>[!NOTE]
>
>Se a tentativa inicial falhar, o intervalo entre as tentativas aumenta exponencialmente a cada duas tentativas.


Quando a opção &quot;Execução concluída automaticamente&quot; está ativada, a execução do cenário é marcada como &quot;Sucesso&quot; porque a repetição automática do manipulador de erros de Interrupção está lidando com o problema automaticamente. Nesse caso, os usuários não recebem um email sobre a execução com falha.

Quando &quot;Execução concluída automaticamente&quot; estiver desativada, a execução é marcada como &quot;Aviso&quot;.

Há algumas exceções para execuções que estão sendo armazenadas em Execuções incompletas e, com alguns tipos de erro, a repetição automática de uma execução de cenário não é possível.

Para obter mais informações, consulte [Permitir o armazenamento de execuções incompletas](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) no artigo [O painel de configurações de cenário no Adobe Workfront Fusion](../../workfront-fusion/scenarios/scenario-settings-panel.md).

Para obter informações adicionais, consulte [Tratamento de erros avançado no Adobe Workfront Fusion](../../workfront-fusion/errors/advanced-error-handling.md).
