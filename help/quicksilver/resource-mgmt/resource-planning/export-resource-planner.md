---
product-area: resource-management
navigation-topic: resource-planning
title: Exportar informações do Planejador de recursos
description: É possível exportar informações de qualquer exibição do Planejador de recursos para um arquivo do Excel (.xlsx) que esteja salvo no computador.
author: Alina
feature: Resource Management
exl-id: 07acd28a-5dc0-45b4-bdf2-20abbd5e098c
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '661'
ht-degree: 3%

---

# Exportar informações do Planejador de recursos

É possível exportar informações de qualquer exibição do Planejador de recursos para um arquivo do Excel (.xlsx) que esteja salvo no computador.

>[!IMPORTANT]
>
>Há limitações em quais informações são exibidas e quais informações você pode exportar do Planejador de recursos. Para obter informações sobre essas limitações, consulte [Limitações de exibição do Planejador de recursos](../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)

## Requisitos de acesso

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
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
   <td> <p>Acesso de visualização ou superior ao Gerenciamento de projetos, usuários e recursos</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões ou superiores para projetos</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Exportar informações do Planejador de recursos

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu principal**, no canto superior direito do Adobe Workfront.

1. Clique em **Recursos**. O **Planejador** é exibido por padrão.

1. Selecione a exibição do Planejador. Você pode selecionar uma das seguintes opções:

   * Visualizar por Usuário
   * Visualizar por Projeto
   * Visualizar por Função

1. Clique em **Exportar**.

   A caixa de diálogo Opções de exportação é exibida.

   ![](assets/rp-export-options-box-350x421.png)

1. Especifique as seguintes informações:\
   **Data de Início**: a data de início da sua exportação. O arquivo exportado contém informações de alocação e disponibilidade começando com o primeiro dia da semana que contém o dia especificado aqui.\
   **Número de Períodos**: o número de períodos que você deseja incluir no arquivo. O padrão é 4 períodos.\
   **Tipo**: o tipo de períodos de tempo pelos quais você deseja exibir as informações no arquivo exportado (semanas, meses ou trimestres).\
   A seguir estão os períodos máximos que você pode exportar:

   * 52 semanas
   * 36 meses
   * 12 trimestres

   **Selecionar para Exportar**: Dependendo do modo de exibição selecionado, você pode optar por exportar as informações de disponibilidade e orçamento de todos os objetos listados na tela ou de objetos específicos.
Você pode optar por exportar as seguintes informações:

   * Na Exibição do Projeto, selecione para exportar:

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

   **Formatação de Dados**: Dependendo de como você deseja que o arquivo do Excel seja exibido, selecione as seguintes opções:

   * **Raw**: selecione para exibir as informações de disponibilidade e alocação desagrupadas pelos objetos aos quais elas pertencem no arquivo do Excel. (esta é a opção padrão)
   * **Agrupado**: selecione para exibir as informações de disponibilidade e alocação agrupadas pelos objetos aos quais pertencem. Isso exibirá as informações exportadas da maneira que aparecem na tela.

   Um exemplo de como as informações são exibidas no arquivo exportado é mostrado na caixa de diálogo Opções de exportação.

1. Clique em **Exportar** para exportar as informações do Planejador de recursos.\
   Somente as informações salvas são exportadas.

1. (Condicional) Se você tem Horas orçadas não salvas nas exibições Função ou Projeto, clique em **Salvar e continuar.**
Um arquivo do Excel (.xlsx) é baixado no computador.\
   A exportação do Planejador de recursos não está disponível enquanto o arquivo está preparado para download.\
   (Condicional) Se exportar uma grande quantidade de dados, você receberá um email com um link para baixar o arquivo.\
   ![RP_email_with_exports_planner_attached.png](assets/rp-eamil-with-exported-planner-attached-350x116.png)

1. (Condicional) Ao receber o email com o arquivo exportado, clique em **Baixar** para baixar o arquivo.\
   Isso leva você de volta à Workfront, onde é possível baixar o arquivo.\
   Você deve estar conectado ao Workfront para que o download seja concluído.\
   Se você não baixar o arquivo quando ele for entregue, o link Download permanecerá ativo por 7 dias após você iniciar a exportação.
