---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: security
title: Impedir usuários duplicados
description: Ao criar um novo usuário no Adobe Workfront, não é mais possível usar um endereço de email que já esteja sendo usado por outro usuário, mesmo que o endereço de email varie de acordo com o caso (por exemplo, JohnDoe@example.com e johndoe@example.com). Além disso, para se preparar para aprimoramentos de autenticação futuros, verifique se todos os usuários têm endereços de email exclusivos em uma instância do Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 84d9a752-e894-42cf-9b40-375e35f02c97
source-git-commit: 6f5b9e7638a85eca16d722cec6185cd5ed755eca
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# Impedir usuários duplicados

Ao criar um novo usuário no Adobe Workfront, não é mais possível usar um endereço de email que já esteja sendo usado por outro usuário, mesmo que o endereço de email varie de acordo com o caso (por exemplo, JohnDoe@example.com e johndoe@example.com). Além disso, para se preparar para aprimoramentos de autenticação futuros, verifique se todos os usuários têm endereços de email exclusivos em uma instância do Workfront.

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
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Walkthrough

<!--WRITER
<iframe class="vimeo-player_0" src="assets/371505632?" frameborder="0" allowfullscreen="1" width="560px" height="315px"></iframe>
-->

[Assista a uma demonstração em vídeo desse recurso.](https://vimeo.com/371505632/2e6938ce06)

## Criar usuários com endereços de email exclusivos

A partir da versão 2019.4, ao criar um novo usuário no Workfront, não será mais possível usar um endereço de email que já esteja sendo usado por outro usuário, mesmo que o endereço de email varie de acordo com o caso. Por exemplo, você não pode criar um usuário com o endereço de email JohnDoe@example.com se outro usuário tiver o endereço de email johndoe@example.com.

## Atualizar endereços de email de usuários existentes na instância do Workfront

Como administrador do Workfront, você deve atualizar os usuários existentes que têm endereços de email correspondentes que diferem somente por caso.
Para corrigir endereços de email duplicados em uma instância do Workfront:

1. Examine qualquer usuário duplicado e decida qual usuário não é mais necessário.

   1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Workfront, em seguida, clique em **Usuários**. ![](assets/users-icon-in-main-menu.png)

   1. No **Filtro** selecione **Todos**.

   1. No **Exibir** selecione **Logon do usuário**.

   1. No **Agrupamento** selecione **Nada**.

   1. Personalize a exibição Logon do usuário .

      1. Clique em **Exibir** > **Personalizar exibição**.

      1. Substitua o **ID** com a **Endereço de email** coluna.

      1. Renomeie a Exibição e salve-a.
   1. Crie um novo Agrupamento.

      1. Clique em **Agrupamento** > **Novo agrupamento**.

      1. Clique em **Alternar para o modo de texto** no canto superior direito da página.
      1. Cole o seguinte código de modo de texto:

         `group.0.linkedname=direct`
         `group.0.namekey=emailAddr`
         `group.0.valueexpression=LOWER({emailAddr})`
         `group.0.valueformat=string`
         `textmode=true`
   1. Renomeie o Grouping e salve-o.



1. Siga um destes procedimentos:

   * (Método preferencial) Adicione um endereço + ao endereço de email do usuário para cada conta adicional.

      Escolha essa opção se um único usuário em sua organização precisar acessar mais de uma conta de usuário. Se o endereço de mais não for suportado pelo seu provedor de email, você deverá fornecer uma conta de email separada para cada conta do Workfront.

      Por exemplo, John Doe pode ter uma conta de usuário para sua conta de uso diário e outra para usar para fins de teste:

      * johndoe@workfront.com
      * johndoe+reviewer@workfront.com
   * Altere o domínio para usar um domínio falso ao anexar o seguinte texto ao endereço de email:

      `.inactive`

      Por exemplo, John Doe pode ter os seguintes domínios: (Eles devem ser exclusivos.)

      * johndoe@workfront.inactive
      * johndoe@workfront.inactive2

      Não é mais possível fazer logon nessas contas porque as redefinições de senha exigem um endereço de email válido. Essas contas podem ser acessadas somente usando o recurso Fazer logon como .

   * Excluir usuários desnecessários

      >[!IMPORTANT]
      >
      >Escolha essa opção somente para contas que foram criadas por engano ou para contas de teste. Essa opção geralmente é executada somente para contas com logon zero ou 1 incorreto. As contas que foram usadas regularmente nunca devem ser excluídas.



Se você tiver usuários em uma instância do Workfront com endereços de email correspondentes que diferem somente por caso, a Workfront entrará em contato com você com informações adicionais e uma linha do tempo quando eles precisarem ser atualizados.
