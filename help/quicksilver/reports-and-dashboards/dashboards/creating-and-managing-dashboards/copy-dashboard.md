---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiar um painel
description: Você pode copiar um painel e todo o seu conteúdo (relatórios, calendários e páginas externas). Ao copiar o conteúdo de um painel, você pode optar por mantê-los como aparecem no painel original ou criar novos itens que sejam cópias daqueles no painel original. Você também pode optar por não transferir ou copiar itens no novo painel.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '898'
ht-degree: 0%

---

# Copiar um painel

<!-- Audited: 1/2025 -->

Você pode copiar um painel e todo o seu conteúdo (relatórios, calendários e páginas externas). Ao copiar o conteúdo de um painel, você pode optar por mantê-los como aparecem no painel original ou criar novos itens que sejam cópias daqueles no painel original. Você também pode optar por não transferir ou copiar itens no novo painel.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plano do Adobe Workfront*</strong></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
    <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Visualizar acesso a um painel</p> <p>Você obterá acesso de Gerenciar ao painel copiado</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Pré-requisitos

Você deve criar um painel antes de poder copiá-lo.

Para obter informações sobre como criar painéis, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiar um painel

1. Clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon.png) no canto superior direito do Adobe Workfront ou (se disponível) clique no ícone **[!UICONTROL Menu Principal]** ![Menu Principal](/help/_includes/assets/main-menu-icon-left-nav.png) no canto superior esquerdo e clique em **[!UICONTROL Painéis]**.

1. Selecione o painel que você deseja copiar e clique em **Copiar** ![Ícone Copiar](assets/copy-icon.png).\
   Ou\
   Abra o painel que deseja copiar e clique em **Ações do Painel** > **Copiar**.\
   A caixa de diálogo Cópia do painel é exibida. Todos os itens no painel original são exibidos.

1. No campo **Nome do Painel**, especifique um novo nome para o painel.
1. Para selecionar todos os itens no painel existente e copiá-los no painel copiado, deixe **Selecionar todos** selecionado. Por padrão, os relatórios, calendários ou listas no painel existente serão copiados para o novo painel.\
   Ou\
   Para transferir somente itens específicos do painel original para o novo, desmarque os itens que você não deseja que apareçam no novo painel e, para cada item selecionado, escolha entre as seguintes opções:

   * **Fazer uma Cópia:** O item é copiado do painel original e uma nova versão desse item é exibida no novo painel. As alterações feitas no item no novo painel não são refletidas no item no painel original. Da mesma forma, as alterações feitas no item no painel original não são refletidas no item no novo painel.\
     Use essa opção quando quiser modificar o relatório original no painel original.\
     Por exemplo, você copia um painel chamado &#39;Equipe B&#39; e o renomeia para &#39;Equipe A&#39;. No painel &#39;Equipe B&#39; há um relatório chamado &#39;Relatório da Equipe B&#39;. Como este relatório contém dados específicos para a Equipe B, você seleciona a opção para fazer uma cópia deste relatório para que você possa personalizá-lo para a Equipe A e renomeá-lo posteriormente para &#39;Relatório da Equipe A&#39;.\
     Com essa opção, você remove as permissões de compartilhamento do relatório original do relatório copiado. A opção Run this report with the Access Rights of information permanece intacta no relatório copiado.

   * **Usar Original:** Exibe o item original no novo painel. As alterações feitas no item no novo painel também são refletidas no item no painel original. Da mesma forma, as alterações feitas no item no painel original são refletidas no item no novo painel.\
     Com essa opção, você mantém as permissões de compartilhamento do relatório original. A opção Run this report with the Access Rights of information também permanece intacta.

1. (Opcional) Renomeie todos os itens selecionados.
1. Clique em **Copiar Painel**.
1. (Opcional) Se quiser editar qualquer um dos relatórios, calendários e páginas externas copiados no painel copiado, siga um destes procedimentos:

   * Para editar qualquer informação referente aos relatórios copiados, clique no nome do relatório no painel e, em seguida, em **Ações de Relatório** > **Editar**.

     Por exemplo, talvez você queira editar a Exibição, o Filtro, o Agrupamento, a Solicitação ou o Gráfico ou um relatório copiado.

   * Para restabelecer as permissões nos relatórios copiados, clique no nome do relatório no novo painel e, em seguida, clique em **Ações de Relatório** > **Compartilhamento** e atualize as permissões no relatório.

     Ao copiar um relatório ao copiar um painel, as permissões desse relatório são removidas.

   * Para modificar Executar este relatório com os Direitos de Acesso às informações, clique no nome do relatório no novo painel e, em seguida, em **Ações de Relatório** > **Editar** > **Opções de Relatório**.\
     Depois de copiar um relatório, a opção Executar este relatório com direitos de acesso de permissões é mantida somente nas seguintes circunstâncias:

     (Se nenhuma dessas condições for verdadeira, a opção Executar este relatório com os direitos de acesso de permissões será removida, e a nova opção Executar este relatório com os direitos de acesso de será alterada para o usuário que criou o relatório copiado.)

     Se o usuário que estiver copiando o painel e seus relatórios tiver direitos de acesso de Administrador.

      * Se o usuário que estiver copiando o painel e seus relatórios tiver direitos de acesso de Administrador.
      * Se o usuário que está copiando o painel e seus relatórios estiver definido no momento como Executar este relatório com os direitos de acesso de para os relatórios que estão sendo copiados.
      * Se o usuário que copiar o relatório tiver permissões Gerenciar no relatório.
