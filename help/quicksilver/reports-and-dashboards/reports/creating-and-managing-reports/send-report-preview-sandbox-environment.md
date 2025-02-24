---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Enviar um relatório no ambiente Visualização da sandbox
description: As informações nesta página se referem à funcionalidade disponível apenas nos ambientes Pré-visualização e Atualização personalizada da sandbox. Essa funcionalidade não está disponível no ambiente de Produção do.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 0%

---

# Enviar um relatório no ambiente Visualização da sandbox

<!-- Audited: 11/2024 -->

As informações nesta página se referem à funcionalidade disponível apenas nos ambientes Pré-visualização e Atualização personalizada da sandbox. Essa funcionalidade não está disponível no ambiente de Produção do.

Você pode configurar as opções de Entrega de relatórios em qualquer ambiente de teste do Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Embora os ambientes de teste devam funcionar o mais próximo possível de seu ambiente de produção, algumas funcionalidades diferem do ambiente de produção.

Você pode agendar relatórios nos ambientes de teste, mas a maneira como eles são entregues difere de como eles são entregues do ambiente de produção.

Para obter informações sobre como agendar relatórios para entrega no ambiente de Produção, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Dependendo de onde você agendar os relatórios, a funcionalidade do delivery será diferente entre as sandboxes Pré-visualização e Atualização personalizada.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
      <td> 
      <p>Novo:</p>
         <ul>
         <li><p>Padrão</p></li>
         </ul>
      <p>Atual:</p>
         <ul>
         <li><p>Plano</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agendar relatórios no ambiente de Pré-visualização

* [Agendar relatórios no ambiente de Pré-visualização](#schedule-reports-in-the-preview-environment)

### Agendar relatórios no ambiente de Pré-visualização

Se um relatório entregue é produzido ou não no ambiente de Pré-visualização depende se **Receber emails deste ambiente de teste** está habilitado ou não.

Para obter informações sobre como habilitar emails do ambiente de sandbox, consulte [Habilitar a entrega de emails do ambiente de sandbox de visualização](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![Receber emails da opção de sandbox](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

O agendamento de relatórios para entrega no ambiente de Pré-visualização é idêntico ao agendamento de relatórios no ambiente de Produção. Para obter informações sobre como agendar um relatório para entrega, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Quando você agenda um relatório para entrega no ambiente de Pré-visualização, os seguintes cenários existem:

* Quando **Receber emails deste ambiente de teste** está desabilitado para o usuário que está recebendo o relatório, nenhum arquivo é produzido ao agendar o relatório para entrega.
* Quando **Receber emails deste ambiente de teste** está habilitado para o usuário que está recebendo o relatório, o arquivo produzido ao agendar o relatório para entrega é adicionado na guia Documentos do usuário.

## Agendar relatórios no ambiente de sandbox de atualização personalizada

Se um relatório entregue é produzido ou não na sandbox de atualização personalizada depende se a configuração Receber emails dessa configuração de ambiente de teste está ativada ou não.

Para obter informações sobre como habilitar emails do ambiente de Visualização, consulte a seção [Exibir e modificar configurações de notificação por email](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) no artigo [Modificar suas próprias notificações por email](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![Receber emails da opção de sandbox](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

O agendamento de relatórios para entrega no ambiente Personalizado de atualização da sandbox é idêntico ao agendamento de relatórios no ambiente de Produção. Para obter informações sobre como agendar um relatório para entrega, consulte [Visão geral da entrega de relatórios](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Ao agendar um relatório para entrega no ambiente Personalizado de atualização da sandbox, existem os seguintes cenários:

* Quando a opção Receber emails desse ambiente de teste estiver desativada para o usuário que está recebendo o relatório, nenhum arquivo será produzido ao agendar o relatório para entrega.
* Quando a opção Receber emails desse ambiente de teste estiver ativada para o usuário que está recebendo o relatório, ele será enviado por email como um anexo ao endereço de email associado ao usuário.

## Como os usuários externos são notificados

Os usuários externos não recebem relatórios enviados dos ambientes de teste do Workfront, nem recebem uma notificação por email.

Os usuários externos só receberão relatórios por email se forem entregues de um ambiente de Produção.
