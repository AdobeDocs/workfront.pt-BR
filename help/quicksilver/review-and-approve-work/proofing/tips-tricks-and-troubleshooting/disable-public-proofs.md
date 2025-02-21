---
content-type: tips-tricks-troubleshooting
product-area: documents
keywords: disable,public,sharing,proof,public,url
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: Desativar o compartilhamento da prova por meio de URL público ou código incorporado
description: Você pode desativar a capacidade de compartilhar uma prova com um URL público ou incorporar código em uma prova por prova ou para usuários individuais.
author: Courtney
feature: Digital Content and Documents
exl-id: 73f08e12-f70d-4347-8a5b-441f94d24590
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 0%

---

# Desativar o compartilhamento da prova por meio de URL público ou código incorporado

Você pode desativar a capacidade de compartilhar uma prova com um URL público ou incorporar código em uma prova por prova ou para usuários individuais.

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
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Desativar por prova

Você deve ser o proprietário ou criador da prova, ou deve ter a função de prova Autor ou Moderador.

1. No projeto que contém a prova, clique em **Documentos** no painel esquerdo.
1. Passe o mouse sobre a prova e selecione **Detalhes do documento**.
1. No painel esquerdo, clique em **Configurações do Visualizador de Revisão de Texto** e desabilite a caixa de seleção **Permitir compartilhamento de prova via URL pública ou código de inserção**.

   ![Configurações do visualizador de provas](assets/proofing-viewer-settings-350x200.png)

1. Clique em **Salvar**.

## Desativar por usuário

Você pode desativar a configuração Prova pública para usuários individuais na instância do Workfront. Você deve ter um Perfil de Permissão de Prova do administrador para fazer essa alteração.

1. Clique no ícone **Menu Principal** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Revisão**.
1. Clique em **Configurações da conta** próximo ao canto superior direito.
1. Clique na guia **Usuários** e depois clique no nome de um usuário.
1. Na seção **Configurações de prova padrão**, desabilite a caixa de seleção **Compartilhamento Público**.

   ![Compartilhamento público](assets/default-proof-settings--public-sharing-350x210.png)
