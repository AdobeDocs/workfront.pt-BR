---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Enviar  [!DNL Adobe Workfront] atualizações de projeto para um item de lista  [!DNL Anaplan] '
description: Este cenário de integração compartilha o progresso, o status e os principais detalhes do agendamento de um projeto  [!DNL Adobe Workfront]  com um item de lista de orçamento  [!DNL Anaplan] . O compartilhamento dessas informações permite que você aproveite melhor a otimização de gastos e a análise financeira que o [!DNL Anaplan] fornece.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 97e9dac6-f5b5-4d6e-b58b-93acd19048ee
source-git-commit: cb38223c4dd8048fd2ab105abce2c9a79b84c43f
workflow-type: tm+mt
source-wordcount: '910'
ht-degree: 1%

---

# Enviar [!DNL Adobe Workfront] atualizações de projeto para um item de lista [!DNL Anaplan]

Este cenário de integração compartilha o progresso, o status e os detalhes-chave do agendamento de um projeto [!DNL Adobe Workfront] com um item de lista de orçamento [!DNL Anaplan]. O compartilhamento dessas informações permite aproveitar melhor a otimização de gastos e a análise financeira fornecidas pelo [!DNL Anaplan].

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

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

## Evento de acionamento

Este cenário é agendado para ser executado a cada 15 minutos.

## Configuração [!DNL Workfront] Esperada

Você deve ter o seguinte em [!DNL Workfront] para usar este cenário:

* Um perfil de usuário em [!DNL Workfront] chamado **[!UICONTROL [!DNL Anaplan]Integração]**, que tem direitos de administrador do sistema.

  Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Um formulário personalizado **[!UICONTROL Resumo da campanha]** anexado ao objeto do projeto para armazenar valores de dados personalizados que você seleciona enviar para Anaplan.

  Os campos a seguir representam exemplos de campos que podem ser incluídos no formulário personalizado para auxiliar no mapeamento de dados para Anaplan, mas não são necessários para este cenário de integração:

  <table style="table-layout:auto"> 
   <col> 
   <col> 
   <thead> 
    <tr> 
     <th>Nome do Campo</th> 
     <th>Tipo de campo</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Na Data de Início do Mercado]</td> 
     <td>[!UICONTROL Data] </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Na Data de Término do Mercado]</td> 
     <td>[!UICONTROL Data]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Visão geral da campanha]</td> 
     <td>[!UICONTROL Parágrafo Campo de Texto]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Mensagem de Chave]</td> 
     <td>[!UICONTROL Parágrafo Campo de Texto]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Público-alvo de destino]</td> 
     <td> <p>[!UICONTROL Lista Suspensa]</p> <p>Inclua opções que se ajustem aos seus processos.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

<!--
<note type="note">  
<p>The above configuration is available through the Marketing Financial Management Configuration blueprint:</p>
<p>https://MYDOMAIN.my.workfront.com/blueprints/7ebe85c4-05a1-4efe-a018-50ee55f5654c/details </p>
<p><span style="color: #ff0000;">This note is currently not marked for publication.</span> </p>
</note>
-->

## Configuração [!DNL Anaplan] Esperada

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] chamado **[!UICONTROL [!DNL Workfront]Integração]**, que tem direitos de administrador do sistema.
* O Modelo [!DNL Anaplan] que você deseja usar para este cenário.
* A Lista do Modelo [!DNL Anaplan] que você deseja usar para este cenário.
* Um arquivo **[!UICONTROL Importação de Atualização de Projeto]** que contém as seguintes colunas, nesta ordem:

1. [!UICONTROL itemID]

2. [!UICONTROL [!DNL Workfront] GUID do Projeto]

3. [!UICONTROL Nome da campanha]

4. [!UICONTROL Percentual concluído]

5. [!UICONTROL Data de Início Planejada]

6. [!UICONTROL Data de Término Planejada]

7. [!UICONTROL Horas planejadas]

8. [!UICONTROL Custo planejado]

9. [!UICONTROL Custo de Despesas Planejado]

10. [!UICONTROL Custo Efetivo do Trabalho]

11. [!UICONTROL Custo de Trabalho Planejado]

12. [!UICONTROL Status]

Para preparar o arquivo [!UICONTROL [!DNL Anaplan] de Importação de Despesas Planejadas]:

1. Copie e cole o seguinte em um editor de texto ou [!DNL Excel]
1. Salvar o arquivo em formato CSV
1. Carregue o arquivo no Anaplan.

   Para obter instruções, consulte a documentação do [!DNL Anaplan] sobre como importar dados para módulos de um arquivo.

1. Anote o nome que você deu ao arquivo; ele será usado durante a implantação do modelo de cenário [!UICONTROL Fusion].

Exemplo de conteúdo CSV

<!-- [Copy](javascript:void(0);) -->
<pre><code>"itemID","Workfront Project GUID","Campaign Name","Percent Complete","Planned Start Date","Planned Completion Date","Planned Hours","Planned Cost","Planned Expense Cost","Actual Labor Cost","Planned Labor Cost","Status","Campaign Overview","Key Message","In Market Start Date","In Market End Date","Target Audience"<br>"202000001019","6182bc1f0025e184b2c00d9205e22c49","Launch Be U APAC Styles Catalog","0","2022-03-31","2022-05-31","88.25","0","0","0","0","Planning","","","","",""</code></pre>As colunas opcionais podem incluir:

1. [!UICONTROL Visão geral da campanha]

2. [!UICONTROL Mensagem principal]

3. [!UICONTROL Data de Início do Mercado]

4. [!UICONTROL Data de Término do Mercado]

5. [!UICONTROL Público-alvo]

Inclua também quaisquer outros campos que deseja definir no mapeamento.

* Um processo de **[!UICONTROL Importação de Atualização do Project]** foi preparado para executar a importação de dados entregues em um carregamento de arquivo.

Para obter instruções sobre qualquer uma dessas ações, consulte a documentação do [!DNL Anaplan].

## Implantando para [!DNL Workfront Fusion]

Conclua as etapas a seguir para implantar esse cenário de integração em sua conta do Fusion. Isso só deve ser feito após a conclusão das configurações necessárias de [!DNL Workfront] e [!DNL Anaplan].

1. Navegue até o menu [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no modelo de cenário **[!UICONTROL Enviar atualizações de projeto do Workfront para o item de lista [!DNL Anaplan]]**.
1. Substitua os valores da variável para as seguintes [!DNL Anaplan] variáveis:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>Nome da variável</th> 
      <th>Substituir valor por</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Workspace ID]</td> 
      <td>A ID de um espaço de trabalho da sua conta [!DNL Anaplan].</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Identificação de Modelo] </td> 
      <td>A ID de um modelo da sua conta [!DNL Anaplan] e do espaço de trabalho selecionado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da Lista de Campanhas]</td> 
      <td>O nome da lista da sua conta [!DNL Anaplan] e o espaço de trabalho e modelo selecionados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Arquivo: Importação de Atualização de Projeto]</td> 
      <td>O nome do arquivo que receberá dados de atualização do projeto.<p>(Exemplo: WorkfrontUpdateLinkedProject.csv)</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Processo: Importação de Atualização de Projeto]</td> 
      <td> <p>O nome do processo que executará a importação de dados do projeto.</p> <p>(Exemplo: WF Int - Atualizar Detalhes da Campanha)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomínio]</td> 
      <td>O subdomínio da sua conta [!DNL Workfront]. Isso é usado para criar um link para o projeto [!DNL Workfront] em uma anotação que pode ser gerada.</td> 
     </tr> 
    </tbody> 
   </table>

   Detalhes sobre como configurar os arquivos e processos são fornecidos na documentação de configuração do [!DNL Anaplan].

1. Selecione ou adicione um perfil de conexão [!DNL Anaplan].
1. Atualize todos os [!DNL Anaplan] módulos restantes com uma conexão [!DNL Anaplan], quando solicitado.
1. Selecione ou adicione um perfil de conexão [!DNL Workfront].

   O filtro está configurado para receber todos os projetos vinculados incompletos e aqueles projetos que foram concluídos nos últimos 29 minutos. Se você alterar a frequência do cenário [!DNL Fusion], atualizará esse valor assim que o modelo de cenário for implantado.

1. No módulo **[!UICONTROL Criar Projetos para Atualizar CSV]**, adicione uma nova estrutura de dados para mapear os atributos do projeto para colunas CSV.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "itemID": 1000001,<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Percent Complete": 10.01,<br>        "Planned Start Date":"2022-02-22",<br>        "Planned Completion Date":"2022-02-22",<br>        "Planned Hours": 12.5,<br>        "Planned Cost": 123.45,<br>        "Planned Expense Cost": 123.45,<br>        "Planned Labor Cost": 123.45,<br>        "Status": "CUR",<br>        "Campaign Overview":"text",<br>        "Key Message":"text",<br>        "In Market Start Date":"2022-02-22",<br>        "In Market End Date":"2022-02-22",<br>        "Target Audience":"text"<br>    }<br>]<br></code></pre>

1. Atualize todos os [!DNL Workfront] módulos restantes com uma conexão [!DNL Workfront], quando solicitado.

## Outros Modelos de Cenário Recomendados

Este modelo de cenário é complementado pelos seguintes modelos de cenário de otimização de gastos que também podem ser implantados:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de horas reais para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] despesas para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Cenários adicionais para vinculação de solicitações de orçamento:

* [[!UICONTROL Criar um [!DNL Anaplan] item de lista a partir de uma [!DNL Adobe Workfront] solicitação de orçamento]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar uma [!DNL Anaplan] alocação de orçamento a um [!DNL Adobe Workfront] projeto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Cenários adicionais para vincular solicitações de campanha:

* [[!UICONTROL Criar um [!DNL Anaplan] item de lista a partir de uma [!DNL Adobe Workfront] solicitação de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar uma [!DNL Anaplan] alocação de orçamento a uma [!DNL Adobe Workfront] solicitação de campanha ou projeto de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
