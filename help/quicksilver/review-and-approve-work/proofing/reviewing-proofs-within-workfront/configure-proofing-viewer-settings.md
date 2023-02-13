---
product-area: documents;setup
navigation-topic: review-a-proof
title: Definir configurações do visualizador de prova
description: Você pode definir as seguintes configurações para o Visualizador de Provas da Web e para o Visualizador de Provas de Desktop - EDITAR-ME.
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# Definir configurações do visualizador de prova

Você pode definir as seguintes configurações para o Visualizador de Provas da Web e para o Visualizador de Provas de Desktop:

* Se as marcações e os pinos de comentário são exibidos nas provas.
* Se as ferramentas de marcação são exibidas na parte superior do visualizador de prova ou em um menu suspenso.
* Quais notificações por email você recebe como revisor na prova aberta.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

Você pode definir as seguintes configurações para o Desktop Proofing Viewer:

* Como você deseja que os links dentro do conteúdo do site sejam abertos no Visualizador.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* O que acontece quando você clica em um link definido para ser aberto em uma nova guia ou janela do navegador.
* Limpe os dados do cache que podem ser salvos com a prova que você está visualizando para permitir que conteúdo como pop-ups (que podem ser bloqueados pelos dados do cache do navegador) sejam exibidos no Visualizador.

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
   <td> <p>Editar acesso a documentos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, função ou Perfil de permissão de prova você possui, entre em contato com o administrador da Workfront ou da Workfront Proof.

## Definir configurações do visualizador de prova

Para definir configurações do visualizador de prova:

1. Abra o Web Proofing Viewer ou o Desktop Proofing Viewer de uma das seguintes maneiras:

   * Se você provar no Adobe Workfront, vá para uma lista de documentos contendo uma prova que deseja exibir, passe o mouse sobre o documento e clique em **Abrir prova**.
   * Se você usar a Workfront Proof, clique no link **Ir para prova** ícone da prova no Painel ou em uma lista de Exibições ![](assets/go-to-proof-blue-icon.png).

1. Se a barra de ferramentas esquerda não estiver sendo exibida, clique no botão **Menu** ícone , localizado no canto superior esquerdo do Visualizador de Verificação de Verificação de Verificação da Web.

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. Na barra de ferramentas esquerda, clique no botão **Configurações** ícone ![](assets/settings-icon-in-pv.png).

1. Configure qualquer um dos seguintes **Configurações** essa exibição.

   As configurações disponíveis podem variar dependendo do tipo de prova aberta.

   * **Mostrar marcações** (sempre disponível no Web Proofing Viewer e no Desktop Proofing Viewer): Essas são as marcas de comentário que os revisores adicionam às provas quando usam as ferramentas de marcação. Se você desativá-los, ainda será possível visualizá-los ao clicar em um comentário na lista de comentários.

      Essa configuração afeta todas as provas que você abrir.

   * **Mostrar pinos** (sempre disponível no Web Proofing Viewer e no Desktop Proofing Viewer): Esses são os pinos numerados que os revisores adicionam às provas quando usam as ferramentas de marcação. Eles indicam onde e em que ordem o revisor adicionou comentários. Se você desativá-los, ainda será possível visualizá-los ao clicar em um comentário na lista de comentários.

      Essa configuração afeta todas as provas que você abrir.

   * **Usar ferramentas de marcação expandidas** (sempre disponível no Web Proofing Viewer e no Desktop Proofing Viewer): Por padrão, as opções da ferramenta de marcação são exibidas na parte superior do visualizador de prova. Você pode configurá-los para serem exibidos em um menu vertical que só é aberto ao clicar nele.

      Essa configuração está em vigor para todas as provas que você abrir.

   * **Enviar notificações por email sobre** (sempre disponível no Web Proofing Viewer e no Desktop Proofing Viewer): Clique em uma das opções abaixo. Essa configuração afeta somente a prova aberta. Para obter mais informações, consulte [Notificações para comentários de prova e visão geral de decisões](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Todas as atividades</td> 
        <td>O Workfront envia um email para o revisor sempre que houver uma atividade na prova, como um novo comentário, resposta ou decisão. <p>Essa é uma ótima opção para a pessoa que está gerenciando o processo de verificação porque permite que ela veja a atividade como ela acontece. </p><p>Os usuários não recebem um alerta por email sobre sua própria atividade.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Respostas aos meus comentários</td> 
        <td>Um email é enviado ao revisor somente se alguém responder explicitamente ao comentário (isso exclui suas próprias respostas em seus próprios comentários). Isso significa que se alguém na prova fizer um novo comentário, o revisor não será notificado.<p>Essa configuração é recomendada para seus clientes na prova, de modo que eles não sejam notificados sobre nenhum outro comentário na prova e sejam notificados apenas das respostas aos próprios comentários.</p><p>Embora os revisores com essa configuração de alerta de email não sejam notificados sobre outros novos comentários, eles ainda podem exibir todos os comentários na prova no visualizador de prova.</p><p>Para obter informações sobre comentários, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">Exibir e responder comentários de prova</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisões</td> 
        <td>O Workfront envia um email para o revisor somente quando alguém toma uma decisão.<p>Isso pode ser útil para a pessoa que gerencia o processo de aprovação (como um gerente de projeto) e precisa monitorar o progresso na prova e ver quais usuários tomaram sua decisão.</p><p>Você não será notificado de sua própria decisão, a menos que selecione uma opção de confirmação por email ao enviar sua decisão.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Decisão final</td> 
        <td>O Workfront envia um email quando o último aprovador na prova tomou a decisão.<p>Esse alerta é frequentemente usado pelo designer, que geralmente não precisa participar da discussão da revisão real. Quando a decisão final é tomada, o criador é notificado e pode tomar medidas relativamente às alterações necessárias.</p><p>Esse alerta também pode ser útil para um líder de departamento que precisa ser notificado somente quando o processo de revisão for concluído.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo por hora</td> 
        <td>O Workfront envia um email para o revisor a cada hora com um resumo de todos os comentários, respostas e decisões que ocorreram na hora.<p>O email é enviado somente quando uma atividade além da sua ocorrer na última hora. </p><p>Esse alerta é uma boa maneira de ver uma visão geral do projeto.</p><p>Um exemplo de uso desse resumo é um revisor sênior que precisa de uma visão geral do projeto, mas não precisa ser notificado imediatamente de todas as atividades na prova.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">Resumo diário</td> 
        <td>O Workfront envia um email com todos os comentários, respostas e decisões listados somente em dias em que há atividade além da sua.<p>Esse alerta é uma boa maneira de ver um resumo do projeto sem ficar sobrecarregado com várias atualizações ao longo do dia.</p><p>Um exemplo de uso deste resumo é um líder de departamento que deseja monitorar o progresso geral do projeto.</p><p>Para obter mais informações, consulte <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">Gerenciar notificações para comentários e decisões de prova</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">Nenhum email</td> 
        <td>A Workfront não envia alertas de email.<br>Isso é útil para uma pessoa que é adicionada a uma prova somente para fins de referência e não precisa ser notificada de quaisquer alterações.<p>O padrão do sistema é o Resumo diário (também visto como Não definido). Se você ou seus revisores não fizerem outras alterações, todas as provas terão essa configuração.</p></td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **Ao clicar em hiperlinks em uma prova** (disponível somente no Desktop Proofing Viewer): Selecione uma opção para especificar o que acontece no Desktop Proofing Viewer ao clicar em um link definido para abrir em uma nova guia ou janela do navegador.

      Essa configuração está em vigor para todas as provas interativas abertas.

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Abrir no visualizador de prova</td> 
        <td>Os links sempre são abertos no Desktop Proofing Viewer e você pode provar o conteúdo vinculado. </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Abrir no navegador</td> 
        <td>Os links sempre são abertos no navegador, não em um visualizador de prova. Não é possível provar o conteúdo vinculado.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Pergunte-me sempre</td> 
        <td> <p>Você será solicitado sempre se deseja abrir o link dentro do Desktop Proofing Viewer ou no navegador. Se você abrir o link no Desktop Proofing Viewer, poderá provar o conteúdo vinculado. Se você abrir o link no navegador, não será possível provar o conteúdo vinculado.</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>Essa configuração afeta somente a prova aberta.</p> </td> 
       </tr> 
      </tbody> 
     </table>

      <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **Limpar cache**: Apaga os dados do cache do navegador que podem ser salvos com uma prova interativa que você está visualizando. Isso permite que conteúdo como pop-ups (que podem ser bloqueados por dados de cache do navegador) sejam exibidos no Desktop Proofing Viewer.

      Os dados que são limpos incluem o cache HTTP (como imagens a serem reutilizadas após a próxima atualização da página) e o cache de dados do armazenamento da Web (como cookies e dados que identificam usuários).

      Essa configuração afeta somente a prova aberta.
