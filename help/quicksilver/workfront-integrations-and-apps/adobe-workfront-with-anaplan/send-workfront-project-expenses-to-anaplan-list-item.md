---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Enviar  [!DNL Adobe Workfront] despesas para um [!DNL Anaplan] item de lista
description: Este cenário de integração compartilha os detalhes relacionados às despesas de um projeto [!DNL Adobe Workfront] com um item de lista de orçamento [!DNL Anaplan] a. O compartilhamento dessas informações permite que você aproveite melhor a otimização de gastos e a análise financeira que o [!DNL Anaplan] fornece.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: f9198017-9bbb-4776-86aa-3f78705dbb22
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '919'
ht-degree: 0%

---

# Enviar despesas de [!DNL Adobe Workfront] para um item de lista [!DNL Anaplan]

Este cenário de integração compartilha detalhes relacionados a despesas de um projeto [!DNL Adobe Workfront] com um item de lista de orçamento [!DNL Anaplan]. O compartilhamento dessas informações permite aproveitar melhor a otimização de gastos e a análise financeira fornecidas pelo [!DNL Anaplan].

>[!IMPORTANT]
>
>&quot;Campanha&quot; neste artigo refere-se ao caso de uso de campanha de marketing que este cenário representa e não está conectado de forma alguma ao conector do Adobe Campaign [!DNL Workfront Fusion] ou ao objeto [!UICONTROL Campanha] recentemente descontinuado em [!DNL Workfront].

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
   <td> <p>Automação e integração do Workfront Fusion for Work </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar o [!DNL Adobe Workfront Fusion] e o [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento de acionamento

Este cenário é agendado para ser executado a cada 15 minutos.

## Configuração [!DNL Workfront] Esperada

Você deve ter o seguinte em [!DNL Workfront] para usar este cenário:

* Um perfil de usuário em [!DNL Workfront] chamado *[!UICONTROL *[!DNL Anaplan] Integração]**, que tem direitos de administrador do sistema.

  Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Um formulário personalizado **[!UICONTROL Resumo da campanha]** anexado ao objeto do projeto para armazenar valores de dados personalizados que você opta por enviar para [!DNL Anaplan].

  O formulário deve conter os seguintes campos:

  | Nome do Campo | Tipo de campo |
  |---|---|
  | [!UICONTROL Data da última transmissão] | Data |
  | [!UICONTROL Notas de integração] | Campo de texto em parágrafo |

  Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuração [!DNL Anaplan] Esperada

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] chamado **[!UICONTROL [!DNL Workfront]Integração]**, que tem direitos de administrador do sistema.
* O Modelo [!DNL Anaplan] que você deseja usar para este cenário.
* A Lista dentro do Modelo [!DNL Anaplan] que você deseja capturar orçamentos de campanha.
* Um arquivo **[!UICONTROL Importação de Despesas Reais do Anaplan]** que contém as seguintes colunas, nesta ordem:

   1. [!UICONTROL [!DNL Workfront] Despesas GUID]

   2. [!UICONTROL [!DNL Workfront] GUID do Projeto]

   3. [!UICONTROL Valor Efetivo]

   4. [!UICONTROL Descrição]

   5. [!UICONTROL Tipo de Despesa]

   6. [!UICONTROL Data efetiva]

   7. [!UICONTROL Nome da campanha]

   8. [!UICONTROL [!DNL Anaplan] ID do Item de Lista]

  Para preparar o arquivo [!UICONTROL [!DNL Anaplan] Importação de Despesas Reais]:

   1. Copie e cole o seguinte em um editor de texto ou [!DNL Excel].
   1. Salve o arquivo em formato CSV.
   1. Carregar o arquivo em [!DNL Anaplan].

      Para obter instruções, consulte a documentação do [!DNL Anaplan] sobre como importar dados para módulos de um arquivo.

   1. Anote o nome que você deu ao arquivo; ele será usado durante a implantação do modelo de cenário [!UICONTROL Fusion].

  Exemplo de conteúdo CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Actual Amount","Description","Expense Type","Effective Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","2345","Expense 1","","2022-03-09","New Project 6","202000001030"</code></pre>

* Um arquivo **[!UICONTROL [!DNL Anaplan]de Importação de Despesas Planejadas]** que contém as seguintes colunas, nesta ordem:

   1. [!UICONTROL [!DNL Workfront] Despesas GUID]

   2. [!UICONTROL [!DNL Workfront] GUID do Projeto]

   3. [!UICONTROL Valor Efetivo]

   4. [!UICONTROL Descrição]

   5. [!UICONTROL Tipo de Despesa]

   6. [!UICONTROL Data efetiva]

   7. [!UICONTROL Nome da campanha]

   8. [!UICONTROL [!DNL Anaplan] ID do Item de Lista]

  Para preparar o arquivo [!UICONTROL [!DNL Anaplan] de Importação de Despesas Planejadas]:

   1. Copie e cole o seguinte em um editor de texto ou [!DNL Excel]
   1. Salvar o arquivo em formato CSV
   1. Carregue o arquivo no Anaplan.

      Para obter instruções, consulte a documentação do [!DNL Anaplan] sobre como importar dados para módulos de um arquivo.

   1. Anote o nome que você deu ao arquivo; ele será usado durante a implantação do modelo de cenário [!UICONTROL Fusion].

  Exemplo de conteúdo CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>"Workfront Expense GUID","Workfront Project GUID","Planned Amount","Description","Expense Type","Planned Date","Campaign Name","Anaplan List Item ID"<br>"622aead400423eb2e4479fece9a72987","6218062a000d0442903fcfa21e11f556","1234","Expense 1","Entertainment","2022-03-08","New Project 6","202000001030"</code></pre>


* Um processo de **[!UICONTROL Importação de Atualização do Project]** foi preparado para executar a importação de dados entregues em um carregamento de arquivo.

>[!NOTE]
>
>Há arquivos de importação separados para despesas planejadas e reais para que eles possam ser relatados independentemente em suas datas planejadas e efetivas, respectivamente.

Para obter instruções sobre qualquer uma dessas ações, consulte a documentação do [!DNL Anaplan].

## Implantando para [!DNL Fusion]

Conclua as etapas a seguir para implantar este cenário de integração na sua conta do [!DNL Fusion]. Isso só deve ser feito após a conclusão das configurações necessárias de [!DNL Workfront] e [!DNL Anaplan].

1. Navegue até o menu [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no **[!UICONTROL Enviar atualizações de despesas do Workfront para o modelo de cenário [!DNL Anaplan] item de lista]**.
1. Substitua os valores da variável para as seguintes [!DNL Anaplan] variáveis:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <thead> 
     <tr> 
      <th>Nome da variável</th> 
      <th>Substituir valor por</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>A ID do espaço de trabalho da sua conta do [!DNL Anaplan] que você deseja usar para este cenário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Identificação de Modelo] </td> 
      <td>A ID do modelo da sua conta [!DNL Anaplan] e o espaço de trabalho selecionado que você deseja usar para este cenário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da Lista de Campanhas]</td> 
      <td>O nome da lista da sua conta [!DNL Anaplan] e o espaço de trabalho e modelo selecionados que você deseja usar para este cenário.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Arquivo: Importação Real de Despesas]</td> 
      <td> <p>O nome do arquivo que receberá os dados de despesas reais do projeto.</p> <p> (Exemplo: WorkfrontUpdateLinkedProjects_ActExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Arquivo: Importação de Despesas Planejada]</td> 
      <td> <p>O nome do arquivo que receberá os dados de despesas planejadas do projeto.</p> <p> (Exemplo: WorkfrontUpdateLinkedProjects_PlannedExpenses.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Processo: Importação de Atualização de Projeto]</td> 
      <td> <p>O nome do processo que executará a importação de dados de despesas do projeto.</p> <p>(Exemplo: WF Int - Carregar Despesas de Projeto)</p> </td> 
     </tr> 
    </tbody> 
   </table>

   Detalhes sobre como configurar os arquivos e processos são fornecidos na documentação de configuração do [!DNL Anaplan].

1. Selecione ou adicione um perfil de conexão [!DNL Anaplan].
1. Atualize todos os [!DNL Anaplan] módulos restantes com uma conexão [!DNL Anaplan], quando solicitado.
1. Selecione ou adicione um perfil de conexão [!DNL Workfront].
1. Atualize todos os [!DNL Workfront] módulos restantes com uma conexão [!DNL Workfront], quando solicitado.
1. No módulo **[!UICONTROL Criar CSV de Despesas Reais]**, adicione uma nova estrutura de dados para mapear os atributos do projeto para colunas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Actual Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Effective Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

1. No módulo **[!UICONTROL Criar CSV de Despesas Planejadas]**, adicione uma nova estrutura de dados para mapear os atributos do projeto para colunas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Workfront Expense GUID":"text",<br>        "Workfront Project GUID":"text",<br>        "Planned Amount": 100.01,<br>        "Description":"text",<br>        "Expense Type":"text",<br>        "Planned Date":"text",<br>        "Campaign Name":"text",<br>        "Anaplan List Item ID": 10000001<br>    }<br>]<br></code></pre>

## Outros Modelos de Cenário Recomendados

Este modelo de cenário é complementado pelos seguintes modelos de cenário de otimização de gastos que também podem ser implantados:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de projeto para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de horas reais para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

Cenários adicionais para vinculação de solicitações de orçamento:

* [[!UICONTROL Criar um [!DNL Anaplan] item de lista a partir de uma [!DNL Adobe Workfront] solicitação de orçamento]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar uma [!DNL Anaplan] alocação de orçamento a um [!DNL Adobe Workfront] projeto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Cenários adicionais para vincular solicitações de campanha:

* [[!UICONTROL Criar um [!DNL Anaplan] item de lista a partir de uma [!DNL Adobe Workfront] solicitação de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar uma [!DNL Anaplan] alocação de orçamento a uma [!DNL Adobe Workfront] solicitação de campanha ou projeto de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
