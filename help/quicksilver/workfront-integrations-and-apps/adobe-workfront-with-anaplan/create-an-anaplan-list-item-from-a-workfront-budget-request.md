---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Criar um item de lista  [!DNL Anaplan]  a partir de uma solicitação de orçamento  [!DNL Adobe Workfront]
description: Este cenário de integração vincula um projeto  [!DNL Adobe Workfront]  (campanha) a um item da lista de orçamento  [!DNL Anaplan] . Isso é feito adicionando uma solicitação de orçamento ao projeto  [!DNL Workfront]  que precisa receber financiamento. Este cenário procura solicitações de orçamento não processadas e executa um processo para criar um item de lista de orçamento vazio em  [!DNL Anaplan]  para iniciar processos de alocação de orçamento em Anaplan.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: e6505ece-21aa-4397-8d68-543bf89d2f00
source-git-commit: 51b8e474cefe63b4db8c42e480990ca0ba431a4d
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 0%

---

# Criar um item de lista [!DNL Anaplan] de uma solicitação de orçamento [!DNL Adobe Workfront]

Este cenário de integração vincula um projeto [!DNL Adobe Workfront] (campanha) a um item da lista de orçamento [!DNL Anaplan]. Isso é feito adicionando uma solicitação de orçamento ao projeto [!DNL Workfront] que precisa receber financiamento. Este cenário procura solicitações de orçamento não processadas e executa um processo para criar um item de lista de orçamento vazio em [!DNL Anaplan] para iniciar processos de alocação de orçamento em [!DNL Anaplan].

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

&#42;&#42;Para obter informações sobre[!DNL  Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Evento de acionamento

Este cenário é agendado para ser executado a cada 15 minutos.

## Configuração [!DNL Workfront] Esperada

Você deve ter o seguinte em [!DNL Workfront] para usar este cenário:

* Um perfil de usuário em [!DNL Workfront] chamado *[!UICONTROL *[!DNL Anaplan] Integração]**, que tem direitos de administrador do sistema.

  Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* Um formulário personalizado **[!UICONTROL Solicitação de Orçamento]** anexado ao objeto [!UICONTROL Solicitação].

  Os seguintes campos obrigatórios devem ser incluídos no formulário personalizado para auxiliar no mapeamento de dados para [!DNL Anaplan]:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
   <thead> 
    <tr> 
     <th>Nome do Campo</th> 
     <th>Tipo de campo</th> 
    </tr> 
   </thead> 
   <tbody> 
    <tr> 
     <td role="rowheader">[!UICONTROL Tipo de Solicitação de Orçamento]</td> 
     <td> <p>[!UICONTROL Lista Suspensa]</p> <p>Opções:</p> 
      <ul> 
       <li> <p>[!UICONTROL Ajuste de Financiamento]</p> </li> 
       <li> <p>[!UICONTROL Financiamento Inicial]</p> </li> 
      </ul> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fundos de Trabalho Solicitados]</td> 
     <td> </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Fundos de Despesas Solicitados]</td> 
     <td> </td> 
    </tr> 
   </tbody> 
  </table>

  Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

* Modelos de projeto que representam campanhas e outros projetos que exigem financiamento, configurados com um tópico de fila [!UICONTROL Solicitação de orçamento]. O tópico da fila [!UICONTROL Solicitação de orçamento] é atribuído para usar o formulário personalizado [!UICONTROL Solicitação de orçamento].
* Um formulário de **[!UICONTROL Resumo da campanha]** para o objeto de projeto.

  Este formulário deve conter os seguintes campos:

  <table style="table-layout:auto"> 
   <col> 
   </col> 
   <col> 
   </col> 
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
     <td>[!UICONTROL Campo Rich Text]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Mensagem de Chave]</td> 
     <td>[!UICONTROL Campo Rich Text]</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Público-alvo de destino]</td> 
     <td> <p>[!UICONTROL Lista Suspensa]</p> <p>Inclua opções que se ajustem aos seus processos.</p> </td> 
    </tr> 
   </tbody> 
  </table>

  Para obter informações sobre como criar formulários personalizados, consulte [Criar um formulário com o designer de formulário](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Configuração [!DNL Anaplan] Esperada

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] chamado **[!UICONTROL [!DNL Workfront]Integração]**, que tem direitos de administrador do sistema.
* O Modelo [!DNL Anaplan] que você deseja usar para este cenário.
* A Lista dentro do Modelo [!DNL Anaplan] que captura os orçamentos da campanha.

  O módulo da lista deve oferecer suporte ao recebimento dos seguintes atributos:

   * [!UICONTROL GUID do Projeto do Workfront]
   * [!UICONTROL Nome da campanha]
   * [!UICONTROL Fundos de trabalho solicitados]
   * [!UICONTROL Fundos de Despesas Solicitados]
   * [!UICONTROL Tipo de Solicitação de Orçamento]
   * [!UICONTROL Motivo do Ajuste de Financiamento]

  Esta lista e este módulo devem armazenar os detalhes adicionais necessários para a funcionalidade normal do [!DNL Anaplan], incluindo a capacidade de definir um orçamento e comunicar que o item da lista de orçamento está pronto para ser sincronizado novamente ao [!DNL Workfront].

Para obter instruções sobre qualquer uma dessas ações, consulte a documentação do [!DNL Anaplan].

## Implantando para [!DNL Workfront Fusion]

Conclua as etapas a seguir para implantar este cenário de integração na sua conta do [!DNL Fusion]. Isso só deve ser feito após a conclusão das configurações necessárias de [!DNL Workfront] e [!DNL Anaplan].

1. Navegue até o menu [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no **[!UICONTROL Criar um item de lista [!DNL Anaplan] a partir de um modelo de cenário de solicitação de orçamento do Workfront]**.
1. Substitua os valores da variável para as seguintes [!DNL Anaplan] variáveis:

   | Nome da variável | Substituir valor por |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] Workspace ID] | A ID de um espaço de trabalho da sua conta [!DNL Anaplan]. |
   | [!UICONTROL [!DNL Anaplan] ID do Modelo] | A ID de um modelo da sua conta [!DNL Anaplan] e do espaço de trabalho selecionado. |
   | [!UICONTROL [!DNL Anaplan] Nome do módulo ] | O nome do módulo que descreve os atributos de campanha na Lista [!DNL Anaplan] selecionada. |
   | [!UICONTROL Nome da Lista de Campanhas] | O nome da lista da sua conta [!DNL Anaplan] e o espaço de trabalho e modelo selecionados. |

   {style="table-layout:auto"}

   Detalhes sobre como configurar os arquivos e processos são fornecidos na documentação de configuração do [!DNL Anaplan].

1. Selecione ou adicione um perfil de conexão [!DNL Anaplan].
1. Atualize todos os [!DNL Anaplan] módulos restantes com uma conexão [!DNL Anaplan], quando solicitado.
1. Selecione ou adicione um perfil de conexão [!DNL Workfront].

   Após implantar o modelo, este é o módulo que você atualizará para adicionar ou remover referências de campo personalizado do valor da propriedade fields se desejar alterar os campos mapeados padrão para [!DNL Anaplan].

1. Atualize todos os [!DNL Workfront] módulos restantes com uma conexão [!DNL Workfront], quando solicitado.

## Outros Modelos de Cenário Recomendados

Para concluir o workflow representado por esse template, você também deve implantar o seguinte template adicional:

* [[!UICONTROL Aplicar uma [!DNL Anaplan] alocação de orçamento a um [!DNL Adobe Workfront] projeto]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-projects.md)

Outros cenários para otimização de gastos incluem:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de projeto para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de horas reais para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)
* [[!UICONTROL Enviar [!DNL Adobe Workfront] despesas para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
