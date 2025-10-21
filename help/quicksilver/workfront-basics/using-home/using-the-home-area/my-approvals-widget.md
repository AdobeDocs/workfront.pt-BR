---
product-area: home
navigation-topic: use-the-home-area
title: Gerenciar suas aprovações com o widget Minhas aprovações
description: O widget Minhas aprovações exibe todas as aprovações pendentes, atribuídas, delegadas e enviadas em um único local. Aqui, você pode filtrar e organizar suas aprovações, tomar decisões e delegar aprovações conforme necessário.
author: Courtney
feature: Get Started with Workfront
source-git-commit: 4981d9adb2cae53e30f13aa2a7aa6857befbf3ca
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 5%

---

# Gerenciar suas aprovações com o widget Minhas aprovações

O widget Minhas aprovações exibe todas as aprovações pendentes, atribuídas, delegadas e enviadas em um único local. Aqui, você pode filtrar e organizar suas aprovações, tomar decisões e delegar aprovações conforme necessário.

O widget Minhas aprovações é compatível com aprovações dos seguintes objetos do Workfront:

* Tarefas
* Problemas
* Projetos
* Documentos
* Provas
* Solicitações de registro de planejamento
* Planilhas de horas

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <p>Colaborador ou superior</p>
   <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Visualizar ou ter maior acesso aos objetos associados às aprovações</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou mais altas para os objetos associados às aprovações</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aprovar trabalho no widget Minhas aprovações

1. Clique no **[!UICONTROL Menu Principal]** ![Ícone do Menu Principal](assets/main-menu-icon.png) no canto superior direito e clique em **[!UICONTROL Página Inicial]**.
1. (Condicional) Clique em **Personalizar** para adicionar o widget **Minhas aprovações**.
1. (Condicional) Clique no menu suspenso **Filtro** e selecione **Todos** para ver as aprovações atribuídas e delegadas a você.

   >[!NOTE]
   >
   >As aprovações atribuídas a funções ou grupos de trabalho não são exibidas na Página inicial. As aprovações atribuídas a equipes são exibidas no widget Minhas aprovações para cada membro da equipe.


1. Selecione o item em que deseja tomar uma decisão de aprovação.

   ![Widget Minhas aprovações](assets/my-approvals-widget.png)

1. Clique em uma das opções disponíveis ao tomar uma decisão de aprovação no painel direito. As seguintes opções são exibidas no canto superior direito da página, dependendo do tipo de item que você está aprovando:

   <table>
   <tr>
      <td>
      <p><strong>Acesso</strong></p>
      </td>
      <td>
      <p><strong>Itens de trabalho</strong></p>
      </td>
      <td>
      <p><strong>Documentos</strong></p>
      </td>
      <td>
      <p><strong>Provas</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>Conceder</li>
      <li>Ignorar</li>
      </ul>
      Você pode ajustar o nível de acesso no menu suspenso <b>Alterar acesso</b>, se desejar.
      </td>
      <td>
         <ul>
         <li>Aprovar</li>
         <li>Rejeitar</li>
         </ul>
      Você pode deixar um comentário com sua decisão clicando no menu suspenso no botão de decisão.
      </td>
      <td>
   Atribuído como um aprovador
         <ul>
         <li>Aprovar</li>
         <li>Aprovar com alterações</li>
         <li>Precisa do trabalho</li>
         </ul>
   Atribuído como revisor
         <ul>
         <li>Concluir minha revisão</li>
         </ul>
      As opções dessa coluna se aplicam somente às Aprovações unificadas. As aprovações de documentos herdados aparecem da mesma forma que as aprovações de itens de Trabalho. 
      </td>
      <td>
         <ul>
         <li>Ir para prova</li>
         </ul>
         Você toma a sua decisão no visualizador de prova. Para obter informações sobre como revisar uma prova, consulte <a href="/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Revisar provas no Adobe Workfront</a>.
      </td>
   </tr>
   </table>

Depois de tomar uma decisão, a aprovação é removida do widget Minha aprovação.