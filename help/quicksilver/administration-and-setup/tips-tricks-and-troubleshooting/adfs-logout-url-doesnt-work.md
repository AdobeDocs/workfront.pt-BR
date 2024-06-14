---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: O URL de logout do ADFS não funciona
description: O procedimento descrito nesta página se aplica apenas a organizações que ainda não foram integradas à Adobe Admin Console.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 4d868625-e976-47b4-9e80-f1eca84a2768
source-git-commit: 8769637342ab65f1e627107f7bfb41f9a3f61cca
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 0%

---

# O URL de logout do ADFS não funciona

<!-- Audited: 1/2024 -->

>[!IMPORTANT]
>
>O procedimento descrito nesta página se aplica somente a organizações que ainda não foram integradas à [!UICONTROL Adobe Admin Console].
>
>Se sua organização foi integrada à [!UICONTROL Adobe Admin Console], consulte [Diferenças de administração baseadas em plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

## Problema

Ao usar o URL de logout do ADFS (https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0), você recebe uma página de mensagem com o erro: &quot;Houve um problema ao acessar o site. Tente navegar até o site novamente.&quot;

Se o problema persistir, entre em contato com o administrador deste site e forneça o seguinte número de referência para identificar o problema: **57092dfc-751a-4915-8e6a-b4c5d413f8c6**

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe [!DNL Workfront] licença</td> 
   <td> 
   <p>Novo: Padrão</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um [!DNL Workfront] administrador. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acesso administrativo total a um usuário</a>.</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solução

1. No servidor do gerenciador ADFS, vá para **[!UICONTROL Relações de confiança]** > **[!UICONTROL Terceiras Partes Confiáveis]** > `<your party trust>` propriedades.

1. No **[!UICONTROL Endpoints]** clique em **[!UICONTROL Adicionar]**.

1. **[!UICONTROL Tipo de Ponto de Extremidade]** = Logout SAML, Ligação = POST, URL = https://myadfsserver.domain.net/adfs/ls/?wa=wsignout1.0

   Você pode definir um URL de resposta se quiser redirecioná-lo para outra página. Mas recomendamos o site do ADFS porque ele avisa que você está desconectado, mas ainda deve fechar o navegador.
