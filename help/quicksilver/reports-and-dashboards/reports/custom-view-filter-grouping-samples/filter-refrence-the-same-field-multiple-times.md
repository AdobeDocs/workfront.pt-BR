---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '"Filtro: crie várias regras de filtro que fazem referência ao mesmo campo (instruções "AND")"'
description: Na interface do modo padrão, ao tentar criar vários filtros que fazem referência ao mesmo campo (usando o qualificador AND), um dos filtros é excluído quando você salva o relatório e sai do Report Builder.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '447'
ht-degree: 0%

---

# Filtro: crie várias regras de filtro que fazem referência ao mesmo campo (&quot;AND&quot; instruções)

Na interface do modo padrão, ao tentar criar vários filtros que fazem referência ao mesmo campo (usando o qualificador AND), um dos filtros é excluído quando você salva o relatório e sai do Report Builder.

**Exemplo:** talvez você queira exibir somente as tarefas que contenham a palavra &quot;verde&quot;, mas que não contenham a palavra &quot;vermelho&quot; no nome. O Adobe Workfront não permite salvar as seguintes regras de filtro usando a interface de modo padrão, pois faz referência ao mesmo campo (Nome da tarefa), mas usa modificadores diferentes e faz referência a valores diferentes:

* Nome da tarefa > Contém > Verde
* Nome da tarefa > Não contém > Vermelho

No entanto, é possível criar esse filtro usando o modo de texto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Solicitação para modificar um filtro </p>
   <p>Planejar a modificação de um relatório</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis e calendários para modificar um relatório</p> <p>Editar acesso a Filtros, Visualizações, Agrupamentos para modificar um filtro</p> <p><b>Nota</b>

Se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

## Criar várias regras de filtro que fazem referência ao mesmo campo

1. Ir para uma lista de tarefas.
1. No menu suspenso **Filtro**, selecione **Novo Filtro**.
1. Clique em **Alternar para Modo de Texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clicar para editar o texto**.
1. Na área Definir regras de filtro para relatórios, adicione o seguinte código:

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

1. Clique em **Concluído** e em **Salvar filtro**.
