---
title: Política de suporte do AtTask OnPremise
user-type: administrator
content-type: faq
product-area: system-administration
navigation-topic: administrator-faqs
description: A Adobe Workfront migrou para um modelo de software como serviço a 100% e parou de vender software local em 31 de dezembro de 2011. A partir de 2014, o AtTask OnPremise não será mais suportado, com exceção dos problemas relacionados à chave de licença. O aplicativo local não está mais disponível para download ou instalação.
feature: System Setup and Administration
role: Admin
exl-id: 37c65360-6587-43b3-8eaf-4f1a9b375c1d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '247'
ht-degree: 0%

---

# Política de suporte do AtTask OnPremise

A Adobe Workfront migrou para um modelo de software como serviço a 100% e parou de vender software local em 31 de dezembro de 2011. A partir de 2014, o AtTask OnPremise não será mais suportado, com exceção dos problemas relacionados à chave de licença. O aplicativo local não está mais disponível para download ou instalação.

Se você já tiver o aplicativo e precisar reinstalar o OnPremise, baixe o guia de instalação .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">OnPremise optimization tips can be found.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more about reporting in AtTask OnPremise, click.</p>
-->

Baixe instruções na configuração SSL/TSL.

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
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront. Para obter mais informações, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder ao usuário acesso administrativo total</a>.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Atualizar a chave de licença OnPremise

Se precisar de uma nova chave de licença, ligue para o Suporte ao cliente da Workfront pelo número 844-306-HELP(4357).

Depois de obter uma nova chave de licença,

1. Pare o servidor atTask.
1. Renomeie o arquivo license.key atual (localizado na pasta AtTaskDoc).
1. Copie o novo arquivo license.key para o lugar.
1. Reinicie o atTask Server.

Este artigo inclui os seguintes anexos:
