---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filtro: crie várias regras de filtro que fazem referência ao mesmo campo (instruções "AND")'
description: Na interface do modo padrão, ao tentar criar vários filtros que fazem referência ao mesmo campo (usando o qualificador AND), um dos filtros é excluído quando você salva o relatório e sai do Report Builder.
author: Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

# Filtro: crie várias regras de filtro que fazem referência ao mesmo campo (&quot;AND&quot; instruções)

<!--Audited: 10/2024-->

Na interface do modo padrão, ao tentar criar vários filtros que fazem referência ao mesmo campo (usando o qualificador AND), um dos filtros é excluído quando você salva o relatório e sai do Report Builder.

**Exemplo:** talvez você queira exibir somente as tarefas que contenham a palavra &quot;verde&quot;, mas que não contenham a palavra &quot;vermelho&quot; no nome. O Adobe Workfront não permite salvar as seguintes regras de filtro usando a interface de modo padrão, pois faz referência ao mesmo campo (Nome da tarefa), mas usa modificadores diferentes e faz referência a valores diferentes:

* Nome da tarefa > Contém > Verde
* Nome da tarefa > Não contém > Vermelho

No entanto, é possível criar esse filtro usando o modo de texto.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td> 
   <p>Colaborador ou Solicitação para modificar um filtro </p>
   <p>Padrão ou Plano para modificar um relatório</p>
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar várias regras de filtro que fazem referência ao mesmo campo

1. Ir para uma lista de tarefas.
1. No menu suspenso **Filtro**, selecione **Novo Filtro**.
1. Clique em **Modo de texto**.
1. Na caixa exibida, adicione o seguinte código:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Para construir filtros semelhantes, crie a primeira instrução primeiro. Por exemplo:
   >
   >```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copie e cole a instrução quantas vezes forem necessárias. Em seguida, você pode adicionar quantas instruções forem necessárias para fazer referência ao mesmo campo (no nosso caso, &quot;nome&quot;) e fazer as seguintes modificações nas instruções adicionais:
   >
   >1. Preceda as duas linhas copiadas com &quot;AND:1:&quot;, &quot;AND:2:&quot;, &quot;AND:3:&quot;, etc. para cada novo valor possível de campo.
   >1. Substitua a linha de campo pelo novo valor de campo (após o sinal &quot;=&quot;).
   >1. Substitua a linha do modificador (_Mod) pelo novo modificador.
   >   
   >Essas instruções fazem distinção entre maiúsculas e minúsculas.

1. Clique em **Aplicar** e em **Salvar como novo**.
