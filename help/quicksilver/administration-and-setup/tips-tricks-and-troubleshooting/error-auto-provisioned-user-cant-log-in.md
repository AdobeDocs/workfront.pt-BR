---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Erro: o usuário provisionado automaticamente não pode fazer logon"
description: Se um usuário provisionado automaticamente tentar fazer logon pela primeira vez e receber um erro informando que o sistema não está atribuindo a ele um nível de acesso, talvez isso ocorra porque seu sistema não tem níveis de acesso associados à licença de solicitação. O provisionamento automático usa o tipo de licença Solicitação, para que você possa corrigir esse problema criando um nível de acesso associado a uma licença Solicitação.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4c88933e-d3da-447e-ab6c-be9261a94a19
source-git-commit: 477f65efb09e8566dd0af88adfbe88135d6c6ae9
workflow-type: tm+mt
source-wordcount: '260'
ht-degree: 1%

---

# Erro: o usuário autoprovisionado não consegue fazer logon

Quando um usuário provisionado automaticamente tenta fazer logon pela primeira vez, ele recebe o seguinte erro:

`Expect one user but found 0. ${subdomain} ${lane} ${email}`

## Problema

O sistema não está atribuindo um nível de acesso ao novo usuário.

Por padrão, o provisionamento automático usa o tipo Solicitar licença. Quando não existem níveis de acesso com uma licença de solicitação, o sistema não pode atribuir um nível de acesso ao usuário.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plano</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p> <p><b>NOTA</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais no seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

Criar um nível de acesso básico com uma licença de Solicitação:

1. Ir para **[!UICONTROL Configuração]** > **[!UICONTROL Níveis de Acesso]**.

1. Clique em **[!UICONTROL Novo Nível de Acesso]**.
1. Insira um **[!UICONTROL Nome]**.
1. No **[!UICONTROL Tipo de licença]** selecione Solicitação.
1. Clique em **[!UICONTROL Salvar alterações]**.

Depois de criar um nível de acesso com uma licença de Solicitação, peça ao usuário para fazer logon com suas credenciais de SSO.


