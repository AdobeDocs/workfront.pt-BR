---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limitações de exibição do Planejador de recursos
description: Para melhorar o desempenho, o Adobe Workfront está limitando a quantidade de informações que podem ser exibidas, bem como a quantidade de informações que podem ser exportadas do Planejador de recursos.
author: Alina
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '948'
ht-degree: 0%

---

# Limitações de exibição do Planejador de recursos

Para melhorar o desempenho, o Adobe Workfront está limitando a quantidade de informações que podem ser exibidas, bem como a quantidade de informações que podem ser exportadas do Planejador de recursos.

Quando esse limite é atingido, o Workfront exibe uma mensagem de aviso para que você saiba que o limite foi atingido.

Se as informações que você espera ver no Planejador de recursos não forem exibidas, é possível que você esteja tentando exibir muitas informações e alguns dados não foram exibidos devido a essa limitação.

Recomendamos o seguinte para obter o desempenho ideal na exibição e exportação do Planejador de recursos:

* Use filtros para reduzir a quantidade de informações exibidas no Planejador de recursos e exibir somente as informações pertinentes.
* Use todas as opções de exportação para reduzir o volume de informações exportadas de uma só vez e garantir que você exporte apenas as informações pertinentes.\
  Para obter mais informações sobre como usar filtros e exportar opções no Planejador de recursos, consulte [Informações de filtro no Planejador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).

  Para obter informações sobre como exportar informações do Planejador de recursos, consulte [Exportar informações do Planejador de recursos](../../resource-mgmt/resource-planning/export-resource-planner.md).

A quantidade de informações que você pode exibir ou exportar depende da exibição aplicada e do ambiente usado para acessar o Planejador de recursos.

## Limitações na Visualização de Projeto

Considere o seguinte ao aplicar a exibição Projeto ao Planejador de Recursos:

* Você só pode ver projetos que tem acesso para gerenciar.
* Você pode expandir cada projeto para visualizar as funções associadas a ele e cada função para visualizar os usuários associados a ele.

  É possível visualizar até 300 projetos ao rolar a tela para a parte inferior da lista, a menos que haja mais de 30.000 linhas de projetos, funções e usuários. Em seguida, você receberá uma mensagem de aviso informando que atingiu o limite de 30.000 linhas.

* É possível exibir três ou quatro períodos de tempo por vez, dependendo do tamanho da tela.

Leve em consideração o seguinte ao exportar informações da visualização Projeto do Planejador de recursos, após aplicar todos os filtros e opções de exportação apropriados:

* Quando você seleciona exportar tudo ( projetos, funções e usuários) no Planejador de recursos, todos os objetos que correspondem aos seus critérios são exibidos no arquivo exportado, independentemente de você ter rolado a tela para a parte inferior da lista para exibi-los ou não.
* Linhas sem informações de alocação são incluídas no arquivo exportado.

* É possível exportar até 30.000 linhas.

## Limitações na visualização Função

Considere o seguinte ao aplicar a visualização Função ao Planejador de recursos, depois de aplicar todos os filtros apropriados:

* Você pode ver somente as funções associadas aos projetos que você pode gerenciar.

* Você pode ver até 300 funções ao rolar para a parte inferior da lista, a menos que haja mais de 30.000 linhas de funções, projetos e usuários. Em seguida, você receberá uma mensagem de aviso informando que atingiu o limite de 30.000 linhas para o que pode visualizar na tela.
* Você pode expandir cada função para exibir uma lista de projetos, e cada projeto para exibir uma lista de usuários que podem desempenhar essas funções nos projetos.

  20 projetos são exibidos por padrão e você pode usar a opção Carregar mais para exibir projetos adicionais ou rolar a tela em cada projeto para carregar mais usuários.

* É possível exibir três ou quatro períodos de tempo, dependendo do tamanho da tela.

Leve em consideração o seguinte ao exportar informações da visualização Função do Planejador de recursos, após aplicar todos os filtros e opções de exportação apropriados:

* Quando você seleciona exportar tudo (funções, projetos e usuários) no Planejador de recursos, todos os objetos que correspondem aos seus critérios são exibidos no arquivo exportado, independentemente de você ter rolado a tela para a parte inferior da lista para exibi-los ou não.
* Linhas sem informações de alocação são incluídas no arquivo exportado.
* É possível exportar até 30.000 linhas.

## Limitações na visualização do usuário

Considere o seguinte ao aplicar a view Usuário ao Planejador de Recursos:

* Você pode exibir todos os usuários que atendem aos seguintes critérios:

   * Você tem acesso para visualizar
   * Estão ativos
   * Efetuou login pelo menos uma vez.

* Você pode expandir cada usuário para exibir os projetos associados a ele e cada projeto para exibir funções associadas a ele.\
  Os primeiros 50 projetos e funções são exibidos por padrão e você pode usar a opção Carregar mais para exibir projetos ou funções adicionais.

  >[!NOTE]
  >
  >Se você tiver filtrado a lista de usuários por projetos, somente os usuários associados aos projetos filtrados poderão ser expandidos e também exibir informações de horas

* Você pode ver até 2.000 usuários na interface da Web. O Workfront exibe uma mensagem de aviso quando você atinge esse limite.
* É possível exibir três ou quatro períodos de tempo, dependendo do tamanho da tela.

Leve em consideração o seguinte ao exportar informações da visualização Usuário do Planejador de recursos, após aplicar todos os filtros e opções de exportação apropriados:

* Quando você seleciona exportar tudo (usuários, funções e projetos) no Planejador de recursos, todas as funções, projetos e usuários são incluídos no arquivo exportado, estejam eles expandidos ou não na interface da Web.

* É possível exportar até 30.000 linhas que contenham usuários, bem como os projetos e funções listados abaixo, independentemente de você ter rolado a tela para a parte inferior da lista para exibi-las ou não. Todos os usuários, projetos e funções são incluídos no arquivo exportado, estejam eles expandidos ou não na interface da Web.
* Linhas sem informações de alocação são incluídas no arquivo exportado.
