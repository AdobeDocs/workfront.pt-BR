---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: "Filtro: criar várias regras de filtro que fazem referência ao mesmo campo (instruções 'AND')"
description: Na interface do modo padrão, ao tentar criar vários filtros que fazem referência ao mesmo campo (usando o qualificador AND), um dos filtros é excluído ao salvar o relatório e sair do construtor de relatórios.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: fb167e9f-c8bd-43f6-84c9-9a87e80c3eb2
source-git-commit: 8b6324302a70319f387d1e09d1eb92fbdabf7e32
workflow-type: tm+mt
source-wordcount: '430'
ht-degree: 0%

---

# Filtro: criar várias regras de filtro que fazem referência ao mesmo campo (instruções &quot;AND&quot;)

Na interface do modo padrão, ao tentar criar vários filtros que fazem referência ao mesmo campo (usando o qualificador AND), um dos filtros é excluído ao salvar o relatório e sair do construtor de relatórios.

**Exemplo:** Talvez você queira exibir apenas as tarefas que contêm a palavra &quot;verde&quot;, mas não contêm a palavra &quot;vermelho&quot; no nome. O Adobe Workfront não permite salvar as seguintes regras de filtro usando a interface de modo padrão, pois ela faz referência ao mesmo campo (Nome da Tarefa), mas usa modificadores diferentes e faz referência a valores diferentes:

* Nome da tarefa > Contém > Verde
* Nome da tarefa > Não contém > Vermelho

No entanto, é possível criar esse filtro usando o modo de texto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Relatórios, Painéis, Calendários</p> <p>Editar acesso a filtros, visualizações, agrupamentos</p> <p>Observação: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Criar várias regras de filtro que fazem referência ao mesmo campo

1. Vá para uma lista de tarefas.
1. No **Filtro** , selecione **Novo filtro**.
1. Clique em **Alternar para o modo de texto**.
1. Passe o mouse sobre a área do modo de texto e clique em **Clique para editar texto**.
1. Na área Definir regras de filtro para seu relatório , adicione o seguinte código:

   ```
   name=green
   name_Mod=cicontains
   AND:1:name=red
   AND:1:name_Mod=cinotcontains
   ```

   >[!TIP]
   >
   >Para criar filtros semelhantes, crie a primeira instrução primeiro. Por exemplo:
   >
   >
   ```
   >name=green
   >name_Mod=cicontains
   >```
   >
   >Copie e cole a declaração quantas vezes forem necessárias. Em seguida, é possível adicionar quantas instruções forem necessárias para fazer referência ao mesmo campo (no nosso caso, &quot;name&quot;) e fazer as seguintes modificações nas declarações adicionais:
   >
   >1. Preceder as duas linhas copiadas com &quot;AND:1:&quot;, &quot;E:2:&quot;, &quot;E:3:&quot;, etc para cada novo valor possível de campo.
   >1. Substitua a linha de campo pelo novo valor de campo (após o sinal &quot;=&quot;).
   >1. Substitua a linha do modificador (_Mod) pelo novo modificador.

   >   
   >Essas instruções diferenciam maiúsculas de minúsculas.

1. Clique em **Concluído**, em seguida **Salvar filtro**.
