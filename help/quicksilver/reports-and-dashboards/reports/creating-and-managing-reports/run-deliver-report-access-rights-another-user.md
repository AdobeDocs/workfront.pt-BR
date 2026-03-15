---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Executar e entregar um relatório com os direitos de acesso de outro usuário
description: Por padrão, os usuários podem ver apenas os objetos em um relatório para os quais têm permissões de Exibição.
author: Courtney
feature: Reports and Dashboards
exl-id: e5e2b683-876c-45b4-ab61-07b1ad0b5650
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '1185'
ht-degree: 17%

---

# Executar e entregar um relatório com os direitos de acesso de outro usuário

<!-- Audited: 11/2024 -->

Por padrão, os usuários podem ver apenas os objetos em um relatório para os quais têm permissões de Exibição.

Você pode permitir que todos os usuários vejam os mesmos resultados em um relatório como outro usuário, independentemente do nível de acesso ou nível de permissão nos objetos dentro do relatório.

Se você executar um relatório com os direitos de acesso de outro usuário com acesso mais alto (por exemplo, os direitos de acesso de um administrador do Adobe Workfront), todos os usuários que têm permissões para Exibir o relatório poderão ver as informações no relatório como o usuário especificado no construtor de relatórios. Essa configuração pode ser definida para ambos os relatórios que os usuários encontram na interface do Workfront ou para relatórios que são entregues aos usuários como um anexo a um email.

>[!TIP]
>
>Você deve substituir o **Executar este relatório pelo campo Direitos de Acesso de:** por um usuário ativo somente quando desejar que o relatório seja exibido com os direitos de acesso desse usuário. Por exemplo, um usuário de licença de trabalho pode não ter permissões para ver todos os itens em um relatório criado por um usuário de licença de plano ou por um administrador do sistema, a menos que o relatório seja exibido com os direitos de acesso de um planejador ou administrador do sistema.\
>Se o relatório for compartilhado com usuários com acesso semelhante ao usuário especificado no campo **Executar este relatório com Direitos de Acesso de:**, você poderá deixar este campo em branco.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
      <p>Padrão</p>
      <p>Plano</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de edição a relatórios, painéis e calendários</p> <p>Editar acesso a filtros, exibições e agrupamentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
     <td> <p>Exibir permissões para um relatório para exibir o relatório entregue</p>
     <p>Gerenciar permissões para um relatório para executar o relatório</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir um relatório com os direitos de acesso de outro usuário

Preencher o campo **Executar este Relatório com Direitos de Acesso de:** garante que um relatório contenha os mesmos dados, independentemente de qual usuário está acessando o relatório. O relatório é exibido como faria para o usuário especificado.

Os usuários que acessam o relatório devem ter pelo menos permissões de Exibição no relatório para poderem vê-lo. Se o usuário listado no campo **Executar este Relatório com Direitos de Acesso de:** estiver desativado, o relatório não será mais exibido para nenhum outro usuário com quem o relatório tenha sido compartilhado.

Para executar um relatório com os direitos de acesso de outro usuário:

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Relatórios]**.

1. Selecione o relatório que deseja exibir com os direitos de acesso de outro usuário.
1. Clique em **Ações de Relatório** e em **Editar**.

1. Clique em **Configurações de Relatório**.

1. No campo **Executar este relatório com Direitos de Acesso de:**, comece a digitar o nome do usuário que você deseja que o relatório exiba e selecione-o quando o vir na lista.\
   ![Executar com direitos de acesso de](assets/unshimmed-access-rights-of.png)

   >[!NOTE]
   >
   >Os usuários com um nível de acesso inferior que têm permissão para criar relatórios não podem selecionar um usuário diferente de si mesmos para o campo **Executar este Relatório com os Direitos de Acesso de:**.

1. Clique em **Concluído**.
1. Clique em **Salvar + Fechar**.\
   O relatório agora é exibido para todos os usuários com os quais o relatório é compartilhado como se fosse visualizado pelo usuário especificado no campo **Executar este relatório com os Direitos de Acesso de:**.

>[!IMPORTANT]
>
>A inserção de um usuário diferente do usuário conectado para o campo **Executar este relatório com Direitos de Acesso de:** afetará as informações exibidas no relatório se ele contiver um filtro que use um curinga referente ao usuário conectado. O relatório é exibido de acordo com o valor especificado no campo **Executar este relatório com os Direitos de Acesso de:**, em vez do valor definido no filtro curinga.
>
>Para obter mais informações sobre curingas para campos de usuário, consulte a seção “Variáveis baseadas no usuário” em [Visão geral das variáveis de filtro de curinga](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## Entregar um relatório com os direitos de acesso de outro usuário

Você pode configurar relatórios para serem entregues como anexo em um email. Você pode configurar esses relatórios entregues para exibição à medida que são exibidos para usuários de nível de acesso mais alto, para que todos os usuários possam ver as mesmas informações nos relatórios entregues. Os usuários que verão o relatório entregue no email devem ser adicionados à lista Enviar para dos destinatários na entrega do relatório. Para obter mais informações sobre a configuração de um relatório para entrega, consulte o artigo [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Para entregar um relatório com os direitos de acesso de outro usuário:

1. Clique no ícone **Menu Principal** ícone ![Menu Principal](assets/main-menu-icon.png) no canto superior direito do Workfront e clique em **Relatórios**.

1. Selecione o relatório que você deseja entregar com os direitos de acesso de outro usuário.
1. Clique no nome do relatório para selecioná-lo.
1. Clique em **Ações de Relatório**.
1. Clique em **Enviar Relatório**.

1. No campo **Entregar este relatório com os Direitos de Acesso de:**, comece a digitar o nome do usuário que você deseja que o relatório exiba quando for entregue em um email e selecione-o quando o vir na lista. O padrão é o nome do usuário que está criando o relatório.\
   ![Relatório enviado com direitos de acesso de](assets/unshimmed-send-report-access-rights-of.png)

   >[!NOTE]
   >
   >Os usuários com um nível de acesso mais baixo que têm permissão para criar relatórios não podem selecionar um usuário diferente de si mesmos para o campo **Entregar este Relatório com os Direitos de Acesso de:**.

1. Selecione o **Formato** que você deseja que o relatório exiba no email:

   * HTML
   * PDF
   * Excel
   * Excel (.xlsx)
   * TSV

1. Clique em **Enviar agora** para enviá-lo imediatamente.\
   Ou\
   Clique em **Fazer Entrega Repetida** para agendar uma entrega recorrente para o relatório.\
   Para obter mais informações sobre entregas de relatório, consulte o artigo [Visão geral da entrega de relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

## Limitações para relatórios com uma coluna Origem

Os seguintes relatórios exibem uma coluna Origem, na qual você pode visualizar informações sobre o objeto-pai:

* Relatórios de problema
* Relatórios de hora
* Relatórios de documento

Se os usuários não tiverem permissões para o objeto-pai de um problema, hora ou documento, a coluna Origem do relatório será exibida em branco, mesmo quando o relatório estiver configurado para ser exibido ou entregue com os direitos de acesso de outro usuário.

Para mostrar informações sobre o objeto-pai no relatório, recomendamos adicionar uma coluna para o objeto pai, onde você pode visualizar o nome do objeto pai.

Por exemplo, você pode adicionar qualquer um dos itens a seguir a um relatório com uma coluna Origem:

* As colunas Nome do projeto, Nome da tarefa ou Nome do problema em um relatório de horas ou de documento.
* As colunas Nome do projeto ou Nome da tarefa em um relatório de problema.
* Uma coluna que usa expressões do modo de texto que faz referência aos três objetos. Este é um exemplo de relatório de uma hora:

  ```
  displayname=Custom Source
  
  linkedname=opTask
  
  namekey=view.relatedcolumn
  
  namekeyargkey.0=opTask
  
  namekeyargkey.1=name
  
  textmode=true
  
  valueexpression=IF(!ISBLANK({opTaskID}),{opTask}.{name},IF(!ISBLANK({taskID}),{task}.{name},IF(!ISBLANK({projectID}),{project}.{name},IF(!ISBLANK({timesheetID}),CONCAT({owner}.{name}," ",{timesheet}.{startDate}," - ",{timesheet}.{endDate}),""))))
  
  valueformat=HTML
  ```

  Para obter informações sobre modos de exibição de texto, consulte [Editar um modo usando o modo de texto](../text-mode/edit-text-mode-in-view.md).
