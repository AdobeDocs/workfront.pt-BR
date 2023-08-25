---
title: Excluir modelos de layout clássicos
user-type: administrator
product-area: system-administration;templates;user-management
navigation-topic: layout-templates
description: Os modelos de layout da experiência Clássica do Workfront não estão mais disponíveis na interface do Workfront, mas ainda podem afetar os dados do Workfront. Isso pode causar inconsistências em campos afetados por modelos de layout (como Compartilhado com) em relatórios ou painéis.
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: c68b63230b07ea8c8475b710e256b5e0f049b1eb
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Conceder acesso administrativo a um modelo de layout

Os modelos de layout da experiência Clássica do Workfront não estão mais disponíveis na interface do Workfront, mas ainda podem afetar os dados do Workfront. Isso pode causar inconsistências em campos afetados por modelos de layout (como Compartilhado com) em relatórios ou painéis.

Você pode resolver essas inconsistências excluindo os modelos de layout Clássicos. Como não estão disponíveis na interface do Workfront, use a API do Workfront para excluí-los.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

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

1. Insira a ID do modelo de layout e a ID da sessão na seguinte chamada de API:
   `https://{yourDomain}.com/attask/api/v16.0/LYTMPL?ID={layoutTemplateID}&method=delete&sessionID={yourSessionID}`
1. Cole a chamada de API da etapa 4 na barra de URL do seu navegador e pressione Enter.

   Isso exclui o modelo de layout.



