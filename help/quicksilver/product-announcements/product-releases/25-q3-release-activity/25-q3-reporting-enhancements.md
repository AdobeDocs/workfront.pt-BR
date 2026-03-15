---
title: Melhorias nos relatórios do terceiro trimestre de 2025
description: Melhorias no projeto do terceiro trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 5%

---

# Melhorias nos relatórios do terceiro trimestre de 2025

Esta página descreve todos os aprimoramentos de relatórios feitos com a versão do terceiro trimestre de 2025 para o ambiente de Visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste ponto do ciclo de lançamento do terceiro trimestre de 2025, consulte [Visão geral da versão do terceiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Segurança de entrega de relatório aprimorada

* Visualização: 26 de junho de 2025
* Produção: implantação em fases de 26 de junho de 2025 a 9 de julho de 2025

Aprimoramos a entrega agendada de relatórios para garantir que as notificações do Workfront sejam enviadas apenas para domínios de email aprovados na lista de permissões.

Anteriormente, se sua organização tivesse definido uma limitação em quais domínios de email as notificações da Workfront, executaríamos uma verificação em relação à lista de permissões à medida que os emails fossem adicionados.

Agora, também executamos uma verificação à medida que o email é enviado para garantir que o endereço de email inserido esteja em conformidade com a lista de permissões de email. Essa verificação aprimorada se aplica a endereços de email associados a usuários e emails ad hoc adicionados à lista de destinatários do relatório.

Para obter mais informações, consulte [Agendar a entrega automática de um relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## Os curingas do usuário não retornam mais resultados com um valor nulo durante a filtragem

>[!NOTE]
>
>* Visualização: 30 de abril de 2025
>* Versão rápida de produção: sexta-feira, 15 de maio de 2025
>* Produção para todos os clientes: 17 de julho de 2025

Atualizamos o comportamento do curinga do usuário para excluir um valor nulo ao filtrar um relatório. Essa alteração ajuda o filtro a produzir resultados mais precisos, em vez de retornar resultados que não tenham um usuário configurado corretamente (um resultado nulo).

Anteriormente, quando um curinga do usuário produzia um valor nulo, um relatório exibia todos os registros que também tinham um valor nulo.

Essa alteração se aplica aos seguintes filtros curinga:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
