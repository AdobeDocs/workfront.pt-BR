---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Definir configurações de prova padrão
description: Essas configurações permitem definir valores padrão que se aplicam a todas as novas provas criadas pelos usuários. No entanto, os usuários podem substituir a maioria dessas configurações ao criar uma prova.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 7%

---

# Definir configurações de prova padrão

Essas configurações permitem definir valores padrão que se aplicam a todas as novas provas criadas pelos usuários. No entanto, os usuários podem substituir a maioria dessas configurações ao criar uma prova.

## Definir novas configurações padrão de prova

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração**.
1. No painel esquerdo, clique em **Provas** > **Configurações de prova**.
1. No **Novos padrões de prova** , defina as seguintes configurações:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Recipients</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Exigir logon</td> 
      <td> <p>Os revisores devem fazer logon usando seu email e senha antes de poderem exibir provas criadas na conta de sua organização. Quando ativado, os usuários não podem compartilhar a prova com os revisores Convidados.</p> <p><b>IMPORTANTE</b>: Quando ativado, o logon é necessário para todas as provas recém-criadas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar proprietário da prova original para novas versões</td> 
      <td> <p>O proprietário da primeira versão de uma prova também é o proprietário de todas as versões consecutivas da prova, independentemente de quem cria essas versões. Essa configuração é ativada por padrão.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permitir que usuários excluam comentários de revisão</td> 
      <td>Os usuários podem excluir seus próprios comentários. Essa configuração é ativada por padrão.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requer decisões assinadas eletronicamente </td> 
      <td> <p>Os tomadores de decisão são solicitados a inserir sua credencial de logon da Workfront quando tomam uma decisão em uma prova.</p> <p><b>IMPORTANTE</b>: Quando ativados, os usuários não podem compartilhar a prova com revisores convidados que não têm credenciais de logon.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Prazo</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Definir o prazo padrão</td> 
      <td> <p>O sistema aplica esse prazo a todas as novas provas em sua conta que não tenham um Fluxo de trabalho automatizado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificar destinatários antes que a prova esteja em risco</td> 
      <td>Os recipients são notificados por email antes que a prova seja considerada em risco, dependendo do prazo especificado acima.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Notificações de email</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificar recipients quando adicionados para uma prova</td> 
      <td>Os recipients são notificados por email quando são adicionados a uma prova.</td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Salvar**.

## Configurar decisões de prova

Os usuários podem usar decisões de prova para indicar o status da prova após a revisão.

>[!NOTE]
>
>A lógica por trás das decisões de prova é usada para calcular o status geral de um workflow de prova se houver várias decisões de vários níveis. As decisões &quot;Aprovado&quot; e &quot;Aprovado com alterações&quot; acionam a próxima etapa em um fluxo de trabalho automático.

Para configurar decisões de prova:

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração**.
1. No painel esquerdo, clique em **Provas** > **Configurações de prova**.
1. No **Decisões** seção , é possível

   1. **Renomear a decisão**: Clique no texto dentro da caixa de decisão e comece a digitar o novo rótulo de decisão.

      >[!TIP]
      >
      >Mantenha a lógica de uma decisão ao renomeá-la. Por exemplo, a decisão padrão Rejeitada pode ser alterada para *Nova versão necessária*, mas não deve ser alterado para *Enviar para Impressoras*.

      ![](assets/rename-decision-350x109.png)

   1. **Reorganizar a ordem de decisão**: Arraste as caixas de decisão na ordem em que deseja que elas apareçam no visualizador de prova.

      ![](assets/move-decision-350x110.png)

   1. **Ocultar uma decisão**: Passe o mouse sobre a caixa de decisão e clique no ícone Ocultar no canto superior direito.

      ![](assets/hide-decision-350x109.png)

1. (Opcional) Para voltar aos padrões da Workfront, clique em **Restaurar padrões**.
1. Clique em **Salvar**.
