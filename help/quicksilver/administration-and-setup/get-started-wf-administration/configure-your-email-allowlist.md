---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar seu Incluo na lista de permissões de email
description: Se sua organização usa o plano WorkfrontEnterprise, você pode criar um incluo na lista de permissões de email do Workfront para controlar quais domínios de email têm permissão para aceitar emails do Workfront e quais domínios de email podem estar no endereço de email que os usuários especificam em seus perfis de usuário. Isso é útil se a política de segurança de sua organização impedir que os usuários enviem dados armazenados no Workfront para endereços de email externos. Você pode incluir somente os domínios internos da empresa no incluo na lista de permissões para garantir que essa política seja seguida.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
TQID: https://experienceleague.adobe.com/a8hcTFpx3LmuGpQM8Wk8BpLDCFUVJWLAcP-YV5ogK0U
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 403
ht-degree: 7%

---

# Configurar seu incluo na lista de permissões de email

Se sua organização usar o plano Workfront Enterprise, você poderá criar um incluo na lista de permissões de email Workfront para controlar:

* Quais domínios de email têm permissão para aceitar emails do Workfront.
* Quais domínios de email podem estar no endereço de email que os usuários especificam em seus perfis de usuário.

Isso é útil se a política de segurança de sua organização impedir que os usuários enviem dados armazenados no Workfront para endereços de email externos. Você pode incluir somente os domínios internos da empresa no incluo na lista de permissões para garantir que essa política seja seguida.

>[!IMPORTANT]
>
>Sua equipe de TI deve garantir que os emails de entrada de `notifications@my.workfront.com` não sejam bloqueados no sistema de sua organização.
>
>Todos os emails do Workfront são enviados desse endereço para aumentar o sucesso do delivery de emails e eliminar a falsificação de emails. Isso inclui alertas automatizados e comunicação entre usuários.
>
>Por exemplo, a linha De em um email do Workfront recebido de um usuário chamado Joan Harris seria semelhante a:
>`Joan Harris <notifications@my.workfront.com>`

Para obter informações sobre como configurar o firewall da sua organização para abrir a comunicação entre o seu ambiente e os servidores da Adobe Workfront, consulte [Configurar o incluo na lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Padrão</p> <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador do Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Outras incluis na lista de permissões

Se o firewall ou servidor de e-mail estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao seu incluo na lista de permissões. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront. Para obter informações sobre isso, consulte [Configurar incluo na lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar seu incluo na lista de permissões de email

{{step-1-to-setup}}

1. Clique em **Sistema** > **Informações do cliente**.
1. Na seção **Incluo na lista de permissões de email**, selecione **Habilitar Incluo na lista de permissões de Domínio** e clique em **Adicionar Domínio**.
1. Na caixa que é exibida, digite um domínio que você deseja permitir, como `ourcompany.com`, e clique em **Adicionar domínio**.
1. Repita a etapa anterior para adicionar outros domínios que você deseja permitir.
1. Quando terminar, clique em **Salvar**.
