---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Criar uma prova interativa para um site ou outro conteúdo da Web
description: Você pode gerar uma nova prova interativa ou uma nova versão de uma prova interativa existente para conteúdo da Web. Pode ser um site ou outros tipos de conteúdo interativo, como anúncios com vídeo ou áudio streaming, animações HTML e banners interativos.
author: Courtney
feature: Digital Content and Documents
exl-id: 56e5eeea-1ab9-43c8-bc84-d10638171871
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '561'
ht-degree: 0%

---

# Criar uma prova interativa para um site ou outro conteúdo da Web

Você pode gerar uma nova prova interativa ou uma nova versão de uma prova interativa existente para conteúdo da Web. Pode ser um site ou outros tipos de conteúdo interativo, como anúncios com vídeo ou áudio streaming, animações HTML e banners interativos.

Em uma prova interativa, os revisores podem navegar e interagir normalmente com o site ou outro conteúdo da Web.

>[!IMPORTANT]
>
>Certifique-se de que o site ou o conteúdo interativo esteja acessível às pessoas que vão revisá-lo. Eles podem acessá-lo no processo de comprovação somente se também puderem acessá-lo na Internet.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano atual: Trabalho ou Plano</p> <p>Plano herdado: Qualquer um (Você deve ter a prova ativada para o usuário)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de Permissões de Prova </td> 
   <td>Gerente ou superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Criar uma prova interativa para um site ou outro conteúdo da Web

1. Vá para o projeto, tarefa ou problema em que deseja criar uma nova prova de site ou uma nova versão de uma existente.
1. Clique em **Documentos** no painel esquerdo.
1. (Condicional) Se estiver criando uma nova prova, clique em **Adicionar novo** e em **Prova** no menu exibido.

1. (Condicional) Na página **Nova prova** será exibida, se você estiver criando uma nova versão de uma prova existente:

   1. Passe o mouse sobre a prova de URL para a qual deseja criar uma nova versão e selecione-a clicando no plano de fundo azul-claro ao redor dela.

      ![Select_proof_by_selection_light_blue_background.png](assets/select-proof-by-selecting-light-blue-background-350x52.png)


   1. No menu suspenso **Adicionar novo**, clique em **Versão** > **Prova**.

1. Na seção **Adicionar arquivos**, digite a URL do site que deseja revisar e pressione **Enter**.  Você pode repetir esse processo para adicionar vários sites a serem revisados.

   ![proof_website.png](assets/proof-website-350x65.png)


   >[!NOTE]
   >
   > A URL deve ter menos de 1.000 caracteres.

1. Clique no URL adicionado.

   ![Clique na URL](assets/click-url-350x137.png)

1. (Opcional) Se você deseja alterar o nome da prova da URL do site para algo diferente, digite um **Nome da prova**.
1. Selecione **Interativo** e clique em **Concluído**.

   >[!NOTE]
   >
   >Se você estiver adicionando uma nova versão a uma prova de URL existente, todas as opções configuradas na prova original ou na versão anterior serão mantidas nesta versão.

1. Clique em **Criar prova** para criar uma prova simples sem processo de revisão.\
   ou\
   Continue configurando uma prova avançada:

   * [Criar uma prova avançada com um fluxo de trabalho básico](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md)
   * [Criar uma prova avançada com um fluxo de trabalho automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
