---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Agrupamento: Agrupamento de Tarefas em 4 níveis para o Proprietário do Portfolio, Proprietário do Programa, Proprietário do Projeto e Status do Projeto'
description: Este Agrupamento de tarefas fornece quatro níveis de Agrupamento. Nesse caso, as tarefas são agrupadas por Proprietário do Portfolio, Proprietário do programa, Proprietário do projeto e Status do projeto. Você pode ter até três níveis de Agrupamento usando a interface padrão. Para adicionar um quarto nível, você deve usar o Modo de texto. Não é possível agrupar relatórios por mais de quatro critérios ao mesmo tempo.
author: Courtney
feature: Reports and Dashboards
exl-id: a1780a57-b94c-4d3a-b526-9bf45dba21f1
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 14%

---

# Agrupamento: agrupamento de tarefas em quatro níveis como proprietário do portfólio, proprietário do programa, proprietário do projeto e status do projeto

<!--Audited: 10/2024-->

Este Agrupamento de tarefas fornece quatro níveis de Agrupamento. Nesse caso, as tarefas são agrupadas por Proprietário do Portfolio, Proprietário do programa, Proprietário do projeto e Status do projeto. Você pode ter até três níveis de Agrupamento usando a interface padrão. Para adicionar um quarto nível, você deve usar o Modo de texto. Não é possível agrupar relatórios por mais de quatro critérios ao mesmo tempo.

![quatro_camadas_agrupamentos_para_tarefas.png](assets/four-tier-grouping-for-tasks-350x239.png)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

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

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crie um Agrupamento de tarefas em 4 níveis para o Proprietário do Portfolio, Proprietário do programa, Proprietário do projeto e Status do projeto

Para aplicar esse agrupamento:

1. Ir para uma lista de tarefas.
1. No menu suspenso **Agrupamento**, selecione **Novo agrupamento**.

1. Clique em **Alternar para Modo de Texto**.
1. Remova o texto da área **Agrupar relatório**.
1. Substitua o texto na caixa exibida com o seguinte código:
   <pre>group.0.linkedname=project<br>group.0.name=Proprietário do Portfolio<br>group.0.notime=false<br>group.0.valuefield=project:portfolio:owner:name<br>group.0.valueformat=string<br>group.1.linkedname=project<br>group.1.name=Program Proprietário<br>group.1.notime=false<br>group.1.valuefield=project:program:owner:name<br>group.1.valueformat=string<br>group.2.linkedname=projectOwnerMM<br>group.2.listgrouingparsedmethod=nested(project).nested(owner).string(name)<br>group.2.namekey=projectownermm<br>group.2.notime=false<br>fieldgroup.name.2.name <br>group.3.linkedname=project<br>group.3.namekey=view.relatedcolumn<br>group.3.namekeyargkey.0=project<br>group.3.namekeyargkey.1=status<br>group.3.notime=false<br>group.3.valuefield=project:status<br>group.3.valueformat=val<br><br></pre>

1. Clique em **Concluído** e em **Salvar agrupamento**.
1. (Opcional) Atualize o nome do agrupamento e clique em **Salvar agrupamento**.
