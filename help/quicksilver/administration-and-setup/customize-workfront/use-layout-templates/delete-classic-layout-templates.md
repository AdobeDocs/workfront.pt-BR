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
TQID: https://experienceleague.adobe.com/AcxOFTyZbrQakRoeBlslCoLJgrgY4HS41vaYLOx5i-I
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 299
ht-degree: 70%

---

# Excluir modelos de layout clássicos

Os modelos de layout da Experiência clássica do Workfront não estão mais disponíveis em sua interface, mas ainda podem afetar seus dados. Isso pode causar inconsistências em campos afetados por modelos de layout (como “Compartilhado com”) em relatórios ou painéis.

Você pode resolver essas inconsistências excluindo os modelos de layout Clássicos. Como não estão disponíveis na interface do Workfront, use a API do Workfront para excluí-los.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Para executar essas etapas no nível do sistema, você precisa do nível de acesso Administrador do sistema.</p>
        <p>Para executá-las para um grupo, você deve ser um gerente desse grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir modelos de layout clássicos usando uma chamada de API

Você pode inserir chamadas de API na barra de URL do navegador e pressionar Enter. A resposta da API é exibida no navegador.

>[!NOTE]
>
>Os modelos de layout Global e Sistema não podem ser excluídos.

1. Faça login no Workfront.
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
