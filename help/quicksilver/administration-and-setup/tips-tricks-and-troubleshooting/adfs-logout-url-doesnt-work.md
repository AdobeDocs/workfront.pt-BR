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
TQID: https://experienceleague.adobe.com/RRaLL70JcSBcvoS6EUFuWj5Ejwljekt4QuQ3kXDx-44
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 250
ht-degree: 13%

---

# O URL de logout do ADFS não funciona

<!-- Audited: 1/2024 -->

<!--Remove me October 2026-->

>[!IMPORTANT]
>
>O procedimento descrito nesta página foi aplicado apenas a organizações que ainda não foram integradas ao [!UICONTROL Adobe Admin Console].
>
>Como todas as organizações foram integradas à Adobe Admin Console, este artigo será removido em breve.
>
>Se sua organização foi integrada ao [!UICONTROL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Ao usar o URL de logout do ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), você recebe uma página de mensagem com o erro: &quot;Houve um problema ao acessar o site. Tente navegar até o site novamente.&quot;

Se o problema persistir, contate o administrador deste site e forneça o seguinte número de referência para identificar o problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

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
   <p>Padrão</p>
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
