---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: O URL de logout do ADFS não funciona
description: O procedimento descrito nesta página se aplica somente a organizações que ainda não estão integradas à Adobe Admin Console.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 0%

---

# O URL de logout do ADFS não funciona

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente às organizações que ainda não estão integradas ao [!UICONTROL Adobe Admin Console].
>
>Se sua organização tiver sido integrada à [!UICONTROL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Ao usar o URL de logout do ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), você recebe uma página de mensagem com o erro: &quot;Ocorreu um problema ao acessar o site. Tente navegar para o site novamente.&quot;

Se o problema persistir, entre em contato com o administrador deste site e forneça o seguinte número de referência para identificar o problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licença</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Se ainda não tiver acesso, pergunte ao seu [!DNL Workfront] administrador se eles definirem restrições adicionais em seu nível de acesso. Para obter informações sobre como uma [!DNL Workfront] administrador pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Solução

1. No servidor do ADFS Manager, acesse **[!UICONTROL Relacionamentos de Confiança]** > **[!UICONTROL Confianças de terceiros confiáveis]** > `<your party trust>` propriedades.

1. Em **[!UICONTROL Endpoints]** clique em **[!UICONTROL Adicionar]**.

1. **[!UICONTROL Tipo de Ponto Final]** = Logout SAML, Vínculo = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Você pode definir um URL de resposta se quiser que ele seja redirecionado para outra página. Mas recomendamos o site ADFS porque ele avisa que você está desconectado, mas você ainda deve fechar seu navegador.
