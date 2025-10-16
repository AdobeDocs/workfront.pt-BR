---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos
description: Após instalar [!DNL Adobe Workfront] por [!DNL Salesforce], you can submit [!DNL Workfront] solicitações de [!DNL Salesforce] Oportunidades e Contas. Essa funcionalidade existe nas estruturas Classic e Lightning Experience.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 1%

---

# Enviar [!DNL Adobe Workfront] solicitações de [!DNL Salesforce] objetos

>[!IMPORTANT]
>
>Para fornecer integrações mais estáveis e escaláveis, estamos mudando para uma abordagem de integração moderna e flexível usando a Automação e Integração do Workfront (Fusion). Como parte desse processo de transição, a integração do Workfront para Salesforce não estará disponível após **28 de fevereiro de 2026**.
>
>Recomendamos usar a Automação e integração do Workfront para as necessidades de integração de sua organização com o Salesforce.
>
>Para obter uma visão geral da Automação e Integração do Workfront, consulte [Visão geral do Adobe Workfront Fusion](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview).
>
>Para obter informações sobre os recursos específicos dos módulos de Automação e Integração do Workfront para Salesforce, consulte [módulos do Salesforce](https://experienceleague.adobe.com/pt-br/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules).

Depois de instalar o [!DNL Adobe Workfront for Salesforce], você pode enviar [!DNL Workfront] solicitações de [!DNL Salesforce] Oportunidades e Contas. Esta funcionalidade existe nas estruturas [!DNL Classic] e [!DNL Lightning Experience].

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td> <p>Standard</p>
   <p>Plano</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Para enviar uma solicitação [!DNL Workfront] de uma Oportunidade ou Conta [!DNL Salesforce], verifique se você tem o seguinte no seu ambiente:

* O administrador do [!DNL Workfront] instalou o [!DNL Workfront for Salesforce].\
   Para obter mais informações sobre como instalar o [!DNL Workfront for Salesforce], consulte [Instalar [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* O administrador [!DNL Workfront] adicionou a seção [!DNL Workfront] aos layouts de página de [!UICONTROL Oportunidade] e [!UICONTROL Conta].\
   Para obter mais informações sobre como adicionar a seção [!DNL Workfront] a um layout de página, consulte [Configurar a [!DNL Adobe Workfront] seção para [!DNL Salesforce] usuários](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* Você tem uma conta [!DNL Workfront] e pode fazer logon nela a partir da seção [!DNL Workfront] dentro da sua Oportunidade ou Conta.\
   Depois de fazer logon, você poderá ver a guia [!UICONTROL Novas solicitações], na qual poderá começar a inserir solicitações.

## Enviar [!DNL Workfront] requisições de [!DNL Salesforce]

1. Vá para uma Oportunidade ou Conta no Salesforce.
1. Vá para a seção [!DNL Workfront].
1. Na guia **[!UICONTROL Novas solicitações]**, selecione um tipo de solicitação no menu suspenso **[!UICONTROL Selecionar um tipo de solicitação]**.

   Você pode ver as mesmas filas de solicitações que você tem acesso para ver no Workfront.

1. Comece a preencher os campos disponíveis para sua solicitação.

   O envio de uma solicitação de [!DNL Salesforce] é idêntico ao envio de uma solicitação no aplicativo web [!DNL Workfront].

   >[!NOTE]
   >
   >O carregamento de um documento usando o plug-in [!DNL Workfront] em [!DNL Salesforce] está temporariamente indisponível.

   Continue seguindo as etapas descritas em [Criar e enviar [!DNL Adobe Workfront] solicitações](../../manage-work/requests/create-requests/create-submit-requests.md).

1. Clique em **[!UICONTROL Enviar]**.

## Exibir [!DNL Workfront] solicitações

1. Ir para uma oportunidade ou conta em [!DNL Salesforce].
1. Vá para a seção **[!DNL Workfront]**.

   >[!NOTE]
   >
   >Dependendo de como o administrador do [!DNL Workfront] configurou esta seção, ela pode ter um nome diferente.

1. Selecione a guia **[!UICONTROL Solicitações enviadas]**.

   Você pode exibir todas as solicitações que você ou outras pessoas enviaram desta Oportunidade ou Conta nesta guia. As solicitações enviadas para esta fila de solicitações no aplicativo Web não são exibidas nesta lista em [!DNL Salesforce].

   >[!NOTE]
   >
   >As solicitações enviadas para essa fila de solicitações no aplicativo web não são exibidas nessa lista no Salesforce.

   ![salesforce_submit_requests.png](assets/salesforce-submitted-requests-350x58.png)

   Você pode exibir as seguintes informações sobre as solicitações submetidas:

   * Nome das Solicitações (na coluna [!UICONTROL Assunto])
   * Número de referência
   * Tipo de requisição
   * Status
   * Enviado na Data
   * Solicitado por nome
   * Atribuído a Nome\

     Quando essas informações são atualizadas em [!DNL Workfront], elas também são atualizadas nesta lista.

1. (Opcional) Clique no nome da solicitação para abri-la em [!DNL Workfront].

1. (Opcional) Clique em **[!UICONTROL Ir para[!DNL Salesforce]]** para acessar a Oportunidade ou Conta em que o problema se originou nas seguintes áreas do Workfront:

   * Na seção [!UICONTROL Detalhes] do problema
   * No painel Resumo, ao selecionar o problema em uma lista, depois de clicar em [!UICONTROL Abrir resumo] ![ícone do painel Resumo](assets/summary-panel-icon.png) na barra de ferramentas da lista.
   * No cabeçalho do problema, quando o campo [!UICONTROL Integrações] estiver disponível. O administrador do sistema ou do grupo deve adicionar o campo [!UICONTROL Integrações] ao Modelo de layout para exibir o link Ir para o Salesforce no cabeçalho do problema. Para obter mais informações, consulte [Personalizar cabeçalhos de objetos usando um modelo de layout](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >O link [!UICONTROL Ir para o Salesforce] está visível para todos os usuários [!DNL Workfront] que podem exibir o problema. Você deve ter uma conta [!DNL Salesforce] para poder acessar a Oportunidade [!DNL Salesforce] ou a Conta onde o problema foi registrado.
