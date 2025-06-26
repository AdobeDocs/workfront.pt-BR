---
title: Melhorias na emissão de relatórios no terceiro trimestre de 2025
description: Aprimoramentos no projeto do terceiro trimestre de 2025
author: Nolan
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
source-git-commit: a0a7ad2770b99ee1d45169372e64e460701ccc10
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

# Melhorias na emissão de relatórios no terceiro trimestre de 2025

Esta página descreve todas as melhorias de relatórios feitas com a versão do terceiro trimestre de 2025 para o ambiente de Pré-visualização. Esses aprimoramentos serão disponibilizados no ambiente de Produção, conforme observado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2025, consulte [Visão geral da versão do terceiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Segurança aprimorada na entrega de relatórios

* Visualização: 26 de junho de 2025
* Produção: implantação em fases de 26 de junho de 2025 a 9 de julho de 2025

Melhoramos a entrega agendada de relatórios para garantir que as notificações do Workfront sejam enviadas apenas para domínios de email aprovados no incluo na lista de permissões de pesquisa.

Anteriormente, se sua organização tivesse definido uma limitação em quais domínios de email as notificações do Workfront, executaríamos uma verificação em relação ao incluo na lista de permissões quando os emails fossem adicionados.

Agora, também realizamos uma verificação à medida que o email é enviado, para garantir que o endereço de email inserido esteja em conformidade com a inclui na lista de permissões de email. Essa verificação aprimorada se aplica a endereços de email associados a usuários e emails ad hoc adicionados à lista de recipients do relatório.

Para obter mais informações, consulte [Agendar uma entrega automática de relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).


## Os curingas do usuário não retornam mais resultados com um valor nulo durante a filtragem

>[!NOTE]
>
>* Visualização: 30 de abril de 2025
>* Versão rápida de produção: 15 de maio de 2025
>* Produção para todos os clientes: 17 de julho de 2025

Atualizamos o comportamento do curinga do usuário para excluir valor nulo ao filtrar um relatório. Essa alteração ajuda o filtro a produzir resultados mais precisos, em vez de retornar resultados que não têm um usuário configurado corretamente (um resultado nulo).

Anteriormente, quando um curinga do usuário produzia um valor nulo, um relatório exibia todos os registros que também tinham um valor nulo.

Essa alteração se aplica aos seguintes filtros curingas:

* `$$USER.homeTeamID`
* `$$USER.otherTeamIDs`
* `$$USER.roleID`
* `$$USER.roleIDs`
* `$$USER.companyID`
