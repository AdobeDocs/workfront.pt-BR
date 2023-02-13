---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Copiar um painel
description: Você pode copiar um painel e todo o seu conteúdo (relatórios, calendários e páginas externas). Ao copiar o conteúdo de um painel, você pode optar por mantê-los à medida que aparecem no painel original ou criar novos itens que são cópias desses itens no painel original. Você também pode optar por não transferir ou copiar itens no novo painel.
author: Nolan
feature: Reports and Dashboards
exl-id: a88cc171-2bb1-40f0-a778-8dac7eecb718
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '901'
ht-degree: 0%

---

# Copiar um painel

Você pode copiar um painel e todo o seu conteúdo (relatórios, calendários e páginas externas). Ao copiar o conteúdo de um painel, você pode optar por mantê-los à medida que aparecem no painel original ou criar novos itens que são cópias desses itens no painel original. Você também pode optar por não transferir ou copiar itens no novo painel.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plano Adobe Workfront*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licença da Adobe Workfront*</strong></td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configurações de nível de acesso*</strong></td> 
   <td> <p>Editar acesso a Relatórios, Painéis e Calendários</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permissões de objeto</strong></td> 
   <td> <p>Visualizar acesso a um painel</p> <p>Você obterá o acesso de Gerenciar ao painel copiado</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Pré-requisitos

Você deve criar um painel antes de poder copiá-lo.

Para obter informações sobre como criar painéis, consulte [Criar um painel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Copiar um painel

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png), depois clique em **Painéis**.

1. Selecione o painel que deseja copiar e clique em **Copiar** ![](assets/copy-icon.png).\
   Ou\
   Abra o painel que deseja copiar e clique em **Ações do painel** > **Copiar**.\
   A caixa de diálogo Cópia do painel é exibida. Todos os itens no painel original são exibidos.

1. No **Nome do painel** , especifique um novo nome para o painel.
1. Para selecionar todos os itens no painel existente e copiá-los para o painel copiado, deixe **Selecionar tudo** selecionado. Por padrão, os relatórios, calendários ou listas no painel existente serão copiados para o novo painel.\
   Ou\
   Para transferir apenas itens específicos do painel original para o novo, desmarque os itens que você não deseja que apareçam no novo painel e, em seguida, para cada item selecionado, escolha entre as seguintes opções:

   * **Fazer uma cópia:** O item é copiado do painel original e uma nova versão desse item é exibida no novo painel. As alterações feitas no item no novo painel não são refletidas no item no painel original. Da mesma forma, as alterações feitas no item no painel original não são refletidas no item no novo painel.\
      Use essa opção quando quiser modificar o relatório original no painel original.\
      Por exemplo, você copia um painel chamado &#39;Equipe B&#39; e o renomeia como &#39;Equipe A&#39;. No painel &#39;Equipe B&#39; há um relatório chamado &#39;Relatório de Equipe B&#39;. Como este relatório contém dados específicos para a Equipe B, você seleciona a opção para fazer uma cópia deste relatório para que você possa personalizá-lo para a Equipe A e renomeá-lo posteriormente para &#39;Relatório da Equipe A&#39;.\
      Com essa opção, você remove as permissões de compartilhamento do relatório original do relatório copiado. A opção Executar este relatório com os Direitos de acesso das informações permanece intacta no relatório copiado.

   * **Usar original:** Exibe o item original no novo painel. As alterações feitas no item no novo painel também são refletidas no item no painel original. Da mesma forma, as alterações feitas no item no painel original são refletidas no item no novo painel.\
      Com essa opção, você mantém as permissões de compartilhamento do relatório original. A opção Executar este relatório com os Direitos de acesso das informações também permanece intacta.

1. (Opcional) Renomeie todos os itens selecionados.
1. Clique em **Copiar painel**.
1. (Opcional) Se você deseja editar relatórios, calendários e páginas externas copiados no painel copiado, siga um destes procedimentos:

   * Para editar qualquer informação para qualquer relatório copiado, clique no nome do relatório no painel e **Ações de Relatório** > **Editar**.

      Por exemplo, você pode editar a Exibição, o Filtro, o Agrupamento, o Aviso ou o Gráfico, ou um relatório copiado.

   * Para restabelecer permissões nos relatórios copiados, clique no nome do relatório no novo painel e clique em **Ações de Relatório** > **Compartilhamento** e atualize as permissões no relatório.

      Ao copiar um relatório ao copiar um painel, as permissões nele são removidas.

   * Para modificar o relatório Executar este relatório com os Direitos de acesso das informações, clique no nome do relatório no novo painel e **Ações de Relatório** > **Editar** > **Opções de relatório**.\
      Depois de copiar um relatório, a opção Executar este relatório com os Direitos de acesso de permissões é mantida somente nas seguintes circunstâncias:

      (Se nenhuma dessas condições for verdadeira, Executar este relatório com os Direitos de acesso das permissões serão removidos e o novo Executar este relatório com os Direitos de acesso do será alterado para o usuário que criou o relatório copiado.)

      Se o usuário copiar o painel e seus relatórios tiver direitos de acesso de Administrador.

      * Se o usuário copiar o painel e seus relatórios tiver direitos de acesso de Administrador.
      * Se o usuário que copia o painel e seus relatórios estiver definido como Executar este relatório com os Direitos de acesso de para os relatórios que estão sendo copiados.
      * Se o usuário que copia o relatório tiver permissões de gerenciamento no relatório.
