---
filename: configure-card-falloff.md
content-type: reference
navigation-topic: boards
title: Configurar queda de cartão
description: Você pode configurar uma placa para que as placas sejam arquivadas, ou cair da placa, de acordo com uma programação.
author: Lisa
feature: Agile
exl-id: 0e4f6b3c-75aa-4314-9cb0-737e5a9d3bda
source-git-commit: df4c2a73b5eb2498564bbf27aa92a297388562cd
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%

---

# Configurar queda de cartão

Você pode configurar uma placa para que as placas sejam arquivadas, ou &quot;cair&quot; da placa, de acordo com uma programação. Você pode definir cartões em uma coluna específica para cair do quadro em um determinado número de dias ou semanas.

Quando um cartão cai da placa, ele é arquivado. Você pode exibir cartões arquivados com um filtro. Para obter mais informações, consulte [Filtrar e pesquisar em um quadro](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td> 
   <p>Novo: [!UICONTROL Contributor] ou superior</p> 
   <p>ou</p>
   <p>Atual: [!UICONTROL Request] ou superior</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar queda de cartão

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
