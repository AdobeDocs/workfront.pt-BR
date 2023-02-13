---
product-area: workfront-integrations;setup
navigation-topic: workfront-for-jira
title: Exibir o registro de atividades do Jira
description: Como um [!DNL Jira] administrador, você pode exibir as exceções e erros que ocorrem durante a sincronização ou criação dos tíquetes entre [!DNL Adobe Workfront] e [!DNL Jira] em um Log de atividades.
author: Becky
feature: Workfront Integrations and Apps
exl-id: 3e66c8e3-94b7-4153-abbb-32b872b9402b
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Visualize o [!UICONTROL [!DNL Jira] Log de atividades]

Como um [!DNL Jira] administrador, você pode exibir as exceções e erros que ocorrem durante a sincronização ou criação dos tíquetes entre [!DNL Adobe Workfront] e [!DNL Jira] em um [!UICONTROL Log de atividades].

É possível visualizar até 500 itens no Log de atividades e eles serão listados começando com os mais recentes.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plano</a>*</td> 
   <td> <p>[!UICONTROL Pro] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe [!DNL Workfront] visão geral das licenças</a>*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Jira] acesso</td> 
   <td> <p>Acesso do administrador do sistema</p> <p>Importante: Recomendamos que você crie contas de administrador de sistema separadas em [!DNL Jira] e [!DNL Workfront] dedicar-se a essa integração, em vez de usar as existentes que podem ser vinculadas aos usuários.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter informações sobre [!DNL Workfront] administradores, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Pré-requisitos

Antes de vincular itens entre [!DNL Workfront] e [!DNL Jira], você deve

* Instalar [!DNL Workfront for Jira]

   Para obter instruções sobre como instalar [!DNL Workfront for Jira], consulte [Instalar [!DNL Adobe Workfront for Jira]](../../workfront-integrations-and-apps/use-workfront-with-jira/install-workfront-for-jira.md).

## Acesse o [!UICONTROL [!DNL Jira] Log de atividades]:

1. Faça logon no Jira como administrador do sistema.
1. Clique em **[!UICONTROL Configurações]** no principal [!DNL Jira] menu.
1. Clique em **[!UICONTROL Complementos]**, em seguida **[!UICONTROL Gerenciar complementos]**.

1. Expanda o **[!DNL Workfront]** complemento.
1. Clique em **[!UICONTROL Configurar]**.
1. Faça logon em [!DNL Workfront] como administrador do sistema.
1. Selecione o **[!UICONTROL Log de atividades]** guia .

   Exibir informações sobre exceções e erros que ocorreram durante a criação de itens ou a sincronização de campos entre os dois aplicativos.

   O log inclui os seguintes campos:

   * Data da ocorrência
   * O nome do usuário em Jira
   * Número da emissão Jira
   * Breve descrição do erro ocorrido.
