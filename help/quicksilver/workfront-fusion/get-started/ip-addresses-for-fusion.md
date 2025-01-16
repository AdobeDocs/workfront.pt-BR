---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Endereços IP para acessar o Adobe Workfront Fusion
description: A documentação do Adobe Workfront Fusion foi movida para um novo local. Este artigo foi descontinuado, mas contém um link para o novo artigo que aborda essa funcionalidade.
author: Becky
feature: Workfront Fusion
exl-id: f6295cc7-367f-4c8b-891b-cc11ff42a225
source-git-commit: 3983d811a849c01b3c34b1cd6ee895e5552225a6
workflow-type: tm+mt
source-wordcount: '422'
ht-degree: 0%

---

# Endereços IP para acessar [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>A documentação do Adobe Workfront Fusion foi movida para um novo local.
>
>As informações neste artigo agora podem ser encontradas no artigo:
>
>* [Configurar Endereços IP para o Fusion no incluo na lista de permissões de sua organização](https://experienceleague.adobe.com/docs/workfront-fusion/using/set-up-and-manage-fusion/set-up-and-manage-orgs-and-teams/set-up-orgs-teams-and-users/set-up-ip-addresses-for-fusion.html)
>
>Atualize todos os marcadores.
>
>Este artigo não está mais sendo atualizado e será removido em breve.

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requer uma licença [!DNL Adobe Workfront Fusion] além de [!DNL Adobe Workfront license].

Incluir na lista de permissões Se o firewall ou o servidor de email estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao respectivo arquivo para permitir a comunicação aberta entre o ambiente e o [!DNL Adobe Workfront Fusion].

Você pode adicionar todos os domínios e endereços IP do Fusion ao seu incluo na lista de permissões do ou localizar o cluster do Fusion e adicionar apenas os domínios e endereços IP desse cluster.

## Adicionar todos os domínios e endereços IP do Fusion

Adicione os seguintes endereços IP ao incluo na lista de permissões:

* 52.30.133.50
* 54.220.93.204
* 34 254 76 122
* 54 244 142 219
* 52.39.217.230
* 44 241 82 96
* 100.20.126.137
* 34.223.32.4
* 52.39.176.220
* 20.36.133.48/28
* 20.81.156.240/28
* 172.172.84.48/28

Incluir na lista de permissões Além disso, se a sua organização usar filtragem de rede de saída, adicione o seguinte domínio ao seu arquivo de pesquisa para permitir que o sistema acesse o Workfront Fusion. Eles são usados para webhooks.

* hook.app.workfrontfusion.com
* hook.app-eu.workfrontfusion.com
* hook.app-az.workfrontfusion.com

## Adicionar domínios e endereços IP do Fusion somente para o cluster

### Identificar o data center

Os endereços IP variam de acordo com o local onde seus dados são armazenados.

Se você acessar o Fusion por meio de um URL, poderá examinar o URL para localizar seu data center.

| URL | Data center |
| --- | --- |
| `https://app.workfrontfusion.com/` | Data center dos EUA |
| `https://app-eu.workfrontfusion.com/` | Data center da UE |
| `https://app-az.workfrontfusion.com/` | Data center do Azure |

Se você acessar o Fusion por meio de experience.adobe.com, poderá verificar a guia Rede no navegador para identificar o data center.

| URL | Data center |
| --- | --- |
| Chamadas para `https://fusion.adobe.com` | Data center dos EUA |
| Chamadas para `https://eu.fusion.adobe.com` | Data center da UE |
| Chamadas para `https://az.fusion.adobe.com` | Data center do Azure |

### Adicione endereços IP e domínios para o seu data center

Adicione os seguintes endereços IP ao seu incluo na lista de permissões para habilitar o [!DNL Workfront Fusion] para acessar seu sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centro de dados da UE</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Data center dos EUA</p> </td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li>
     <li>100.20.126.137</li>
     <li>34.223.32.4</li>
     <li>52.39.176.220</li>
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] no cluster do Microsoft Azure</td> 
   <td> 
    <ul> 
     <li>20.36.133.48/28</li> 
     <li>20.81.156.240/28</li> 
     <li>172.172.84.48/28</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Incluir na lista de permissões Além disso, se a sua organização usar filtragem de rede de saída, adicione o seguinte domínio ao seu arquivo de pesquisa para permitir que o sistema acesse o Workfront Fusion.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] Centro de dados da UE</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] Data center dos EUA</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront Fusion] no cluster do Microsoft Azure</p> </td> 
   <td> <p>hook.app-az.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Filtragem de rede de saída incomum. Consulte o administrador da rede para verificar se é necessário atualizar a inclui na lista de permissões do para acomodá-la.

Incluir na lista de permissões Para obter mais informações sobre como configurar o arquivo de da sua organização, consulte [Configurar a inclui na lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).
