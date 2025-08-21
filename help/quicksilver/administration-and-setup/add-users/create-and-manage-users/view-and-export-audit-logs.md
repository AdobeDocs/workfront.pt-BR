---
title: Visualizar e exportar logs de auditoria
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Você pode exibir todos os logs de auditoria no sistema ou aqueles que atendem a determinados critérios de filtragem. Você também pode exportar logs de auditoria. Os logs de auditoria listam as alterações de usuário acionadas no sistema durante os últimos 90 dias.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b04e8ba5-c3f2-4838-8df1-35e90de5c7bd
source-git-commit: 4569b5bd004a93396257f3f1f8964831f69399dc
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 1%

---

# Exibir e exportar logs de auditoria

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **
-->

Você pode exibir todos os logs de auditoria no sistema ou aqueles que atendem a determinados critérios de filtragem. Você também pode exportar logs de auditoria para um arquivo CSV.

Os logs de auditoria listam as alterações de usuário acionadas no sistema durante os últimos 90 dias.

Para obter informações sobre todos os tipos de log de auditoria e o que os gera, consulte [Logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p>
       <p>Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td><p>Administrador de Sistema</p></td>
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Exibir logs de auditoria

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema > Logs de auditoria**.
1. No menu suspenso **Tipo de ação**, selecione o tipo de auditoria que deseja exibir.

   >[!NOTE]
   >
   >As opções no menu suspenso Tipo de ação variam de acordo com o log de auditoria selecionado.

1. No menu suspenso **Tipo de Log**, selecione o tipo de log de auditoria que deseja exibir.

   **Todos os Tipos de Log** está selecionado por padrão.

   Para obter uma lista de todos os tipos de log de auditoria que você pode exibir e as informações que eles incluem, consulte [Logs de auditoria](../../../administration-and-setup/add-users/create-and-manage-users/audit-logs.md).

1. (Opcional) Defina qualquer um dos filtros disponíveis para os seguintes campos:

   * **Usuários**: digite o nome do usuário que fez uma alteração.
   * **De**: Data inicial do período em que a alteração foi feita.
   * **Até**: Data final do período de tempo em que a alteração foi feita.

   ![Logs de auditoria](assets/audit-logs.png)

1. Clique em **Aplicar**.
1. (Opcional) Clique em **Limpar** para redefinir as alterações feitas nos filtros.

## Exportar logs de auditoria

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Sistema** > **Logs de auditoria**.

1. No menu suspenso **Tipo de Log**, selecione um log de auditoria.

   **Todos os Tipos de Log** está selecionado por padrão.

1. Defina qualquer um dos filtros disponíveis e clique em **Aplicar**.

   >[!IMPORTANT]
   >
   >Você não pode exportar mais de 50.000 logs de uma só vez. O Workfront exporta logs com base nos filtros definidos, não no número de logs exibidos na página. Você pode visualizar o número total de logs filtrados no canto inferior direito da página.

1. Clique em **Exportar**.

   A caixa Salvar arquivo é aberta e você pode salvar o arquivo exportado em seu computador.

   Você pode salvar os logs de auditoria somente em um formato CSV.

   Termine de salvar o arquivo exportado. Agora você pode encontrá-lo em seu computador e compartilhá-lo com outras pessoas.
