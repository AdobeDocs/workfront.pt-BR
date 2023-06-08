---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Impedir usuários duplicados
description: Ao criar um novo usuário no Adobe Workfront, você não pode mais usar um endereço de email que já esteja sendo usado por outro usuário, mesmo que o endereço de email varie de acordo com letras maiúsculas e minúsculas (por exemplo, JohnDoe@example.com e johndoe@example.com). Além disso, para se preparar para futuros aprimoramentos de autenticação, verifique se todos os usuários têm endereços de email exclusivos em uma instância do Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 8bcc2859b3b6ce7a264c8f234536a93b7761ab6b
workflow-type: tm+mt
source-wordcount: '608'
ht-degree: 0%

---

# Impedir usuários duplicados

Ao criar um novo usuário no Adobe Workfront, você não pode mais usar um endereço de email que já esteja sendo usado por outro usuário, mesmo que o endereço de email varie de acordo com letras maiúsculas e minúsculas (por exemplo, JohnDoe@example.com e johndoe@example.com). Além disso, para se preparar para futuros aprimoramentos de autenticação, verifique se todos os usuários têm endereços de email exclusivos em uma instância do Workfront.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>NOTA</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Criar usuários com endereços de email exclusivos

A partir da versão 2019.4, ao criar um novo usuário no Workfront, não será mais possível usar um endereço de email que já esteja sendo usado por outro usuário, mesmo que o endereço de email varie de acordo com cada caso. Por exemplo, não é possível criar um usuário com o endereço de email JohnDoe@example.com se outro usuário tiver o endereço de email johndoe@example.com.

## Atualizar endereços de email de usuários existentes na instância do Workfront

Como administrador do Workfront, você deve atualizar os usuários existentes que têm endereços de email correspondentes que diferem apenas em maiúsculas e minúsculas.
Para corrigir endereços de email duplicados em uma instância do Workfront:

1. Examine todos os usuários duplicados e decida qual usuário não é mais necessário.

   1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront e clique em **Usuários**. ![](assets/users-icon-in-main-menu.png)

   1. No **Filtro** selecione **Todos**.

   1. No **Exibir** selecione **Logon de usuário**.

   1. No **Agrupamento** selecione **Nada**.

   1. Personalize a visualização Logon do usuário.

      1. Clique em **Exibir** > **Personalizar visualização**.

      1. Substitua o **ID** com a variável **Endereço de e-mail** coluna.

      1. Renomeie a Exibição e salve-a.
   1. Crie um novo Agrupamento.

      1. Clique em **Agrupamento** > **Novo Agrupamento**.

      1. Clique em **Alternar para modo de texto** no canto superior direito da página.
      1. Cole o seguinte código de Modo de texto:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. Renomeie o agrupamento e salve-o.



1. Siga um destes procedimentos:

   * (Método preferencial) Adicione um endereço + ao endereço de email do usuário para cada conta adicional.

      Escolha essa opção se um único usuário em sua organização precisar acessar mais de uma conta de usuário. Se o endereçamento plus não for suportado pelo seu provedor de email, você deverá fornecer uma conta de email separada para cada conta do Workfront.

      Por exemplo, John Doe pode ter uma conta de usuário para sua conta de uso diário e uma para usar para fins de teste:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * Altere o domínio para usar um domínio falso anexando o seguinte texto ao endereço de email:

      `.inactive`

      Por exemplo, João da Silva pode ter os seguintes domínios: (eles devem ser exclusivos.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      Você não pode mais fazer logon nessas contas porque as redefinições de senha exigem um endereço de email válido. Essas contas podem ser acessadas somente usando o recurso Fazer logon como.

   * Excluir usuários desnecessários

      >[!IMPORTANT]
      >
      >Escolha essa opção somente para contas que foram criadas por engano ou para contas de teste. Normalmente, essa opção é executada somente para contas com zero ou 1 logon incorreto. As contas que foram usadas regularmente nunca devem ser excluídas.



Se você tiver usuários em uma instância do Workfront com endereços de email correspondentes que diferem apenas por letras maiúsculas e minúsculas, a Workfront entrará em contato com você com informações adicionais e uma linha do tempo quando eles precisarem ser atualizados.
