---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: 'Mensagem de erro: Erro SAML 2.0: Identificador de usuário não encontrado'
description: Não é possível estabelecer uma conexão bem-sucedida com o ADFS.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c4c70532-de4f-4264-b661-2d30cefd403c
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 1%

---

# Mensagem de erro: Erro SAML 2.0: Identificador de usuário não encontrado

## Problema

Não é possível estabelecer uma conexão bem-sucedida com o ADFS.

![identifier_not_found.png](assets/identifier-not-found.png)

>[!NOTE]
>
>Se você estabelecer uma conexão de teste bem-sucedida e ainda tiver problemas, poderá ter mapeamentos de atributo incorretos ou problemas com as IDs de federação. Entre em contato com o suporte ao cliente com perguntas.

## Causa:

As afirmações no servidor ADFS estão incorretas

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

No servidor ADFS, verifique se há uma reivindicação para ID de nome:

1. No Windows, clique em **[!UICONTROL Iniciar]** > **[!UICONTROL Administração]** > **[!UICONTROL Gerenciamento ADFS 2.0]**.\
   A caixa de diálogo Gerenciamento do ADFS 2.0 é exibida.

1. Selecionar **[!UICONTROL Relação de Confiança]** > **[!UICONTROL Confianças de terceiros confiáveis]** no painel esquerdo.

1. Clique com o botão direito do mouse na confiança da terceira parte confiável relacionada ao Adobe Workfront e selecione **[!UICONTROL Editar regras de solicitação]**.
1. Verifique se a solicitação tem uma **[!UICONTROL Tipo de Declaração de Saída]** de **[!UICONTROL ID do nome]**.

![1.png](assets/1-350x287.png)
