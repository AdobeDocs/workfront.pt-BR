---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Criar uma prova para um documento
description: Você pode gerar uma prova para um documento no momento em que estiver fazendo upload para o Workfront. Você também pode gerar uma prova para um documento já carregado no Adobe Workfront ou para uma nova versão de uma prova já no Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 4572ea9bb0679c599a55d5a87c1397c7b819c963
workflow-type: tm+mt
source-wordcount: '667'
ht-degree: 0%

---

# Criar uma prova para um documento

<!-- Audited: 1/2024 -->

Você pode gerar uma prova para um documento no momento em que estiver fazendo upload para o Workfront.

Você também pode gerar uma prova para um documento já carregado no Adobe Workfront ou para uma nova versão de uma prova já no Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> 
   <p>Novo: Qualquer um </p>
   <p>Atual: Pro ou superior</p> <p>Plano herdado: Select ou Premium</p> <p>Para obter mais informações sobre acesso de prova com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Novo: Padrão</p>
   <p>Atual : Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Carregar um documento e criar uma prova

1. Vá para o projeto, tarefa ou problema em que deseja criar uma nova prova.
1. Clique em **Documentos** guia.
1. Clique em Documentos ![](assets/document-icon.png) no painel esquerdo.
1. Clique em **Adicionar novo** e, em seguida, clique em **Prova** no menu exibido.

   >[!TIP]
   >
   >Você pode ativar o **Gerar provas automaticamente ao carregar documentos** configuração no seu perfil de usuário para automatizar esse processo. Para obter mais informações, consulte [Definir minhas configurações](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. No **Nova prova** que for exibida, você poderá

   * [Criar uma prova avançada com um fluxo de trabalho básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Carregar um documento e criar uma nova versão de uma prova

1. Vá para o projeto, tarefa ou problema em que deseja criar uma nova versão de uma prova existente.
1. Clique em **Documentos** guia.
1. Selecione o documento no qual deseja adicionar uma nova versão.
1. Clique em **Adicionar novo** > **Versão** > **Prova**.
1. No **Nova versão da prova** que for exibida, você poderá

   * [Criar uma prova avançada com um fluxo de trabalho básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Usar o arrastar e soltar para gerar uma prova simples para uma nova versão

Você pode arrastar e soltar um documento do seu sistema de arquivos (como a área de trabalho) para criar uma nova prova ou uma nova versão de uma prova existente. A prova contém as seguintes configurações, dependendo se você está criando uma nova prova ou uma nova versão:

* **Nova prova:** Cria uma prova simples que é compartilhada somente com você. Você poderá modificar as configurações de compartilhamento depois que a prova for criada, conforme descrito em [Editar configurações de prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nova versão da prova existente:** Cria uma nova versão com as mesmas configurações de prova da versão anterior.

Para usar o arrastar e soltar a fim de gerar uma nova prova ou nova versão de prova:

1. Verifique se as provas estão configuradas para serem geradas automaticamente, conforme descrito em .
1. Continuar com  [Adicionar documentos ao Adobe Workfront a partir do sistema de arquivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), que explica o método de arrastar e soltar usado para adicionar documentos. 

## Criar uma prova para um documento existente

1. Vá para o projeto, tarefa ou problema em que deseja a prova e clique no link **Documentos** seção.
1. Passe o mouse sobre o documento, em seguida clique no **Criar prova** link que aparece abaixo do nome do documento.

   >[!NOTE]
   >
   >Se você tiver **Gerar provas automaticamente ao carregar documentos** habilitado no seu perfil de usuário, o sistema cria automaticamente uma prova simples.

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
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho básico</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
