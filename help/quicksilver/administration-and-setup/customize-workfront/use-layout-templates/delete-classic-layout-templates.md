---
title: Excluir modelos de layout clássicos
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Os modelos de layout da Experiência clássica do Workfront não estão mais disponíveis em sua interface, mas ainda podem afetar seus dados. Isso pode causar inconsistências em campos afetados por modelos de layout (como “Compartilhado com”) em relatórios ou painéis.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: c6d33d5d-da93-4aba-8897-f177c1171595
source-git-commit: 80bdc2f2c1bedbc5a894b5a474425c5544c039fd
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 52%

---

# Excluir modelos de layout clássicos

Os modelos de layout da Experiência clássica do Workfront não estão mais disponíveis em sua interface, mas ainda podem afetar seus dados. Isso pode causar inconsistências em campos afetados por modelos de layout (como “Compartilhado com”) em relatórios ou painéis.

Você pode resolver essas inconsistências excluindo os modelos de layout Clássicos. Como não estão disponíveis na interface do Workfront, use a API do Workfront para excluí-los.

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
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td><p>Novo: Padrão</p>
  <p> Atual: Plano</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.
Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir os modelos de layout clássicos usando uma chamada de API

Você pode inserir chamadas de API na barra de URL do navegador e pressionar Enter. A resposta da API é exibida no navegador.

>[!NOTE]
>
>Os modelos de layout Global e Sistema não podem ser excluídos.

1. Faça logon no Workfront.
1. Localize o modelo de layout que deseja excluir usando a seguinte chamada de API:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL/search`
1. Anote a ID do modelo de layout que deseja excluir.
1. Localize sua ID de sessão usando a seguinte chamada de API:
   `https://{yourDomain}.com/attask/api/v16.0/session`

   >[!IMPORTANT]
   >
   >Nunca compartilhe sua ID de sessão com ninguém.

1. Insira a ID do modelo de layout e a ID de sessão na seguinte chamada de API:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Cole a chamada de API da etapa 4 na barra de URL do navegador e pressione Enter.

   Isso excluirá o modelo de layout.
