---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Endereços IP para acessar o Adobe Workfront Fusion
description: O Adobe Workfront Fusion exige uma licença do Adobe Workfront Fusion além de uma licença da Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '158'
ht-degree: 3%

---

# Endereços IP para acessar [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] exige um [!DNL Adobe Workfront Fusion] além de um [!DNL Adobe Workfront license].

Se o firewall ou servidor de email estiver configurado para permitir acesso somente a determinados fornecedores, você deverá adicionar determinados endereços IP à sua lista de permissões para permitir a comunicação aberta entre o seu ambiente e a [!DNL Adobe Workfront Fusion].

Adicione os seguintes endereços IP à sua lista de permissões para habilitar o [!DNL Workfront Fusion] para acessar seu sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Data center da UE</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Data center dos EUA</p> </td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Além disso, se sua organização usar filtragem de rede de saída, adicione o seguinte domínio à sua lista de permissões para permitir que seu sistema acesse o Workfront Fusion.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Data center da UE</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Data center dos EUA</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>A filtragem de rede de saída é incomum. Consulte o administrador da rede para verificar se é necessário atualizar a  de lista de permissões para acomodá-la.

Para obter mais informações sobre como configurar a  de lista de permissões da sua organização, consulte [Configurar a  lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
