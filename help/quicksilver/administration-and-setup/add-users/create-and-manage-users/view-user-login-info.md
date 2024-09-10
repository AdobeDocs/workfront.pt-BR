---
title: Exibir informações de logon do usuário
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Você pode ver a frequência com que os usuários fazem logon no Workfront, bem como a última vez que fizeram logon, indicando que você deseja incluir essas informações na exibição de uma lista de usuários ou em um relatório para usuários.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 1%

---

# Exibir informações de logon do usuário

Você pode ver a frequência com que os usuários fazem logon no Adobe Workfront, bem como a última vez que fizeram logon, indicando que você deseja incluir essas informações na exibição de uma lista de usuários ou em um relatório para usuários.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td><p>Novo: Padrão</p><p>Ou</p><p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ter um dos seguintes:</p> 
    <ul> 
     <li> <p>O nível de acesso Administrador do sistema. </li> 
     <li> <p>A configuração <b>Usuários</b> no seu nível de acesso foi configurada para <b>Editar</b> acesso, com as opções <b>Criar</b> e pelo menos uma das duas opções <b>Administrador de Usuários</b> habilitadas em <b>Ajustar suas configurações</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>Dessas duas opções, se o Usuário <b>Administrador (Usuários de Grupo)</b> estiver habilitado, você deverá ser um administrador de grupo de um grupo do qual o usuário seja membro.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Como o Workfront registra as informações de logon

O Workfront registra as seguintes informações sobre os usuários que fazem logon no sistema:

* **Contagem de logon**: o Workfront conta um usuário que está fazendo logon no aplicativo uma vez a cada 24 horas. Se um usuário fizer logon várias vezes usando navegadores, computadores ou dispositivos móveis diferentes, o Workfront contará todos os logons que ocorreram em um dia como um logon. A Contagem de logon inclui informações que começam com quando o usuário foi criado.
* **Data do último logon**: a última data em que um usuário fez logon. A data de cada logon de qualquer navegador, dispositivo móvel ou outros aplicativos é registrada neste campo.

Fazer logon no Workfront de qualquer uma das seguintes maneiras conta como um logon no Workfront:

* A aplicação web do Workfront
* Os aplicativos móveis do Workfront (dispositivos iOS ou Android)
* Qualquer integração do Workfront compatível com outro aplicativo de terceiros (Slack, Jira)
* Qualquer integração personalizada entre o Workfront e outro aplicativo de terceiros.
* A API do Workfront

  >[!NOTE]
  >
  >Fazer logon no Workfront por meio da API do Workfront só está disponível para organizações que ainda não estão integradas à Plataforma comercial Adobe.

## Exibir informações de uso em uma lista de usuários ou relatório

Você pode exibir os campos Contagem de logon e Data do último logon na exibição de uma lista de usuários ou em um relatório para usuários.\
Para obter mais informações sobre como criar um relatório, consulte [Criar um relatório personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

Para exibir informações de uso na view de uma lista de usuários:

1. Ir para uma lista de usuários no Workfront.
1. No menu suspenso **Exibir**, selecione **Nova Exibição**.

1. Clique em **Adicionar coluna** próximo ao canto inferior direito da tela.
1. No campo **Mostrar nesta coluna**, comece digitando **Contagem de Logons** e selecione-a quando ela aparecer na lista em **Usuário**.

1. Clique em **Adicionar coluna** novamente.
1. No campo **Mostrar na coluna**, comece digitando **Data do Último Logon** e selecione-a quando ela aparecer na lista em **Usuário**.

1. (Opcional) Clique em **Opções Avançadas** e selecione um **Formato de Campo** no menu suspenso para incluir a hora ou o dia da semana do último logon na coluna.

1. Clique em **Salvar visualização**.\
   A visualização inclui informações sobre quantas vezes os usuários se conectaram e quando fizeram logon pela última vez.
