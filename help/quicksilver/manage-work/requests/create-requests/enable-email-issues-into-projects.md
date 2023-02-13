---
product-area: requests
navigation-topic: create-requests
title: Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações
description: Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações
author: Alina
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: ca3c28174dca24f14a75869bdc209569d8d8d1a0
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Você pode configurar um projeto para permitir que os usuários adicionem problemas ao projeto por email. Você pode permitir que os problemas sejam enviados por email para um projeto somente se o projeto for designado como uma Fila de solicitações. Para obter mais informações sobre como criar um projeto de Fila de solicitações, consulte [Criar uma fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a problemas</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Object permissions</td> 
    <td> <p>To configure the request queue, you must have Manage permissions to the project.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.<br></p> </td> 
   </tr>
  --> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Os pré-requisitos a seguir são necessários para configurar um projeto para permitir que os usuários adicionem problemas ao projeto por email.

Essas condições devem ser atendidas antes de habilitar esse recurso:

* Os usuários que estão enviando problemas por email para essa conta devem ser usuários ativos com uma licença para o Workfront.
* Usuários externos não podem enviar emails para uma fila de solicitações porque não têm acesso para criar problemas.
* Os usuários que estão enviando problemas por email para essa conta devem ter permissões para Adicionar problema no projeto.
* Os emails provenientes do endereço de email associado a um usuário ativo do Workfront são os únicos emails permitidos para enviar problemas ao projeto.
* O projeto é configurado como uma Fila de solicitações.
* A conta de email associada ao projeto não está vinculada a uma conta de usuário do Workfront.

## Configurar o projeto no Workfront

>[!NOTE]
>
>Lembre-se do seguinte ao ativar as configurações de fila de email:
>
>* O Workfront permite um email único por fila de solicitações em todos os clusters. Se você optar por desabilitar a fila de solicitações, manterá o endereço de email criado, desde que ele ainda esteja na caixa Endereço de email de entrada. Se você optar por descontinuar o uso do email de entrada, deverá excluí-lo do Campo de email de entrada para que ele possa ser disponibilizado para uso futuro.
>
>* Se a fila de solicitações tiver vários tópicos de fila ou grupos de tópicos, o Workfront selecionará aleatoriamente o tópico da fila para o qual as solicitações enviadas por email terão dificuldade de gerenciar.
   >Recomendamos que o projeto configurado para receber solicitações por meio de emails não tenha mais de um tópico da fila. Se as solicitações enviadas se destinarem a recursos ou projetos diferentes, você deve roteá-las ou movê-las manualmente, após terem sido enviadas.


1. Vá para o projeto que deseja habilitar para receber problemas por email.
1. Clique em **Detalhes da fila** no painel esquerdo. Talvez seja necessário clicar em **Mostrar mais** primeiro.
1. No **Tipo de fila** , selecione **Publicar como fila de solicitações de ajuda**.

1. Role para baixo até a **Configurações da fila de emails** e selecione **Habilitar a entrada de solicitação por email**.

1. Insira o início do endereço de email no **Endereço de email de entrada** caixa.

   Você deve criar um endereço de email exclusivo. Recomendamos usar o nome da sua empresa como parte do seu endereço de email de entrada.

   >[!CAUTION]
   >
   >* Esse endereço de email não poderá ser recuperado da lixeira se o projeto que contém a fila de solicitações for excluído.
   >
   >* Como esse endereço de email deve ser exclusivo, ele pode não estar disponível no futuro se for excluído.

   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Opcional) Selecione o **Encaminhar todos os problemas que não forem enviados por email**, em seguida, insira um endereço de email de encaminhamento na caixa abaixo.

   Esse endereço de email recebe informações sobre emails que não foram enviados ao projeto.

1. Clique em **Salvar**. Agora, quando usuários com uma conta ativa do Workfront enviam um email para esse endereço de email, um problema é criado no projeto do Workfront.

   >[!NOTE]
   >
   >Os usuários devem ter acesso para criar problemas no projeto para enviar por email. Você pode conceder esse acesso na caixa de diálogo Compartilhamento, em Configurações avançadas.
   >
   >Usuários externos não podem enviar emails para uma fila de solicitações porque não têm acesso para criar problemas.

## Receba o problema no Workfront

Quando um usuário do Workfront envia um email para o Workfront, as seguintes coisas acontecem:

* A linha Assunto do email torna-se o Nome do problema.
* O corpo do email torna-se a Descrição do problema.
* Se houver documentos anexados ao email, esses documentos serão anexados ao problema no Workfront.
* O usuário que está enviando o email se torna o Contato principal do novo problema no Workfront.
* O texto do corpo do email não pode exceder 4.000 caracteres.
* Os anexos de email não podem exceder o total de 7 MB.
