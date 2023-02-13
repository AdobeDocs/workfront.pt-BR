---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erro: O usuário provisionado automaticamente não pode fazer logon"
description: Se um usuário provisionado automaticamente tentar fazer logon pela primeira vez e receber um erro informando que o sistema não está atribuindo a ele um nível de acesso, isso pode ocorrer porque o sistema não tem níveis de acesso associados à licença de solicitação. O provisionamento automático usa o tipo de licença Solicitar , para que você possa corrigir esse problema criando um nível de acesso associado a uma licença Solicitar .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Erro: O usuário provisionado automaticamente não pode fazer logon

Quando um usuário provisionado automaticamente tenta fazer logon pela primeira vez, ele recebe o seguinte erro:

## Problema

O sistema não está atribuindo ao novo usuário um nível de acesso.

Por padrão, o provisionamento automático usa o tipo de licença Solicitar . Quando não existem níveis de acesso com uma licença de Solicitação, o sistema não pode atribuir um nível de acesso ao usuário.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

Crie um nível de acesso básico com uma licença de Solicitação:

1. Ir para **[!UICONTROL Configuração]** > **[!UICONTROL Níveis de acesso]**.

1. Clique em **[!UICONTROL Novo nível de acesso]**.
1. Insira um **[!UICONTROL Nome]**.
1. No **[!UICONTROL Tipo de licença]** selecione Solicitação no menu suspenso.
1. Clique em **[!UICONTROL Salvar alterações]**.

Depois de criar um nível de acesso com uma licença de Solicitação, faça com que o usuário faça logon com suas credenciais de SSO.
