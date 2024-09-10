---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: "Mensagem de erro: falha na autenticação do SAML 2.0: identificador de usuário não encontrado"
description: Quando você está usando o SAML 2.0, o erro "Falha na autenticação SAML 2.0 - Identificador de usuário não encontrado" significa que uma UID ou ID NAME não é transmitida das regras de Declaração do ADFS.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 9467cdff-7965-49ba-ac13-ed79c496a725
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Mensagem de erro: Falha na autenticação do SAML 2.0: identificador de usuário não encontrado

## Problema

Estou recebendo este erro ao usar o SAML 2.0: &quot;Falha na autenticação SAML 2.0: identificador de usuário não encontrado.&quot;

## Causa

Isso acontece quando uma **UID** ou **NAME ID** não é passada das **Regras de Declaração do ADFS**.

No ADFS, a **Terceira Parte Confiável** precisa ter uma **Regra de declaração** que passe um valor de **UID** ou de **NAME ID**. Quando você executa uma **[!DNL Workfront]Conexão de Teste**, ela deve mostrar isso se for bem-sucedida.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

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
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solução

1. Ao editar as **[!UICONTROL INFORMAÇÕES DO ADFS]**, em **[!UICONTROL Confiança da Terceira Parte Confiável]** > Selecionar objeto >**[!UICONTROL Editar Regras de Declaração]**.

1. O **[!UICONTROL Atributo LDAP]** (coluna à esquerda) deve ter **[!UICONTROL Endereços de Email]** (ou qualquer identificador exclusivo).

1. O **[!UICONTROL Tipo de Declaração de Saída]** (coluna da direita) deve ser **[!UICONTROL ID de Nome]**.

   >[!NOTE]
   >
   >Ele não precisa ter os endereços de e-mail do atributo LDAP. Qualquer identificador exclusivo que identificará o usuário pode ser usado, mas deve ser passado para [!DNL Adobe Workfront] como o **NAME ID**.
