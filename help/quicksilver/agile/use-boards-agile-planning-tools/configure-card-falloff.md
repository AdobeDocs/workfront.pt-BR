---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Configurar queda de cartão
description: Você pode configurar uma placa para que as placas sejam arquivadas, ou cair da placa, de acordo com uma programação.
author: Courtney
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/iSsqfrcgbod28qez5XkHDP-nDSQO-UKDGm13zPeeBZ0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 228
ht-degree: 17%

---

# Configurar atenuação dos cartões

Você pode configurar uma placa para que as placas sejam arquivadas, ou &quot;cair&quot; da placa, de acordo com uma programação. Você pode definir cartões em uma coluna específica para cair do quadro em um determinado número de dias ou semanas.

Quando um cartão cai da placa, ele é arquivado. Você pode exibir cartões arquivados com um filtro. Para obter mais informações, consulte [Filtrar e pesquisar em um quadro](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou posterior</p> 
   <p>Solicitação ou posterior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar atenuação dos cartões

{{step1-to-boards}}

1. Acessar um quadro. Para obter informações, consulte [Criar ou editar um quadro](../../agile/get-started-with-boards/create-edit-board.md).
1. Clique em **[!UICONTROL Configurar]** à direita do quadro para abrir o painel Configurar.
1. Expanda **[!UICONTROL Cartões]**.
1. Ative o **[!UICONTROL Arquivar automaticamente cartões do quadro]**.

   ![Configurações de fallout do cartão](assets/card-falloff-switch.png)

1. Selecione quando arquivar cartões do quadro. Você pode escolher até 8 semanas ou até 60 dias.

   A data é determinada a partir de quando o cartão foi modificado pela última vez.

1. Selecione de qual coluna remover cartões.
1. Clique em **[!UICONTROL Salvar]** na mensagem de confirmação.
1. Clique em **[!UICONTROL Ocultar configuração]** para fechar o painel [!UICONTROL Configurar]. As definições de configuração são aplicadas automaticamente quando você atualiza a placa.
