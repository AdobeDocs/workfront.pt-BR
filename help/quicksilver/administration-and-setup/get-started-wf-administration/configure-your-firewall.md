---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Incluir na lista de permissões Configurar o arquivo de pesquisa do firewall
description: Incluir na lista de permissões Se o firewall ou o servidor de e-mail estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao seu arquivo. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront e permite que seus usuários enviem mensagens do Workfront e usem o SSO com o Ative Diretory ou o LDAP.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 264eed40-6d90-498b-83cc-2500c8b19c84
source-git-commit: 84444753db0e5c496f013e0245988e62fddad585
workflow-type: tm+mt
source-wordcount: '1635'
ht-degree: 0%

---

# Incluir na lista de permissões Configurar o arquivo de pesquisa do firewall

<!-- Audited: 12/2023 -->

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas ao Admin Console. Se sua organização tiver sido integrada à Adobe Admin Console, você deverá executar essa ação por meio da Adobe Admin Console.
>
>Para configurar sua inclui na lista de permissões se sua organização foi integrada à Adobe Admin Console, consulte [Domínios a serem permitidos para Aplicativos e Serviços Adobe](https://helpx.adobe.com/enterprise/kb/network-endpoints.html).
>
>Para obter uma lista de procedimentos que diferem com base no fato de sua organização ter sido integrada à Adobe Admin Console, consulte [Diferenças de administração baseadas em plataforma (Adobe Workfront/Adobe Business Platform)](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

>[!NOTE]
>
>A forma como uma organização configura sua inclui na lista de permissões é exclusiva para cada organização. Trabalhe com sua equipe de TI para identificar os procedimentos de sua organização e implementar essas adições.

Incluir na lista de permissões Se o firewall ou o servidor de e-mail estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao seu arquivo. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront e permite os seguintes processos:

* Envio de mensagens do aplicativo do Workfront

  >[!NOTE]
  >
  >Isso não estará disponível se a instância Workfront da sua organização estiver habilitada com o Adobe IMS. Consulte o administrador de rede ou de TI se precisar de mais informações.

* Uso de webhooks de documentos ao configurar integrações de documentos personalizadas
* Uso de assinaturas de evento do Workfront

  Para obter mais informações, consulte [API de Assinatura de Evento](https://experience.workfront.com/s/article/Event-Subscription-API-2100945680).

Você também precisa abrir determinadas portas para que as mensagens de email sejam criptografadas quando forem entregues.

## Workfront ➡ incluis na lista de permissões que você pode usar

Se sua organização tiver o plano Enterprise, você também poderá configurar duas Workfront do incluir na lista de permissões:

* **inclui na lista de permissões por email**: permite que você controle onde os usuários podem enviar dados de email armazenados no Workfront. Incluir na lista de permissões Para obter mais informações, consulte [Configurar a pesquisa de email](../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).
* **inclui na lista de permissões de IP**: limita o acesso ao Workfront a 45 endereços IP ou intervalos de endereços IP especificados, fornecendo uma camada adicional de segurança para o aplicativo Workfront. Para obter mais informações, consulte [Restringir acesso ao Adobe Workfront pelo endereço IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

## Localizar o cluster do Workfront

Os endereços IP que você deve adicionar ao arquivo de inclui na lista de permissões dependem do cluster em que o ambiente de Produção é executado.

Para localizar o cluster da organização:

1. Como administrador do Workfront, clique no ícone **Menu Principal** ![Menu Principal](assets/main-menu-icon.png) e em **Instalação**.
1. Na navegação à esquerda, clique em **Sistema** e selecione **Informações do cliente**.
1. Localize o campo **Configuração do Cluster** no canto superior direito da página. O cluster da sua organização está listado aqui.

   CL01 refere-se ao Cluster 1, CL02 é Cluster 2 e assim por diante.

Para obter mais informações, consulte a seção [Exibir o cluster da sua organização e o plano do Workfront](../../administration-and-setup/get-started-wf-administration/firewall-overview.md#view-your-organizations-cluster-and-workfront-plan) no artigo [Visão geral do firewall](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

## Endereços IP a serem adicionados ao incluo na lista de permissões

>[!IMPORTANT]
>
>Algumas integrações do Workfront não funcionam quando a inclui na lista de permissões é ativada porque não podem ser configuradas com um endereço IP estático. Para usar as integrações a seguir, é necessário desativar a inclui na lista de permissões.
>
>* Workfront para Google Workspace
>* Workfront para Outlook
>* Workfront para Salesforce

* [Endereços IP para permitir Clusters 1, 2, 3, 5, 7, 8 e 9](#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9)
* [Endereços IP para permitir para o Cluster 4](#ip-addresses-to-allow-for-cluster-4)
* [Endereços IP para permitir para o Cluster 6](#ip-addresses-to-allow-for-cluster-6)
* [Endereços IP para permitir uma Unidade de Teste](#IP%20Addre2)
* [Endereços IP permitidos ao implementar assinaturas de evento](#ip-addresses-to-allow-when-implementing-event-subscriptions)
* [Endereços IP para permitir autenticação aprimorada](#ip-addresses-to-allow-for-enhanced-authentication)
* [Endereços IP a serem adicionados para acessar o Workfront Fusion](#ip-addresses-to-add-for-accessing-workfront-fusion)
* [Endereços IP a serem adicionados para usar o Workfront para Jira](#ip-addresses-to-add-for-using-workfront-for-jira)
* [URLs a serem adicionados para todos os clusters do Workfront](#urls-to-add-for-all-clusters-workfront)

### Endereços IP para permitir Clusters 1, 2, 3, 5, 7, 8 e 9 {#ip-addresses-to-allow-for-clusters-1-2-3-5-7-8-and-9}

Se o ambiente de Produção estiver no cluster 1, 2, 3, 5 ou 7, você deverá permitir os seguintes endereços IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para SSO, webhooks de documentos ou outras funcionalidades</td> 
   <td> 
    <ul> 
     <li>35.160.0.242</li> 
     <li>34 213 36 118</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>34.211.224.9</li> 
     <li>54 218 48 56</li> 
     <li>52.36.154.34</li> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li> 
     <li>54.203.255.135/32</li> 
     <li>35.155.2.51/32</li> 
     <li>52.34.192.77/32</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para receber emails do aplicativo Workfront</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35 161 82 137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54 71 252 65</li> 
    </ul> <p>Para obter informações sobre os seguintes endereços IP, consulte <a href="../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md" class="MCXref xref">Novos endereços IP para email do Adobe Workfront com a versão 21.1</a></p> 
    <ul> 
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>23 251 237 109</li> 
     <li>23 251 237 106</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP a serem permitidos para Cluster 4 {#ip-addresses-to-allow-for-cluster-4}

Se o ambiente de Produção estiver no Cluster 4, adicione os seguintes endereços IP para SSO, integrações de webhook de documento e para receber email do aplicativo do Workfront:

* 52.31.132.175
* 52.19.188.226
* 52.28.49.94
* 52.29.41.175
* 52.29.197,69
* 52.48.124.108
* 69.169.230.231
* 69.169. 230,232
* 3.121.91.129
* 3.122.11.35
* 34 246 27 40
* 52 208 123 166
* 52.208.159.124
* 52.17.130.201
* 34 252 250 191
* 52.30.133.50
* 54.220.93.204
* 34 254 76 122
* 34.242.62.80/32
* 46.51.194.192/32
* 54.229.129.66/32

Para obter informações sobre os seguintes endereços IP, consulte [Novos endereços IP para email do Adobe Workfront com a versão 21.1](../../product-announcements/announcements/announcement-archive/new-email-ip-21-1.md)

* 23 251 239 98
* 23 251 239 99

### Endereços IP a serem permitidos para Cluster 6 {#ip-addresses-to-allow-for-cluster-6}

Se o ambiente de Produção estiver no Cluster 6, adicione os seguintes endereços IP.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para receber emails do aplicativo Workfront</td> 
   <td> 
    <ul> 
     <li>34.94.227.64</li> 
     <li>34.94.227,65</li> 
     <li>34.94.227,66</li> 
     <li>34.94.227.67</li> 
     <li>34.66.82.64</li> 
     <li>34.66.82.65</li> 
     <li>34.66.82.66</li> 
     <li>34.66.82.67</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para usar o serviço de email</td> 
   <td> 
    <ul> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
     <li>13.58.86.183</li> 
     <li>34.209.181.84</li> 
     <li>35 161 82 137</li> 
     <li>52.14.70.114</li> 
     <li>52.15.230.220</li> 
     <li>54 71 252 65 </li> 
    </ul> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">Para usar o serviço de email Mailgun</td> 
   <td> 
    <ul> 
     <li>143.55.228.56 </li> 
     <li>209.61.151.229</li> 
     <li>69.72.43.7</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP para permitir uma Unidade de Teste

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para receber emails do aplicativo Workfront ao usar um Test Drive</td> 
   <td> 
    <ul> 
     <li>69.42.126.188 </li> 
     <li>66 119 37 185</li> 
     <li>66 119 37 186</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para integrações de SSO e webhook de documento ao usar um Test Drive</td> 
   <td> 
    <ul> 
     <li> <p>69.42.126.188</p> <p>Esse endereço também deve ser adicionado ao incluo na lista de permissões para que seus usuários recebam emails do Workfront.</p> </li> 
     <li>66 119 37 186</li> 
     <li>66 119 37 167</li> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP permitidos ao implementar assinaturas de evento  {#ip-addresses-to-allow-when-implementing-event-subscriptions}

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
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para clientes em locais diferentes da Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54 218 48 56</li> 
     <li>52.39.217.230</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP para permitir autenticação aprimorada {#ip-addresses-to-allow-for-enhanced-authentication}

Adicione os seguintes endereços IP para usar a autenticação aprimorada para Pré-visualização ou Produção.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Se seu ambiente estiver no Cluster 1, 2, 3, 5, 7, 8 ou 9</td> 
   <td> 
    <ul> 
     <li>35 167 74 121</li> 
     <li>35 166 202 113</li> 
     <li>35.160.3.103</li> 
     <li>54 183 64 135</li> 
     <li>54.67.77.38</li> 
     <li>54.67.15.170</li> 
     <li>54 183 204 205</li> 
     <li>35 171 156 124</li> 
     <li>18.233.90.226</li> 
     <li>3.211.189.167</li> 
     <li>18.232.225.224</li> 
     <li>34.233.19.82</li> 
     <li>52.204.128.250</li> 
     <li>3.132.201.78</li> 
     <li>3.19.44.88</li> 
     <li>3.20.244.231</li> 
     <li>54 244 142 219</li> 
     <li>52.39.217.230</li> 
     <li>44 241 82 96</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Se seu ambiente estiver no Cluster 4</td> 
   <td> 
    <ul> 
     <li>52.28.56.226</li> 
     <li>52.28.45.240</li> 
     <li>52.16.224.164</li> 
     <li>52.16.193,66</li> 
     <li>34.253.4.94</li> 
     <li>52.50.106.250</li> 
     <li>52 211 56 181</li> 
     <li>52 213 38 246</li> 
     <li>52 213 74 69</li> 
     <li>52 213 216 142</li> 
     <li>35 156 51 163</li> 
     <li>35 157 221 52</li> 
     <li>52.28.184.187</li> 
     <li>52.28.212.16</li> 
     <li>52.29.176.99</li> 
     <li>52.57.230.214</li> 
     <li>54.76.184.103</li> 
     <li>52.210.122.50</li> 
     <li>52 208 95 174</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Endereços IP a serem adicionados para acessar o Workfront Fusion  {#ip-addresses-to-add-for-accessing-workfront-fusion}

Adicione os seguintes endereços IP ao seu arquivo de inclui na lista de permissões para habilitar o Workfront para acessar seu sistema.

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
     <li>34 254 76 122</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
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
   <td role="rowheader">Adobe Workfront EU Datacenter</td> 
   <td> <p> hook.app-eu.workfrontfusion.com </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront US Datacenter</p> </td> 
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

### Endereços IP a serem adicionados para usar o Workfront para Jira {#ip-addresses-to-add-for-using-workfront-for-jira}

Adicione os seguintes endereços IP à inclui na lista de permissões para usar a integração do Workfront para Jira.

O domínio jira.workfront.com também deve ser acessível a partir dos servidores corporativos. Esse domínio é necessário porque serve como middleware entre o Workfront e o Jira.

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
     <li>34 254 76 122</li> 
     <li>34 252 250 191</li> 
     <li>35 162 128 73</li> 
     <li>52.42.25.64</li> 
     <li>34 213 36 118</li> 
     <li>35.160.0.242 </li> 
     <li> <p>3.209.27.146</p> </li> 
     <li> <p>18.205.251.4</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para clientes em locais diferentes da Europa</td> 
   <td> 
    <ul> 
     <li>54 244 142 219</li> 
     <li>44 241 82 96</li> 
     <li>52.36.154.34</li> 
     <li>34.211.224.9</li> 
     <li>54 218 48 56</li> 
     <li>52.39.217.230</li> 
     <li>35 162 128 73</li> 
     <li>52.42.25.64</li> 
     <li>34 213 36 118</li> 
     <li>35.160.0.242 </li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Domínios a serem adicionados para acessar o Workfront

Incluir na lista de permissões Se sua organização usar filtragem de rede de saída, adicione os seguintes domínios ao seu arquivo de pesquisa para habilitar seu sistema a acessar o Workfront.

>[!NOTE]
>
>Filtragem de rede de saída incomum. Consulte o administrador da rede para verificar se é necessário atualizar a inclui na lista de permissões do para acomodá-la.

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
* *.static.workfront.com

  Este é um domínio estático que abrange todos os domínios a seguir. Você pode adicionar os domínios individuais se preferir:

   * mfe.static.workfront.com
   * mfe-c.static.workfront.com
   * mfe-preview-c.static.workfront.com
   * mfe-preview.static.workfront.com
   * mfe-review.static.workfront.com


## URLs a serem adicionados para todos os clusters do Workfront {#urls-to-add-for-all-clusters-workfront}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Para permitir que o conteúdo da ajuda seja exibido em seu ambiente do Workfront</td> 
   <td> 
    <ul> 
     <li>https://app.pendo.io/</li> 
     <li>https://cdn.pendo.io/</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Para permitir que o Workfront Proof acesse o Workfront em qualquer cluster, adicione-os a todos os ambientes</td> 
   <td> 
    <ul> 
     <li>*.workfront.com - Obrigatório para exibir provas no Workfront</li> 
     <li>*.proofhq.com - Obrigatório para exibir provas no Workfront Proof</li> 
     <li>*.proofhq.eu - obrigatório para exibir provas no Workfront Proof</li> 
    </ul> <p><b>NOTA</b>:  <p>Não oferecemos suporte à adição de endereços IP ao seu arquivo de inclui na lista de permissões para Workfront Proof. Eles se tornaram dinâmicos depois que o Workfront mudou para o AWS. Em vez disso, recomendamos que você permita somente domínios do Workfront Proof.</p> <p>Incluir na lista de permissões Se houver um problema com a adição desses domínios ao seu arquivo e você precisar de um endereço IP, entre em contato com o Suporte ao cliente da Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

## Endereços IP e URLs a serem adicionados para acessar o Workfront Proof

Você deve adicionar os seguintes endereços IP ao seu arquivo de inclui na lista de permissões para usar várias funções.

* [Para retornos de chamada e provas de captura na Web](#for-callbacks-and-webcapture-proofs)
* [Para email de saída](#for-outgoing-email)

### Para retornos de chamada e provas de captura na Web {#for-callbacks-and-webcapture-proofs}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Prod-US (clusters 1, 2, 3, 5 e 7)</td> 
   <td> 
    <ul> 
    <li>35.84.172.250</li>
     <li>34 213 36 118</li> 
     <li>35.160.0.242</li> 
     <li>3.209.27.146</li> 
     <li>18.205.251.4</li> 
     <li>35 165 152 202</li> 
     <li>54 184 151 122</li> 
     <li>35.84.40.190</li> 
     <li>54 218 48 56</li> 
     <li>34.211.224.9</li> 
     <li>52.36.154.34</li> 
     <li>34.232.138,38</li> 
     <li>54 237 6 156</li> 
     <li>54 237 12 32</li> 
     <li>44 241 82 96</li> 
     <li>54 244 142 219</li> 
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
    <li>34 255 252 190</li>
     <li>34 246 27 40</li> 
     <li>52 208 123 166</li> 
     <li>3.121.91.129</li> 
     <li>3.122.11.35</li> 
     <li>34 241 103 51</li> 
     <li>46.51.203.201</li> 
     <li>54 247 174 227</li> 
     <li>52.208.159.124</li> 
     <li>52.17.130.201</li> 
     <li>34 252 250 191</li> 
     <li>52.30.133.50</li> 
     <li>54.220.93.204</li> 
     <li>34 254 76 122</li> 
    </ul> <p><b>OBSERVAÇÃO</b>: não há mais suporte para opções de servidor DNS.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Para email de saída {#for-outgoing-email}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Prod-US (clusters 1, 2, 3, 5 e 7)</p> </td> 
   <td> 
    <ul> 
     <li> 23 251 237 106</li> 
     <li>23 251 237 107</li> 
     <li>23 251 237 108</li> 
     <li>54 240 60 174</li> 
     <li>54 240 60 175</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Prod-EU (Cluster 4)</td> 
   <td> 
    <ul> 
     <li>23 251 239 98</li> 
     <li>69.169.230.231</li> 
     <li>69 169 230 232</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Portas a serem abertas para obter o melhor desempenho do Workfront Proof

Abra as seguintes portas se tiver problemas com o carregamento de provas ou se não estiver trabalhando no Workfront Proof:

* 5671
* 5672
* 15671

## Portas a serem abertas para email criptografado

Os emails do aplicativo Workfront são enviados criptografados usando as portas 465 e 587. Se seu servidor de e-mail não suportar e-mails criptografados, os e-mails serão entregues descriptografados usando a porta 25.

## Notificações por email do Suporte da Workfront

Se você não estiver recebendo emails do Suporte da Workfront, adicione os domínios e endereços IP da Salesforce necessários. Para obter mais informações, consulte o artigo de ajuda do Salesforce sobre endereços IP e domínios que o Salesforce deve permitir.
