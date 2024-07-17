---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Aplicar uma alocação de orçamento  [!DNL Anaplan]  a um projeto  [!DNL Adobe Workfront]
description: Este cenário de integração sincroniza todas as alocações de orçamento que foram feitas em [!DNL Anaplan] de volta a [!DNL Workfront]. O cenário extrai todos os itens de orçamento vinculados da campanha e passa o valor orçado para o projeto vinculado do Workfront, se o valor do orçamento tiver sido alterado.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '678'
ht-degree: 0%

---

# Aplicar uma alocação de orçamento [!DNL Anaplan] a um projeto [!DNL Adobe Workfront]

Este cenário de integração sincroniza todas as alocações de orçamento feitas em [!DNL Anaplan] de volta para [!DNL Workfront]. O cenário extrai todos os itens de orçamento de campanha vinculados e passa o valor orçado para o projeto [!DNL Workfront] vinculado se o valor de orçamento tiver sido alterado.

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
   <td> <p>[!UICONTROL Workfront Fusion para Automação e Integração do Trabalho] </p> </td> 
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

* Um perfil de usuário em [!DNL Workfront] chamado **Integração com Anaplan**, que tem direitos de administrador do sistema.

  Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Configuração [!DNL Anaplan] Esperada

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] chamado **[!DNL Workfront]Integração**, que tem direitos de administrador do sistema.
* O Modelo [!DNL Anaplan] que você deseja usar para este cenário.
* A Lista dentro do Modelo [!DNL Anaplan] que captura os orçamentos da campanha.

  O módulo da lista deve oferecer suporte ao recebimento dos seguintes atributos:

   * [!UICONTROL GUID do Projeto do Workfront]
   * [!UICONTROL Nome da campanha]
   * [!UICONTROL Fundos de trabalho solicitados]
   * [!UICONTROL Receita estimada]
   * [!UICONTROL Marca]

  Esta lista e este módulo devem armazenar os detalhes adicionais necessários para a funcionalidade normal do [!DNL Anaplan], incluindo a capacidade de definir um orçamento e comunicar que o item da lista de orçamento está pronto para ser sincronizado novamente ao [!DNL Workfront].

* Uma exibição em [!DNL Anaplan] chamada **[!UICONTROL Campanhas.Atualizar Campanhas no Adobe Workfront]**.

  Essa exibição deve conter as seguintes colunas, nesta ordem:

   1. [!UICONTROL Nome do Item]

   2. [!UICONTROL [!DNL Workfront] GUID do Projeto]

   3. [!UICONTROL Nome da campanha]

   4. [!UICONTROL Orçamento]

   5. [!UICONTROL Receita estimada]

   6. [!UICONTROL Marca]

  A exibição deve ser filtrada para exibir itens que tenham um [!UICONTROL [!DNL Workfront] GUID de Projeto] e algum indicador de que as alocações de orçamento devem ser transmitidas para [!DNL Workfront].

Para obter instruções sobre qualquer uma dessas ações, consulte a documentação do [!DNL Anaplan].

## Implantando para [!DNL Workfront Fusion]

Conclua as etapas a seguir para implantar este cenário de integração na sua conta do [!DNL Fusion]. Isso só deve ser feito após a conclusão das configurações necessárias de [!DNL Workfront] e [!DNL Anaplan].

1. Navegue até o menu [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no **[!UICONTROL Aplicar [!DNL Anaplan] alocações de orçamento ao modelo de cenário de projetos do Workfront]**.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nome do Módulo]</td> 
      <td>O nome do módulo que descreve os atributos de campanha na Lista [!DNL Anaplan] selecionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da Lista de Campanhas]</td> 
      <td>O nome da lista da sua conta [!DNL Anaplan] e o espaço de trabalho e modelo selecionados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Exibir Nome]</td> 
      <td> <p>O nome da exibição que contém orçamentos de campanha prontos para transmissão para [!DNL Workfront].</p> <p>(Exemplo: [!UICONTROL Campanhas.Carregar Campanhas para [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Detalhes sobre como configurar os arquivos e processos são fornecidos na documentação de configuração do [!DNL Anaplan].

1. Selecione ou adicione um perfil de conexão [!DNL Anaplan].
1. Atualize todos os [!DNL Anaplan] módulos restantes com uma conexão [!DNL Anaplan], quando solicitado.
1. Em **[!UICONTROL Converter CSV em módulo de Objeto JSON]**, adicione uma nova estrutura de dados para mapear as colunas CSV para um objeto JSON utilizável.

   <!-- [Copy](javascript:void(0);) -->
   <pre><code>[<br>    {<br>        "Anaplan Name":"text",<br>        "Workfront Project GUID":"text",<br>        "Campaign Name":"text",<br>        "Budget": 100.01,<br>        "Estimated Revenue": 100.01,<br>        "Brand":"text"<br>    }<br>]<br></code></pre>

1. Quando solicitado, selecione essa estrutura de dados para outros módulos nesta implantação de cenário.
1. No módulo **[!UICONTROL Verificar Projeto Vinculado]**, selecione ou adicione um perfil de conexão [!DNL Workfront].
1. Atualize todos os [!DNL Workfront] módulos restantes com uma conexão [!DNL Workfront], quando solicitado.

## Outros Modelos de Cenário Recomendados

Para concluir o workflow representado por esse template, você também deve implantar o seguinte template adicional:

* [[!UICONTROL Criar um [!DNL Anaplan] item de lista a partir de uma [!DNL Adobe Workfront] solicitação de orçamento]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Outros cenários para otimização de gastos incluem:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de projeto para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de horas reais para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] despesas para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
