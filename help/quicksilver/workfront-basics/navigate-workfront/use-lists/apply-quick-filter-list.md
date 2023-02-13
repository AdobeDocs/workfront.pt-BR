---
navigation-topic: use-lists
title: Aplicar o filtro rápido a uma lista
description: Você pode usar o filtro rápido em uma lista de objetos para ajudar a localizar apenas itens importantes para você, de modo que possa revisá-los, atualizá-los ou compartilhá-los com outras pessoas rapidamente.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 1ab76287062598a526dcf2420845498f8f749453
workflow-type: tm+mt
source-wordcount: '886'
ht-degree: 0%

---

# Aplicar o filtro rápido a uma lista

<!--
{{highlighted-preview}}
-->

Você pode usar o filtro rápido em uma lista de objetos para ajudar a localizar apenas itens importantes para você, de modo que possa revisá-los, atualizá-los ou compartilhá-los com outras pessoas rapidamente.

>[!IMPORTANT]
>
>Você pode encontrar itens que contenham uma palavra de pesquisa usando filtros rápidos, independentemente de esse item ter sido fisicamente exibido na sua tela ou será exibido depois de ter rolado para a parte inferior da página. Ao usar os recursos de pesquisa do seu navegador, você só pode encontrar itens que são fisicamente exibidos na tela. Se a lista tiver várias páginas, os filtros rápidos não encontrarão itens que estejam nas páginas que não são exibidas.

Se quiser salvar um filtro rápido, recomendamos criar um filtro permanente para sua lista.\
Para obter informações sobre como criar filtros em [!DNL Adobe Workfront], consulte o artigo [Visão geral dos filtros em [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

O filtro rápido está disponível nas seguintes áreas


Você pode usar filtros rápidos temporários em todas as listas, exceto o seguinte:

* O [!UICONTROL Relatórios] area
* Listas e relatórios de documentos
* Vários [!UICONTROL Configuração] áreas
   >[!NOTE]
   >
   >Os filtros rápidos estão disponíveis nas seguintes áreas de configuração: [!UICONTROL Grupos], [!UICONTROL Equipes], [!UICONTROL Empresas], [!UICONTROL Agendamentos], [!UICONTROL Modelos de layout]e [!UICONTROL Forms personalizada].


Considere o seguinte ao aplicar filtros rápidos a uma lista:

* Você pode usar palavras-chave para filtrar qualquer campo exibido na exibição da lista. Isso inclui campos personalizados ou campos complexos, como [!UICONTROL Predecessores], [!UICONTROL Atribuições], [!UICONTROL Atribuição] e [!UICONTROL Status], [!UICONTROL Aprovador] e [!UICONTROL Status], etc.
* Se a lista tiver agrupamentos recolhidos, eles serão expandidos automaticamente quando você usar filtros rápidos. Ao remover o filtro rápido, os agrupamentos são recolhidos novamente.
* Os agrupamentos retêm as informações agregadas da lista original, independentemente dos filtros rápidos aplicados ou de quaisquer alterações feitas nos objetos da lista.
* Os filtros rápidos são temporários. Alterar o agrupamento, a visualização, o filtro ou a classificação da lista remove os critérios de filtro rápido.
* Não é possível salvar um filtro rápido. Se quiser salvar um filtro para usá-lo novamente, considere criar um filtro permanente para a lista.
* Se você tiver mais de um agrupamento na lista e o filtro rápido encontrar itens em apenas um agrupamento, somente esse agrupamento será exibido com os itens encontrados. Todos os outros agrupamentos estão ocultos.
* Em uma lista de tarefas ou subtarefas, a hierarquia de tarefas é removida quando os resultados do filtro rápido são exibidos.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] plano*</b></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] licença*</b></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Configurações de nível de acesso*</b></td> 
   <td> <p>Exibir o acesso à área em que a lista está</p> <p>Por exemplo, para aplicar um filtro rápido a um projeto, é necessário ter acesso à [!UICONTROL Exibição] para Projetos.</p> <p>Observação: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso.<br>Para obter informações sobre como uma [!DNL Workfront] administrador pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Permissões de objeto</b></td> 
   <td> <p>[!UICONTROL View]</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Aplicar um filtro rápido a uma lista

1. Vá para uma lista ou relatório que oferece suporte a filtros rápidos e clique no link **[!UICONTROL Filtro rápido] ícone** ![](assets/qs-quick-filter-icon.png) na barra de ferramentas.

   Ou

   Dependendo do seu sistema operacional ou navegador e ao usar um teclado QWERTY padrão, pressione o seguinte conjunto de comandos para iniciar o filtro rápido:

   * ALT+F para [!DNL Windows] computadores
   * ALT/Opção+F para [!DNL Mac] computadores

      >[!TIP]
      >
      >Se você pressionar CTRL+F ou CMD+F, uma dica de ferramenta será exibida ao lado do filtro rápido para lembrá-lo sobre esses comandos. Os comandos também são exibidos dentro da caixa de pesquisa de filtro rápido.

1. No **[!UICONTROL Filtrar página]** , digite a palavra-chave pela qual deseja filtrar.

   Você pode usar qualquer palavra que seja exibida atualmente na exibição da lista.

   >[!NOTE]
   >
   >Se você usar uma palavra que possa ser exibida em outra página da lista, o filtro rápido não encontrará resultados.

   Uma lista de itens que correspondem aos critérios de pesquisa é exibida dinamicamente na lista, à medida que você digita, e todos os outros itens ficam ocultos. A palavra-chave que você usou em sua pesquisa é realçada em amarelo em todos os campos independentes e complexos. Alguns exemplos de campos complexos são colunas compartilhadas ou qualquer um dos seguintes: [!UICONTROL Atribuições], [!UICONTROL Atribuições] e [!UICONTROL Status], [!UICONTROL Porcentagem concluída], [!UICONTROL Predecessores], [!UICONTROL Aprovadores e status], [!UICONTROL Gerentes de recursos], [!UICONTROL Categorias], [!UICONTROL Condição], [!UICONTROL Atualização de condição], etc.

1. (Opcional) Para editar itens em massa encontrados pelo filtro rápido:

   1. Selecione todos ou vários itens na lista e clique em **[!UICONTROL Editar]** para editar os itens em massa.
   1. Após concluir as edições, clique em **[!UICONTROL Salvar alterações]**.

1. (Opcional) Para exportar os itens encontrados pelo filtro rápido, selecione todos ou vários itens na lista e clique em **[!UICONTROL Exportar]**.

   ![select_all_projects_with_highlight_1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Somente os itens que você encontrou no filtro rápido pesquisam para exportar para o arquivo selecionado. Se você não selecionar nenhum item antes de exportar a lista, a lista completa e não filtrada é exportada.\
   >Para obter mais informações, consulte [Exportar uma lista](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Opcional) Para limpar os resultados filtrados, clique no botão **[!UICONTROL Filtro rápido]** no canto superior direito da janela.\
   Ou\
   Atualize a página.
