---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensagem de erro: Falha na autenticação do SAML 2.0: Identificador de usuário não encontrado'
description: Quando estiver usando o SAML 2.0, o erro "Identificador de usuário com falha de autenticação SAML 2.0 não encontrado" significa que uma ID de UID ou de NOME não é passada pelas regras de solicitação ADFS. No ADFS, a Confiança da terceira parte confiável precisa ter uma regra de Reivindicação que transmita um UID ou um valor de ID de NOME. Ao executar um [!DNL Workfront] Testar conexão, ela deve mostrar isso se bem-sucedida.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '292'
ht-degree: 1%

---

# Mensagem de erro: Falha na autenticação do SAML 2.0: Identificador de usuário não encontrado

## Problema

Estou recebendo este erro ao usar o SAML 2.0: &quot;Falha na autenticação do SAML 2.0: Identificador de usuário não encontrado.&quot;

## Causa

Isso acontece quando uma **UID** ou **ID DE NOME** não é passado do **Regras de Declaração ADFS**.

No ADFS, a variável **Confiança da Entidade Confiadora** precisa ter uma **Regra de solicitação** que passa por uma **UID** ou **ID DE NOME** valor. Ao executar um **[!DNL Workfront]Testar conexão**, isso deve mostrar se bem-sucedido.

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

1. Ao editar o **[!UICONTROL INFORMAÇÕES DO ADFS]** no **[!UICONTROL Confianças de terceiros confiáveis]** > Selecionar objeto >**[!UICONTROL Editar regras de solicitação]**.

1. O **[!UICONTROL Atributo LDAP]** (coluna à esquerda) deve ter **[!UICONTROL Endereços de email]** (ou qualquer identificador exclusivo).

1. O **[!UICONTROL Tipo de Declaração de Saída]** (coluna à direita) deve ser **[!UICONTROL ID do nome]**.

   >[!NOTE]
   >
   >Ele não precisa ter os endereços de email do atributo LDAP. Qualquer identificador exclusivo que identificará o usuário pode ser usado, mas deve ser passado para [!DNL Adobe Workfront] como **ID DE NOME**.
