---
filename: configure-backlog-workstream-board.md
content-type: reference
navigation-topic: boards
title: Configurar o backlog em uma placa de fluxo de trabalho
description: Você pode optar por exibir uma coluna de backlog em um quadro em um fluxo de trabalho e definir uma consulta para os cartões que são extraídos para o backlog do quadro na lista de cartões de fluxo de trabalho.
author: Lisa
exl-id: fd2f6eeb-a565-4461-a153-0504ad3c07d7
source-git-commit: 75bb5af9564947a39e1cb46f9d6be2c03eb07acc
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 0%

---

# Configurar o backlog em uma placa de fluxo de trabalho

Você pode optar por exibir uma coluna de backlog em um quadro em um fluxo de trabalho e definir uma consulta para os cartões que são extraídos para o backlog do quadro na lista de cartões de fluxo de trabalho. Essas opções não estão disponíveis em placas independentes. Para obter informações sobre como adicionar uma coluna de entrada a um quadro independente, consulte [Adicionar uma coluna de entrada a um quadro](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plano*</strong></td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licença*</strong></td> 
   <td> <p>[!UICONTROL Solicitação] ou superior</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com seu [!DNL Workfront] administrador.

## Configurar o backlog em uma placa de fluxo de trabalho

{{step1-to-boards}}

1. Abra a sequência de trabalho na qual deseja trabalhar. Para abrir um fluxo de trabalho, clique em [!UICONTROL **Exibir fluxo de trabalho**].
1. Clique em qualquer quadro na sequência de trabalho para abri-lo.
1. Clique em [!UICONTROL **Configurar**] à direita do quadro para abrir o painel Configurar .
1. Ligar [!UICONTROL **Incluir uma coluna de registro retroativo neste quadro**].

   A coluna de backlog é adicionada à esquerda do quadro. Permanece em branco até que você aplique uma consulta a ele.

1. Expandir [!UICONTROL **Consulta de backlog**].

   >[!NOTE]
   >
   >Uma consulta padrão pode já ser aplicada ao registro retroativo, mostrando todos os itens de trabalho da lista de cartões que não pertencem a uma iteração e que não estão no status Concluído.

1. Clique em [!UICONTROL **Adicionar condição**] e clique em no campo &quot;empty&quot; .
1. Selecione o campo para o qual consultar.

   Os campos que você pode escolher são os campos padrão em um cartão.

1. Selecione o modificador de consulta.

   As opções do modificador dependem dos campos aos quais podem ser aplicadas. Por exemplo, o campo &quot;name&quot; não tem &quot;greater than&quot; ou &quot;less than&quot; como opções do modificador, pois esses modificadores se aplicam apenas a números.

1. Selecione o valor .

   O valor não está disponível quando você usa &quot;existe&quot; ou &quot;não existe&quot; como o modificador.

   Por exemplo, se você escolher &quot;Data de vencimento&quot; e &quot;existe&quot;, o registro retroativo exibirá cartões com datas de vencimento atribuídas. Qualquer cartão sem data de vencimento não será recebido no backlog.

1. (Opcional) Clique em [!UICONTROL **Adicionar condição**] para adicionar outra condição ao query.

   ![Consulta de lista de pendências](assets/backlog-query-wrkstrm-board.png)

1. (Opcional) Clique em [!UICONTROL **Criar grupo**] para adicionar um grupo de condições conectadas à primeira condição com um operador OR.
1. Clique em [!UICONTROL **Salvar consulta**].

   A query é aplicada e os cartões que atendem aos critérios são exibidos na coluna de backlog.
