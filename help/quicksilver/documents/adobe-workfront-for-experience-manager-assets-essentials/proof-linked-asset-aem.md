---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Teste de um ativo vinculado para Experience Manager Assets ou Assets Essentials
description: Depois de vincular uma ativo da Experience Manager Assets Essentials, você pode criar um prova e atribuir usuários para revisar e adicionar comentários ao ativo.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abd641a1-081b-4b86-95ee-f0ed030d704c
source-git-commit: 5d818b2e3c3314c6af076df46f7f806214f97bab
workflow-type: tm+mt
source-wordcount: '506'
ht-degree: 1%

---

# Teste de um ativo vinculado para Experience Manager Assets ou Assets Essentials

Depois de vincular uma ativo da Experience Manager Assets Essentials, você pode criar um prova e atribuir usuários para revisar e adicionar comentários ao ativo.

## Requisitos de acesso

<!-- Audited: 4/2025 -->

+++ Expanda para visualização requisitos de acesso do funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems plano da Workfront</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças da Adobe Systems Workfront</td> 
   <td> 
   <p>Novo: Padrão</p>
   <p>Ou</p>
   <p>Atual: trabalho ou superior</p>
   <p>A prova deve estar ativada para o usuário.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produto</td> 
   <td>Você deve ter o Experience Manager as a Cloud Service ou o Assets Essentials e deve ser adicionado ao produto como usuário na Admin Console. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir acesso ou superior</p> <p>Para obter informações sobre a solicitação de acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Os requisitos de acesso na documentação](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) da Workfront.

+++

## Pré-requisitos

Antes de começar:

* O administrador da Workfront deve configurar uma integração Experience Manager. Para obter mais informações, consulte [Configurar a Experience Manager Assets como uma integração](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) Cloud Service ou [configurar a integração](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md) Experience Manager Assets Essentials.

## Criar uma prova

Você pode criar provas estáticas, de vídeo ou interativas.

Para criar um prova:

1. Vá para o projeto, tarefa ou emite onde deseja a prova e clique na **seção Documentos** .
1. Passe o mouse sobre a documento e clique na **Criar Proof** link exibida abaixo do nome documento.

   >[!NOTE]
   >
   >Se você tiver o **Gerar provas automaticamente ao carregar documentos** habilitado no seu perfil de usuário, o sistema criará automaticamente uma prova simples.

1. Escolha uma das seguintes opções no menu suspenso:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Prova simples</strong></td> 
      <td>Essa opção cria uma prova sem fluxo de trabalho anexado e aplica as configurações de prova padrão. Você pode atualizar as configurações de prova padrão ou adicionar um fluxo de trabalho depois de criar a prova. Para obter mais informações sobre configurações de prova, consulte <a href="../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configurações de prova</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prova avançada</strong></td> 
      <td> <p>Essa opção permite configurar um fluxo de trabalho Básico ou Avançado e modificar configurações de prova para a prova criada. Para obter mais informações, consulte: </p> 
       <ul> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho Básico</a> </p> </li> 
        <li> <p><a href="../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

## Gerenciar uma prova existente

Depois de criar uma prova, faça o seguinte:

* Exibir atividade do estágio atual
* Atualizar revisores e prazos
* Editar o fluxo de Trabalho

Para obter mais informações sobre como gerenciar um prova existente, consulte [Gerenciar provas Adobe Systems Workfront: índice](../../review-and-approve-work/proofing/managing-proofs-within-workfront/manage-proofs-in-wf.md) de artigo.

## Revisar uma prova

Os revisores atribuídos podem fazer o seguinte:

* Exibir o ativo e fazer comentários
* Adicionar ações a comentários
* Comparar versões
* Aprovar ou rejeitar a prova

Para obter mais informações sobre o que você pode fazer com a ferramenta de revisão, consulte [Revisar provas no Adobe Workfront: índice do artigo](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).
