---
content-type: tips-tricks-troubleshooting
product-area: user-management
navigation-topic: tips-tricks-and-troubleshooting-groups
title: O nome de usuário já está em uso
description: Leia estas dicas quando você receber um erro de que o nome de usuário já está sendo usado.
author: Lisa
feature: People Teams and Groups
exl-id: dc9accf0-7ef4-4555-9b1c-d69b2110f3da
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '318'
ht-degree: 1%

---

# O nome de usuário já está em uso

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Administrador do sistema</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Questão

Ao criar um novo usuário, um erro [!UICONTROL Ops] é exibido informando que o nome de usuário já está em uso. Não há outras ocorrências deste email no sistema. Por que isso está sendo exibido?

## Solução

Isso pode ocorrer porque o nome de usuário ou o endereço de email não é exclusivo na instância [!DNL Adobe Workfront] atual. Os usuários podem ter o mesmo nome de usuário ou endereço de email em instâncias separadas. Por exemplo, o Usuário A pode ter os seguintes endereços de email associados a uma conta do [!DNL Workfront]: usera@company1.com e usera@company2.com.

>[!NOTE]
>
>O administrador [!DNL Workfront] principal não pode ter o mesmo nome de usuário ou endereço de email se estiver em instâncias separadas do Workfront no mesmo cluster.
>
>Se as instâncias estiverem em clusters diferentes, o administrador principal poderá ter o mesmo nome de usuário ou endereço de email. Você pode exibir o cluster em que sua instância está em [!UICONTROL Configuração] > [!UICONTROL Sistema] > [!UICONTROL Informações do Cliente].

### Verifique se o seu nome de usuário é exclusivo na instância

Verifique se o nome de usuário e o endereço de email são exclusivos na instância [!DNL Workfront] atual:

{{step-1-to-users}}

1. Na lista de pessoas, verifique na coluna **[!UICONTROL Email]** se não há emails duplicados.
1. Adicione uma coluna para o nome de usuário à visualização.

   1. No menu suspenso **[!UICONTROL Exibir]**, clique em **[!UICONTROL Personalizar Exibição]**.
   1. Clique em **[!UICONTROL Adicionar coluna]**.
   1. No campo de pesquisa, digite *[!UICONTROL username]*.
   1. Selecione **[!UICONTROL Usuário]** > **[!UICONTROL Nome de Usuário]**.
   1. Salve a exibição.\
      Isso resulta em uma visualização para exibir os nomes de usuário nos quais você pode procurar a duplicata.

1. Na lista de pessoas, verifique na coluna **[!UICONTROL Username]** se não há nomes de usuário duplicados.
