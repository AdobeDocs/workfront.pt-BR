---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Exibição: exibir uma imagem em vez de uma cadeia de caracteres em uma coluna'
description: Você pode substituir o nome de um objeto em uma visualização por uma imagem usando o modo de texto. Você também pode adicionar um link para a imagem que pode abrir o objeto substituído.
author: Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '497'
ht-degree: 0%

---

# Exibição: exibir uma imagem em vez de uma cadeia de caracteres em uma coluna

<!--Audited: 11/2024-->

Você pode substituir o nome de um objeto em uma visualização por uma imagem usando o modo de texto. Você também pode adicionar um link para a imagem que pode abrir o objeto substituído.

>[!NOTE]
>
>As imagens aparecem em sua resolução real, portanto, tente usar imagens pequenas.

![Substituir nome do projeto por imagem e link](assets/replace-project-name-with-image-and-link-350x125.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> 
    <p>Novo:</p>
   <ul><li><p>Colaborador para modificar um filtro </p></li>
   <li><p>Padrão para modificar um relatório</p></li> </ul>

<p>Atual:</p>
   <ul><li><p>Solicitação para modificar um filtro </p></li>
   <li><p>Planejar a modificação de um relatório</p></li> </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exemplo: substituir o nome de um projeto em uma visualização de projeto por uma imagem:

1. Faça upload de uma imagem para um site ou servidor externo do Adobe Workfront. Você deve conseguir acessar a imagem usando o navegador da Web.

   >[!TIP]
   >
   >* Cada tipo de navegador é diferente, mas todos são capazes de exibir URLs.
   >* Evite usar imagens carregadas no Workfront. Como as imagens armazenadas no Workfront não estão disponíveis publicamente e têm uma chave de acesso que expira após um período de tempo, essas imagens param de ser exibidas na visualização ao longo do tempo.
   >* Uma imagem salva no computador não tem um URL inerente. Encontre um site que forneça hospedagem de imagens e hospede sua imagem lá. Sua organização pode já ter esse site.

1. Usando o navegador da Web, vá para a imagem salva.
1. Obtenha o URL da imagem fazendo o seguinte:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Clique com o botão direito do mouse e selecione **Copiar local da imagem** ou **Obter link**, dependendo do seu navegador. Agora você tem o URL para essa imagem específica e pode colá-lo da área de transferência.
   1. Certifique-se de que todos os usuários com esse link têm permissões para visualizar a imagem apenas acessando o link e que não precisam de um logon para acessá-la.

1. Vá para um projeto, clique no **Mais** ícone ![Mais](assets/more-icon-45x33.png) ao lado do nome do projeto e clique em **Editar**.

1. No campo **URL**, adicione o link à imagem.
1. Ir para uma exibição de projeto em uma lista de projetos.
1. Clique no menu suspenso **Exibir** e em **Nova Exibição**.
1. Clique no cabeçalho da coluna para o **Nome do Projeto** e clique em **Alternar para Modo de Texto**.

1. Adicione o seguinte código à coluna do código existente:

   ```
   displayname=Link Project
   image.name=Link Project
   image.valuefield=URL
   link.linkproperty.0.name=projectID
   link.linkproperty.0.value=ID
   link.lookup=link.edit
   link.page=/view
   link.valuefield=objCode
   link.valueformat=val
   textmode=true
   type=image
   valueformat=
   ```

1. Clique em **Concluído** > **Salvar exibição**.
A imagem selecionada substitui o Nome do projeto na visualização do projeto e a imagem é um link para o projeto.
