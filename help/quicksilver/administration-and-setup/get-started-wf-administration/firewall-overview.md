---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Visão geral do firewall
description: Como a Adobe Workfront se comunica com a rede de sua organização, o firewall da organização deve ser configurado para permitir essa comunicação. Os firewalls são medidas de segurança altamente eficazes que funcionam separando a rede de uma organização da Internet. Eles garantem que somente os dados e o tráfego de rede selecionados possam se mover para dentro ou para fora da rede da organização. O firewall permite ou bloqueia dados com base no site que está enviando ou recebendo os dados. Como administrador da Adobe Workfront, você deve garantir que os dados enviados para ou da Workfront possam passar pelo firewall de sua organização.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Visão geral do firewall

Como a Adobe Workfront se comunica com a rede de sua organização, o firewall da organização deve ser configurado para permitir essa comunicação. Os firewalls são medidas de segurança altamente eficazes que funcionam separando a rede de uma organização da Internet. Eles garantem que somente os dados e o tráfego de rede selecionados possam se mover para dentro ou para fora da rede da organização. O firewall permite ou bloqueia dados com base no site que está enviando ou recebendo os dados. Como administrador da Adobe Workfront, você deve garantir que os dados enviados para ou da Workfront possam passar pelo firewall de sua organização.

Isso é feito por meio de uma  lista de permissões, que é essencialmente uma &quot;lista&quot; de sites &quot;permitidos&quot; a enviar ou receber dados por meio do firewall. Os sites podem ser identificados de uma das duas maneiras:

* **Endereço IP**: uma série de números como 52.31.132.175
* **Domínio**: parte de um URL, como &quot;this domain&quot; em www.thisdomain.com

O Workfront usa domínios e endereços IP específicos para comunicação da Web. Eles devem ser adicionados à  de lista de permissões de sua organização antes que você possa usar o Workfront em sua organização.

Geralmente, um  lista de permissões é configurado por um administrador de rede. Trabalhe com o administrador de rede da organização para garantir que o firewall permita esses endereços IP. Caso não saiba quem é o administrador da rede, o departamento de TI de sua organização pode apontá-lo na direção correta.

>[!IMPORTANT]
>
>Como administrador da Workfront, você deve garantir que esses endereços IP e domínios sejam adicionados à  de lista de permissões da sua organização. Isso é verdade mesmo se você não as adicionar. A Workfront não pode configurar a  de lista de permissões da sua organização.

## Coletar informações para configurar seu firewall

Para configurar o firewall para o Workfront, o administrador de rede precisa saber quais endereços IP e domínios serão adicionados. Algumas dessas informações estão disponíveis somente para um administrador do Workfront. Como administrador da Workfront, você deve localizar essas informações e fornecê-las ao administrador da rede.

>[!NOTE]
>
>A prática recomendada para a segurança é adicionar somente os domínios e endereços IP que se conectam à funcionalidade usada ativamente pela sua organização. Ao fornecer essas informações, você pode garantir que essa prática recomendada seja seguida.

Forneça ao administrador da rede as seguintes informações:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Endereços IP e domínios específicos para permitir</td> 
   <td> <p>O artigo <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configurar a  lista de permissões do firewall</a> contém a lista de endereços IP e domínios que sua organização deve adicionar à  de lista de permissões. </p> <p>O administrador de rede pode não ter acesso ao artigo "Configurar o firewall". Nesse caso, você deve fornecê-lo a eles. Não recomendamos imprimir uma cópia impressa (papel). Uma cópia digital permite que o administrador da rede copie e cole os endereços, o que é mais rápido e preciso do que digitar em uma cópia impressa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seu cluster</td> 
   <td>Para localizar o cluster de sua organização, consulte <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visualizar o cluster e o plano da Workfront de sua organização</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seu plano Workfront</td> 
   <td> <p>O plano de sua organização é um dos seguintes:</p> 
    <ul> 
     <li> <p>Enterprise </p> </li> 
     <li> <p>Negócio </p> </li> 
     <li> <p>Pro </p> </li> 
     <li> <p>Equipe </p> </li> 
    </ul> <p>Para localizar o plano, consulte <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Visualize o cluster da sua organização e o plano da Workfront.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Seu domínio</td> 
   <td> <p>Para localizar seu domínio, verifique o endereço da Web usado para se conectar ao Workfront.</p> <p>Exemplo: no endereço web <code>greatcompany.my.workfront.com</code>, o domínio é "grande empresa"</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Outros produtos Adobe Workfront</td> 
   <td> <p>Informe o administrador da rede se você tiver licenças para um dos seguintes:</p> 
    <ul> 
     <li> <p>Adobe Workfront Proof</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Integrações do Adobe Workfront</td> 
   <td>Informe o administrador da rede se você utilizar um dos seguintes procedimentos:
    <ul>
     <li><p><p>Workfront para Jira</p></p></li>
     <li><p>Workfront para G Suite</p></li>
     <li><p>Workfront para Microsoft Teams</p></li>
     <li><p>Workfront para Outlook</p></li>
     <li><p>Workfront para Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Funcionalidade adicional</td> 
   <td> <p>Informe o administrador da rede se você usar uma das seguintes opções:</p> 
    <ul> 
     <li> <p>Uma unidade de teste Workfront</p> </li> 
     <li> <p>Workfront Ascendente</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Se você adicionar algum desses produtos, integrações ou funcionalidades em uma data posterior, você deve entrar em contato com o administrador da rede para que eles possam ajustar a  da lista de permissões.

### Visualizar o cluster e o plano da Workfront de sua organização {#view-your-organization-s-cluster-and-workfront-plan}

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** no painel esquerdo
1. Para visualizar seu cluster, selecione **Informações do cliente**.

   Seu cluster é exibido perto do canto superior direito do **Informações básicas** seção.

   ![](assets/locate-cluster.png)

1. Para exibir o plano do Workfront, selecione **Licenças**.

   Seu plano é exibido próximo à parte inferior da página.

   ![](assets/locate-plan.png)
