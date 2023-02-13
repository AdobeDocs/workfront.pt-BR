---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Limitações de exibição do Planejador de recursos
description: Para melhorar o desempenho, a Adobe Workfront está limitando a quantidade de informações que você pode exibir, bem como a quantidade de informações que você pode exportar do Planejador de Recursos.
author: Alina
feature: Resource Management
exl-id: 12f56f11-59fb-4318-b43a-5ac695ca1e7e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 0%

---

# Limitações de exibição do Planejador de recursos

Para melhorar o desempenho, a Adobe Workfront está limitando a quantidade de informações que você pode exibir, bem como a quantidade de informações que você pode exportar do Planejador de Recursos.

Quando você se aproxima desse limite, o Workfront exibe uma mensagem de aviso para que saiba que você atingiu esse limite.

Se as informações que você espera ver no Planejador de Recursos não forem exibidas, é possível que você esteja tentando exibir informações demais e alguns dados não foram exibidos devido a essa limitação.

Recomendamos o seguinte para obter o desempenho ideal na exibição e exportação do Planejador de Recursos:

* Use filtros para reduzir a quantidade de informações exibidas no Planejador de Recursos e exibir apenas as informações pertinentes a você.
* Use todas as opções de exportação para reduzir a quantidade de informações exportadas de uma vez e garantir a exportação apenas das informações pertinentes.\
   Para obter mais informações sobre o uso de filtros e opções de exportação no Planejador de Recursos, consulte [Filtrar informações no Planejador de Recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).

   Para obter informações sobre exportação de informações do Planejador de Recursos, consulte [Exportar informações do Planejador de Recursos](../../resource-mgmt/resource-planning/export-resource-planner.md).

A quantidade de informações que você pode exibir ou exportar depende da exibição aplicada e do ambiente usado para acessar o Planejador de Recursos.

## Limitações na exibição Projeto

Considere o seguinte ao aplicar a exibição Projeto ao Planejador de Recursos:

* Você só pode ver projetos que tenham acesso para gerenciar.
* Você pode expandir cada projeto para exibir as funções associadas a ele e cada função para visualizar os usuários associados a ele.

   É possível visualizar até 300 projetos ao rolar para a parte inferior da lista, a menos que haja mais de 30.000 linhas de projetos, funções e usuários. Em seguida, você receberá uma mensagem de aviso informando que atingiu o limite de 30.000 linhas.

* É possível visualizar três ou quatro períodos de tempo por vez, dependendo do tamanho da tela.

Considere o seguinte ao exportar informações da exibição Projeto do Planejador de Recursos, após ter aplicado todos os filtros e opções de exportação apropriados:

* Quando você seleciona exportar tudo (projetos, funções e usuários) no Planejador de Recursos, todos os objetos que correspondem aos seus critérios serão exibidos no arquivo exportado, independentemente de você ter rolado para a parte inferior da lista para exibi-los ou não.
* As linhas sem informações de alocação são incluídas no arquivo exportado.

* É possível exportar até 30.000 linhas.

## Limitações na exibição de funções

Considere o seguinte ao aplicar a exibição Função ao Planejador de Recursos, após ter aplicado todos os filtros apropriados:

* Você pode ver somente funções associadas a projetos que você pode gerenciar.

* É possível visualizar até 300 funções ao rolar para a parte inferior da lista, a menos que haja mais de 30.000 linhas de funções, projetos e usuários. Em seguida, você receberá uma mensagem de aviso informando que atingiu o limite de 30.000 linhas para o que pode ser visualizado na tela.
* Você pode expandir cada função para exibir uma lista de projetos e cada projeto para exibir uma lista de usuários que podem atender a essas funções nos projetos.

   20 projetos são exibidos por padrão e você pode usar a opção Carregar mais para exibir projetos adicionais ou rolar em cada projeto para carregar mais usuários.

* É possível visualizar três ou quatro períodos de tempo, dependendo do tamanho da tela.

Considere o seguinte ao exportar informações da exibição Função do Planejador de Recursos, após ter aplicado todos os filtros apropriados e opções de exportação:

* Quando você seleciona exportar tudo (funções, projetos e usuários) no Planejador de Recursos, todos os objetos que correspondem aos seus critérios serão exibidos no arquivo exportado, independentemente de você ter rolado para a parte inferior da lista para exibi-los ou não.
* As linhas sem informações de alocação são incluídas no arquivo exportado.
* É possível exportar até 30.000 linhas.

## Limitações na exibição do usuário

Considere o seguinte ao aplicar a exibição Usuário ao Planejador de Recursos:

* Você pode exibir todos os usuários que atendem aos seguintes critérios:

   * Você tem acesso à visualização
   * Estão ativos
   * Ter feito logon pelo menos uma vez.

* Você pode expandir cada usuário para exibir os projetos associados a ele e cada projeto para exibir as funções associadas a ele.\
   Os primeiros 50 projetos e funções são exibidos por padrão, e você pode usar a opção Carregar mais para exibir projetos ou funções adicionais.

   >[!NOTE]
   >
   >Se você tiver filtrado a lista de usuários por projetos, somente os usuários associados aos projetos filtrados poderão ser expandidos e também exibir as informações da hora

* É possível visualizar até 2.000 usuários na interface da Web. O Workfront exibe uma mensagem de aviso ao atingir esse limite.
* É possível visualizar três ou quatro períodos de tempo, dependendo do tamanho da tela.

Considere o seguinte ao exportar informações da exibição Usuário do Planejador de Recursos, após ter aplicado todos os filtros apropriados e opções de exportação:

* Quando você seleciona exportar tudo (usuários, funções e projetos) no Planejador de Recursos, todas as funções, projetos e usuários são incluídos no arquivo exportado, sejam eles expandidos ou não na interface da Web.

* É possível exportar até 30.000 linhas que contêm usuários, bem como os projetos e funções listados abaixo, independentemente de você ter rolado para a parte inferior da lista para exibi-los ou não. Todos os usuários, projetos e funções são incluídos no arquivo exportado, sejam eles expandidos ou não na interface da Web.
* As linhas sem informações de alocação são incluídas no arquivo exportado.
