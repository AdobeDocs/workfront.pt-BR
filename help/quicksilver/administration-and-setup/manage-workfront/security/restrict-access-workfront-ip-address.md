---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Restringir o acesso ao Adobe Workfront por endereço IP
description: Você pode configurar uma Adobe Workfront de lista de permissões IP do que limite o acesso ao Workfront a 45 endereços IP ou intervalos de endereço IP especificados por você. Isso fornece uma camada adicional de segurança para o aplicativo Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '448'
ht-degree: 1%

---

# Restringir o acesso ao Adobe Workfront por endereço IP

Você pode configurar uma Adobe Workfront de lista de permissões IP do que limite o acesso ao Workfront a 45 endereços IP ou intervalos de endereço IP especificados por você. Isso fornece uma camada adicional de segurança para o aplicativo Workfront.

Esses endereços IP ou intervalos de endereço IP devem ser fornecidos pelo administrador da rede.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td> <p>Enterprise</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Outras lista de permissões

Se o firewall ou servidor de email estiver configurado para permitir acesso somente a determinados fornecedores, você deverá adicionar determinados endereços IP à sua lista de permissões. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront. Para obter informações sobre isso, consulte [Configurar a  lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Além disso, se sua organização usar o Enterprise plan, você pode configurar a Workfront de lista de permissões de email do para controlar quais domínios de email têm permissão para aceitar emails do Workfront e quais domínios de email podem estar no endereço de email especificado pelos usuários no perfil de usuário do Workfront. Para obter mais informações, consulte [Configurar sua  de lista de permissões de email](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Adicionar endereços IP à  de lista de permissões

Após adicionar endereços IP à Workfront de lista de permissões da, somente esses endereços IP poderão ser usados para acessar o Workfront. Os usuários que tentarem acessar o Workfront a partir de outro endereço IP recebem uma mensagem de erro indicando que seu endereço IP está bloqueado.

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Informações do cliente.**

1. No **lista de permissões IP** seção , selecione **Habilite a  de lista de permissões IP.**

   Essa opção é desativada por padrão.

1. Especifique o endereço IP que você está usando no momento para acessar o sistema do Workfront.

   Ou

   Especifique um intervalo de endereços IP que inclua o que você está usando no momento para acessar o sistema do Workfront.

   O endereço IP que você está usando para acessar o Workfront deve ser adicionado à  de lista de permissões antes que a  de lista de permissões seja ativada.

1. Clique em **Adicionar intervalo IP,** em seguida, especifique o endereço IP ou o intervalo de endereços IP que você deseja que possa acessar o Workfront.
1. (Opcional) Repita a etapa anterior para adicionar outros endereços IP ou intervalos de endereço IP.

   É possível adicionar até 45 endereços ou intervalos.

1. Clique em **Salvar.**
