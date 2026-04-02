---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-locations
title: Configurar colaboradores de IA
description: Como administrador do Adobe Workfront, você pode configurar os Colaboradores de IA e atribuí-los a projetos e tarefas.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c38801ee-9750-4ffb-a912-cdcccfc7c60a
source-git-commit: 25c4d4435cc3507ab2d163600a8c42be66efd4c2
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 5%

---

# Configurar colaboradores de IA

{{highlighted-preview-article-level}}

Os Colaboradores de IA são uma maneira de integrar agentes de IA em seus projetos e tarefas. Você pode configurar um Colaborador de IA e atribuí-lo como faria com um usuário.

Por exemplo, você pode configurar um Colaborador de IA do tipo revisor com diretrizes da marca e, em seguida, atribuir esse colaborador para revisar um documento.

Os tipos disponíveis do AI Collaborator incluem:

* Revisor: crie um colaborador usando marcas ou cérebro de marca e atribua o colaborador como um revisor em ativos.

  Para obter mais informações, consulte [Introdução ao Workfront Content Reviewer](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/wf-ai-reviewer.md).

  >[!NOTE]
  >
  >Atualmente, o Revisor é o único tipo disponível de Colaborador de IA. Mais recursos do AI Collaborator estarão disponíveis no futuro.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] pacote</td> 
   <td><p>Standard, Prime ou Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licença</td> 
   <td><p>[!UICONTROL Padrão]</p>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
  </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos



* Sua organização deve ter um Contrato de IA de geração da Adobe assinado em arquivo.

  Para obter mais informações, consulte [Assinar o contrato da Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) no artigo Assistente de IA na Workfront.
* Você deve configurar uma marca no Workfront antes de usá-la para um Colaborador de IA do tipo Revisor.

  Para obter instruções, consulte [Criar e gerenciar marcas para o Revisor de Conteúdo](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/create-a-brand.md).

## Criar um novo Colaborador de IA do tipo Revisor

{{step-1-to-setup}}

1. Na navegação à esquerda, clique em **Colaboradores de IA**.
1. Clique em **Novo Colaborador** no canto superior direito da tela.
1. Clique em **Revisor** e em **Continuar**.

   >[!NOTE]
   >
   >Atualmente, somente o tipo Revisor está disponível. Mais tipos de colaborador de IA estarão disponíveis no futuro.

1. No campo Nome do Colaborador, informe um nome para o colaborador. Esse é o nome que aparece na lista de responsáveis disponíveis em uma tarefa.
1. Escolha se o colaborador usará uma marca ou um cérebro de marca para suas análises.
1. (Condicional) Se o Colaborador de IA usar um Cérebro de marca, selecione o locatário que ele usará.
1. (Condicional) Se o Colaborador de IA usar uma Marca, selecione a marca e a diretriz da marca que ele usará.
1. Clique em **Salvar**.

## Gerenciar colaboradores de IA

Você pode editar, copiar e excluir os colaboradores de IA existentes.

{{step-1-to-setup}}

1. Na navegação à esquerda, clique em **Colaboradores de IA**.
1. (Condicional) Para editar um Collaborator, clique no nome do Collaborator que deseja editar, faça qualquer edição na janela Editar Collaborator e clique em **Salvar**.
1. (Condicional) Para copiar um Collaborator, clique no ícone Copiar ![ícone Copiar](assets/copy-ai-collaborator.png) na linha do AI Collaborator que você deseja copiar, clique no nome da cópia, faça qualquer edição na janela Editar Collaborator e clique em **Salvar**.
1. (Condicional) Para excluir um Colaborador, clique no ícone Excluir ![ícone Excluir](assets/delete-collaborator-icon.png) na linha do Colaborador de IA que você deseja excluir e clique em **Excluir**.
