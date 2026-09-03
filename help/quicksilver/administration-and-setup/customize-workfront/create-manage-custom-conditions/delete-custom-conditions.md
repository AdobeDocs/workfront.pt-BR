---
title: Excluir uma condição personalizada
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: Você pode excluir uma condição personalizada.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
TQID: https://experienceleague.adobe.com/jHR0a3-MzkRRrlZ-h-X9f0n5HQbO9nDhWSxqy8KnWa8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: d5694e2f94ded811e90b31f315896914ca31fc9f
workflow-type: tm+mt
source-wordcount: 256
ht-degree: 16%

---

# Excluir uma condição personalizada

{{preview-fast-release-general}}

Você poderá excluir uma condição personalizada se ela não for mais necessária.

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
   <td>Administrador de sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Excluir uma condição personalizada

{{step-1-to-setup}}

1. Clique em **Preferências do projeto** > **Condições**.

1. Selecione a guia do tipo de objeto (**Projeto**, **Tarefa** ou **Problema**) onde está localizada a condição que você deseja excluir.
1. No ambiente de Produção, clique em **Excluir** ao lado do nome da condição que deseja excluir.
   <span class="preview">No ambiente de Visualização, marque a caixa de seleção ao lado do nome da condição que você deseja excluir e clique em **Excluir** na barra de ações na parte inferior da tela.</span>

1. Na caixa **Excluir condição** exibida, selecione uma nova condição na lista suspensa para todos os projetos, tarefas ou problemas que estavam usando a condição que você está excluindo.

   As condições personalizadas só estarão disponíveis na lista suspensa se forem equivalentes à mesma condição interna que aquela que você está excluindo. Por exemplo, se você estiver excluindo uma condição que equivale a Em risco, apenas condições personalizadas que também equivalem a Em risco estarão disponíveis para seleção.

1. Clique em **Excluir condição**.

>[!NOTE]
>
>Não é possível excluir as condições incorporadas, que são No destino, Em risco e Com problema. Entretanto, é possível alterar os nomes e as cores.
>
>Para obter informações sobre como editar condições personalizadas, consulte [Criar ou editar uma condição personalizada](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
