---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Usar o relatório de aprovação de prova
description: Você pode usar o relatório de aprovação de prova para exibir informações sobre provas no seu ambiente.
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# Usar o relatório de aprovação de prova

Você pode usar o relatório de aprovação de prova para exibir informações sobre provas no seu ambiente.

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>plano do Workfront*</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Visão geral das licenças da Adobe Workfront*</p> </td> 
   <td> <p>Plano</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Nível de acesso*</strong> </td> 
   <td> <p>Editar acesso a:</p> 
    <ul> 
     <li> <p>Criar relatórios, painéis e calendários</p> </li> 
     <li> <p>Criar filtros, visualizações e agrupamentos</p> </li> 
    </ul> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Usar o relatório de aprovação de prova

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal** no canto superior direito do Adobe Workfront e em **Relatórios**.
1. Clique em **Novo relatório** e role para selecionar **Aprovação de prova**.

   ![](assets/proof-approval-report.png)

1. (Opcional) Adicione quaisquer campos adicionais.
1. Clique em **Salvar + Fechar**.

## Campos adicionais

Você pode adicionar os seguintes campos ao relatório de aprovação de prova:

* **Data da decisão**: exibe a data em que um aprovador toma uma decisão sobre uma prova. Você também pode encontrar essa data no Resumo de impressão da prova.
* **Estágio de Aprovador**: exibe as informações do estágio atual.
* **Modelo de fluxo de trabalho**: exibe todos os modelos de fluxo de trabalho anexados à prova. Se não houver um modelo anexado, a coluna ficará em branco.
* **Aguardando decisão**: exibe verdadeiro para sinalizar que uma decisão não foi atendida na versão mais recente quando os itens a seguir são verdadeiros:

   * A prova não foi arquivada
   * O estágio em que o aprovador está ativo
   * A prova está aguardando aprovação

* **Prazo da prova**: exibe o prazo da prova. Cada estágio deve ter um prazo atribuído para que esse campo seja preenchido. O campo exibe o prazo da etapa ativada mais recentemente.

 
