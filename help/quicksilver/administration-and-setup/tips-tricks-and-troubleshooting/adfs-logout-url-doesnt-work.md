---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: O URL de Logout do ADFS não Funciona
description: O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas à Adobe Admin Console.
author: Becky, Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: fb555df123701c62e9a0f2d451ad6dcd16586595
workflow-type: tm+mt
source-wordcount: '217'
ht-degree: 1%

---

# O URL de logout do ADFS não funciona

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>O procedimento descrito nesta página aplica-se apenas a organizações que ainda não foram integradas ao [!UICONTROL Adobe Admin Console].
>
>Se sua organização foi integrada ao [!UICONTROL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Ao usar o URL de logout do ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), você recebe uma página de mensagem com o erro: &quot;Houve um problema ao acessar o site. Tente navegar até o site novamente.&quot;

Se o problema persistir, contate o administrador deste site e forneça o seguinte número de referência para identificar o problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote [!DNL Workfront] do Adobe</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe [!DNL Workfront]</td> 
   <td>
   <p>Standard</p>
   <p>Plano</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>[!UICONTROL Administrador do Sistema]</td>  
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solução

1. No servidor do gerenciador ADFS, vá para **[!UICONTROL Relações de Confiança]** > **[!UICONTROL Relações de Confiança de Terceira Parte Confiável]** > `<your party trust>` propriedades.

1. Na guia **[!UICONTROL Pontos de extremidade]**, clique em **[!UICONTROL Adicionar]**.

1. **[!UICONTROL Tipo de Ponto de Extremidade]** = SAML Logout, Associação = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Você pode definir um URL de resposta se quiser redirecioná-lo para outra página. Mas recomendamos o site do ADFS porque ele avisa que você está desconectado, mas ainda deve fechar o navegador.
