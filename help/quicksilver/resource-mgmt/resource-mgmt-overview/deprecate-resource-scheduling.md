---
content-type: reference
product-area: resource-management
keywords: carga de trabalho, balanceador
navigation-topic: resource-management-overview
title: Substituição das ferramentas de Agendamento de Recursos no Adobe Workfront
description: No momento, estamos descontinuando todas as ferramentas de Agendamento do Adobe Workfront e substituindo-as pelo Balanceador de Carga de Trabalho.
author: Alina
feature: Resource Management
exl-id: 7fa644cd-cf6a-40f8-ae28-bf222bb45d3f
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 0%

---

# Substituição das ferramentas de Agendamento de Recursos no Adobe Workfront

>[!IMPORTANT]
>  
><span class="preview">A funcionalidade de Agendamento descrita neste artigo foi descontinuada e removida do Adobe Workfront a partir da versão 23.1 em janeiro de 2023.   </span>
>  
> <span class="preview"> Este artigo também será removido logo após a versão 23.1, no início de 2023. Nesse momento, recomendamos que você atualize todos os marcadores adequadamente. </span>
> 
><span class="preview"> Agora você pode usar o Balanceador de Carga de Trabalho para agendar o trabalho de seus recursos. </span>
>  
> <span class="preview">Para obter informações sobre como programar recursos usando o Balanceador de Carga de Trabalho, consulte a seção [O Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/workload-balancer.md). </span>

<!--
We are currently in the process of removing all Scheduling tools from Adobe Workfront and replacing them with the Workload Balancer.

>[!IMPORTANT]
>
>We are no longer implementing new feature functionality for the current Scheduling solution and we no longer consider nor prioritize defects for a fix in this area of Adobe Workfront.

This article describes the timeline for this deprecation and it compares the functionality of the Scheduling tools and that of the Workload Balancer to indicate which Scheduling capabilities are already supported in the Workload Balancer. 

We have been announcing a more exact timeline through the Announcement Center at key milestones during the deprecation process and this article has been updated as this process continues.

>[!NOTE]
>
>The changes described in this article do not affect any other resource management tools. For example, they do not affect the [!UICONTROL Resource Planner] or the [!UICONTROL Utilization] report.
-->

## Como se deve preparar

Para obter informações detalhadas sobre como se preparar para a transição entre o Scheduling e o Balanceador de Carga de Trabalho, consulte [Migrar do Agendamento de Recursos para o Balanceador de Carga de Trabalho](../../resource-mgmt/resource-mgmt-overview/migrate-resource-scheduling-to-workload-balancer.md).

Se você usa ferramentas de Agendamento, recomendamos que você as descontinue e comece a usar o Balanceador de Carga de Trabalho.

![A área Agendamento global de recursos](assets/resource-scheduler-global-350x127.png)

Quase todos os recursos disponíveis anteriormente nas áreas de Agendamento estão disponíveis no Balanceador de Carga de Trabalho. Para obter mais informações, consulte a seção [Disponibilidade de recursos](#feature-availability) neste artigo. Você pode continuar programando seus recursos para trabalhar exclusivamente no Balanceador de Carga de Trabalho.

![A área Balanceador de Carga de Trabalho global](assets/workload-balancer-pti-350x111.png)

## Informações que não serão transferidas para o Balanceador de Carga de Trabalho

As seguintes informações não serão transferidas das ferramentas de Agendamento para o Balanceador de Carga de Trabalho:

* **Alocações diárias para usuários**: Você não deve usar a Programação e o Balanceador de Carga de Trabalho ao mesmo tempo para ajustar as mesmas alocações de usuário. Se você gerenciou alocações de usuários nas ferramentas de Programação, as alocações diárias ajustadas não são transferidas para o Balanceador de Carga de Trabalho. Da mesma forma, se você tiver ajustado as alocações de usuários no Balanceador de Carga de Trabalho, elas não serão transferidas para as ferramentas de Programação. Recomendamos que você garanta que as alocações diárias sejam precisas no Balanceador de Carga de Trabalho para se preparar para essa transição. Para obter mais informações, consulte [Gerenciar alocações de usuários no Balanceador de Carga de Trabalho](../workload-balancer/manage-user-allocations-workload-balancer.md).
* **Filtros**: Se você tiver salvo filtros nas áreas de Agendamento, eles não serão transferidos para o Balanceador de Carga de Trabalho. Você deve recriar os filtros no Balanceador de Carga de Trabalho. Para obter mais informações, consulte [Filtrar informações no Balanceador de Carga de Trabalho](../workload-balancer/filter-information-workload-balancer.md).

## Destaques da linha do tempo de descontinuação

>[!IMPORTANT]
>
>Use este artigo para entender a linha do tempo mais recente para descontinuar as ferramentas de Agendamento . Todas as atualizações nessa linha do tempo serão comunicadas neste artigo e nas mensagens da Central de anúncios.

Veja a seguir uma linha do tempo para o processo de descontinuação das ferramentas de Agendamento de Recursos:

* [Versão 2020.4 (novembro de 2020)](#2020-4-release-november-2020)
* [Versão 2021.4 (outubro de 2021)](#2021-4-release-october-2021)
* [Versões 2022.4 - 2023.1 (outubro de 2022 - janeiro de 2023)](#2022-4-2023-1-releases)

### Versão 2020.4 (novembro de 2020) {#2020-4-release-november-2020}

* A nova funcionalidade de recurso não é mais implementada para a solução de agendamento
* Somente defeitos de severidade Alta e Crítica serão priorizados para uma correção
* Novos recursos de balanceador de carga de trabalho adicionados ao Workfront

### Versão 2021.4 (outubro de 2021) {#2021-4-release-october-2021}

* O Balanceador de Carga de Trabalho é definido como padrão para qualquer usuário novo do Workfront
* Filtros aprimorados que podem ser compartilhados e incluir campos adicionais

### Versões 2022.4 - 2023.1 (outubro de 2022 - janeiro de 2023) {#2022-4-2023-1-releases}

* Nenhum defeito será priorizado para uma correção durante e após as versões 2022.4 ou 2023.1
* Todas as áreas de Agendamento são removidas do ambiente de Visualização (**20 de outubro de 2022**)
* Todas as áreas de Agendamento são removidas do ambiente Produção (**Janeiro de 2023**)
* O Balanceador de Carga de Trabalho é a única ferramenta de agendamento de recursos disponível no Workfront (após **Janeiro de 2023**)

## Disponibilidade de recursos {#feature-availability}

Salvo especificação em contrário, todos os recursos de Agendamento de Recursos foram ou estarão disponíveis no Balanceador de Carga de Trabalho. Para obter informações sobre o Balanceador de Carga de Trabalho, consulte [Visão Geral do Balanceador de Carga de Trabalho](../../resource-mgmt/workload-balancer/overview-workload-balancer.md).

Além dos recursos existentes, o Balanceador de Carga de Trabalho tem ou terá novas funcionalidades que não existiam nas ferramentas de Agendamento de Recursos, conforme mostrado na tabela a seguir:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td rowspan="2"><span style="font-weight: normal;"><b>Recursos</b></span> </td> 
   <td rowspan="2"> <b>Disponibilidade de recursos das ferramentas de Agendamento de Recursos</b></td> 
   <td colspan="3"><b>Disponibilidade de recursos do Balanceador de Carga de Trabalho</b></td> 
  </tr> 
  <tr> 
   <td><b>Disponível agora</b></td> 
   <td><b>Disponível em breve</b></td> 
   <td><b>Não planejado</b></td> 
  </tr> 
  <tr> 
   <td> <p>Acessar ferramenta da área Recursos</p> </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Áreas separadas para trabalhos não atribuídos e atribuídos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Aplicar e criar filtros para trabalhos não atribuídos e atribuídos</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Acessar itens de trabalho diretamente da ferramenta</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Atribuir ou cancelar a atribuição manual de tarefas e problemas</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Ajustar alocações individuais</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Incluir tempo de ocorrência</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir datas projetadas </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir trabalho concluído</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Mostrar tempo limite do usuário, fim de semana e exceções de programação</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Atribua usuários rapidamente com base em funções*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Substitua rapidamente os usuários*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><span>Cancelar a atribuição rápida de usuários*</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Acessar ferramenta de uma equipe</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Acessar ferramenta de um projeto</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr>
   <td>Usuários de licença de trabalho podem ajustar alocações de usuários ao acessar o Balanceador de Carga de Trabalho de um projeto </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td>Exibir problemas na área de trabalho não atribuída</td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td></td> 
  </tr> 
  <tr> 
   <td><span>Atribua e cancele a atribuição de tarefas e problemas arrastando e soltando *</span> </td> 
   <td>✓</td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Visível para todos os usuários do Plano, sem ter sido designado um Gerenciador de Recursos no projeto.</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Informações do grupo por projeto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Compartilhe o Balanceador de Carga de Trabalho com usuários sem acesso à área Recursos</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir e ajustar alocações por semana</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Acessar usuários diretamente da ferramenta</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Acesse mais informações sobre itens de trabalho sem sair, usando o painel Resumo*</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir e ajustar a alocação como um valor de porcentagem </td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir a diferença entre o tempo disponível e o tempo alocado</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Exibir a disponibilidade do usuário em um gráfico</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Itens de trabalho e projetos com código de cores por Status do Projeto</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Atualizar automaticamente as horas planejadas conforme você ajusta a alocação de usuário (para tarefas com um Tipo de duração simples)</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Sugerir atribuições com base no padrão de atribuição do usuário, Atribuições de Função ou de Equipe existentes</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Filtros aprimorados que podem ser compartilhados e incluir campos adicionais</td> 
   <td> </td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td><span>Fazer atribuições avançadas</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td> 
  </tr>

<tr> 
   <td><span>Codificar a cor dos itens de trabalho por projetos e status do projeto</span> </td> 
   <td> </td> 
   <td><span>✓</span> </td> 
   <td> </td> 
   <td> </td>

<tr> 
   <td>Adicionar usuários à equipe do projeto (realocado para a <b>Pessoas</b> guia do projeto) </td> 
   <td>✓</td> 
   <td>✓</td> 
   <td></td> 
   <td> </td>

</tr>
   <tr> 
   <td>Atribuir tarefas e problemas automaticamente</td> 
   <td>✓</td> 
   <td> </td> 
   <td> </td> 
   <td>✓</td> 
  </tr>

</tbody> 
</table>

*Esses recursos estão disponíveis somente na nova experiência do Adobe Workfront.
