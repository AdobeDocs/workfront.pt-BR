---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: Revisar um ativo vinculado com o conector aprimorado
description: Depois de vincular um ativo do Experience Manager Assets, você pode criar uma prova e atribuir usuários para revisar e adicionar comentários ao ativo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d72ac84f-1865-4122-bc77-d8200a4d0f69
TQID: https://experienceleague.adobe.com/hM4RFyi3jYJivKSovgU5lqP4zhdQSeH6SCWDgxL-rMk
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 387
ht-degree: 17%

---

# Revisar um ativo vinculado com o conector aprimorado

Depois de vincular um ativo do Experience Manager Assets, você pode criar uma prova e atribuir usuários para revisar e adicionar comentários ao ativo. Provas criadas a partir de ativos vinculados são contabilizadas em relação à cota de armazenamento de prova.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Padrão</p>
   <p>Trabalho ou maior</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produtos adicionais</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Acesso de visualização ou superior em um documento</p> </td> 
  </tr> 
 </tbody> 
</table>


Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Antes de começar, você deve

* Instale o conector aprimorado do Workfront para Experience Manager

## Criar uma prova

É possível criar provas estáticas, de vídeo ou interativas.

Para criar uma prova:

1. Vá para o projeto, tarefa ou problema em que deseja a prova e clique na seção **Documentos**.
1. Passe o mouse sobre o documento e clique no link **Criar prova**, que aparece abaixo do nome do documento.

   >[!NOTE]
   >
   >Se você tiver o **Gerar provas automaticamente ao carregar documentos** habilitado no seu perfil de usuário, o sistema criará automaticamente uma prova simples.

1. Escolha uma das seguintes opções:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Prova simples</td> 
      <td>Essa opção cria uma prova sem fluxo de trabalho anexado e aplica as configurações de prova padrão. Você pode atualizar as configurações de prova padrão ou adicionar um fluxo de trabalho depois de criar a prova. Para obter mais informações sobre configurações de prova, consulte <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configurações de prova</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prova avançada</td> 
      <td> <p>Essa opção permite configurar um fluxo de trabalho Básico ou Avançado e modificar configurações de prova para a prova criada. Para obter mais informações, consulte </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho Básico</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gerenciar uma prova existente

Depois de criar uma prova, você pode fazer coisas como

* Exibir atividade de estágio atual
* Atualizar revisores e prazos
* Editar o fluxo de trabalho

Para obter mais informações sobre como gerenciar uma prova existente, consulte [Gerenciar provas no Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md).

## Revisar uma prova

Os revisores atribuídos podem fazer coisas como

* Exibir o ativo e fazer comentários
* Adicionar ações a comentários
* Comparar versões
* Aprovar ou rejeitar a prova

Para obter mais informações sobre o que você pode fazer com a ferramenta de revisão, consulte [Revisar provas no Adobe Workfront](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
