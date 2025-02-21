---
product-area: documents
navigation-topic: approvals
title: Solicitar aprovações de documentos
description: Você pode solicitar aprovação de gerentes ou outros usuários para um documento no Adobe Workfront. Você também pode solicitar aprovações de documentos de pessoas sem contas do Workfront se o administrador do Workfront tiver ativado esse recurso, conforme descrito em Configurar preferências de segurança do sistema.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 1%

---

# Solicitar aprovações de documentos

Você pode solicitar aprovação de gerentes ou outros usuários para um documento no Adobe Workfront. Você também pode solicitar aprovações de documentos de pessoas sem contas do Workfront se o administrador do Workfront tiver habilitado esse recurso, conforme descrito em [Configurar preferências de segurança do sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualize ou tenha acesso superior a projetos, tarefas, problemas, modelos, portfólios, programas, relatórios, painéis e calendários, documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso ao objeto associado à solicitação de acesso ou aprovação </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

+++

## Solicitar uma aprovação de documento

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a seção **Aprovações** no Resumo e comece a digitar na caixa de texto **Adicionar aprovador**. Você pode adicionar usuários do Workfront por nome ou usuários externos por email.

1. Se o administrador do Adobe Workfront tiver habilitado a capacidade de colaborar com pessoas que não usam o Workfront, conforme descrito em [Configurar preferências de segurança do sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), você poderá digitar seus endereços de email para incluí-los.

   Não é possível solicitar aprovação de equipes ou grupos.

1. Repita a etapa anterior para adicionar outros aprovadores.

## Reenviar uma aprovação para uma nova versão

As decisões de aprovação de documentos não são redefinidas automaticamente ao carregar uma nova versão. Por exemplo, se o documento for aprovado com alterações, a decisão mostrará &quot;alterações&quot; como a decisão, mesmo que você carregue uma nova versão com as alterações especificadas. Você pode limpar a decisão sobre uma nova versão se reenviar manualmente a aprovação.

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a seção **Aprovações** no Resumo, clique no ícone Mais e, em seguida, clique em Reenviar.

   ![Reenviar aprovação](assets/nwe-resubmit-approval-350x149.png)

## Excluir uma solicitação de aprovação de documento

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a seção **Aprovações** no Resumo e clique no menu **Mais** incorporado com o nome do aprovador e selecione **Excluir**.

   A solicitação de aprovação é removida e o aprovador recebe uma notificação de que sua aprovação não é mais necessária. O acesso compartilhado relacionado à aprovação também é removido.

## Enviar um lembrete a um aprovador

Você pode enviar uma mensagem para lembrar um documento a um aprovador que você está esperando pelo feedback dele.

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a seção **Aprovações** no Resumo e clique no menu **Mais** incorporado com o nome do aprovador e selecione **Lembrar**.

   O aprovador recebe uma notificação informando que a aprovação ainda está pendente. Eles também podem receber um lembrete por email se tiverem essa opção ativada.
