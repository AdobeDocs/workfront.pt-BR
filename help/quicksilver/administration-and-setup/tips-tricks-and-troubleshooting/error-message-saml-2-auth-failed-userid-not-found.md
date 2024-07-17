---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensagem de erro: falha na autenticação do SAML 2.0: identificador de usuário não encontrado"
description: Quando você está usando o SAML 2.0, o erro "Falha na autenticação SAML 2.0 - Identificador de usuário não encontrado" significa que um UID ou ID NAME não é transmitido das regras de Declaração do ADFS. No ADFS, a Terceira Parte Confiável precisa ter uma regra de Declaração que passe um UID ou um valor de ID de NOME. Quando você executa uma  [!DNL Workfront] Conexão de Teste, ela deve mostrar isso se for bem-sucedida.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '298'
ht-degree: 0%

---

# Mensagem de erro: Falha na autenticação do SAML 2.0: identificador de usuário não encontrado

## Problema

Estou recebendo este erro ao usar o SAML 2.0: &quot;Falha na autenticação SAML 2.0: identificador de usuário não encontrado.&quot;

## Causa

Isso acontece quando uma **UID** ou **NAME ID** não é passada das **Regras de Declaração do ADFS**.

No ADFS, a **Terceira Parte Confiável** precisa ter uma **Regra de declaração** que passe um valor de **UID** ou **NAME ID**. Quando você executa uma **[!DNL Workfront]Conexão de Teste**, ela deve mostrar isso se for bem-sucedida.

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
   <td> <p>Você deve ser um administrador [!DNL Workfront]. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a um usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do [!DNL Workfront] se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do [!DNL Workfront] pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

1. Ao editar as **[!UICONTROL INFORMAÇÕES DO ADFS]**, em **[!UICONTROL Confiança da Terceira Parte Confiável]** > Selecionar objeto >**[!UICONTROL Editar Regras de Declaração]**.

1. O **[!UICONTROL Atributo LDAP]** (coluna à esquerda) deve ter **[!UICONTROL Endereços de Email]** (ou qualquer identificador exclusivo).

1. O **[!UICONTROL Tipo de Declaração de Saída]** (coluna da direita) deve ser **[!UICONTROL ID de Nome]**.

   >[!NOTE]
   >
   >Ele não precisa ter os endereços de e-mail do atributo LDAP. Qualquer identificador exclusivo que identificará o usuário pode ser usado, mas deve ser passado para [!DNL Adobe Workfront] como o **NAME ID**.
