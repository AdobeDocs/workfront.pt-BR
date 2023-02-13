---
title: Exibir informações de logon do usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Você pode ver a frequência com que os usuários fazem logon no Workfront, bem como a última vez que fizeram logon, indicando que deseja incluir essas informações na exibição de uma lista de usuários ou em um relatório para usuários.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# Exibir informações de logon do usuário

Você pode ver a frequência com que os usuários fazem logon no Adobe Workfront, bem como a última vez que fizeram logon, indicando que deseja incluir essas informações na exibição de uma lista de usuários ou em um relatório para usuários.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

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
   <td> <p>Plano </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter uma das seguintes opções:</p> 
    <ul> 
     <li> <p>O nível de acesso do Administrador do sistema. Para obter mais informações, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>. </p> </li> 
     <li> <p><b>Usuários</b> na configuração do seu nível de acesso configurado como <b>Editar</b> acesso, com <b>Criar</b> e pelo menos um dos dois <b>Administrador do usuário</b> opções ativadas em <b>Ajustar as configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se Usuário <b>Administrador (usuários do grupo)</b> estiver habilitado, você deve ser um administrador de grupo de um grupo no qual o usuário é membro.</p> <p>Para obter mais informações sobre o <b>Usuários</b> configurar em um nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Como o Workfront registra informações de logon

A Workfront registra as seguintes informações sobre os usuários que estão fazendo logon no sistema:

* **Contagem de logon**: O Workfront conta um usuário fazendo logon no aplicativo uma vez a cada 24 horas. Se um usuário fizer logon várias vezes usando navegadores, computadores ou dispositivos móveis diferentes, o Workfront contará todos os logons que ocorreram em um dia como um login. A Contagem de logon inclui informações que começam com quando o usuário foi criado.
* **Data do último logon**: A última data em que um usuário fez logon. A data de cada logon de qualquer navegador, dispositivo móvel ou outros aplicativos é registrada neste campo.

Fazer logon no Workfront de qualquer uma das seguintes maneiras conta como um logon no Workfront:

* A Aplicação Web Workfront
* Os aplicativos móveis do Workfront (dispositivos iOS ou Android)
* Qualquer integração do Workfront compatível com outro aplicativo de terceiros (Slack, Jira)
* Qualquer integração personalizada entre o Workfront e outro aplicativo de terceiros.
* A API do Workfront

   >[!NOTE]
   >
   >Fazer logon no Workfront por meio da API do Workfront só está disponível para organizações que ainda não estão integradas à Adobe Business Platform.

## Exibir informações de uso em uma lista de usuários ou relatório

Você pode exibir os campos Contagem de logon e Data do último logon na exibição de uma lista de usuários ou em um relatório para usuários.\
Para obter mais informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para exibir informações de uso na exibição de uma lista de usuários:

1. Vá para uma lista de usuários no Workfront.
1. No **Exibir** , selecione **Nova exibição**.

1. Clique em **Adicionar coluna** próximo ao canto inferior direito da tela.
1. No **Mostrar nesta coluna** , comece a digitar **Contagem de logon**, em seguida, selecione-o quando aparecer na lista em **Usuário**.

1. Clique em **Adicionar coluna** novamente.
1. No **Mostrar na coluna** , comece a digitar **Data do último logon**, em seguida, selecione-o quando aparecer na lista em **Usuário**.

1. (Opcional) Clique em **Opções avançadas**, em seguida selecione um **Formato de campo** no menu suspenso para incluir a hora ou o dia da semana do último logon na coluna .

1. Clique em **Salvar exibição**.\
   A exibição inclui informações sobre quantas vezes os usuários fizeram logon e quando fizeram logon por último.
