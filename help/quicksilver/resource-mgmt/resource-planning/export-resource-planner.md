---
product-area: resource-management
navigation-topic: resource-planning
title: Exportar informações do Planejador de Recursos
description: Você pode exportar informações de qualquer exibição do Planejador de Recursos para um arquivo Excel (.xlsx) que é salvo em seu computador.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# Exportar informações do Planejador de Recursos

Você pode exportar informações de qualquer exibição do Planejador de Recursos para um arquivo Excel (.xlsx) que é salvo em seu computador.

>[!IMPORTANT]
>
>Há limitações nas informações exibidas e nas informações que podem ser exportadas do Planejador de Recursos. Para obter informações sobre essas limitações, consulte [Limitações de exibição do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Pro e superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Revisar ou superior <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Visualizar ou obter mais acesso a Projetos, Usuários e Gerenciamento de Recursos</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superior para projetos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exportar informações do Planejador de Recursos

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**. O **Planejador** é exibido por padrão.

1. Selecione a exibição do Planejador. Você pode selecionar uma das seguintes opções:

   * Visualizar por Usuário
   * Visualizar por Projeto
   * Visualizar por Função

1. Clique em **Exportar**.

   A caixa de diálogo Opções de exportação é exibida.

   ![](assets/rp-export-options-box-350x421.png)

1. Especifique as seguintes informações:\
   **Data inicial**: A data de início da exportação. O arquivo exportado contém informações de alocação e disponibilidade começando com o primeiro dia da semana que contém o dia especificado aqui.\
   **Número de Períodos**: O número de períodos que você deseja incluir no arquivo. O padrão é 4 períodos.\
   **Tipo**: O tipo de período durante o qual você deseja exibir as informações no arquivo exportado (semanas, meses ou trimestres).\
   A seguir estão os períodos máximos que você pode exportar:

   * 52 semanas
   * 36 meses
   * 12 trimestres

   **Selecionar para exportar**: Dependendo de qual exibição tiver selecionado, você poderá optar por exportar as informações de disponibilidade e orçamento para todos os objetos listados na tela ou para objetos específicos.
Você pode optar por exportar as seguintes informações:

   * Na Exibição do projeto, selecione para exportar:

      * Projetos
      * Projetos e funções
      * Tudo (esta é a opção padrão)
   * Na Exibição de usuário, selecione para exportar:

      * Usuários
      * Usuários e projetos
      * Tudo (esta é a opção padrão)
   * Na Exibição de função, selecione para exportar:

      * Funções
      * Funções e projetos
      * Tudo (esta é a opção padrão)

   **Formatação de dados**: Dependendo de como você deseja que o arquivo Excel seja exibido, selecione as seguintes opções:

   * **Bruto**: Selecione para exibir as informações de disponibilidade e alocação desagrupadas pelos objetos aos quais pertence no arquivo Excel. (esta é a opção padrão)
   * **Agrupado**: Selecione para exibir as informações de disponibilidade e alocação agrupadas pelos objetos aos quais pertence. Isso exibe as informações exportadas conforme elas são exibidas na tela.

   Uma amostra de como as informações aparecem no arquivo exportado é mostrada na caixa de diálogo Opções de exportação .

1. Clique em **Exportar** para exportar as informações do Planejador de Recursos.\
   Somente as informações salvas são exportadas.

1. (Condicional) Se você tiver Horas Orçadas não salvas nas exibições Função ou Projeto , clique em **Salve e continue.**
Um arquivo Excel (.xlsx) é baixado no computador.
\
   A exportação do Planejador de Recursos não está disponível enquanto o arquivo está preparado para download.\
   (Condicional) Se exportar uma grande quantidade de dados, você receberá um email com um link onde poderá baixar o arquivo.\
   ![RP_email_com_exportado_planejador_anexado.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Condicional) Ao receber o email com o arquivo exportado, clique em **Baixar** para baixar o arquivo.\
   Isso leva você de volta à Workfront, onde é possível baixar o arquivo.\
   Você deve estar conectado ao Workfront para que o download seja concluído.\
   Se você não baixar o arquivo quando ele for entregue, o link Download permanecerá ativo por 7 dias após iniciar a exportação.
