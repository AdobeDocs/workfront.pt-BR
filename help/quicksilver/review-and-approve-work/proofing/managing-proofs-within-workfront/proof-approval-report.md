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
   <td role="rowheader"> <p>Plano Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Visão geral das licenças do Adobe Workfront*</p> </td> 
   <td> <p>Plano</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Nível de acesso*</strong> </td> 
   <td> <p>Editar acesso a:</p> 
    <ul> 
     <li> <p>Criar relatórios, painéis e calendários</p> </li> 
     <li> <p>Criar filtros, visualizações e agrupamentos</p> </li> 
    </ul> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Usar o relatório de aprovação de prova

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Relatórios**.
1. Clique em **Novo relatório**, em seguida, role para selecionar **Aprovação de prova**.

   ![](assets/proof-approval-report.png)

1. (Opcional) Adicione quaisquer campos adicionais.
1. Clique em **Salvar + Fechar**.

## Campos adicionais

Você pode adicionar os seguintes campos ao relatório de aprovação de prova:

* **Data da decisão**: Exibe a data em que um aprovador toma uma decisão em uma prova. Também é possível encontrar essa data no Resumo de impressão da prova.
* **Estágio do Aprovador**: Exibe as informações do estágio atual.
* **Modelo de fluxo de trabalho**: Exibe qualquer modelo de workflow anexado à prova. Se não houver nenhum modelo anexado, a coluna ficará em branco.
* **Decisão de espera**: Exibe verdadeiro para sinalizar que uma decisão não foi cumprida na versão mais recente quando o seguinte é verdadeiro:

   * A prova não foi arquivada
   * O estágio em que o aprovador está ativo
   * A prova está pendente de aprovação

* **Prazo da prova**: Exibe o prazo da prova. Cada estágio deve ter um prazo atribuído para que esse campo seja preenchido. O campo exibe o prazo para o estágio ativado mais recentemente.

 
