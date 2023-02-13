---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Enviar [!DNL Adobe Workfront] as horas reais são atualizadas para um [!DNL Anaplan] item de lista
description: Esse cenário de integração compartilha detalhes de horas reais capturados em um [!DNL Adobe Workfront] projeto com um [!DNL Anaplan] item da lista de orçamento. O compartilhamento dessas informações permite aproveitar melhor a otimização de gastos e a análise financeira que [!DNL Anaplan] fornece.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 450b9a87-79c6-4d10-a9ea-29766b4f5962
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '725'
ht-degree: 0%

---

# Enviar [!DNL Adobe Workfront] as horas reais são atualizadas para um [!DNL Anaplan] item de lista

Esse cenário de integração compartilha detalhes de horas reais capturados em um [!DNL Adobe Workfront] projeto com um [!DNL Anaplan] item da lista de orçamento. O compartilhamento dessas informações permite aproveitar melhor a otimização de gastos e a análise financeira que [!DNL Anaplan] fornece.

Este modelo de cenário fornece uma lista de horas resumidas por projeto, dia e função registradas em projetos ativos nos últimos 3 meses.

>[!IMPORTANT]
>
>&quot;Campanha&quot; neste artigo se refere ao caso de uso da campanha de marketing que este cenário representa e não está de forma alguma conectado ao cenário [!DNL Workfront Fusion] Conector do Adobe Campaign ou ao recentemente obsoleto [!UICONTROL Campanha] em [!DNL Workfront].

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] para automação e integração de trabalho] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Sua organização deve comprar [!DNL Adobe Workfront Fusion] bem como [!DNL Adobe Workfront] para usar a funcionalidade descrita neste artigo.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

&#42;&#42;Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Acionando evento

Esse cenário é agendado para ser executado a cada 15 minutos.

## Esperado [!DNL Workfront] Configuração

Você deve ter o seguinte em [!DNL Workfront] para usar este cenário:

* Um perfil de usuário em [!DNL Workfront] nomeado **[!UICONTROL Integração Anaplan]**, que tem direitos de administrador do sistema.

   Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Esperado [!DNL Anaplan] Configuração

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] nomeado **[!UICONTROL [!DNL Workfront ]Integração]**, que tem direitos de administrador do sistema.
* O [!DNL Anaplan] Modelo que você deseja usar para este cenário.
* A lista no [!DNL Anaplan] Modelo que você deseja usar para este cenário.
* Um arquivo em [!DNL Anaplan] nomeado **[!UICONTROL Importação de Horas Reais de Anaplan]** que contém as seguintes colunas, nesta ordem:

   1. [!UICONTROL GUID do projeto do Workfront]

   2. [!UICONTROL Horas]

   3. [!UICONTROL Custo estimado de horas]

   4. [!UICONTROL Data de Entrada]

   5. [!UICONTROL Nome da função]

   6. [!UICONTROL Nome da campanha]

   7. [!UICONTROL [!DNL Anaplan] ID de item de lista]
   Para preparar a [!DNL Anaplan] Arquivo de Relatório de Despesas Reais:

   1. Copie e cole o seguinte em um editor de texto ou [!DNL Excel]
   1. Salve o arquivo em um formato CSV
   1. Faça upload do arquivo para [!DNL Anaplan].

      Para obter instruções, consulte o [!DNL Anaplan] documentação sobre como importar dados para módulos de um arquivo.

   1. Anote o nome que deu ao processo; será usado durante a implantação do [!UICONTROL Fusão] modelo de cenário.

   Exemplo de conteúdo CSV

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

* A **[!UICONTROL Importação de Horas Reais do Projeto]** processo preparado para executar a importação de dados entregues em um upload de arquivo.

Para obter instruções sobre qualquer uma dessas ações, consulte a [!DNL Anaplan] documentação.

## Implantação do para [!DNL Workfront Fusion]

Complete as etapas a seguir para implantar este cenário de integração no seu [!DNL Fusion] conta. Isso só deve ser feito após completar o [!DNL Workfront] e [!DNL Anaplan] configuração.

1. Navegue até o [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no botão **[!UICONTROL Enviar atualizações de horas reais do Workfront para o [!DNL Anaplan] item de lista]** modelo de cenário.
1. Substitua os valores da variável para o seguinte [!DNL Anaplan] variáveis:

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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID do espaço de trabalho]</td> 
      <td>A ID de um espaço de trabalho da [!DNL Anaplan] conta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] ID do modelo] </td> 
      <td>A ID de um modelo da [!DNL Anaplan] e o espaço de trabalho selecionado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da lista de campanhas]</td> 
      <td>O nome da lista da sua [!DNL Anaplan] e o espaço de trabalho e modelo selecionados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do arquivo: Importação de Horas Reais]</td> 
      <td> <p>O nome do arquivo que receberá os dados de horas reais do projeto.</p> <p> (Exemplo: WorkfrontUpdateLinkedProjects_HoursRoles.csv) </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome do processo: Importação de Horas Reais]</td> 
      <td> <p>O nome do processo que executará a importação de dados de horas do projeto.</p> <p>(Exemplo: WF Int - Carregar Horas do Projeto por Função)</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Workfront] Subdomínio]</td> 
      <td>O subdomínio de [!DNL Workfront] conta. Isso é usado para criar um link para o [!DNL Workfront] projeto em uma nota que pode ser gerada.</td> 
     </tr> 
    </tbody> 
   </table>

   Os detalhes sobre como configurar os arquivos e processos são fornecidos no [!DNL Anaplan] documentação de configuração.

1. Selecione ou adicione um [!DNL Anaplan] perfil de conexão.
1. Atualizar todas as restantes [!DNL Anaplan] módulos com uma [!DNL Anaplan] , quando solicitado.
1. Selecione ou adicione um [!DNL Workfront] perfil de conexão.
1. Atualizar todas as restantes [!DNL Workfront] módulos com uma [!DNL Workfront] , quando solicitado.

## Outros modelos de cenário recomendados

Esse modelo de cenário é complementado pelos seguintes modelos de cenário de otimização de gastos que também podem ser implantados:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de projeto para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] despesas de [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)

Cenários adicionais para vincular solicitações de orçamento:

* [[!UICONTROL Crie um [!DNL Anaplan] item de lista de um [!DNL Adobe Workfront] solicitação de orçamento]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)
* [[!UICONTROL Aplique um [!DNL Anaplan] alocação de orçamento para um [!DNL Adobe Workfront] projeto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Cenários adicionais para vincular solicitações de campanha:

* [[!UICONTROL Crie um [!DNL Anaplan] item de lista de um [!DNL Adobe Workfront] solicitação de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-campaign-request.md)
* [[!UICONTROL Aplique um [!DNL Anaplan] alocação de orçamento para um [!DNL Adobe Workfront] solicitação de campanha ou projeto de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)
