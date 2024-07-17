---
navigation-topic: use-lists
title: Aplicar o filtro rápido a uma lista
description: Você pode usar o filtro rápido em uma lista de objetos para ajudá-lo a localizar somente itens importantes para você, para que possa revisá-los, atualizá-los ou compartilhá-los rapidamente com outras pessoas.
feature: Get Started with Workfront
author: Lisa
exl-id: 363f7ad1-f4f8-4cb1-a631-ee4e5ea28e5a
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '880'
ht-degree: 0%

---

# Aplicar o filtro rápido a uma lista

<!--
{{highlighted-preview}}
-->

Você pode usar o filtro rápido em uma lista de objetos para ajudá-lo a localizar somente itens importantes para você, para que possa revisá-los, atualizá-los ou compartilhá-los rapidamente com outras pessoas.

>[!IMPORTANT]
>
>Você pode encontrar itens que contenham uma palavra de pesquisa usando filtros rápidos, independentemente de esse item ter sido fisicamente exibido na tela ou ser exibido depois que você rolar para a parte inferior da página. Ao usar os recursos de pesquisa do seu navegador, você só pode encontrar itens que são fisicamente exibidos na tela. Se sua lista tem várias páginas, os filtros rápidos não localizam itens que estejam em páginas que não são exibidas.

Se quiser salvar um filtro rápido, recomendamos que você crie um filtro permanente para sua lista.\
Para obter informações sobre como criar filtros no [!DNL Adobe Workfront], consulte o artigo [Visão geral dos filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

O filtro rápido está disponível atualmente nas seguintes áreas


É possível usar filtros rápidos temporários em todas as listas, exceto os seguintes:

* A área [!UICONTROL Relatórios]
* Listas de documentos e relatórios
* Várias áreas de [!UICONTROL Instalação]
  >[!NOTE]
  >
  >Filtros rápidos estão disponíveis nas seguintes áreas de configuração: [!UICONTROL Grupos], [!UICONTROL Equipes], [!UICONTROL Empresas], [!UICONTROL Agendamentos], [!UICONTROL Modelos de Layout] e [!UICONTROL Forms Personalizada].


Considere o seguinte ao aplicar filtros rápidos a uma lista:

* Você pode usar palavras-chave para filtrar qualquer campo exibido na visualização da lista. Isso inclui campos personalizados ou campos complexos como [!UICONTROL Predecessores], [!UICONTROL Atribuições], [!UICONTROL Atribuição] e [!UICONTROL Status], [!UICONTROL Aprovador] e [!UICONTROL Status], etc.
* Se a lista tiver agrupamentos recolhidos, eles serão expandidos automaticamente ao usar filtros rápidos. Ao remover o filtro rápido, os agrupamentos são recolhidos novamente.
* Os agrupamentos retêm as informações agregadas da lista original, independentemente dos filtros rápidos aplicados ou de quaisquer alterações feitas nos objetos na lista.
* Filtros rápidos são temporários. Alterar o agrupamento, a exibição, o filtro ou a classificação da lista remove os critérios do filtro rápido.
* Não é possível salvar um filtro rápido. Se quiser salvar um filtro para usá-lo novamente, considere criar um filtro permanente para a lista.
* Se houver mais de um agrupamento na lista e o filtro rápido encontrar itens em apenas um, somente esse agrupamento será exibido com os itens encontrados. Todos os outros agrupamentos estão ocultos.
* Em uma lista de tarefas ou subtarefas, a hierarquia de tarefas é removida quando os resultados do filtro rápido são exibidos.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] plano*</b></td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>[!DNL Adobe Workfront] licença*</b></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Configurações de nível de acesso*</b></td> 
   <td> <p>Visualizar o acesso à área em que a lista está</p> <p>Por exemplo, para aplicar um filtro rápido a um projeto, é necessário ter acesso à [!UICONTROL View] para Projetos.</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso.<br>Para obter informações sobre como um administrador do [!DNL Workfront] pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><b>Permissões de objeto</b></td> 
   <td> <p>[!UICONTROL Exibir]</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do [!DNL Workfront].

## Aplicar um filtro rápido a uma lista

1. Vá para uma lista ou um relatório que tenha suporte para filtros rápidos e clique no ícone **[!UICONTROL Filtro Rápido]** ![](assets/qs-quick-filter-icon.png) na barra de ferramentas.

   Ou

   Dependendo do seu sistema operacional ou navegador e ao usar um teclado QWERTY padrão, pressione o seguinte conjunto de comandos para iniciar o filtro rápido:

   * ALT+F para [!DNL Windows] computadores
   * ALT/ Option+F para [!DNL Mac] computadores

     >[!TIP]
     >
     >Se você pressionar CTRL+F ou CMD+F, uma dica de ferramenta será exibida ao lado do filtro rápido para lembrá-lo sobre esses comandos. Os comandos também são exibidos dentro da caixa de pesquisa de filtro rápido.

1. Na caixa **[!UICONTROL Filtrar página]**, digite a palavra-chave pela qual deseja filtrar.

   Você pode usar qualquer palavra exibida atualmente na exibição da lista.

   >[!NOTE]
   >
   >Se você usar uma palavra que pode ser exibida em outra página da lista, o filtro rápido não encontrará resultados.

   Uma lista de itens que correspondem aos critérios de pesquisa é exibida dinamicamente na lista à medida que você digita e todos os outros itens são ocultados. A palavra-chave usada na pesquisa é realçada em amarelo em todos os campos independentes e complexos. Alguns exemplos de campos complexos são colunas compartilhadas ou qualquer um dos seguintes: [!UICONTROL Atribuições], [!UICONTROL Atribuições] e [!UICONTROL Status], [!UICONTROL Percentual Concluído], [!UICONTROL Predecessoras], [!UICONTROL Aprovadores e Status], [!UICONTROL Gerentes de Recursos], [!UICONTROL Categorias], [!UICONTROL Condição], [!UICONTROL Atualização de Condição], etc.

1. (Opcional) Para editar em massa os itens encontrados pelo filtro rápido:

   1. Selecione todos ou vários itens na lista e clique em **[!UICONTROL Editar]** para editar os itens em massa.
   1. Após concluir as edições, clique em **[!UICONTROL Salvar alterações]**.

1. (Opcional) Para exportar os itens encontrados pelo filtro rápido, selecione todos ou vários itens na lista e clique em **[!UICONTROL Exportar]**.

   ![select_all_projects_with_highlight__1_.png](assets/select-all-projects-with-highlight--1--350x173.png)

   >[!NOTE]
   >
   >Somente os itens encontrados na exportação da pesquisa de filtro rápido para o arquivo selecionado. Se você não selecionar nenhum item antes de exportar a lista, a lista completa e não filtrada será exportada.\
   >Para obter mais informações, consulte [Exportar uma lista](../../../workfront-basics/navigate-workfront/use-lists/export-lists.md).

1. (Opcional) Para limpar os resultados filtrados, clique no ícone **[!UICONTROL Filtro rápido]**, no canto superior direito da janela.\
   Ou\
   Atualize a página.
