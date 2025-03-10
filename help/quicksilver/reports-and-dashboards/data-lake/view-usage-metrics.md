---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Exibir métricas de uso do Workfront Data Connect
description: Usando a guia Métricas da Workfront Data Connect, você pode visualizar as métricas de uso de sua organização de acordo com as horas de computação mensais usadas e o número de consultas executadas.
author: Nolan
feature: Reports and Dashboards
exl-id: 29185bd1-e058-4b42-a508-53406fb9ddd2
source-git-commit: ea9c674b798c48927c7a0a542d36d5ded15ea3f1
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Visualizar [!DNL Workfront Data Connect] métricas de uso

Usando a guia [!DNL Workfront Data Connect] [!UICONTROL Métricas], você pode exibir as métricas de uso de sua organização de acordo com as horas de computação usadas e o número de consultas executadas. As organizações têm um número limitado de horas mensais de computação disponíveis com base em seu tipo de licença e compras complementares do Data Connect. A guia [!UICONTROL Métricas] exibe informações sobre as horas de computação mensais disponíveis relacionadas ao que foi usado.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td><p>Incluído nos seguintes planos:</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <!--<p>Can be purchased as an add-on to the following plans:</p> 
    <ul>
        <li>Select</li> 
        <li>Prime</li>
    </ul>--> 
    <p>O Workfront Data Connect não está disponível para planos Workfront herdados.</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir métricas de uso e horas de computação disponíveis

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em [!UICONTROL **Instalação**].

1. No painel esquerdo, clique em [!UICONTROL **Sistema**] > [!UICONTROL **Acesso a Dados**].

1. Clique na guia [!UICONTROL **Métricas**]. Suas métricas de uso são exibidas no gráfico **Uso do Cálculo**, enquanto o número de consultas executadas é exibido no gráfico **Contagem de Consultas**.

   ![Métricas de uso da Conexão de Dados](/help/quicksilver/reports-and-dashboards/data-lake/assets/data-connect-usage-metrics.png)

1. (Opcional) Você pode usar o menu suspenso [!UICONTROL **Selecionar um modo de exibição**] para alterar o intervalo de tempo das informações incluídas em ambos os gráficos.

1. (Opcional) Você pode usar as caixas de seleção acima do gráfico **Uso da Computação** para mostrar ou ocultar:
   * [!UICONTROL **Horas de Computação Diárias**] - O número de horas de computação usadas diariamente pela sua organização.
   * [!UICONTROL **Horas mensais cumulativas de computação**] - O número total de horas de computação usadas pela sua organização em um mês. Redefine para zero todo mês.
   * [!UICONTROL **Permissão de Horas de Computação Mensal**] - O número de horas de computação disponíveis para sua organização com base em compras de licença e/ou complemento.
