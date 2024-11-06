---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Visualização: Remover link para um objeto em uma coluna"
description: Alguns objetos exibidos em uma view são vinculados à página Detalhes do objeto, por padrão. Por exemplo, a coluna que exibe o Nome de um projeto é um link para o projeto; a coluna que exibe o Nome de um usuário é um link para a página de perfil do usuário.
author: Nolan
feature: Reports and Dashboards
exl-id: 08264437-f12d-43fa-8cb4-264806c6479b
source-git-commit: 17a277a5a63a521ec7285e3f5051bfd42fc204bf
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Exibir: remover link de um objeto em uma coluna

<!--Audited: 11/2024-->

Alguns objetos exibidos em uma view são vinculados à página Detalhes do objeto, por padrão. Por exemplo, a coluna que exibe o Nome de um projeto é um link para o projeto; a coluna que exibe o Nome de um usuário é um link para a página de perfil do usuário.

Você pode remover esse link usando o modo de texto em colunas exibidas em todas as exibições.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> <p> Atual: 
   <ul>
   <li>Solicitação para modificar uma exibição</li> 
   <li>Planejar a modificação de um relatório</li>
   </ul>
     </p>
     <p> Novo: 
   <ul>
   <li>Colaborador para modificar uma visualização</li> 
   <li>Padrão para modificar um relatório</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar uma visualização</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Exemplo: Remova o link para uma tarefa da coluna Nome da Tarefa em uma exibição de tarefa:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Exibir**, clique em **Nova Exibição** para criar uma nova exibição.

   Ou

   Clique no **ícone Editar** ![](assets/edit-icon.png)

   para editar uma exibição existente, selecione-a.

1. Clique em **Adicionar coluna** para adicionar uma nova coluna.

   Ou

   Clique em uma coluna existente com um link para um objeto.

1. Clique em **Alternar para Modo de Texto** > **Editar Modo de Texto**.
1. Remova o texto localizado na caixa **Editar Modo de Texto** e substitua-o pelo seguinte código:

   ```
   displayname=Task Name
   linkedname=direct
   namekey=name
   querysort=name
   textmode=true
   valueexpression={name}
   valueformat=Compound
   ```

   >[!TIP]
   >
   >Você pode usar um código semelhante para outros objetos ajustando o seguinte:
   >
   >* Substitua a linha `valuefield` do código por `valueexpression` e mantenha o mesmo nome incluído entre chaves após o sinal de igual.
   >* Eliminar todas as linhas que começam com `link.` do texto original da coluna. Por exemplo, elimine todas as linhas a seguir:
   >
   >  ```
   >  link.linkproperty.0.name=ID
   >  link.linkproperty.0.valuefield=ID
   >  link.linkproperty.0.valueformat=string
   >  link.lookup=link.view
   >  link.value=val(objCode)
   >  ```
   >

1. Clique em **Concluído** e depois em **Salvar exibição**.

