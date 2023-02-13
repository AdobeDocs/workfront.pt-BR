---
title: 2.2 Melhorias no gerenciamento de recursos
description: 2.2 Melhorias no gerenciamento de recursos
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: be4904f0b37870c1bfc8ec345e468d5fc283aa36
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# 2.2 Melhorias no gerenciamento de recursos

Esta página descreve todas as melhorias no Gerenciamento de recursos realizadas com a versão 2.2 para o ambiente de Visualização. Esses aprimoramentos serão disponibilizados no ambiente Produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 4 de abril de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.2, consulte [Visão geral da versão 2.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Melhorias na navegação do Balanceador de Carga de Trabalho

Para melhorar sua experiência ao usar o Balanceador de carga de trabalho, introduzimos os seguintes aprimoramentos:

* Os botões Cancelar e Salvar ao ajustar alocações agora são fixos, mesmo quando a tarefa é maior que o período de tempo incluído na tela ou quando o painel Resumo é exibido.
* O painel esquerdo que exibe os nomes dos usuários e dos itens de trabalho agora é aderente, para permitir que você role horizontalmente por períodos mais longos e ainda possa ler os nomes dos itens listados no painel.
* Você pode recolher e expandir todos os itens listados no painel esquerdo com um clique em vez de no nível do usuário ou do projeto.
* O painel esquerdo também pode ser redimensionado.
* Agora há um modo de tela cheia para o Balanceador de carga de trabalho.

Para obter mais informações sobre como navegar no Balanceador de Carga de Trabalho, consulte [Navegar pelo Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Acessar atribuições avançadas no balanceador de carga de trabalho

Para tornar a atribuição de itens de trabalho mais fácil e precisa, agora é possível fazer atribuições avançadas ao atribuir itens de trabalho manualmente no Balanceador de Carga de Trabalho. Antes desse aprimoramento, você podia acessar Atribuições avançadas ao editar itens, nos cabeçalhos dos itens ou em listas.

Para obter mais informações, consulte [Atribuir trabalho manualmente usando o Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nova fórmula para calcular a disponibilidade do usuário quando a preferência Programação Padrão é selecionada

Para fornecer informações mais precisas nas ferramentas de gerenciamento de recursos, alteramos a fórmula que o Workfront usa para calcular a disponibilidade do usuário quando o administrador do Workfront seleciona A programação padrão nas Preferências de gerenciamento de recursos. Com a nova atualização, o Workfront usa a seguinte fórmula para calcular a disponibilidade do usuário:

Horas Disponíveis do Usuário = (Horas de Programação Padrão - Exceções) &#42; FTE - Tempo limite

Antes dessa atualização, o Workfront usava a seguinte fórmula para calcular a disponibilidade do usuário quando a Programação Padrão era selecionada:

Horas Disponíveis do Usuário = (Horas de Programação Padrão - (Exceções de Programação + Tempo de Desativação) &#42; Valor FTE do usuário

Para obter mais informações, consulte [Configurar preferências do Gerenciamento de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

