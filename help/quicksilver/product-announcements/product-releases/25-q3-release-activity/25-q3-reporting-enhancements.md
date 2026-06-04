---
title: Melhorias na emissão de relatórios no terceiro trimestre de 2025
description: Aprimoramentos no projeto do terceiro trimestre de 2025
author: Courtney
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 6e53dca8-285a-471b-a646-1773722554f3
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/XN5rfSeje0azVxpC4uBSDn5mg2C9Oyik2awD5pQy3Jo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 282
ht-degree: 4%

---

# Melhorias na emissão de relatórios no terceiro trimestre de 2025

Esta página descreve todas as melhorias de relatórios feitas com a versão do terceiro trimestre de 2025 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento no ciclo de lançamento do terceiro trimestre de 2025, consulte [Visão geral da versão do terceiro trimestre de 2025](/help/quicksilver/product-announcements/product-releases/25-q3-release-activity/25-q3-release-overview.md).

## Segurança aprimorada na entrega de relatórios

* Visualização: 26 de junho de 2025
* Produção: implantação em fases de 26 de junho de 2025 a 9 de julho de 2025

Aprimoramos a entrega agendada de relatórios para garantir que as notificações do Workfront sejam enviadas apenas a domínios de email aprovados no incluo na lista de permissões.

Anteriormente, se sua organização tivesse definido uma limitação em quais domínios de email as notificações do Workfront, executaríamos uma verificação em relação ao incluo na lista de permissões quando os emails fossem adicionados.

Agora, também realizamos uma verificação à medida que o email é enviado, para garantir que o endereço de email inserido esteja em conformidade com o incluo na lista de permissões de email. Essa verificação aprimorada se aplica a endereços de email associados a usuários e emails ad hoc adicionados à lista de recipients do relatório.

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
