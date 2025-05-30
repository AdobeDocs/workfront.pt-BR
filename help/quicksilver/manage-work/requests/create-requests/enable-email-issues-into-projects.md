---
product-area: requests
navigation-topic: create-requests
title: Permitir que os usuários enviem por email um problema para um projeto da fila de solicitações
description: Você pode configurar um projeto para permitir que os usuários adicionem problemas ao projeto por email.
author: Alina, Courtney
feature: Work Management
exl-id: 556775e8-7ac9-482d-8c1c-863678584aa4
source-git-commit: 06e42fa713bc9b0c1e308feb2b84ca62dafa416c
workflow-type: tm+mt
source-wordcount: '782'
ht-degree: 0%

---

# Permitir que os usuários enviem um problema por email para um projeto da Fila de solicitações

<!-- Audited: 4/2025 -->

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;When updating POP account information here, also update information in these articles: Allowing users to reply to email notifications, Configuring Email Notifications, Understanding the Queue Details Tab in a Project )</p>
-->

Você pode configurar um projeto para permitir que os usuários adicionem problemas ao projeto por email. Você só poderá permitir que problemas sejam enviados por email para um projeto se ele for designado como uma Fila de solicitação. Para obter mais informações sobre como criar um projeto da Fila de solicitações, consulte [Criar uma Fila de solicitações](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p>Novo: Colaborador ou superior</p>
   Ou
   <p>Atual: solicitação ou superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a ocorrências</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

As seguintes condições são necessárias para configurar um projeto e permitir que os usuários adicionem problemas ao projeto por email:

* Os usuários que estão enviando problemas por email para esta conta devem ser usuários ativos com uma licença do Workfront.
* Os usuários que estão enviando problemas para esta conta devem ter permissões para Adicionar problema no projeto.
* Usuários externos não podem enviar problemas por email para uma fila de solicitações porque não têm acesso para criar problemas.
* Somente emails provenientes de um endereço de email associado a um usuário ativo do Workfront têm permissão para enviar problemas para o projeto. Os emails encaminhados para um email de usuário ativo do Workfront de um email não associado a uma conta do Workfront não podem criar problemas no projeto, pois o endereço de email do remetente original deve ser associado a uma conta ativa do Workfront.
* O projeto está configurado como uma Fila de solicitações.
* A conta de email associada ao projeto não está vinculada a uma conta de usuário do Workfront.

## Configurar o projeto no Workfront

>[!NOTE]
>
>Lembre-se do seguinte ao ativar as configurações de fila de emails:
>
>* O Workfront permite um email exclusivo por fila de solicitações em todos os clusters. Se optar por desativar a fila de solicitações, você manterá o endereço de email criado, desde que ele ainda esteja na caixa Endereço de email de entrada. Se optar por descontinuar o uso do email de entrada, você deverá excluí-lo do Campo Email de entrada para que ele possa estar disponível para uso futuro.
>
>* Se a fila de solicitações tiver vários tópicos da fila ou grupos de tópicos, o Workfront selecionará aleatoriamente o tópico da fila para o qual as solicitações enviadas por email serão direcionadas, tornando as solicitações enviadas por email difíceis de gerenciar.
>Recomendamos que o projeto configurado para receber solicitações por emails não tenha mais de um tópico de fila. Se as solicitações enviadas se destinam a recursos ou projetos diferentes, você deve direcioná-las ou movê-las manualmente após o envio.

1. Vá para o projeto que você deseja habilitar para receber problemas por email.
1. Clique em **Detalhes da fila** no painel esquerdo.
1. Na área **Tipo de Fila**, selecione **Publicar como Fila de Solicitação de Ajuda**.

1. Role para baixo até a área **Configurações da fila de emails** e selecione **Habilitar entrada de solicitação por email**.

1. Digite o início do endereço de email na caixa **Endereço de email de entrada**.

   Você deve criar um endereço de email exclusivo. Recomendamos usar o nome da sua empresa como parte do seu endereço de email de entrada.

   >[!CAUTION]
   >
   >* Esse endereço de email não poderá ser recuperado da lixeira se o projeto que contém a fila de solicitações for excluído.
   >
   >* Como esse endereço de email deve ser exclusivo, ele pode não estar disponível no futuro se for excluído.
   <!--
   >This was the case previously, but it's not working this way anymore, since August 2022: * Emails forwarded to this email address are not added as issues to the project in&nbsp;Workfront. Only emails created from this email address are added as issues.
   -->

1. (Opcional) Selecione a opção **Encaminhar todos os problemas que não forem enviados por email** e digite um endereço de email de encaminhamento na caixa abaixo.

   Esse endereço de email recebe informações sobre emails que não foram enviados para o projeto.

1. Clique em **Salvar**. Agora, quando usuários com uma conta ativa do Workfront enviam um email para esse endereço de email, um problema é criado no projeto do Workfront.

   >[!NOTE]
   >
   >Os usuários devem ter acesso para criar problemas no projeto a fim de enviar por email. Você pode conceder esse acesso na caixa de diálogo Compartilhamento, em Configurações avançadas.
   >
   >Usuários externos não podem enviar problemas por email para uma fila de solicitações porque não têm acesso para criar problemas.

## Receba o problema no Workfront

Quando um usuário do Workfront envia um email para o Workfront, as seguintes coisas acontecem:

* A linha Assunto do email se torna o Nome da ocorrência.
* O corpo do email se torna a Descrição do problema.
* Se houver documentos anexados ao email, eles serão anexados ao problema no Workfront.
* O usuário que está enviando o email se torna o contato principal do novo problema no Workfront.
* O corpo do texto do email não pode exceder 4.000 caracteres.
* Os anexos de email não podem exceder o total de 7 MB.
