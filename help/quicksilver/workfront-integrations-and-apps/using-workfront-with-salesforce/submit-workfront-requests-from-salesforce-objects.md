---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos
description: Depois de instalar [!DNL Adobe Workfront] para [!DNL Salesforce], you can submit [!DNL Workfront] solicitações de [!DNL Salesforce] Oportunidades e Contas. Essa funcionalidade existe nas estruturas do Classic e do Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos

Depois de instalar [!DNL Adobe Workfront for Salesforce], você pode enviar [!DNL Workfront] solicitações de [!DNL Salesforce] Oportunidades e Contas. Essa funcionalidade existe em [!DNL Classic] e [!DNL Lightning Experience] quadros.

## Requisitos de acesso

Você deve ter o seguinte acesso para usar a funcionalidade descrita neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] plano*</p></td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] licença*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Para enviar uma [!DNL Workfront] de um [!DNL Salesforce] A oportunidade ou a conta garantem que você tenha o seguinte em seu ambiente:

* Seu [!DNL Workfront] administrador instalado [!DNL Workfront for Salesforce].\
   Para obter mais informações sobre a instalação [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* Seu [!DNL Workfront] o administrador adicionou o [!DNL Workfront] seção à sua [!UICONTROL Oportunidade] e [!UICONTROL Conta] layouts de página.\
   Para obter mais informações sobre como adicionar o [!DNL Workfront] para um layout de página, consulte [Configure o [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Você tem um [!DNL Workfront] e você pode fazer logon nela pelo [!DNL Workfront] dentro de sua Oportunidade ou Conta.\
   Depois de fazer logon, você poderá ver a variável [!UICONTROL Novas solicitações] , onde você pode começar a inserir solicitações.

## Enviar [!DNL Workfront] solicitações de [!DNL Salesforce]

1. Acesse uma Oportunidade ou Conta no Salesforce.
1. Vá para o [!DNL Workfront] seção.
1. No **[!UICONTROL Novas solicitações]** selecione um tipo de solicitação no **[!UICONTROL Selecionar um Tipo de Solicitação]** menu suspenso.

   Você pode ver as mesmas filas de solicitação que têm acesso no Workfront.

1. Comece a preencher os campos disponíveis para sua solicitação.

   Envio de um pedido de [!DNL Salesforce] é idêntico ao envio de uma solicitação no [!DNL Workfront] aplicação web.

   >[!NOTE]
   >
   >Fazer upload de um documento usando o [!DNL Workfront] plugin [!DNL Salesforce] está temporariamente indisponível.

   Continue a seguir as etapas descritas em [Criar e enviar [!DNL Adobe Workfront] requests](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Clique em **[!UICONTROL Enviar]**.

## Exibir [!DNL Workfront] requests

1. Ir para uma Oportunidade ou Conta em [!DNL Salesforce].
1. Vá para o **[!DNL Workfront]** seção.

   >[!NOTE]
   >
   >Dependendo de como o [!DNL Workfront] O administrador configurou esta seção e pode ter um nome diferente.

1. Selecione o **[!UICONTROL Solicitações enviadas]** guia .

   Você pode exibir todas as solicitações que você ou outras pessoas enviaram desta Oportunidade ou Conta nesta guia.As solicitações enviadas para esta fila de solicitações na aplicação Web não são exibidas nessa lista em [!DNL Salesforce].

   >[!NOTE]
   >
   >As solicitações enviadas para essa fila de solicitações no aplicativo Web não são exibidas nessa lista no Salesforce.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Você pode exibir as seguintes informações sobre as solicitações enviadas:

   * Nome da solicitação (na variável [!UICONTROL Assunto] column)
   * Número de Referência
   * Tipo de requisição
   * Status
   * Enviado na Data
   * Solicitado por nome
   * Atribuído ao Nome\

      Quando essas informações são atualizadas em [!DNL Workfront], também é atualizado nesta lista.

1. (Opcional) Clique no nome da solicitação para abri-la em [!DNL Workfront].

1. (Opcional) Clique em **[!UICONTROL Ir para[!DNL Salesforce]]** para acessar a Oportunidade ou a Conta em que o problema se originou das seguintes áreas do Workfront:

   * No [!UICONTROL Detalhes] seção do problema
   * No painel Resumo ao selecionar o problema em uma lista, depois de clicar em [!UICONTROL Abrir resumo] ![](assets/summary-panel-icon.png) na barra de ferramentas da lista.
   * No cabeçalho do problema, quando a variável [!UICONTROL Integrações] está disponível. O administrador do sistema ou do grupo deve adicionar a variável [!UICONTROL Integrações] para seu Modelo de layout para exibir o link Ir para o Salesforce no cabeçalho da edição. Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >O [!UICONTROL Ir para o Salesforce] link é visível para todos [!DNL Workfront] usuários que podem visualizar o problema. Você deve ter um [!DNL Salesforce] para poder acessar a [!DNL Salesforce] Oportunidade ou Conta em que o problema foi registrado.
