---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Restringir acesso ao Adobe Workfront pelo endereço IP
description: Você pode configurar um Adobe Workfront IP do incluir na lista de permissões que limita o acesso ao Workfront a 75 endereços IP ou intervalos de endereços IP especificados. Isso fornece uma camada adicional de segurança para o aplicativo do Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 65121fae364683373d2bc9abbe6672755d0cd09c
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# Restringir o acesso ao Adobe Workfront pelo endereço IP

>[!IMPORTANT]
>
>No momento, essa funcionalidade não está disponível para organizações que foram integradas à Adobe Admin Console. Ele estará disponível na Adobe Admin Console em uma versão futura.

Você pode configurar um Adobe Workfront IP do incluir na lista de permissões que limita o acesso ao Workfront a 75 endereços IP ou intervalos de endereços IP especificados. Isso fornece uma camada adicional de segurança para o aplicativo do Workfront.

Esses endereços IP ou intervalos de endereços IP devem ser fornecidos pelo administrador da rede.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Enterprise</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Outras listas de permissões

Incluir na lista de permissões Se o firewall ou o servidor de e-mail estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao seu arquivo. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront. Incluir na lista de permissões Para obter informações sobre isso, consulte [Configurar o arquivo de consulta do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Além disso, se sua organização usar o plano Enterprise, você poderá configurar o Workfront de email do incluir na lista de permissões para controlar quais domínios de email têm permissão para aceitar emails do Workfront e quais domínios de email podem estar no endereço de email especificado pelos usuários em seus perfis de usuário do Workfront. Incluir na lista de permissões Para obter mais informações, consulte [Configurar a pesquisa de email](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Adição de endereços IP ao incluo na lista de permissões

Depois de adicionar endereços IP ao arquivo de Workfront do incluir na lista de permissões, somente esses endereços IP poderão ser usados para acessar o Workfront. Os usuários que tentam acessar o Workfront a partir de outro endereço IP recebem uma mensagem de erro indicando que o endereço IP está bloqueado.

{{step-1-to-setup}}

1. Clique em **Sistema** > **Informações do Cliente.**

1. Na seção **inclui na lista de permissões de IP**, selecione **Habilitar inclui na lista de permissões de IP.**

   Essa opção está desabilitada por padrão.

1. Especifique o endereço IP que você está usando no momento para acessar o sistema Workfront.

   Ou

   Especifique um intervalo de endereços IP que inclua aquele que você está usando no momento para acessar o sistema Workfront.

   O endereço IP que você está usando para acessar o Workfront deve ser adicionado ao incluo na lista de permissões antes que a inclui na lista de permissões seja ativada.

1. Clique em **Adicionar intervalo de IPs** e especifique o endereço IP ou intervalo de endereços IP que você deseja que acesse o Workfront.
1. (Opcional) Repita a etapa anterior para adicionar mais endereços IP ou intervalos de endereço IP.

   Você pode adicionar até 75 endereços ou intervalos.

1. Clique em **Salvar.**
