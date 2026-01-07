---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: 'Enviar  [!DNL Adobe Workfront] atualizações de horas reais para um item de lista  [!DNL Anaplan] '
description: Este cenário de integração compartilha os detalhes de horas reais capturados em um projeto [!DNL Adobe Workfront] com um item de lista de orçamento [!DNL Anaplan] . O compartilhamento dessas informações permite que você aproveite melhor a otimização de gastos e a análise financeira que o [!DNL Anaplan] fornece.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '781'
ht-degree: 15%

---

# Enviar [!DNL Adobe Workfront] atualizações de horas reais para um item de lista [!DNL Anaplan]

Este cenário de integração compartilha detalhes de horas reais capturados em um projeto [!DNL Adobe Workfront] com um item de lista de orçamento [!DNL Anaplan]. O compartilhamento dessas informações permite aproveitar melhor a otimização de gastos e a análise financeira fornecidas pelo [!DNL Anaplan].

Este modelo de cenário fornece uma lista de horas resumidas por projeto, dia e função registradas em projetos ativos nos últimos 3 meses.

>[!IMPORTANT]
>
>&quot;Campanha&quot; neste artigo refere-se ao caso de uso de campanha de marketing que este cenário representa e não está conectado de forma alguma ao conector do Adobe Campaign [!DNL Workfront Fusion] ou ao objeto [!UICONTROL Campanha] recentemente descontinuado em [!DNL Workfront].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer pacote de fluxo de trabalho do Adobe Workfront e qualquer pacote do Adobe Workfront Automation and Integration</p><p>Workfront Ultimate</p><p>Os pacotes Workfront Prime e Select, com uma compra adicional do Workfront Fusion.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Licenças do Adobe Workfront</td> 
   <td> <p>Padrão</p><p>Trabalho ou maior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront Fusion</td> 
   <td>
   <p>Baseado em operação: nenhum requisito de licença do Workfront Fusion</p>
   <p>Baseado em conector (legado): Workfront Fusion for Work Automation and Integration </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>
   <p>Se sua organização tiver um pacote Workfront Select ou Prime, ele não inclui o Workfront Automation and Integration. É necessário comprar o Adobe Workfront Fusion.</li></ul>
   </td> 
  </tr>
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre licenças do Adobe Workfront Fusion, consulte [Licenças do Adobe Workfront Fusion](https://experienceleague.adobe.com/en/docs/workfront-fusion/using/set-up-and-manage-fusion/licensing-and-operations-overviews/license-automation-vs-integration).

+++

## Evento de acionamento

Este cenário é agendado para ser executado a cada 15 minutos.

## Configuração [!DNL Workfront] Esperada

Você deve ter o seguinte em [!DNL Workfront] para usar este cenário:

* Um perfil de usuário em [!DNL Workfront] chamado **[!UICONTROL Integração com Anaplan]**, que tem direitos de administrador do sistema.

  Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuração [!DNL Anaplan] Esperada

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] chamado **[!UICONTROL [!DNL Workfront]Integração]**, que tem direitos de administrador do sistema.
* O Modelo [!DNL Anaplan] que você deseja usar para este cenário.
* A Lista do Modelo [!DNL Anaplan] que você deseja usar para este cenário.
* Um arquivo em [!DNL Anaplan] chamado **[!UICONTROL Importação de Horas Reais Anaplan]** que contém as seguintes colunas, nesta ordem:

   1. [!UICONTROL GUID do Projeto do Workfront]

   2. [!UICONTROL Horas]

   3. [!UICONTROL Custo Estimado de Horas]

   4. [!UICONTROL Data de entrada]

   5. [!UICONTROL Nome da Função]

   6. [!UICONTROL Nome da campanha]

   7. [!UICONTROL [!DNL Anaplan] ID do Item de Lista]

  Para preparar o arquivo de Relatório de Despesas Reais [!DNL Anaplan]:

   1. Copie e cole o seguinte em um editor de texto ou [!DNL Excel]
   1. Salvar o arquivo em formato CSV
   1. Carregar o arquivo em [!DNL Anaplan].

      Para obter instruções, consulte a documentação do [!DNL Anaplan] sobre como importar dados para módulos de um arquivo.

   1. Anote o nome que você deu ao arquivo; ele será usado durante a implantação do modelo de cenário [!UICONTROL Fusion].

  Exemplo de conteúdo CSV

  <!-- [Copy](javascript:void(0);) -->
  <pre><code>[!DNL Workfront] Project GUID,Hours,Hours Estimated Cost,Entry Date,Role Name,Workfront Project Name,Item ID<br>6218062a000d0442903fcfa21e11f556,2,0,3/7/22,Designer,New Project 6,202000001030</code></pre>

* Um processo de **[!UICONTROL Importação de Horas Reais do Projeto]** foi preparado para executar a importação de dados entregues em um upload de arquivo.

Para obter instruções sobre qualquer uma dessas ações, consulte a documentação do [!DNL Anaplan].

## Implantando para [!DNL Workfront Fusion]

Conclua as etapas a seguir para implantar este cenário de integração na sua conta do [!DNL Fusion]. Isso só deve ser feito após a conclusão das configurações necessárias de [!DNL Workfront] e [!DNL Anaplan].

1. Navegue até o menu [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no **[!UICONTROL Enviar atualizações de horas reais do Workfront para o modelo de cenário [!DNL Anaplan] item de lista]**.
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
      <td role="rowheader">[!UICONTROL Nome do Arquivo: Importação de Horas Reais]</td> 
      <td> <p>O nome do arquivo que receberá os dados de horas reais do projeto.</p> <p> (Exemplo: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do Processo: Importação de Horas Reais]</td> 
      <td> <p>O nome do processo que executará a importação de dados de horas do projeto.</p> <p>(Exemplo: WF Int - Carregar horas do projeto por função)</p> </td> 
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
1. Atualize todos os [!DNL Workfront] módulos restantes com uma conexão [!DNL Workfront], quando solicitado.

## Outros Modelos de Cenário Recomendados

Este modelo de cenário é complementado pelos seguintes modelos de cenário de otimização de gastos que também podem ser implantados:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de projeto para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] despesas para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Cenários adicionais para vinculação de solicitações de orçamento:

* [[!UICONTROL Criar um [!DNL Anaplan] item de lista a partir de uma [!DNL Adobe Workfront] solicitação de orçamento]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplicar uma [!DNL Anaplan] alocação de orçamento a um [!DNL Adobe Workfront] projeto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Cenários adicionais para vincular solicitações de campanha:

* [[!UICONTROL Criar um [!DNL Anaplan] item de lista a partir de uma [!DNL Adobe Workfront] solicitação de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplicar uma [!DNL Anaplan] alocação de orçamento a uma [!DNL Adobe Workfront] solicitação de campanha ou projeto de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
