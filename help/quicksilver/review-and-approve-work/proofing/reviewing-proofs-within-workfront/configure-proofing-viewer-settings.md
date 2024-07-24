---
product-area: documents;setup
navigation-topic: review-a-proof
title: Definir configurações do revisor de provas
description: Você pode definir as configurações do Visualizador de provas da web e do Visualizador de provas da área de trabalho.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 8af531868249f609113af6d2a8465af01edcbc3f
workflow-type: tm+mt
source-wordcount: '1417'
ht-degree: 0%

---

# Definir configurações do revisor de provas

Você pode definir as seguintes configurações para o Visualizador de provas da web e o Visualizador de provas da área de trabalho:

* Se as marcações e marcações de comentário são exibidas nas provas.
* Se as ferramentas de marcação são exibidas na parte superior do revisor de provas ou em um menu suspenso.
* Quais notificações por email você recebe como revisor na prova que você abriu.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

Você pode definir as seguintes configurações para o Visualizador de provas de desktop:

* Como você deseja que os links dentro do conteúdo do site sejam abertos no Visualizador.

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* O que acontece quando você clica em um link definido para ser aberto em uma nova guia ou janela do navegador.
* Limpe os dados do cache que podem ser salvos com a prova que você está visualizando para permitir que conteúdo como pop-ups (que podem ser bloqueados pelos dados do cache do navegador) sejam exibidos no Visualizador.

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
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual perfil de plano, função ou permissão de prova você tem, contate o administrador do Workfront ou do Workfront Proof.

+++

## Definir configurações do revisor de provas

Para definir as configurações do revisor de provas:

1. Abra o Visualizador de provas da Web ou o Visualizador de provas da área de trabalho de uma das seguintes maneiras:

   * Se você revisar no Adobe Workfront, vá para uma lista de documentos que contém uma prova que deseja exibir, passe o mouse sobre o documento e clique em **Abrir prova**.
   * Se você usa o Workfront Proof, clique no ícone **Ir para Prova** para a prova no Painel ou em uma lista de Exibições ![](assets/go-to-proof-blue-icon.png).

1. Se a barra de ferramentas esquerda não for exibida, clique no ícone **Menu**, localizado no canto superior esquerdo do Visualizador de Provas da Web.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Na barra de ferramentas esquerda, clique no ícone ![](assets/settings-icon-in-pv.png) de **Configurações**.

1. Defina qualquer uma das **Configurações** a seguir que forem exibidas.

   As configurações disponíveis podem variar dependendo do tipo de prova que você abriu.

   * **Mostrar marcações** (sempre disponível no Visualizador de Revisão de Texto da Web e no Visualizador de Revisão de Texto da Área de Trabalho): Essas são as marcas de comentário que os revisores adicionam às provas quando usam as ferramentas de marcação. Se você desativá-los, ainda poderá vê-los ao clicar em um comentário na lista de comentários.

     Essa configuração afeta todas as provas abertas.

   * **Mostrar pinos** (sempre disponível no Visualizador de Provas da Web e no Visualizador de Provas da Área de Trabalho): são os pinos numerados que os revisores adicionam às provas quando usam as ferramentas de marcação. Eles indicam onde e em que ordem o revisor adicionou comentários. Se você desativá-los, ainda poderá vê-los ao clicar em um comentário na lista de comentários.

     Essa configuração afeta todas as provas abertas.

   * **Usar ferramentas de marcação expandidas** (sempre disponíveis no Visualizador de Provas da Web e no Visualizador de Provas da Área de Trabalho): por padrão, as opções da ferramenta de marcação são exibidas na parte superior do visualizador de provas. É possível configurá-los para serem exibidos em um menu vertical que é aberto somente quando você clica nele.

     Essa configuração está em vigor para todas as provas que você abrir.

   * **Enviar notificações por email sobre** (sempre disponível no Visualizador de Provas da Web e no Visualizador de Provas da Área de Trabalho): Clique em uma das opções abaixo. Essa configuração afeta somente a prova que você abriu. Para obter mais informações, consulte [Notificações para obter a visão geral de comentários de prova e decisões](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Todas as atividades</td> 
        <td>O Workfront envia um email para o revisor sempre que há uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de prova, pois permite que ela veja a atividade enquanto ela acontece. </p><p>Os usuários não recebem um alerta por email sobre suas próprias atividades.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Respostas aos meus comentários</td> 
        <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui as próprias respostas nos comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para os clientes na prova, para que não sejam notificados de nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta por email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador da prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder aos comentários de prova</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisões</td> 
        <td>O Workfront envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que está gerenciando o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não é notificado sobre sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisão final</td> 
        <td>O Workfront envia um email quando o último aprovador na prova toma sua decisão.<p>Esse alerta é usado com frequência pelo designer, que geralmente não precisa participar da discussão de revisão real. Quando a decisão final é tomada, o designer é notificado e pode então tomar medidas em relação a quaisquer alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precise ser notificado somente quando o processo de revisão for concluído.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo por Hora</td> 
        <td>O Workfront envia um email ao revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando a atividade além da sua ocorre na última hora. </p><p>Este alerta é uma boa maneira de ter uma visão geral do projeto.</p><p>Um exemplo de caso de uso para este resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo Diário</td> 
        <td>O Workfront envia um email com todos os comentários, respostas e decisões listados somente em dias quando houver atividade além da sua.<p>Este alerta é uma boa maneira de ver um resumo do projeto sem precisar de várias atualizações ao longo do dia.</p><p>Um exemplo de caso de uso para este resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários de prova e decisões</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Nenhum email</td> 
        <td>O Workfront não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de nenhuma alteração.<p>O padrão do sistema é Resumo diário (também visto como Não definido). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **Ao clicar em hiperlinks em uma prova** (disponível apenas no Visualizador de Prova de Área de Trabalho): Selecione uma opção para especificar o que acontece no Visualizador de Prova de Área de Trabalho quando você clica em um link definido para ser aberto em uma nova guia do navegador ou janela.

     Esta configuração está em vigor para todas as provas interativas que você abrir.

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Abrir no visualizador de revisões</td> 
        <td>Os links sempre abrem no Visualizador de provas de desktop e você pode revisar o conteúdo vinculado. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Abrir no navegador</td> 
        <td>Os links sempre abrem no navegador, não em um visualizador de provas. Não é possível revisar o conteúdo vinculado.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Pergunte-me sempre</td> 
        <td> <p>Você será sempre perguntado se deseja abrir o link no Visualizador de provas de desktop ou no navegador. Se você abrir o link no Visualizador de provas de desktop, poderá revisar o conteúdo vinculado. Se você abrir o link no navegador, não será possível revisar o conteúdo vinculado.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>Essa configuração afeta somente a prova que você abriu.</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Limpar cache**: limpa os dados do cache do navegador que podem ser salvos com uma prova interativa que você está visualizando. Isso permite que conteúdo como pop-ups (que podem ser bloqueados pelos dados de cache do navegador) sejam exibidos no Visualizador de provas de desktop.

     Os dados limpos incluem o cache HTTP (como imagens a serem reutilizadas após a próxima atualização da página) e o cache de dados de armazenamento na Web (como cookies e dados que identificam usuários).

     Essa configuração afeta somente a prova que você abriu.
