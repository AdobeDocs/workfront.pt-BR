---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar a  lista de permissões do firewall
description: Se o firewall ou servidor de email estiver configurado para permitir acesso somente a determinados fornecedores, você deverá adicionar determinados endereços IP à sua lista de permissões. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront e permite que seus usuários enviem mensagens do Workfront e usem SSO com o Ative Diretory ou LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '1496'
ht-degree: 13%

---

# Configurar a  lista de permissões do firewall

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para configurar sua lista de permissões se a organização tiver sido integrada à Adobe Admin Console, consulte [Domínios permitidos para aplicativos e serviços do Adobe](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Para obter uma lista de procedimentos diferentes com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Se o firewall ou servidor de email estiver configurado para permitir acesso somente a determinados fornecedores, você deverá adicionar determinados endereços IP à sua lista de permissões. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront e permite os seguintes processos:

* Envio de mensagens do aplicativo Workfront

   >[!NOTE]
   >
   >Isso não estará disponível se a instância do Workfront de sua organização estiver habilitada com o Adobe IMS. Consulte seu administrador de rede ou de TI se precisar de mais informações.

* Uso de webhooks de documento ao configurar integrações de documento personalizadas
* Uso de assinaturas de evento do Workfront

   Para obter mais informações, consulte [API de assinatura de evento](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Você também precisa abrir determinadas portas para que as mensagens de email sejam criptografadas quando forem entregues.

## Workfront lista de permissões que você pode usar

Se sua organização tiver o Enterprise plan, você também pode configurar duas Workfront lista de permissões:

* **de lista de permissões de email**: Permite controlar onde os usuários podem enviar dados de email armazenados no Workfront. Para obter mais informações, consulte [Configurar sua  de lista de permissões de email](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **lista de permissões IP**: Limita o acesso ao Workfront a 45 endereços IP ou intervalos de endereço IP especificados por você, fornecendo uma camada adicional de segurança para o aplicativo Workfront. Para obter mais informações, consulte [Restringir o acesso ao Adobe Workfront por endereço IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Endereços IP para adicionar à lista de permissões

Os endereços IP que você deve adicionar à sua listas de permissões no firewall dependem do cluster em que seu ambiente de Produção é executado. Você pode descobrir qual cluster está exibindo Configuração > Sistema > Informações Personalizadas. Para obter mais informações, consulte a seção [Configurar informações básicas](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md#configuring-basic-info) no artigo [Configurar informações básicas para seu sistema](../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

>[!IMPORTANT]
>
>Algumas integrações do Workfront não funcionam quando a  de lista de permissões é ativada porque elas não podem ser configuradas com um endereço IP estático. Para usar as integrações a seguir, você deve desativar a  de lista de permissões.
>
>* Workfront para G Suite
>* Workfront para Outlook
>* Workfront para Salesforce


* [Endereços IP para permitir Clusters 1, 2, 3, 5, 7, 8 e 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Endereços IP para permitir o Cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [Endereços IP para permitir o Cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [Endereços IP para permitir uma unidade de teste](#IP%20Addre2)
* [Endereços IP a serem permitidos ao implementar assinaturas de evento](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Endereços IP para permitir autenticação aprimorada](#ip-addresses-to-allow-for-enhanced-authentication)
* [Endereços IP a serem adicionados para acessar o Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Endereços IP a serem adicionados para uso do Workfront para Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [Endereços IP a serem adicionados para uso do Workfront Ascent](#ip-addresses-to-add-for-using-workfront-ascent)
* [URLs a serem adicionados para todos os clusters Workfront](#urls-to-add-for-all-clusters-workfront)

### Endereços IP para permitir Clusters 1, 2, 3, 5, 7, 8 e 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Se o ambiente de Produção estiver no Cluster 1, 2, 3, 5 ou 7, você deve permitir os seguintes endereços IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para SSO, webhooks de documento ou outra funcionalidade</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34.213.36.118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.36.154.34</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para receber email do aplicativo Workfront</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65</li> 
    </ul> <p>Para obter informações sobre os seguintes endereços IP, consulte <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md" class="MCXref xref">Novos endereços IP para email do Adobe Workfront com a versão 21.1</a></p> 
    <ul> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>23.251.237.109</li> 
     <li>23.251.237.106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP para permitir o Cluster 4 {#ip-addresses-to-allow-for-cluster-4}

Se o ambiente de Produção estiver no Cluster 4, adicione os seguintes endereços IP para SSO, integração de webhook de documento e para receber email do aplicativo Workfront:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197.69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230.232
* 3.121.91.129
* 3.122.11.35
* 34.246.27.40
* 52.208.123.166
* 52.208.159.124
* 52.17.130.201
* 34.252.250.191
* 52.30.133.50
* 54.220.93.204
* 34.254.76.122

Para obter informações sobre os seguintes endereços IP, consulte [Novos endereços IP para email do Adobe Workfront com a versão 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21.1.md)

* 23.251.239.98
* 23.251.239.99

### Endereços IP para permitir o Cluster 6 {#ip-addresses-to-allow-for-cluster-6}

Se o ambiente de Produção estiver no Cluster 6, adicione os seguintes endereços IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para receber email do aplicativo Workfront</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227.65</li> 
     <li>34.94.227.66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para usar o serviço de email do AWS</td> 
   <td> 
    <ul> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35.161.82.137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54.71.252.65 </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP para permitir uma unidade de teste

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para receber email do aplicativo Workfront ao usar uma unidade de teste</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66.119.37.185</li> 
     <li>66.119.37.186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para SSO e integração de webhook de documento ao usar uma unidade de teste</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188:</p> <p>Esse endereço também deve ser adicionado à sua lista de permissões para que os usuários recebam emails do Workfront.</p> </li> 
     <li>66.119.37.186</li> 
     <li>66.119.37.167</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP a serem permitidos ao implementar assinaturas de evento  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

Para todos os ambientes, adicione os seguintes endereços IP para receber cargas das assinaturas de evento do Workfront.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Para clientes na Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para clientes em locais diferentes da Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP para permitir autenticação aprimorada {#ip-addresses-to-allow-for-enhanced-authentication}

Adicione os seguintes endereços IP para usar a autenticação aprimorada para Visualização ou Produção.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se o seu ambiente estiver no Cluster 1, 2, 3, 5, 7, 8 ou 9</td> 
   <td> 
    <ul> 
     <li>35.167.74.121</li> 
     <li>35.166.202.113</li> 
     <li>35.160.3.103</li> 
     <li>54.183.64.135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54.183.204.205</li> 
     <li>35.171.156.124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>44.241.82.96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se o seu ambiente estiver no Cluster 4</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193.66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52.211.56.181</li> 
     <li>52.213.38.246</li> 
     <li>52.213.74.69</li> 
     <li>52.213.216.142</li> 
     <li>35.156.51.163</li> 
     <li>35.157.221.52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52.208.95.174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP a serem adicionados para acessar o Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Adicione os seguintes endereços IP à sua lista de permissões para habilitar o Workfront Fusion a acessar o sistema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
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
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
   <td> <p>hook.app.workfrontfusion.com </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>A filtragem de rede de saída é incomum. Consulte o administrador da rede para verificar se é necessário atualizar a  de lista de permissões para acomodá-la.

### Endereços IP a serem adicionados para uso do Workfront para Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Adicione os seguintes endereços IP à sua lista de permissões para usar o Workfront para integração com Jira.

O domínio jira.workfront.com também deve estar acessível dos servidores corporativos. Esse domínio é necessário porque serve como middleware entre a Workfront e Jira.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> Para clientes na Europa</td> 
   <td> 
    <ul> 
     <li>52.30.133.50</li> 
     <li>52.208.159.124</li> 
     <li>54.220.93.204</li> 
     <li>52.17.130.201</li> 
     <li>34.254.76.122</li> 
     <li>34.252.250.191</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para clientes em locais diferentes da Europa</td> 
   <td> 
    <ul> 
     <li>54.244.142.219</li> 
     <li>44.241.82.96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54.218.48.56</li> 
     <li>52.39.217.230</li> 
     <li>35.162.128.73</li> 
     <li>52.42.25.64</li> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP a serem adicionados para uso do Workfront Ascent {#ip-addresses-to-add-for-using-workfront-ascent}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para acessar os recursos de treinamento do Workfront via Workfront Ascent</td> 
   <td> 
    <ul> 
     <li>18.223.140.34</li> 
     <li>3.13.223.30</li> 
     <li>3.13.19.112</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para receber notificações por email do Workfront Ascent</td> 
   <td> 
    <ul> 
     <li>23.251.227.75</li> 
     <li>23.251.227.76</li> 
     <li>23.251.227.77</li> 
     <li>23.251.227.78</li> 
     <li>23.251.227.79</li> 
     <li>23.251.227.80</li> 
     <li>23.251.227.81</li> 
     <li>23.251.227.82</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domínios a serem adicionados para acessar o Workfront

Se sua organização usar a filtragem de rede de saída, adicione os seguintes domínios à sua lista de permissões para permitir que seu sistema acesse o Workfront.

>[!NOTE]
>
>A filtragem de rede de saída é incomum. Consulte o administrador da rede para verificar se é necessário atualizar a  de lista de permissões para acomodá-la.

* `<your domain>`.my.workfront.com
* `<your domain>`.preview.workfront.com
* `<your domain>`.sb01.workfront.com
* `<your domain>`.sb02.workfront.com
* events.split.io
* sdk.split.io
* auth.split.io
* rum-http-intake.logs.datadoghq.com
* mfe.static.workfront.com
* https://app.pendo.io/
* https://cdn.pendo.io/

## URLs a serem adicionados para todos os clusters Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para permitir que o conteúdo da ajuda seja exibido no ambiente do Workfront</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para permitir que a Workfront Proof acesse o Workfront em qualquer cluster, adicione-os a todos os ambientes</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Necessário para exibir provas no Workfront</li> 
     <li>*.proofhq.com - Obrigatório para exibir provas na Workfront Proof</li> 
     <li>*.proofhq.eu - Obrigatório para exibir provas na Workfront Proof</li> 
    </ul> <p><b>Nota</b>:  <p>Não oferecemos suporte à adição de endereços IP à sua lista de permissões de  do Workfront Proof. Eles foram dinâmicos depois que o Workfront foi movido para o AWS. Em vez disso, recomendamos que você permita somente domínios da Workfront Proof.</p> <p>Se houver um problema ao adicionar esses domínios à sua lista de permissões e você precisar de um endereço IP, entre em contato com o Suporte ao cliente da Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Endereços IP e URLs a serem adicionados para acessar a Workfront Proof

Você deve adicionar os seguintes endereços IP à sua lista de permissões para usar várias funções.

* [Para retornos de chamada e provas de captura da Web](#for-callbacks-and-webcapture-proofs)
* [Para email de saída](#for-outgoing-email)

### Para retornos de chamada e provas de captura da Web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (Clusters 1, 2, 3, 5 e 7)</td> 
   <td> 
    <ul> 
     <li>34.213.36.118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35.165.152.202</li> 
     <li>54.184.151.122</li> 
     <li>35.84.40.190</li> 
     <li>54.218.48.56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138.38</li> 
     <li>54.237.6.156</li> 
     <li>54.237.12.32</li> 
     <li>44.241.82.96</li> 
     <li>54.244.142.219</li> 
     <li>52.39.217.230</li> 
     <li>52.207.47.153</li> 
     <li>50.16.118.214</li> 
     <li>52.54.180.191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>34.246.27.40</li> 
     <li>52.208.123.166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34.241.103.51</li> 
     <li>46.51.203.201</li> 
     <li>54.247.174.227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34.252.250.191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34.254.76.122</li> 
    </ul> <p><b>OBSERVAÇÃO</b>: As opções do servidor DNS não são mais suportadas.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Para email de saída {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (Clusters 1, 2, 3, 5 e 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23.251.237.106</li> 
     <li>23.251.237.107</li> 
     <li>23.251.237.108</li> 
     <li>54.240.60.174</li> 
     <li>54.240.60.175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>23.251.239.98</li> 
     <li>69.169.230.231</li> 
     <li>69.169.230.232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Portas a serem abertas para obter o melhor desempenho da Workfront Proof

Abra as seguintes portas se tiver problemas com o carregamento de provas ou se não estiver funcionando na Workfront Proof:

* 5671
* 5672
* 15671

## Portas para abrir para email criptografado

Os emails do aplicativo Workfront são enviados criptografados usando as portas 465 e 587. Se o seu servidor de e-mail não suporta e-mail criptografado, os e-mails são entregues sem criptografia usando a porta 25.

## Notificações por email do Suporte Workfront

Se não estiver recebendo emails do Suporte da Workfront, adicione os domínios e endereços IP do Salesforce que você precisar. Para obter mais informações, consulte o artigo de ajuda do Salesforce sobre domínios e endereços IP do Salesforce a serem permitidos.
