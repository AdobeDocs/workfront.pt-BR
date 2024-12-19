---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Usar cURL para adicionar um módulo HTTP
description: Você pode colar uma solicitação cURL no seu cenário e o Fusion cria um módulo HTTP configurado a partir da solicitação cURL.
author: Becky
feature: Workfront Fusion
source-git-commit: 4cc881f4f5a28bd105e6898ad7ffb57c1dafb563
workflow-type: tm+mt
source-wordcount: '321'
ht-degree: 0%

---

# Usar cURL para adicionar um módulo HTTP

Você pode colar uma solicitação cURL no seu cenário e o Fusion cria um módulo HTTP configurado a partir da solicitação cURL.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para usar a funcionalidade neste artigo:

<table style="table-layout:auto"> 
  <tbody>  
    <tr>  
      <td>plano do Adobe Workfront</td>  
      <td>Qualquer</td>  
    </tr>  
    <tr>  
      <td>Licença do Adobe Workfront</td>  
      <td>
        Novo: Padrão<br>
        Ou<br>
        Atual: trabalho ou superior
      </td>  
    </tr>  
    <tr>  
      <td>Licença do Adobe Workfront Fusion</td>  
      <td> 
        Atual: nenhum requisito de licença do Workfront Fusion.<br>
        Ou<br>
        Herdados: Qualquer um
      </td>  
    </tr>  
    <tr>  
      <td>Produto</td>  
      <td> 
        Novo: Selecione ou Prime Workfront Plan: sua organização deve comprar o Adobe Workfront Fusion.<br>
        Plano do Ultimate Workfront: o Workfront Fusion está incluído.<br>
        Ou<br>
        Atual: sua organização deve comprar o Adobe Workfront Fusion.
      </td>  
    </tr> 
  </tbody>  
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Para obter informações sobre [!DNL Adobe Workfront Fusion] licenças, consulte [[!DNL Adobe Workfront Fusion] licenças](../../workfront-fusion/get-started/license-automation-vs-integration.md).

+++

## Criar um módulo HTTP a partir de uma solicitação cURL


Para criar um módulo HTTP usando cURL:

1. Crie o texto da solicitação cURL fora do Fusion, como em um editor de texto.

   >[!IMPORTANT]
   >
   >Se você estiver usando o Fusion em uma máquina com Windows, sua solicitação de cURL não deverá incluir quebras de linha.
1. Copie a solicitação cURL para a área de transferência.
1. Clique na guia **[!UICONTROL Cenário]** no painel esquerdo.
1. Selecione o cenário em que deseja criar o módulo.
1. Clique em qualquer lugar no cenário para entrar no editor de cenários.
1. Clique com o botão direito do mouse em qualquer espaço em branco no editor de cenários e selecione **Colar**.

   Ou

   Pressione Ctrl + V (Windows) ou Cmd + V (Mac).


   Um módulo HTML é criado.
1. Arraste o módulo para conectá-lo ao seu cenário.

## Solução de problemas

Se o cURL não estiver colando no cenário, verifique o seguinte:

* Verifique as configurações do navegador para garantir que a colagem da área de transferência esteja ativada.
* Se você estiver executando o Windows, verifique a solicitação cURL para garantir que ela não inclua quebras de linha.



