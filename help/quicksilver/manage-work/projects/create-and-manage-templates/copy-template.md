---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiar um modelo de projeto
description: Em vez de criar um novo modelo de projeto do zero, você pode copiar um modelo existente e fazer alterações, se necessário.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: e416a23cab139bff6d0d59b3816fb192c8f92b0b
workflow-type: tm+mt
source-wordcount: '333'
ht-degree: 3%

---

# Copiar um modelo de projeto

Em vez de criar um novo modelo de projeto do zero, você pode copiar um modelo existente e fazer alterações, se necessário.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a modelos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir ou aumentar as permissões de um modelo</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.


## Considerações sobre a cópia de modelos

Os seguintes itens são sempre copiados de um projeto existente para um novo:

* Modelo de Tarefa
* Informações Padrão de Tarefas de Modelo (Processo de Aprovação Padrão de Tarefa, Forms Personalizado Padrão de Tarefa)
* Formulários personalizados
* Riscos
* Informações de Configuração da Fila
* Portfolio e Programa
* Aprovações
* Documentos
* Os dias das tarefas do modelo original são transferidos para o novo modelo. Você deve alterar o dia de Início ou Conclusão do modelo (dependendo de seu Modo de Programação) para atualizar os dias nas tarefas do modelo, se necessário.

Os seguintes itens nunca são copiados de um projeto existente para um novo:

* Preços
* Comentários do usuário

## Copiar um modelo

1. Vá para o template que deseja copiar.
1. Clique no menu **Mais** ![](assets/qs-more-icon-on-an-object.png) e em **Copiar**.
1. Especifique um nome para o modelo no campo **Novo Nome do Modelo**.

   Por padrão, o novo nome é **Cópia de `<original template name>`.**

1. Selecione se deseja **Reter atribuições de usuário em tarefas e modelo**: selecione esta opção para carregar todas as atribuições de tarefa e modelo do modelo original para o novo modelo.
1. Clique em **Salvar** para criar uma cópia do modelo.
