---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar a inclui na lista de permissões por email
description: Se sua organização usa o plano WorkfrontEnterprise, você pode criar um Workfront de email do incluir na lista de permissões para controlar quais domínios de email têm permissão para aceitar emails do Workfront e quais domínios de email podem estar no endereço de email especificado pelos usuários em seus perfis de usuário. Isso é útil se a política de segurança de sua organização impedir que os usuários enviem dados armazenados no Workfront para endereços de email externos — você pode incluir somente domínios internos da empresa no incluir na lista de permissões para garantir que essa política seja seguida.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '511'
ht-degree: 0%

---

# Configurar a inclui na lista de permissões por email

Se a sua organização usar o plano Workfront Enterprise, você poderá criar uma Workfront por email do incluir na lista de permissões para controlar:

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
>
```
>Joan Harris <notifications@my.workfront.com>
>```

Para obter informações sobre como configurar o firewall da sua organização para abrir a comunicação entre o seu ambiente e os servidores da Adobe Workfront incluir na lista de permissões, consulte [Configurar o arquivo do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Outras listas de permissões

Se sua organização tiver o plano Enterprise, você poderá configurar um Adobe Workfront incluir na lista de permissões IP que limite o acesso a 45 endereços IP da Workfront ou a intervalos de endereços IP especificados. Isso fornece uma camada adicional de segurança para o aplicativo do Workfront. Para obter mais informações, consulte [Restringir acesso ao Adobe Workfront pelo endereço IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Além disso, se o firewall ou servidor de e-mail estiver configurado para permitir o acesso a apenas determinados fornecedores, você deverá adicionar determinados endereços IP ao seu incluo na lista de permissões. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront. Incluir na lista de permissões Para obter informações sobre isso, consulte [Configurar o arquivo de consulta do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar a inclui na lista de permissões por email

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Informações do cliente**.

1. Na seção **Inclui na lista de permissões de email**, selecione **Habilitar Inclui na lista de permissões de Domínio** e clique em **Adicionar Domínio**.
1. Na caixa que é exibida, digite um domínio que você deseja permitir, como `ourcompany.com`, e clique em **Adicionar domínio**.

1. Repita a etapa anterior para adicionar outros domínios que você deseja permitir.
1. Quando terminar, clique em **Salvar**.
