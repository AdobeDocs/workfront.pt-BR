---
title: Aprimoramentos no gerenciamento de recursos na 22.2
description: Aprimoramentos no gerenciamento de recursos na 22.2
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 5f11c43c-3aa8-4135-b6bf-07b9993e63d9
TQID: https://experienceleague.adobe.com/X2dBmB8Qyiwg9hM60af6GRBDGT4KkH6Jjs2A-S-TWVg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: c33d85a1-be85-4290-854c-87408c10aa80
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 376
ht-degree: 5%

---

# Aprimoramentos no gerenciamento de recursos na 22.2

Esta página descreve todas as melhorias no Gerenciamento de recursos feitas com a versão 22.2 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de produção

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
in January 2022
</MadCap:conditionalText>
-->

a semana de 4 de abril de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.2, consulte a [Visão geral da versão 22.2](../../../product-announcements/product-releases/22.2-release-activity/22-2-release-overview.md).

## Melhorias na navegação do Balanceador de carga de trabalho

Para melhorar sua experiência ao usar o Balanceador de carga de trabalho, introduzimos os seguintes aprimoramentos:

* Os botões Cancelar e Salvar ao ajustar alocações agora são fixos, mesmo quando a tarefa é mais longa do que o período incluído na tela ou quando o painel Resumo é exibido.
* O painel esquerdo que exibe os nomes de usuários e itens de trabalho agora é fixo, para permitir rolar horizontalmente por períodos mais longos e ainda poder ler os nomes dos itens listados no painel.
* Você pode recolher e expandir todos os itens listados no painel esquerdo com um clique em vez de no nível do usuário ou do projeto.
* Agora, o painel esquerdo também pode ser redimensionado.
* Agora há um modo de tela cheia para o Balanceador de carga de trabalho.

Para obter mais informações sobre como navegar no Balanceador de carga de trabalho, consulte [Navegar no Balanceador de carga de trabalho](../../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Acessar atribuições avançadas no Balanceador de carga de trabalho

Para tornar a atribuição de itens de trabalho mais fácil e precisa, agora é possível fazer atribuições avançadas ao atribuir itens de trabalho manualmente no Balanceador de carga de trabalho. Antes desse aprimoramento, você poderia acessar as Atribuições avançadas ao editar itens, nos cabeçalhos dos itens ou em listas.

Para obter mais informações, consulte [Atribuir trabalho manualmente usando o Balanceador de Carga de Trabalho](../../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-manually.md).

## Nova fórmula para calcular a disponibilidade do usuário quando a preferência Agendamento padrão é selecionada

Para fornecer informações mais precisas nas ferramentas de gerenciamento de recursos, alteramos a fórmula usada pelo Workfront para calcular a disponibilidade dos usuários quando o administrador do Workfront seleciona A programação padrão nas Preferências de gerenciamento de recursos. Com a nova atualização, o Workfront usa a seguinte fórmula para calcular a disponibilidade do usuário:

Horas Disponíveis do Usuário = (Horas Programadas Padrão - Exceções) &#42; FTE - Horas de folga

Antes dessa atualização, o Workfront usava a seguinte fórmula para calcular a disponibilidade do usuário quando o Agendamento padrão era selecionado:

Horas Disponíveis do Usuário = (Horas Programadas Padrão - (Exceções de Programação + Horas de folga)) &#42; Valor FTE do Usuário

Para obter mais informações, consulte [Configurar preferências de gerenciamento de recursos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

