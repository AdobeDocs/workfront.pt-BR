---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Enviar um relatório no ambiente de sandbox de visualização
description: As informações nesta página se referem à funcionalidade disponível apenas nos ambientes Preview e Custom Refresh Sandbox. Essa funcionalidade não está disponível no ambiente de Produção.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Enviar um relatório no ambiente de sandbox de visualização

As informações nesta página se referem à funcionalidade disponível apenas nos ambientes Preview e Custom Refresh Sandbox. Essa funcionalidade não está disponível no ambiente de Produção.

Você pode configurar as opções de Entrega de relatório em qualquer ambiente de teste do Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Embora os ambientes de teste devam funcionar o mais próximo possível do ambiente de produção, algumas funcionalidades diferem do ambiente de produção.

Você pode agendar relatórios nos ambientes de teste, mas a maneira como eles são entregues difere de como são entregues no ambiente de Produção.

Para obter informações sobre como programar relatórios para entrega no ambiente Produção, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Dependendo de onde você agenda os relatórios, a funcionalidade de entrega difere entre as sandboxes de Visualização e Atualização personalizada.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Agendar relatórios no ambiente de Visualização

* [Agendar relatórios no ambiente de Visualização](#schedule-reports-in-the-preview-environment)

### Agendar relatórios no ambiente de Visualização

Se um relatório entregue é produzido ou não no ambiente de Visualização depende de **Receber emails deste ambiente de teste** está ativado ou não.

Para obter informações sobre como ativar emails do ambiente de sandbox, consulte [Ativar a entrega de emails do ambiente Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

O agendamento de relatórios para entrega no ambiente de Pré-visualização é idêntico ao agendamento de relatórios no ambiente de Produção. Para obter informações sobre como programar um relatório para entrega, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Quando você agenda um relatório para entrega no ambiente de Visualização, os seguintes cenários existem:

* When **Receber emails deste ambiente de teste** estiver desabilitado para o usuário que está recebendo o relatório, nenhum arquivo será produzido durante a programação do relatório para entrega.
* When **Receber emails deste ambiente de teste** estiver habilitado para o usuário que está recebendo o relatório, o arquivo produzido durante a programação do relatório para entrega será adicionado na guia Documents do usuário.

## Agendar relatórios no ambiente Sandbox de atualização personalizada

Se um relatório entregue é produzido ou não no Sandbox de atualização personalizada depende de a configuração Receber emails desse ambiente de teste estar ativada ou não.

Para obter informações sobre como ativar emails do ambiente de Visualização, consulte a seção [Exibir e modificar as configurações de notificação por email](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) no artigo [Ativar ou desativar suas próprias notificações de evento](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

O agendamento de relatórios para entrega no ambiente de sandbox de atualização personalizada é idêntico ao agendamento de relatórios no ambiente de Produção. Para obter informações sobre como programar um relatório para entrega, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Quando você agenda um relatório para entrega no ambiente Sandbox de atualização personalizada, os seguintes cenários existem:

* Quando o recurso Receber emails desse ambiente de teste está desativado para o usuário que recebe o relatório, nenhum arquivo é produzido durante a programação do relatório para entrega.
* Quando a opção Receber emails desse ambiente de teste estiver ativada para o usuário que está recebendo o relatório, o relatório será enviado por email como anexo ao endereço de email associado ao usuário.

## Como os usuários externos são notificados

Usuários externos não recebem relatórios enviados dos ambientes de teste do Workfront, nem recebem uma notificação por email.

Usuários externos só recebem relatórios por email se forem entregues a partir de um ambiente de Produção.
