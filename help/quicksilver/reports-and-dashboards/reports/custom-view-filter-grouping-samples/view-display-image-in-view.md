---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Exibir: exibir uma imagem em vez de uma string em uma coluna'''
description: É possível substituir o nome de um objeto em uma exibição por uma imagem usando o modo de texto. Você também pode adicionar um link à imagem que pode abrir o objeto que ela substitui.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e1e4a993-f05c-4b6e-b00a-e96c9ab4c94f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Exibir: exibir uma imagem em vez de uma string em uma coluna

É possível substituir o nome de um objeto em uma exibição por uma imagem usando o modo de texto. Você também pode adicionar um link à imagem que pode abrir o objeto que ela substitui.

>[!NOTE]
>
>As imagens aparecem em sua resolução real para tentar usar imagens pequenas.

![](assets/replace-project-name-with-image-and-link-350x125.png)

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exemplo: Substitua o nome de um projeto em uma visualização de projeto por uma imagem:

1. Carregue uma imagem em um site da Web ou servidor externo ao Adobe Workfront. Você deve conseguir acessar a imagem usando o navegador da Web.

   >[!TIP]
   >
   >* Cada tipo de navegador é diferente, mas todos são capazes de exibir URLs.
   >* Evite usar imagens que são carregadas no Workfront. Como as imagens armazenadas no Workfront não estão disponíveis publicamente e têm uma chave de acesso que expira após um período de tempo, essas imagens param de ser exibidas na visualização ao longo do tempo.
   >* Uma imagem salva em seu computador não tem um URL inerente. Localize um site que forneça hospedagem de imagens e hospede sua imagem lá. Sua organização pode já ter esse site.


1. Usando seu navegador da Web, vá para a imagem que você salvou.
1. Obtenha o URL da imagem fazendo o seguinte:

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: I used this blog post to document what kind of image we need for this: https://www.canto.com/blog/image-url/ (consulting uses this)) </p>
   -->

   1. Clique com o botão direito do mouse e selecione **Copiar local da imagem** ou **Obter link**, dependendo do navegador. Agora você tem o URL para essa imagem específica e pode colá-la da área de transferência.
   1. Certifique-se de que todos com esse link tenham permissões para exibir a imagem acessando o link e que eles não precisem de um logon para acessá-la.

1. Vá para um projeto e clique no botão **Mais** menu ![](assets/more-icon-45x33.png) ao lado do nome do projeto, clique em **Editar**.

1. No **URL** , adicione o link à imagem.
1. Navegue até uma exibição de projeto em uma lista ou relatório e personalize a exibição.
1. Clique no cabeçalho da coluna para a **Nome do projeto**, depois clique em **Alternar para o modo de texto**.

1. Adicione o seguinte código à coluna do código existente:

   ```
   displayname=Link Project
   ```

   ```
   image.name=Link Project
   ```

   ```
   image.valuefield=URL
   ```

   ```
   link.linkproperty.0.name=projectID
   ```

   ```
   link.linkproperty.0.value=ID
   ```

   ```
   link.lookup=link.edit
   ```

   ```
   link.page=/view
   ```

   ```
   link.valuefield=objCode
   ```

   ```
   link.valueformat=val
   ```

   ```
   textmode=true
   ```

   ```
   type=image
   ```

   ```
   valueformat=
   ```

   A imagem selecionada substitui o Nome do projeto na exibição do projeto e a imagem é um link para o projeto.

1. Clique em **Salvar exibição**.
