---
title: Desabilitar a opção de atualização automática para usuários não pagos no novo plano de licenciamento
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,nível,sistema,administrador,padrão,claro,colaborador
navigation-topic: access-levels
description: Todos os usuários devem ter um nível de acesso para fazer logon e trabalhar no Workfront. Você usa o nível de acesso para controlar o que um usuário pode ver e fazer com determinados objetos e áreas do Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 58c76187-fc74-4ab4-80e8-c3e296a84f27
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '205'
ht-degree: 1%

---

# Desabilitar a opção de atualização automática para usuários não pagos no novo plano de licenciamento

As decisões de prova e documento são limitadas para todas as licenças não pagas do Workfront nos novos planos. Quando os usuários atingem o número permitido de decisões, eles são atualizados para uma licença Light por padrão.

Você pode desativar a opção de atualização automática na área de configuração. Para saber mais sobre como as atualizações automáticas funcionam, consulte [Visão geral sobre documento limitado e decisão de prova para usuários não pagos](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

>[!IMPORTANT]
>
>Uma vez desativado, qualquer usuário não pago que exceda o número alocado de decisões não será atualizado automaticamente.

## Requisitos de acesso

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
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Novo plano: Padrão
   <p>ou</p>
   <p>Plano atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Desabilitar atualizações automáticas para usuários não pagos

{{step-1-to-setup}}

1. Expanda [!UICONTROL **Sistema**] na navegação à esquerda e clique em [!UICONTROL **Preferências**].
1. Na seção [!UICONTROL **Preferências Gerais**], marque a caixa [!UICONTROL **Desabilitar atualização automática em Níveis de Acesso**].
1. Clique em [!UICONTROL **Salvar**].
