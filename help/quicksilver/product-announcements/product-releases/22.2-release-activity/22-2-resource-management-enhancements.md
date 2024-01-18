---
title: 22.2 Aprimoramentos no gerenciamento de recursos
description: 22.2 Aprimoramentos no gerenciamento de recursos
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '373'
ht-degree: 0%

---

# 22.2 Aprimoramentos no gerenciamento de recursos

Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 22.2 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 4 de abril de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.2, consulte [Visão geral da versão 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Melhorias na navegação do Balanceador de carga de trabalho

Para melhorar sua experiência ao usar o Balanceador de carga de trabalho, introduzimos os seguintes aprimoramentos:

* Os botões Cancelar e Salvar ao ajustar alocações agora são fixos, mesmo quando a tarefa é mais longa do que o período incluído na tela ou quando o painel Resumo é exibido.
* O painel esquerdo que exibe os nomes de usuários e itens de trabalho agora é fixo, para permitir rolar horizontalmente por períodos mais longos e ainda poder ler os nomes dos itens listados no painel.
* Você pode recolher e expandir todos os itens listados no painel esquerdo com um clique em vez de no nível do usuário ou do projeto.
* Agora, o painel esquerdo também pode ser redimensionado.
* Agora há um modo de tela cheia para o Balanceador de carga de trabalho.

Para obter mais informações sobre como navegar no Balanceador de carga de trabalho, consulte [Navegar pelo Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Acessar atribuições avançadas no Balanceador de carga de trabalho

Para tornar a atribuição de itens de trabalho mais fácil e precisa, agora é possível fazer atribuições avançadas ao atribuir itens de trabalho manualmente no Balanceador de carga de trabalho. Antes desse aprimoramento, você poderia acessar as Atribuições avançadas ao editar itens, nos cabeçalhos dos itens ou em listas.

Para obter mais informações, consulte [Atribuir trabalho manualmente usando o Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nova fórmula para calcular a disponibilidade do usuário quando a preferência Agendamento padrão é selecionada

Para fornecer informações mais precisas nas ferramentas de gerenciamento de recursos, alteramos a fórmula usada pelo Workfront para calcular a disponibilidade dos usuários quando o administrador do Workfront seleciona A programação padrão nas Preferências de gerenciamento de recursos. Com a nova atualização, o Workfront usa a seguinte fórmula para calcular a disponibilidade do usuário:

Horas Disponíveis do Usuário = (Horas Programadas Padrão - Exceções) &#42; FTE - Tempo livre (horas)

Antes dessa atualização, o Workfront usava a seguinte fórmula para calcular a disponibilidade do usuário quando o Agendamento padrão era selecionado:

Horas Disponíveis do Usuário = (Horas Programadas Padrão - (Exceções Programadas + Horas de folga)) &#42; Valor FTE do usuário

Para obter mais informações, consulte [Configurar preferências de gerenciamento de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

