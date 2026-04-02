---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Restringir acesso ao Adobe Workfront pelo endereço IP
description: Você pode configurar um incluo na lista de permissões IP da Adobe Workfront que limite o acesso ao Workfront a 75 endereços IP ou intervalos de endereços IP especificados. Isso fornece uma camada adicional de segurança para o aplicativo do Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 10%

---

# Restringir o acesso ao Adobe Workfront pelo endereço IP

<!--
>[!IMPORTANT]
>
>This functionality is not currently available to organizations that have been onboarded to the Adobe Admin Console. It will be available in the Adobe Admin Console in a future release.
-->

Você pode configurar um incluo na lista de permissões IP da Adobe Workfront que limite o acesso ao Workfront a 75 endereços IP ou intervalos de endereços IP especificados. Isso fornece uma camada adicional de segurança para o aplicativo do Workfront.

Esses endereços IP ou intervalos de endereços IP devem ser fornecidos pelo administrador da rede.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p><p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Outras incluis na lista de permissões

Se o firewall ou servidor de e-mail estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao seu incluo na lista de permissões. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront. Para obter informações sobre isso, consulte [Configurar incluo na lista de permissões do firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Além disso, se sua organização usar o plano Enterprise, você poderá configurar o incluo na lista de permissões de email do Workfront para controlar quais domínios de email têm permissão para aceitar emails do Workfront e quais domínios de email podem estar no endereço de email especificado pelos usuários em seus perfis de usuário do Workfront. Para obter mais informações, consulte [Configurar seu incluo na lista de permissões de email](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Adicionar endereços IP ao incluo na lista de permissões

Depois de adicionar endereços IP ao incluo na lista de permissões Workfront, somente esses endereços IP podem ser usados para acessar o Workfront. Os usuários que tentam acessar o Workfront a partir de outro endereço IP recebem uma mensagem de erro indicando que o endereço IP está bloqueado.

{{step-1-to-setup}}

1. Clique em **Sistema** > **Informações do cliente.**

1. Na seção **incluo na lista de permissões IP**, selecione **Habilitar incluo na lista de permissões IP.**

   Essa opção está desabilitada por padrão.

1. Especifique o endereço IP que você está usando no momento para acessar o sistema Workfront.

   Ou

   Especifique um intervalo de endereços IP que inclua aquele que você está usando no momento para acessar o sistema Workfront.

   O endereço IP que você está usando para acessar o Workfront deve ser adicionado ao incluo na lista de permissões antes que o incluo na lista de permissões seja ativado.

1. Clique em **Adicionar intervalo de IPs** e especifique o endereço IP ou intervalo de endereços IP que você deseja que acesse o Workfront.
1. (Opcional) Repita a etapa anterior para adicionar mais endereços IP ou intervalos de endereço IP.

   Você pode adicionar até 75 endereços ou intervalos.

1. Clique em **Salvar.**
