---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Compartilhar um relatório no Adobe Workfront
description: O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar relatórios quando eles atribuírem níveis de acesso. Para obter mais informações sobre como conceder acesso a problemas, consulte Conceder acesso a relatórios, painéis e calendários.
author: Nolan
feature: Reports and Dashboards
exl-id: 225e815a-0354-493d-bbcf-59304ef77570
source-git-commit: c8a25bcc8c9b56a649ca7764918c86f9cdd5b3e2
workflow-type: tm+mt
source-wordcount: '826'
ht-degree: 0%

---

# Compartilhar um relatório no Adobe Workfront

<!-- Audited: 11/2024 -->

O administrador do Adobe Workfront concede aos usuários acesso para visualizar ou editar relatórios quando eles atribuírem níveis de acesso. Para obter mais informações sobre como conceder acesso a problemas, consulte [Conceder acesso a relatórios, painéis e calendários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

Juntamente com o nível de acesso concedido aos usuários, você também pode conceder a eles permissões para Exibir ou Gerenciar relatórios específicos que você tenha acesso para compartilhar. Para obter mais informações sobre níveis de acesso e permissões, consulte [Como os níveis de acesso e as permissões funcionam juntos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

As permissões são específicas a um item no Workfront e definem quais ações podem ser executadas nesse item.

>[!NOTE]
>
>Um administrador do Workfront pode adicionar ou remover permissões a qualquer item no sistema, para todos os usuários, sem ser o proprietário desses itens.

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
      <p>Leve</p>
      <p>Revisar</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso de visualização ou superior a relatórios, painéis, calendários</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores para o relatório</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre o compartilhamento de relatórios

Além das considerações abaixo, consulte também [Compartilhar relatórios, painéis e calendários](../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md).

* Você pode compartilhar relatórios criados com outros indivíduos, equipes, grupos, funções de trabalho ou empresas. Você também pode compartilhar relatórios criados por outras pessoas e compartilhados com você.
* Você pode compartilhar relatórios com toda a organização ou torná-los públicos. Tornar um relatório público gera um URL que pode ser compartilhado com outras pessoas.
* Você pode compartilhar um relatório individual ou vários relatórios de uma lista de relatórios.

## Maneiras de compartilhar relatórios

Você pode compartilhar relatórios no Workfront da seguinte maneira:

* Manualmente, conforme descrito na seção [Compartilhar um relatório](#share-a-report) abaixo.
* Automaticamente herdando permissões de exibição de um painel que contém o relatório que foi compartilhado. Para obter informações sobre a exibição de permissões herdadas em objetos, consulte [Exibir permissões herdadas em objetos](../../../workfront-basics/grant-and-request-access-to-objects/view-inherited-permissions-on-objects.md).

## Compartilhar um relatório {#share-a-report}

O compartilhamento de um ou vários relatórios de uma lista é idêntico.

1. Vá para uma lista de relatórios, selecione um ou vários relatórios e clique no **ícone Compartilhar** ![ícone Compartilhar](assets/share-icon.png).

   Ou

   Clique no nome de um relatório e em **Ações de Relatório** > **Compartilhamento**. A caixa **Compartilhar [NOME DO RELATÓRIO]** é aberta.

   ![Opção de compartilhamento](assets/unshimmed-report-actions-sharing.png)

1. No campo **Conceder acesso ao relatório para**, comece digitando o nome do usuário, da equipe, da função de trabalho, do grupo ou da empresa com a qual deseja compartilhar o relatório e selecione-o quando ele for exibido.

1. Para ajustar o nível de acesso a um nome adicionado, clique no menu suspenso à direita do nome e escolha uma das opções abaixo.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Exibir</td> 
      <td> <p>Permite que o destinatário acesse para ver o relatório na área <strong>Relatórios</strong> e executá-lo.</p> <p>Você pode clicar no ícone <strong>Configurações avançadas</strong> à direita para especificar se deseja que o usuário ou usuários <strong>compartilhem</strong> com qualquer pessoa no sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Gerenciar</td> 
      <td> <p>Permite ao recipient acesso completo de edição ao relatório.</p> <p>Você pode clicar no ícone <strong>Configurações avançadas</strong> à direita para especificar se deseja que o usuário ou usuários <strong>excluam</strong> o relatório do sistema e <strong>o compartilhem</strong> com qualquer pessoa no sistema.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita as duas etapas anteriores para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Clique no menu suspenso **Somente pessoas convidadas podem acessar** na caixa de compartilhamento e escolha entre as seguintes opções:

   * **Somente pessoas convidadas podem acessar**: selecione esta opção para que somente os usuários aos quais foi concedido acesso ao relatório possam exibi-lo.

   * **Todos no sistema podem exibir**: selecione esta opção para que todos no Workfront com acesso a relatórios possam exibir o relatório.

1. (Opcional) Clique no ícone de **engrenagem** ![configurações do ícone de engrenagem](assets/gear-icon-settings-with-dn-arrow.jpg) no canto superior direito da caixa de compartilhamento e, opcionalmente, selecione a seguinte opção:

   * **Tornar público para usuários externos**: selecione esta opção para gerar uma URL que possa ser compartilhada com outras pessoas. Qualquer pessoa com o URL pode acessar o relatório, sem ter uma licença do Adobe Workfront.

     >[!CAUTION]
     >
     >Recomendamos que você tenha cuidado ao compartilhar com usuários externos um objeto que contém informações confidenciais. Isso permite que eles visualizem informações sem ser um usuário da Workfront ou parte da organização.

     >[!NOTE]
     >
     >Se o relatório tiver um prompt e você compartilhá-lo publicamente, os usuários que executam o relatório por meio do link de compartilhamento público não poderão executar o relatório usando o prompt. Eles verão o relatório sem o prompt aplicado, a menos que façam logon no Workfront e acessem o relatório sem usar o link de compartilhamento público. Para obter mais informações sobre as limitações do compartilhamento de relatórios com prompts, consulte a seção [Limitações do compartilhamento de relatórios solicitados](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md#limitations-of-running-public-prompted-reports) no artigo [Adicionar prompt a um relatório](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Clique em **Salvar**.
