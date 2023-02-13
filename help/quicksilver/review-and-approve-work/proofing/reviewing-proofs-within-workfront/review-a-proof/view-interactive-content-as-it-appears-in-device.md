---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: Alterar resolução de prova interativa no visualizador de prova
description: Você pode visualizar a aparência de uma prova interativa em vários dispositivos, permitindo que você veja como o conteúdo é exibido e responde com base em diferentes resoluções.
author: Courtney
feature: Digital Content and Documents
exl-id: 99165790-0c34-4540-92d9-956ae178a874
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 1%

---

# Alterar resolução de prova interativa no visualizador de prova

Você pode visualizar a aparência de uma prova interativa em vários dispositivos, permitindo que você veja como o conteúdo é exibido e responde com base em diferentes resoluções.

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
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Visualizações de Dispositivo e Resolução no Visualizador de Verificação de Verificação de Verificação Linguagem de Desktop vs. Visualizador de Verificação de Verificação Linguística da Web

O administrador do Adobe Workfront configurou o sistema para que você revise o conteúdo interativo no Visualizador de Verificação de Verificação de Verificação de Desktop ou, como o conteúdo empacotado em um arquivo ZIP, no Visualizador de Verificação de Verificação de Verificação Linguística da Web:

* No Desktop Proofing Viewer, você pode visualizar como o conteúdo é exibido e responde em várias resoluções e em vários dispositivos. Quando um revisor especifica um determinado dispositivo, o conteúdo é exibido como seria nesse dispositivo, com as especificações da interface do usuário para o dispositivo. Por exemplo, um botão vermelho em uma marca de smartphone pode ser azul em uma marca diferente.

* No Web Proofing Viewer, você pode exibir o conteúdo interativo como ele aparece nas resoluções para os vários dispositivos. Mas o Web Proofing Viewer não emula o conteúdo usando especificações de interface nesses dispositivos, como a cor do botão.

   >[!NOTE]
   >
   >O administrador do Workfront pode configurar dispositivos personalizados para usuários em sua organização, conforme descrito em Configuração de dispositivos personalizados para provas interativas no artigo .

## Exibir uma prova com um dispositivo predefinido ou uma configuração de resolução

1. Vá para a lista de documentos que contém a prova que deseja abrir.
1. Passe o mouse sobre o documento e clique em **Abrir prova**.
1. Clique em **Responsivo** no centro da parte inferior do visualizador de prova.

   ![Resolution_option_in_DPV.png](assets/resolution-option-in-dpv-350x64.png)

1. No Desktop Proofing Viewer, na lista de dispositivos e resoluções que aparece, clique no que você deseja.

   Ou

   No Web Proofing Viewer, na lista de resoluções que aparece, clique no que você deseja.

   Se precisar de informações sobre como esses dois visualizadores diferem, consulte [Diferenças entre o Visualizador de Provas da Web e a visão geral do Visualizador de Provas de Desktop](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

   A prova interativa é renderizada na resolução selecionada.

## Exibir uma prova com uma configuração de resolução personalizada

1. Vá para a lista de documentos que contém a prova que deseja abrir.
1. Passe o mouse sobre o documento e clique em **Abrir prova**.
1. Clique em **Responsivo** no centro da parte inferior do Visualizador de Verificação de Provas.
1. Digite um **Responsivo** resolução.

   ![Type_a_custom_resolution_DPV.png](assets/type-a-custom-resolution-dpv.png)

   Ou

   Passe o mouse sobre seu conteúdo interativo e arraste a borda azul no canto inferior direito, ou na borda direita ou inferior, para a resolução desejada.

   ![Drag_blue_edge_for_resolution.png](assets/drag-blue-edges-for-resolution-350x251.png)

   A resolução personalizada é exibida nos seguintes locais:

   * No **Resolução** no centro inferior do visualizador.\
      ![Captura de tela_2018-05-15_10-27-54.png](assets/screenshot-2018-05-15-10-27-54.png)

   * Em qualquer comentário, os revisores adicionam à prova. Cada comentário inclui a resolução da tela que foi selecionada quando o revisor criou o comentário.
