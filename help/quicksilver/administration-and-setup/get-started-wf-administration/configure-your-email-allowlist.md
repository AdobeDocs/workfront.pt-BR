---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar Sua Inclui na lista de permissões De Email
description: Se sua organização usa o plano WorkfrontEnterprise, você pode criar um Workfront de email do incluir na lista de permissões para controlar quais domínios de email têm permissão para aceitar emails do Workfront e quais domínios de email podem estar no endereço de email especificado pelos usuários em seus perfis de usuário. Isso é útil se a política de segurança de sua organização impedir que os usuários enviem dados armazenados no Workfront para endereços de email externos — você pode incluir somente domínios internos da empresa no incluir na lista de permissões para garantir que essa política seja seguida.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: 15ea03bf586054f7ef421f8cacede6f42835a6e4
workflow-type: tm+mt
source-wordcount: '399'
ht-degree: 0%

---

# Configurar a inclui na lista de permissões por email

Se sua organização usar o plano Workfront Enterprise, você poderá criar um incluo na lista de permissões de e-mail Workfront para controlar:

* Quais domínios de email têm permissão para aceitar emails do Workfront.
* Quais domínios de email podem estar no endereço de email que os usuários especificam em seus perfis de usuário.

Isso é útil se a política de segurança de sua organização impedir que os usuários enviem dados armazenados no Workfront para endereços de email externos. Você pode incluir somente os domínios internos de sua empresa no incluo na lista de permissões para garantir que essa política seja seguida.

>[!IMPORTANT]
>
>Sua equipe de TI deve garantir que os emails de entrada de `notifications@my.workfront.com` não sejam bloqueados no sistema de sua organização.
>
>Todos os emails do Workfront são enviados desse endereço para aumentar o sucesso do delivery de emails e eliminar a falsificação de emails. Isso inclui alertas automatizados e comunicação entre usuários.
>
>Por exemplo, a linha De em um email do Workfront recebido de um usuário chamado Joan Harris seria semelhante a:
>&#x200B;>`Joan Harris <notifications@my.workfront.com>`

Para obter informações sobre como configurar o firewall da sua organização para abrir a comunicação entre o seu ambiente e os servidores da Adobe Workfront incluir na lista de permissões, consulte [Configurar o arquivo do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td><p>Standard</p> <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador do Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Outras listas de permissões

Incluir na lista de permissões Se o firewall ou o servidor de e-mail estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao seu arquivo. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront. Incluir na lista de permissões Para obter informações sobre isso, consulte [Configurar o arquivo de consulta do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar a inclui na lista de permissões por email

{{step-1-to-setup}}

1. Clique em **Sistema** > **Informações do cliente**.
1. Na seção **Inclui na lista de permissões de email**, selecione **Habilitar Inclui na lista de permissões de Domínio** e clique em **Adicionar Domínio**.
1. Na caixa que é exibida, digite um domínio que você deseja permitir, como `ourcompany.com`, e clique em **Adicionar domínio**.
1. Repita a etapa anterior para adicionar outros domínios que você deseja permitir.
1. Quando terminar, clique em **Salvar**.
