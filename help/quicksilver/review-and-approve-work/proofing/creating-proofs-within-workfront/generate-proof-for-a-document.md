---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Criar uma prova para um documento
description: Você pode gerar uma prova para um documento no momento em que estiver fazendo upload para o Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 609e95fa-1fb3-4cc4-9ee8-403fd2f30e10
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# Criar uma prova para um documento

Você pode gerar uma prova para um documento no momento em que estiver fazendo upload para o Workfront.

Você também pode gerar uma prova para um documento já carregado no Adobe Workfront ou para uma nova versão de uma prova já no Workfront.

<!--
If a proof fails to generate after following the steps described in the following sections, see [Troubleshoot proof creation failures](../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/troubleshooting-proof-creation-failures.md).
-->

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou superior</p> <p>ou</p> <p>Plano herdado: Selecionar ou Premium</p> <p>Para obter mais informações sobre como revisar o acesso com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de prova no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer (É necessário ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Carregar um documento e criar uma prova

1. Vá para o projeto, tarefa ou problema onde deseja criar uma nova prova.
1. Clique no botão **Documentos** guia .
1. Clique em Documentos ![](assets/document-icon.png) no painel esquerdo.
1. Clique em **Adicionar novo**, depois clique em **Prova** no menu exibido.

   >[!TIP]
   >
   >Você pode ativar a variável **Gerar provas automaticamente ao carregar documentos** configuração no perfil do usuário para automatizar esse processo. Para obter mais informações, consulte [Definir minhas configurações](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md) .

1. No **Nova prova** página que aparece, é possível

   * [Criar uma prova avançada com um workflow básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Carregar um documento e criar uma nova versão de uma prova

1. Vá para o projeto, tarefa ou problema em que deseja criar uma nova versão de uma prova existente.
1. Clique no botão **Documentos** guia .
1. Selecione o documento ao qual deseja adicionar uma nova versão.
1. Clique em **Adicionar novo** > **Versão** > **Prova**.
1. No **Nova versão de prova** página que aparece, é possível

   * [Criar uma prova avançada com um workflow básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Criar uma prova avançada com um fluxo de trabalho Automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)

## Use arrastar e soltar para gerar uma prova simples para uma nova versão

Você pode arrastar e soltar um documento do seu sistema de arquivos (como a área de trabalho) para criar uma nova prova ou uma nova versão de uma prova existente. A prova contém as seguintes configurações, dependendo se você está criando uma nova prova ou uma nova versão:

* **Nova prova:** Cria uma prova simples que é compartilhada somente com você. Você pode modificar as configurações de compartilhamento após a criação da prova, conforme descrito em [Editar configurações de prova](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md).

* **Nova versão da prova existente:** Cria uma nova versão com as mesmas configurações de prova da versão anterior.

Para usar o recurso arrastar e soltar para gerar uma nova prova ou versão de prova:

1. Verifique se as provas estão configuradas para serem geradas automaticamente, conforme descrito em .
1. Continue com  [Adicionar documentos ao Adobe Workfront a partir do seu sistema de arquivos](../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md), que explica o método de arrastar e soltar da adição de documentos. 

## Criar uma prova para um documento existente

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
      <td role="rowheader">Prova simples</td> 
      <td>Essa opção cria uma prova sem workflow anexado e aplica as configurações de prova padrão. Você pode atualizar as configurações de prova padrão ou adicionar um fluxo de trabalho depois de criar a prova. Para obter mais informações sobre configurações de prova, consulte <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/edit-proof-settings.md" class="MCXref xref">Editar configurações de prova</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prova avançada</td> 
      <td> <p>Essa opção permite configurar um workflow básico ou avançado e modificar as configurações de prova da prova criada. Para obter mais informações, consulte </p> 
       <ul> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um workflow básico</a> </p> </li> 
        <li> <p><a href="../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md" class="MCXref xref">Criar uma prova avançada com um fluxo de trabalho Automatizado</a> </p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>
