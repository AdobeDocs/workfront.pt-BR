---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-with-anaplan
title: Aplique um [!DNL Anaplan] alocação de orçamento para um [!DNL Adobe Workfront] projeto
description: Esse cenário de integração sincroniza todas as alocações de orçamento que foram feitas em [!DNL Anaplan] voltar para [!DNL Workfront]. O cenário extrai todos os itens de orçamento de campanha vinculados e passa o valor orçado para o projeto do Workfront vinculado, se o valor de orçamento tiver sido alterado.
author: Becky
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: 9b8add8f-1978-4ab4-87ac-f1159e7d6cbb
source-git-commit: 4ab731b14dc5435386fd0d887501788fa37223a2
workflow-type: tm+mt
source-wordcount: '677'
ht-degree: 0%

---

# Aplique um [!DNL Anaplan] alocação de orçamento para um [!DNL Adobe Workfront] projeto

Esse cenário de integração sincroniza todas as alocações de orçamento que foram feitas em [!DNL Anaplan] voltar para [!DNL Workfront]. O cenário extrai todos os itens de orçamento de campanha vinculados e passa o valor orçado para o vinculado [!DNL Workfront] projeto se o valor do orçamento tiver sido alterado.

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
   <td> <p>[!UICONTROL Workfront Fusion for Work Automation and Integration] </p> </td> 
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

* Um perfil de usuário em [!DNL Workfront] nomeado **Integração Anaplan**, que tem direitos de administrador do sistema.

   Para obter informações sobre como criar um usuário em [!DNL Workfront], consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

## Esperado [!DNL Anaplan] Configuração

Você deve ter o seguinte em [!DNL Anaplan] para usar este cenário:

* Um perfil de usuário em [!DNL Anaplan] nomeado **[!DNL Workfront]Integração**, que tem direitos de administrador do sistema.
* O [!DNL Anaplan] Modelo que você deseja usar para este cenário.
* A lista no [!DNL Anaplan] Modelo que captura orçamentos de campanha.

   O módulo da lista deve suportar o recebimento dos seguintes atributos:

   * [!UICONTROL GUID do projeto do Workfront]
   * [!UICONTROL Nome da campanha]
   * [!UICONTROL Fundos de mão de obra solicitados]
   * [!UICONTROL Receita estimada]
   * [!UICONTROL Marca]

   Esta lista e o módulo devem armazenar detalhes adicionais necessários para a funcionalidade normal do [!DNL Anaplan], incluindo a capacidade de definir um orçamento e comunicar que o item da lista de orçamento está pronto para ser sincronizado novamente [!DNL Workfront].

* Uma exibição em [!DNL Anaplan] nomeado **[!UICONTROL Campanhas.Update no Adobe Workfront]**.

   Essa exibição deve conter as seguintes colunas, nesta ordem:

   1. [!UICONTROL Nome do item]

   2. [!UICONTROL [!DNL Workfront] GUID do projeto]

   3. [!UICONTROL Nome da campanha]

   4. [!UICONTROL Orçamento]

   5. [!UICONTROL Receita estimada]

   6. [!UICONTROL Marca]
   A exibição deve ser filtrada para exibir itens que tenham um [!UICONTROL [!DNL Workfront] GUID do projeto] e alguns indicam que as dotações orçamentais devem ser transmitidas para [!DNL Workfront].

Para obter instruções sobre qualquer uma dessas ações, consulte a [!DNL Anaplan] documentação.

## Implantação do para [!DNL Workfront Fusion]

Complete as etapas a seguir para implantar este cenário de integração no seu [!DNL Fusion] conta. Isso só deve ser feito após completar o [!DNL Workfront] e [!DNL Anaplan] configuração.

1. Navegue até o [!UICONTROL Modelos] em [!DNL Workfront Fusion] e clique no botão **[!UICONTROL Aplicar [!DNL Anaplan] alocações de orçamento para projetos Workfront]** modelo de cenário.
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
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nome do módulo]</td> 
      <td>O nome do módulo que descreve os atributos da campanha no [!DNL Anaplan] Lista.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nome da lista de campanhas]</td> 
      <td>O nome da lista da sua [!DNL Anaplan] e o espaço de trabalho e modelo selecionados.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL Anaplan] Nome da exibição]</td> 
      <td> <p>O nome da exibição que contém orçamentos de campanha prontos para transmissão para [!DNL Workfront].</p> <p>(Exemplo: [!UICONTROL Campaigns.Load Campaigns to [!DNL Adobe Workfront]]) </p> </td> 
     </tr> 
    </tbody> 
   </table>

   Os detalhes sobre como configurar os arquivos e processos são fornecidos no [!DNL Anaplan] documentação de configuração.

1. Selecione ou adicione um [!DNL Anaplan] perfil de conexão.
1. Atualizar todas as restantes [!DNL Anaplan] módulos com uma [!DNL Anaplan] , quando solicitado.
1. No **[!UICONTROL Converter CSV em módulo de objeto JSON]**, adicione uma nova estrutura de dados para mapear as colunas CSV a um objeto JSON utilizável.

   <!-- [Copy](javascript:void(0);) -->
   <pre></pre>

1. Quando solicitado, selecione essa estrutura de dados para outros módulos nesta implantação de cenário.
1. No **[!UICONTROL Verificar projeto vinculado]** , selecione ou adicione um [!DNL Workfront] perfil de conexão.
1. Atualizar todas as restantes [!DNL Workfront] módulos com uma [!DNL Workfront] , quando solicitado.

## Outros modelos de cenário recomendados

Para concluir o workflow representado por este template, você também deve implantar o seguinte template adicional:

* [[!UICONTROL Crie um [!DNL Anaplan] item de lista de um [!DNL Adobe Workfront] solicitação de orçamento]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/create-an-anaplan-list-item-from-a-workfront-budget-request.md)

Os cenários adicionais para otimização de gastos incluem:

* [[!UICONTROL Enviar [!DNL Adobe Workfront] atualizações de projeto para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] as horas reais são atualizadas para um [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-actual-hours-updates-to-anaplan-list-item.md)

* [[!UICONTROL Enviar [!DNL Adobe Workfront] despesas de [!DNL Anaplan] item de lista]](../../workfront-integrations-and-apps/adobe-workfront-with-anaplan/send-workfront-project-expenses-to-anaplan-list-item.md)
