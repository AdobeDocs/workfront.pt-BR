---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Compartilhar um relatório no Adobe Workfront
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar relatórios quando eles atribuírem níveis de acesso. Para obter mais informações sobre como conceder acesso a problemas, consulte Conceder acesso a relatórios, painéis e calendários.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: 28dd016d5edf51807c35cb392706107a08fb95f2
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Compartilhar um relatório no Adobe Workfront

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar relatórios quando eles atribuírem níveis de acesso. Para obter mais informações sobre como conceder acesso a problemas, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir ou Gerenciar relatórios específicos que você tenha acesso para compartilhar. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

## Requisitos de acesso

Você deve ter o seguinte para compartilhar objetos:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso de visualização ou superior a relatórios, painéis, calendários</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou aumentar o relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Considerações sobre o compartilhamento de relatórios

Além das considerações abaixo, consulte também [Compartilhar relatórios, painéis e calendários](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Você pode compartilhar relatórios criados com outros indivíduos, equipes, grupos, funções de trabalho ou empresas. Você também pode compartilhar relatórios criados por outras pessoas e compartilhados com você.
* Você também pode compartilhá-los com toda a organização ou torná-los públicos. Tornar um relatório público gera um URL que pode ser compartilhado com outras pessoas.
* Você pode compartilhar um relatório individual ou vários relatórios de uma lista de relatórios.

## Maneiras de compartilhar relatórios

Você pode compartilhar relatórios no Workfront da seguinte maneira:

* Manualmente, conforme descrito na seção [Compartilhar um relatório](#share-a-report) abaixo.
* Automaticamente, herdando permissões de Exibição de um painel que contém o relatório que foi compartilhado. Para obter informações sobre a exibição de permissões herdadas em objetos, consulte [Exibir permissões herdadas em objetos](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Compartilhar um relatório {#share-a-report}

O compartilhamento de um ou vários relatórios de uma lista é idêntico.

1. Vá para uma lista de relatórios, selecione um ou vários relatórios e clique em **Compartilhar**.

   Ou

   Clique no nome de um relatório e em **Ações de Relatório >****Compartilhamento**.

   ![](assets/qs-report-actions-sharing.png)

1. Na caixa que é exibida, no campo **Adicionar pessoas, equipes, funções, grupos ou empresas ...**, comece digitando o nome do usuário, equipe, função de trabalho, grupo ou empresa com a qual deseja compartilhar o relatório e pressione **Enter** quando o nome for exibido.

1. Para ajustar o nível de acesso a um nome adicionado, clique no menu suspenso à direita do nome e escolha uma das opções abaixo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Visualizar o projeto</td> 
      <td> <p>Permite que o destinatário acesse para ver o relatório na área <strong>Relatórios</strong> <img src="assets/reports-in-main-menu.png"> e executá-lo.</p> <p>Você pode clicar em <strong>Configurações Avançadas</strong> para especificar se deseja que o usuário ou usuários possam <strong>Compartilhar</strong> com qualquer pessoa no sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar o projeto</td> 
      <td> <p>Permite ao recipient acesso completo de edição ao relatório.</p> <p>Você pode clicar em <strong>Configurações avançadas</strong> para especificar se deseja que o usuário ou usuários <strong>excluam</strong> o relatório do sistema e <strong>compartilhem</strong> com qualquer pessoa no sistema.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita as duas etapas anteriores para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Clique no ícone de **engrenagem** ![](assets/gear-icon-settings-with-dn-arrow.jpg) no canto superior direito da caixa de compartilhamento e selecione uma das seguintes opções:

   * **Tornar público para usuários externos:** selecione esta opção para gerar uma URL que possa ser compartilhada com outras pessoas. Qualquer pessoa com o URL pode acessar o relatório, sem ter uma licença do Adobe Workfront.

     >[!CAUTION]
     >
     >Recomendamos que você tenha cuidado ao compartilhar com usuários externos um objeto que contém informações confidenciais. Isso permite que eles visualizem informações sem ser um usuário da Workfront ou parte da organização.

     >[!NOTE]
     >
     >Se o relatório tiver um prompt e você compartilhá-lo publicamente, os usuários que executam o relatório por meio do link de compartilhamento público não poderão executar o relatório usando o prompt. Eles verão o relatório sem o prompt aplicado, a menos que façam logon no Workfront e acessem o relatório sem usar o link de compartilhamento público. Para obter mais informações sobre as limitações do compartilhamento de relatórios com prompts, consulte a seção [Limitações do compartilhamento de relatórios solicitados](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) no artigo [Adicionar prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

   * **Tornar isto visível em todo o sistema:** Selecione esta opção para que todos no Workfront com acesso aos relatórios possam ver o relatório.

1. Clique em **Salvar**.
