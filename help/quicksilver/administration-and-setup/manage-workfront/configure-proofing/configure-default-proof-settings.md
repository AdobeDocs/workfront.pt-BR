---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Definir configurações padrão de prova
description: Essas configurações permitem que você defina valores padrão que se aplicam a todas as novas provas criadas pelos usuários. No entanto, os usuários podem substituir a maioria dessas configurações ao criar uma prova.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f391f43e96add70f8a5aeed259eee1259ed786a3
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 6%

---

# Definir configurações padrão de prova

Essas configurações permitem que você defina valores padrão que se aplicam a todas as novas provas criadas pelos usuários. No entanto, os usuários podem substituir a maioria dessas configurações ao criar uma prova.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>
   <p>Novo: Padrão</p>
   ou
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter informações sobre administradores do Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Definir novas configurações padrão de prova

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Instalação**.
1. No painel esquerdo, clique em **Provas** > **Configurações de prova**.
1. Na seção **Novos padrões de prova**, defina as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Recipients</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exigir logon</td> 
      <td> <p>Os revisores são solicitados a fazer logon usando seu email e senha para que possam exibir as provas criadas na conta da organização. Quando ativados, os usuários não podem compartilhar a prova com os revisores Convidados.</p> <p><b>IMPORTANTE</b>: quando habilitado, o logon é necessário para todas as provas recém-criadas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar proprietário da prova original para novas versões</td> 
      <td> <p>O proprietário da primeira versão que uma prova é também o proprietário de todas as versões consecutivas da prova, independentemente de quem cria essas versões. Essa configuração é ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que usuários excluam comentários de revisão</td> 
      <td>Os usuários podem excluir seus próprios comentários. Essa configuração é ativada por padrão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente </td> 
      <td> <p>Os tomadores de decisão são solicitados a inserir sua credencial de logon do Workfront ao tomarem uma decisão sobre uma prova.</p> <p><b>IMPORTANTE</b>: quando habilitado, os usuários não podem compartilhar a prova com revisores Convidados que não têm credenciais de logon.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Prazo</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Definir o prazo final padrão</td> 
      <td> <p>O sistema aplica esse prazo final a todas as novas provas em sua conta que não tenham um Fluxo de trabalho automatizado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificar recipients antes que a prova esteja em risco</td> 
      <td>Os recipients são notificados por email antes que a prova seja considerada em risco, dependendo do prazo especificado acima.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Notificações de email</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificar recipients quando adicionados para uma prova</td> 
      <td>Os recipients são notificados por email quando adicionados a uma prova.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

## Configurar decisões de prova

Os usuários podem usar decisões de prova para indicar o status da prova após a revisão.

>[!NOTE]
>
>A lógica por trás das decisões de prova é usada para calcular o status geral de um fluxo de trabalho de prova se houver várias decisões de vários níveis. As decisões &quot;Aprovado&quot; e &quot;Aprovado com alterações&quot; acionam o próximo estágio em um fluxo de trabalho automático.

Para configurar decisões de prova:

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Instalação**.
1. No painel esquerdo, clique em **Provas** > **Configurações de prova**.
1. Na seção **Decisões** você pode

   1. **Renomear a decisão**: clique no texto dentro da caixa de decisão e comece a digitar o novo rótulo de decisão.

      >[!TIP]
      >
      >Mantenha a lógica de uma decisão ao renomeá-la. Por exemplo, a decisão padrão Rejeitada pode ser alterada para *Nova versão necessária*, mas não deve ser alterada para *Enviar para Impressoras*.

      ![](assets/rename-decision-350x109.png)

   1. **Reorganizar a ordem de decisão**: arraste as caixas de decisão na ordem em que você deseja que elas apareçam no visualizador de revisões.

      ![](assets/move-decision-350x110.png)

   1. **Ocultar uma decisão**: passe o mouse sobre a caixa de decisão e clique no ícone Ocultar no canto superior direito.

      ![](assets/hide-decision-350x109.png)

1. (Opcional) Para voltar aos padrões do Workfront, clique em **Restaurar padrões**.
1. Clique em **Salvar**.
