---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Alterar resolução de prova interativa no visualizador de provas
description: Você pode visualizar como uma prova interativa ficará em vários dispositivos, permitindo que você veja como o conteúdo é exibido e responde com base em diferentes resoluções.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 1%

---

# Alterar resolução de prova interativa no visualizador de provas

Você pode visualizar como uma prova interativa ficará em vários dispositivos, permitindo que você veja como o conteúdo é exibido e responde com base em diferentes resoluções.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Plano atual: Pro ou Superior</p> <p>ou</p> <p>Plano herdado: Select ou Premium</p> <p>Para obter mais informações sobre acesso de revisão de texto com os diferentes planos, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acesso à funcionalidade de revisão de texto no Workfront</a>.</p> </td> 
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
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Visualizações de dispositivo e resolução no Visualizador de provas de desktop vs. Visualizador de provas de web

O administrador do Adobe Workfront configurou o sistema para que você revise o conteúdo interativo no Desktop Proofing Viewer ou, como conteúdo empacotado em um arquivo ZIP, no Web Proofing Viewer:

* No Visualizador de provas de desktop, você pode visualizar como o conteúdo aparece e responde em várias resoluções e em vários dispositivos. Quando um revisor especifica um determinado dispositivo, o conteúdo aparece como apareceria nesse dispositivo, com as especificações da interface do usuário para o dispositivo. Por exemplo, um botão vermelho em uma marca de smartphone pode estar azul em uma marca diferente.

* No Visualizador de provas da Web, você pode exibir o conteúdo interativo como ele aparece nas resoluções para os vários dispositivos. Mas o Visualizador de provas da Web não emula o conteúdo usando especificações de interface nesses dispositivos, como cor de botão.

  >[!NOTE]
  >
  >O administrador do Workfront pode configurar dispositivos personalizados para usuários em sua organização, conforme descrito em [Configurando Dispositivos Personalizados para Provas](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#configure-custom-devices-for-proofs) no artigo [Definir configurações de prova para sua organização](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

## Exibir uma prova com um dispositivo predefinido ou uma configuração de resolução

1. Vá para a lista de documentos que contém a prova que deseja abrir.
1. Passe o mouse sobre o documento e clique em **Abrir prova**.
1. Clique em **Responsivo** na parte inferior central do visualizador de provas.

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. No Visualizador de provas de desktop, na lista de dispositivos e resoluções exibida, clique naquele que você deseja.

   Ou

   No Visualizador de provas da Web, na lista de resoluções exibida, clique na que você deseja.

   Se precisar de informações sobre a diferença entre esses dois visualizadores, consulte [Diferenças entre o Visualizador de Provas da Web e a visão geral do Visualizador de Provas do Desktop](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   A prova interativa é renderizada na resolução selecionada.

## Exibir uma prova com uma configuração de resolução personalizada

1. Vá para a lista de documentos que contém a prova que deseja abrir.
1. Passe o mouse sobre o documento e clique em **Abrir prova**.
1. Clique em **Responsivo** na parte inferior central do Visualizador de provas.
1. Digite uma resolução personalizada **Responsiva**.

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   Ou

   Passe o mouse sobre o conteúdo interativo e arraste a borda azul no canto inferior direito, ou na borda direita ou inferior, para a resolução desejada.

   ![Arrastar_bordas_azuis_para_resolução.png](assets/drag-blue-edges-for-resolution-350x251.png)

   A resolução personalizada é exibida nos seguintes locais:

   * No painel **Resolução**, na parte inferior central do visualizador.\
     ![Captura_de_tela_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * Em qualquer comentário, os revisores adicionam à prova. Cada comentário inclui a resolução de tela selecionada quando o revisor criou o comentário.
