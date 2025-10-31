---
product-area: templates
navigation-topic: templates-navigation-topic
title: Copiar um modelo de projeto
description: Além de criar um modelo de projeto do zero, também é possível copiar um modelo existente e modificá-lo.
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
source-git-commit: 76379d5433cc13ee412c8c1045316ef253b3ee7d
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 3%

---

# Copiar um modelo de projeto

<!--Audited: 5/2025-->

Além de criar um modelo de projeto do zero, você também pode copiar um modelo existente e modificá-lo no Adobe Workfront.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

Você deve ter o seguinte acesso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p> 
   <p>Plano</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a modelos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir ou aumentar as permissões de um modelo</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## Considerações sobre a cópia de modelos

Os itens a seguir são sempre copiados de um modelo existente para um novo:

* Modelo de Tarefa
* Informações Padrão de Tarefas de Modelo (Processo de Aprovação Padrão de Tarefa, Forms Personalizado Padrão de Tarefa)
* Formulários personalizados
* Riscos
* Informações de Configuração da Fila
* Portfolio e Programa
* Aprovações
* Documentos
* Os dias das tarefas do modelo original são transferidos para o novo modelo. Você deve alterar o dia de Início ou Conclusão do modelo (dependendo de seu Modo de Programação) para atualizar os dias nas tarefas do modelo, se necessário.

Os itens a seguir nunca são copiados de um modelo existente para um novo:

* Taxas de cobrança
* Comentários do usuário

## Copiar um modelo

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. Vá para o template que deseja copiar.
1. Clique no **Mais** ícone ![Mais](assets/more-icon.png) do menu à direita do nome do modelo no cabeçalho e clique em **Copiar**.

   A caixa **Copiar Modelo** é aberta.

   ![Copiar caixa de modelo](assets/copy-template-box.png)

1. Especifique um nome para o modelo no campo **Novo Nome do Modelo**.

   Por padrão, o Workfront define o novo nome seguindo este formato: `Copy of Original template name`.

1. Selecione a opção **Reter atribuições de usuário nas tarefas e no modelo** se desejar carregar todas as atribuições de tarefa e modelo do modelo original para o novo modelo. As atribuições de modelo de tarefa e o Proprietário e Patrocinador do Modelo são transferidos para o modelo copiado.
1. Clique em **Salvar** para criar uma cópia do modelo.

   O novo modelo é exibido na lista de modelos na área Modelo do Workfront.
