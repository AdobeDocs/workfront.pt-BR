---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Prova de um ativo vinculado para Experience Manager Assets ou Assets Essentials
description: Depois de vincular um ativo do Experience Manager Assets Essentials, você pode criar uma prova e atribuir usuários para revisar e adicionar comentários ao ativo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 3b063899c5c7992aad71d1eb8c8fafff7fda84c3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Prova de um ativo vinculado para Experience Manager Assets ou Assets Essentials

Depois de vincular um ativo do Experience Manager Assets Essentials, você pode criar uma prova e atribuir usuários para revisar e adicionar comentários ao ativo.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p> Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças Adobe Workfront*</td> 
   <td> <p>Trabalho ou superior</p>
   <p>Você deve ter a prova ativada para o usuário.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou Assets Essentials e deve ser adicionado ao produto como um usuário no Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Pré-requisitos

Antes de começar,

* O administrador do Workfront deve configurar uma integração com o Experience Manager. Para obter mais informações, consulte [Configurar a integração as a Cloud Service do Experience Manager Assets](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) ou [Configurar a integração do Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

## Criar uma prova

Você pode criar provas estáticas, de vídeo ou interativas.

Para criar uma prova:

1. Vá para o projeto, tarefa ou problema onde deseja obter a prova e clique no botão **Documentos** seção.
1. Passe o mouse sobre o documento e clique no botão **Criar prova** link que aparece abaixo do nome do documento.

   >[!NOTE]
   >
   >Se tiver **Gerar provas automaticamente ao carregar documentos** habilitado no perfil do usuário, o sistema cria automaticamente uma prova simples.

1. Escolha uma das opções a seguir:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Prova simples</strong></td> 
      <td>Essa opção cria uma prova sem workflow anexado e aplica as configurações de prova padrão. Você pode atualizar as configurações de prova padrão ou adicionar um fluxo de trabalho depois de criar a prova. Para obter mais informações sobre configurações de prova, consulte <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configurações de prova</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prova avançada</strong></td> 
      <td> <p>Essa opção permite configurar um workflow básico ou avançado e modificar as configurações de prova da prova criada. Para obter mais informações, consulte </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um workflow básico</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho Automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gerenciar uma prova existente

Depois de criar uma prova, você pode fazer coisas como

* Exibir atividade de estágio atual
* Atualizar revisores e prazos
* Editar o fluxo de trabalho

Para obter mais informações sobre como gerenciar uma prova existente, consulte [Gerenciar provas no Adobe Workfront](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Revisar uma prova

Os revisores atribuídos podem fazer coisas como

* Exibir o ativo e fazer comentários
* Adicionar ações aos comentários
* Comparar versões
* Aprovar ou rejeitar a prova

Para obter mais informações sobre o que você pode fazer com a ferramenta de prova, consulte [Revisar provas no Adobe Workfront](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
