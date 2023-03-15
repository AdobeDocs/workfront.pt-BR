---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Crie um [!DNL Anaplan] item de lista de um [!DNL Adobe Workfront] solicitação de campanha
description: Esse cenário de integração vincula um [!DNL Adobe Workfront] projeto com um [!DNL Anaplan] item da lista de orçamento.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: daf6a18d-a3df-497d-a612-8a4645b1a8c9
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 2%

---

# Crie um [!DNL Anaplan] item de lista de um [!DNL Adobe Workfront] solicitação de campanha

Esse cenário de integração vincula um [!DNL Adobe Workfront] projeto com um [!DNL Anaplan] item da lista de orçamento.

Este cenário observa novas solicitações de campanha adicionadas a uma fila de solicitações. Assim que uma solicitação de campanha é registrada, um item de linha de orçamento é adicionado em [!DNL Anaplan] iniciar o processo de financiamento.

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
   <td role="rowheader">Plano da [!UICONTROL Adobe Workfront]*</td> 
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

* Um perfil de usuário em [!DNL Workfront] nomeado **[!UICONTROL [!DNL Anaplan]Integração]**, que tem direitos de administrador do sistema.

   Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

* A **[!UICONTROL resumo da campanha]** formulário personalizado anexado ao [!UICONTROL Solicitação] objeto.

   Os seguintes campos obrigatórios devem ser incluídos no formulário personalizado para auxiliar no mapeamento de dados para Anaplan:

   | Nome do Campo | Tipo de campo |
   |---|---|
   | [!UICONTROL Total dos Fundos Solicitados] |  |
   | [!UICONTROL Fundos de mão de obra solicitados] |  |
   | [!UICONTROL Fundos de Despesas Solicitados] |  |
   | [!UICONTROL Enviada para [!DNL Anaplan]] | Caixa de seleção |

   Os seguintes campos opcionais podem estar presentes no formulário. Esse cenário mapeia apenas os campos acima, mas qualquer campo adicional no resumo da campanha pode ser mapeado.

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
     <td role="rowheader">[!UICONTROL Na Data De Início Do Mercado]</td> 
     <td>Data </td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Na Data Final Do Mercado]</td> 
     <td>Data</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Visão geral da campanha]</td> 
     <td>Campo de texto em parágrafo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Mensagem principal]</td> 
     <td>Campo de texto em parágrafo</td> 
    </tr> 
    <tr> 
     <td role="rowheader">[!UICONTROL Público-alvo]</td> 
     <td> <p>Suspenso</p> <p>Inclua opções que se ajustem aos seus processos.</p> </td> 
    </tr> 
   </tbody> 
  </table>

   Para obter informações sobre como criar formulários personalizados, consulte [Criar ou editar um formulário personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)

* Um projeto configurado como uma fila de solicitações para capturar novas solicitações de campanha. O [!UICONTROL resumo da campanha] deve ser anexado a essas solicitações.

## Esperado [!DNL Anaplan] Configuração

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] nomeado **[!UICONTROL [!DNL Workfront]Integração]**, que tem direitos de administrador do sistema.
* O [!DNL Anaplan] Modelo que você deseja usar para este cenário.
* A lista no [!DNL Anaplan] Modelo que captura orçamentos de campanha.

   O módulo da lista deve suportar o recebimento dos seguintes atributos:

   * [!UICONTROL [!DNL Workfront] GUID da solicitação]
   * [!UICONTROL [!DNL Workfront] GUID do projeto]
   * [!UICONTROL Nome da campanha]
   * [!UICONTROL Fundos de mão de obra solicitados]
   * [!UICONTROL Fundos de Despesas Solicitados]
   * [!UICONTROL Tipo de Solicitação de Orçamento]

   Esta lista e o módulo devem armazenar detalhes adicionais necessários para a funcionalidade normal do [!DNL Anaplan], incluindo a capacidade de definir um orçamento e comunicar que o item da lista de orçamento está pronto para ser sincronizado novamente [!DNL Workfront].

Para obter instruções sobre qualquer uma dessas ações, consulte a [!DNL Anaplan] documentação.

## Implantação do para [!DNL Workfront Fusion]

Complete as etapas a seguir para implantar este cenário de integração no seu [!DNL Fusion] conta. Isso só deve ser feito após completar o [!DNL Workfront] e [!DNL Anaplan] configuração.

1. Navegue até o [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no botão **[!UICONTROL Crie um [!DNL Anaplan] item de lista de uma solicitação de campanha do Workfront]** modelo de cenário.
1. Substitua os valores da variável para o seguinte [!DNL Anaplan] variáveis:

   | Nome da variável | Substituir valor por |
   |---|---|
   | [!UICONTROL [!DNL Anaplan] ID do espaço de trabalho] | A ID de um espaço de trabalho da [!DNL Anaplan] conta. |
   | [!UICONTROL [!DNL Anaplan] ID do modelo] | A ID de um modelo da [!DNL Anaplan] e o espaço de trabalho selecionado. |
   | [!UICONTROL [!DNL Anaplan] Nome do módulo] | O nome do módulo que descreve os atributos da campanha no [!DNL Anaplan] Lista. |
   | [!UICONTROL Nome da lista de campanha] | O nome da lista da sua [!DNL Anaplan] e o espaço de trabalho e modelo selecionados. |

   {style="table-layout:auto"}

   Os detalhes sobre como configurar os arquivos e processos são fornecidos no [!DNL Anaplan] documentação de configuração.

1. Selecione ou adicione um [!DNL Anaplan] perfil de conexão.
1. Atualizar todas as restantes [!DNL Anaplan] módulos com uma [!DNL Anaplan] , quando solicitado.
1. Selecione ou adicione um [!DNL Workfront] perfil de conexão.

   Depois de implantar o modelo, esse é o módulo que você atualizará para adicionar ou remover referências de campo personalizadas do valor da propriedade fields se desejar alterar os campos mapeados padrão para [!DNL Anaplan].

1. Atualizar todas as restantes [!DNL Workfront] módulos com uma [!DNL Workfront] , quando solicitado.

## Outros modelos de cenário recomendados

Para concluir o workflow representado por este template, você também deve implantar o seguinte template adicional:

* [[!UICONTROL Aplique um [!DNL Anaplan] alocação de orçamento para um [!DNL Adobe Workfront] solicitação de campanha ou projeto de campanha]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/apply-anaplan-budget-allocation-to-workfront-campaign-requests-and-projects.md)

Os cenários adicionais para otimização de gastos incluem:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de projeto para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] as horas reais são atualizadas para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] despesas de [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
