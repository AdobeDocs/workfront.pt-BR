---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: Configurar sua  de lista de permissões de email
description: Se sua organização usar o plano WorkfrontEnterprise, você poderá criar uma Workfront de lista de permissões de email do para controlar quais domínios de email têm permissão para aceitar emails do Workfront e quais domínios de email podem estar no endereço de email especificado pelos usuários em seu perfil de usuário. Isso é útil se a política de segurança de sua organização impedir que os usuários enviem dados armazenados no Workfront para endereços de email externos. Você pode incluir somente os domínios internos da empresa na lista de permissões para garantir que essa política seja seguida.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 76b6acc4-c432-47b4-90bf-6e37e970625f
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# Configurar sua  de lista de permissões de email

Se sua organização usar o plano WorkfrontEnterprise, você poderá criar uma Workfront de lista de permissões de email da para controlar:

* Quais domínios de email têm permissão para aceitar emails do Workfront.
* Quais domínios de email podem estar no endereço de email especificado pelos usuários em seus perfis de usuário.

Isso é útil se a política de segurança de sua organização impedir que os usuários enviem dados armazenados no Workfront para endereços de email externos. Você pode incluir somente os domínios internos da empresa na lista de permissões para garantir que essa política seja seguida.

>[!IMPORTANT]
>
>Sua equipe de TI deve garantir que o email recebido da `notifications@my.workfront.com` não está bloqueado no sistema de sua organização.
>
>Todos os emails do Workfront são enviados a partir desse endereço para aumentar o sucesso da entrega de email e eliminar a falsificação de emails. Isso inclui alertas automatizados e comunicação usuário a usuário.
>
>Por exemplo, a linha De em um email do Workfront recebido de um usuário chamado Joan Harris seria semelhante a:
>
```
>Joan Harris <notifications@my.workfront.com>
>```

Para obter informações sobre como configurar o firewall de sua organização para abrir a comunicação entre seu ambiente e os servidores da Adobe Workfront, consulte [Configurar a  lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Outras lista de permissões

Se sua organização tiver o Enterprise plan, você pode configurar uma Adobe Workfront de lista de permissões IP da que limita o acesso ao Workfront a 45 endereços IP ou intervalos de endereço IP especificados por você. Isso fornece uma camada adicional de segurança para o aplicativo Workfront. Para obter mais informações, consulte [Restringir o acesso ao Adobe Workfront por endereço IP](../../administration-and-setup/manage-workfront/security/restrict-access-workfront-ip-address.md).

Além disso, se o firewall ou servidor de email estiver configurado para permitir acesso somente a determinados fornecedores, você deverá adicionar determinados endereços IP à sua lista de permissões. Isso abre a comunicação entre seu ambiente e os servidores da Adobe Workfront. Para obter informações sobre isso, consulte [Configurar a  lista de permissões do firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

## Configurar sua  de lista de permissões de email

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Clique em **Sistema** > **Informações do cliente**.

1. No **de Lista de permissões de email** seção , selecione **Habilitar  de Lista de permissões de Domínio**, depois clique em **Adicionar domínio**.
1. Na caixa exibida, digite um domínio que você deseja permitir, como `ourcompany.com`, depois clique em **Adicionar domínio**.

1. Repita a etapa anterior para adicionar outros domínios que desejar permitir.
1. Quando terminar, clique em **Salvar**.
