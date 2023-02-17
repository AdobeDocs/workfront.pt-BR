---
product-area: documents
navigation-topic: approvals
title: Solicitar aprovações de documento
description: Você pode solicitar aprovação de gerentes ou outros usuários para um documento no Adobe Workfront. Você também pode solicitar aprovações de documentos de pessoas sem contas Workfront se o administrador do Workfront tiver habilitado esse recurso, conforme descrito em Configurar preferências de segurança do sistema.
author: Courtney
feature: Work Management
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
source-git-commit: 8e903592456512f1ebf5f1e8d6e496e577a7b352
workflow-type: tm+mt
source-wordcount: '569'
ht-degree: 0%

---

# Solicitar aprovações de documento

Você pode solicitar aprovação de gerentes ou outros usuários para um documento no Adobe Workfront. Você também pode solicitar aprovações de documentos de pessoas sem contas da Workfront se o administrador da Workfront tiver habilitado esse recurso, conforme descrito em [Configurar preferências de segurança do sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou aumentar o acesso a Projetos, Tarefas, Problemas, Modelos, Portfolio, Programas, Relatórios, Painéis e Calendários, Documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar acesso ao objeto associado à solicitação de acesso ou aprovação </p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Solicitar aprovação de documento

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a **Aprovações** no Resumo e comece a digitar no **Adicionar Aprovador** caixa de texto. Você pode adicionar usuários do Workfront por nome ou usuários externos por email.

1. Se o administrador do Adobe Workfront tiver habilitado a capacidade de colaborar com pessoas que não usam o Workfront, conforme descrito em [Configurar preferências de segurança do sistema](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md), você pode digitar os endereços de email para incluí-los.

   Não é possível solicitar aprovação de equipes ou grupos.

1. Repita a etapa anterior para adicionar outros aprovadores.

## Reenviar uma aprovação em uma nova versão

As decisões de aprovação de documentos não são redefinidas automaticamente ao carregar uma nova versão. Por exemplo, se seu documento for aprovado com alterações, a decisão mostrará &quot;alterações&quot; como a decisão, mesmo se você carregar uma nova versão com as alterações especificadas. Você pode limpar a decisão de uma nova versão se enviar novamente a aprovação manualmente.

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a **Aprovações** na seção Resumo, clique no ícone Mais e em Enviar novamente.

   ![](assets/nwe-resubmit-approval-350x149.png)

## Excluir uma solicitação de aprovação de documento

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a **Aprovações** na seção Resumo, em seguida, clique no botão **Mais** menu em linha com o nome do aprovador e selecione **Excluir**.

   A solicitação de aprovação é removida e o aprovador recebe uma notificação de que sua aprovação não é mais necessária. O acesso a compartilhamento relacionado à aprovação também é removido.

## Enviar um lembrete para um aprovador

Você pode enviar uma mensagem para lembrar um documento a um aprovador de que você está esperando seus comentários.

1. Vá para o projeto, tarefa ou problema que contém o documento e selecione **Documentos**.
1. Localize o documento necessário.

1. Role para baixo até a **Aprovações** na seção Resumo, em seguida, clique no botão **Mais** menu em linha com o nome do aprovador e selecione **Lembrar**.

   O aprovador recebe uma notificação informando que a aprovação ainda está pendente. Eles também podem receber um lembrete por email se tiverem isso ativado.
