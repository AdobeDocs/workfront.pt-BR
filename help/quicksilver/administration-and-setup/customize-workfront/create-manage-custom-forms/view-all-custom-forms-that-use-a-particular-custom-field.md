---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Exibir todos os Forms personalizados que usam um determinado campo personalizado ou widget
description: Você pode descobrir quais formulários personalizados estão usando um campo ou widget personalizado que deseja alterar ou excluir. É importante avaliar se esses formulários personalizados precisarão de ajustes para continuar funcionando corretamente ou para continuar sendo útil após alterar ou excluir o campo ou widget.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 40722f2b-f8b2-4dc5-805e-2b434a0d46c3
TQID: https://experienceleague.adobe.com/aDc3yeQukT9pIRezV0OnfXuXkxfdDXE7WVZybDbPIVw
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
source-wordcount: 360
ht-degree: 10%

---

# Exibir todos os formulários personalizados que usam um campo ou widget personalizado específico

Você pode descobrir quais formulários personalizados estão usando um campo ou widget personalizado que deseja alterar ou excluir. É importante avaliar se esses formulários personalizados precisarão de ajustes para continuar funcionando corretamente ou para continuar sendo útil após alterar ou excluir o campo ou widget.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Descubra quais formulários personalizados usam um determinado campo ou widget personalizado

Para ver o uso de um campo na lista de todos os campos personalizados:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Clique em **Campos**, procure o campo ou widget na coluna **Nome** e exiba a coluna **Forms** para ver quais formulários personalizados estão usando o campo ou widget.
1. (Opcional) Clique no nome de qualquer um desses formulários personalizados para ir para o formulário e considerar quais alterações você pode precisar fazer lá se modificar o campo ou widget.

Para ver o uso de um campo em um formulário personalizado:

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Abra um formulário personalizado e adicione um campo da biblioteca ou selecione um campo existente no formulário.

   O indicador de uso à direita do designer de formulário mostra quantos outros formulários personalizados usam esse campo.

1. Clique em **Exibir Forms Relacionada**.

   Na lista de formulários, você pode clicar em qualquer nome de formulário para abrir o formulário e ver como o campo é usado. Um indicador mostra se cada formulário está ativo ou inativo.


