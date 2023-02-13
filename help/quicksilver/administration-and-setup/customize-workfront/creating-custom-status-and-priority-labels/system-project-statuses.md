---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Status do projeto do sistema
description: A Workfront tem 9 status de projeto do sistema integrado. Os primeiros 3 da tabela abaixo são obrigatórios, o que significa que você pode desbloquear, renomear e reorganizá-los, mas não pode ocultá-los ou excluí-los. A alteração do status de um projeto geralmente é um processo manual. No entanto, às vezes, o status de um projeto é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1536'
ht-degree: 0%

---

# Status do projeto do sistema

A Workfront tem 9 status de projeto do sistema integrado.

Os primeiros 3 da tabela abaixo são obrigatórios, o que significa que você pode desbloquear, renomear e reorganizá-los, mas não pode ocultá-los ou excluí-los.

A alteração do status de um projeto geralmente é um processo manual. No entanto, há alguns cenários descritos na lista a seguir quando um status de projeto é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.

Os seguintes status do projeto são fornecidos com sua instância do Workfront:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <col> 
 </col> 
 <thead> 
  <tr> 
   <th>Status do projeto do sistema</th> 
   <th>Este status do projeto ocorre quando</th> 
   <th>O que acontece com esse status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejamento (status necessário)</td> 
   <td> <p>O gerente do projeto está planejando a linha do tempo do projeto, a atribuição das tarefas e as aprovações. O gerente do projeto define esse status em um projeto manualmente.</p> <p>Dica: Recomendamos que você defina o status padrão para novos projetos no Workfront para Planning. Como administrador da Workfront, você pode alterar o status padrão de todos os novos projetos na área Projetos das Preferências do projeto.</p> </td> 
   <td> <p>Os usuários da equipe do projeto podem ver o projeto em suas listas de Projetos por padrão, na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto não preenchem a Lista de trabalho. Somente aprovações e itens de trabalho aceitos são exibidos na Lista de Trabalho Inicial.</p> <p>Nenhuma notificação é enviada enquanto um projeto tem esse status.</p> <p>Recomendamos que todas as alterações que podem acionar uma atualização na linha do tempo do projeto, ou quaisquer alterações nas tarefas e atribuições de emissão, sejam feitas enquanto o projeto estiver no status de Planejamento. Isso minimiza a quantidade de notificações que os usuários recebem.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Atual (status obrigatório)</td> 
   <td> <p>Os usuários estão trabalhando nisso. O gerente do projeto deve transformar um projeto em Atual para sinalizar que ele foi iniciado.</p> <p>Este é o status padrão para novos projetos no Workfront.</p> <p>Dica: Como administrador do Workfront, você pode alterar o status padrão de novos projetos na área Projetos das Preferências do projeto. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </td> 
   <td> <p>Os usuários da equipe do projeto podem ver o projeto em suas listas de Projetos por padrão, na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto preenchem a Lista de trabalho. Eles podem começar a aceitar trabalhos em tarefas e problemas e movê-los para a lista Trabalhar em.</p> <p>Além disso, em um projeto atual, todas as notificações sobre alterações na linha do tempo, atribuições, ações necessárias e aprovações são enviadas aos usuários da equipe do projeto.</p> <p>E a linha do tempo do projeto é calculada automaticamente pelo sistema, se o Tipo de atualização do projeto estiver definido como Automático, On Change ou Automático e On Change.</p> <p>Dica: É uma boa ideia manter os ajustes do plano do projeto no mínimo, quando um projeto estiver nesse status, para que os usuários não recebam muitas notificações.</p> </td> 
  </tr> 
  <tr> 
   <td>Concluído (status necessário)</td> 
   <td> <p> O projeto está concluído:</p> 
    <ul> 
     <li> <p>Se o Modo de conclusão do projeto estiver definido como Manual, o gerente do projeto escolhe esse status manualmente para informar os usuários da equipe do projeto para parar de trabalhar no projeto.</p> </li> 
    </ul> 
    <ul> 
     <li>Se o Modo de conclusão do projeto estiver definido como Automático, o Workfront marca automaticamente um projeto como Concluído quando todas as tarefas e problemas no projeto estiverem marcados como Concluído. </li> 
    </ul> <p><b>IMPORTANTE</b>: Você pode marcar um projeto como Concluído somente quando todas as tarefas, problemas e aprovações no projeto forem resolvidas.</p> </td> 
   <td>
    <ul>
     <li>Por padrão, os usuários da equipe do projeto não podem ver o projeto em suas listas de Projetos na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto não preenchem as solicitações de trabalho ou as listas Trabalhar em.</li>
     <li>Todas as notificações relacionadas ao projeto, exceto uma notificação de alteração de status, param de ser enviadas aos usuários na equipe do projeto. </li>
     <li>A linha do tempo do projeto não é mais calculada pelo sistema.</li>
     <li>O projeto não pode ser copiado.</li>
    </ul><p>Você pode impedir que os usuários executem ações adicionais quando um projeto é marcado como Concluído. </p><p>Para obter mais informações sobre como restringir ações em projetos que estão marcados como Concluído, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Parado</td> 
   <td>O projeto ainda não terminou, mas devido a bloqueios de estradas ou mudanças de escopo, o projeto não pode continuar sendo trabalhado e foi abandonado. O gerente do projeto altera o status para Morto para alertar os usuários na equipe do projeto de que esse projeto nunca será concluído e que eles não devem mais trabalhar nele.</td> 
   <td> <p>Por padrão, os usuários da equipe do projeto não podem ver o projeto em suas listas de Projetos na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto desaparecem de sua Lista de Trabalho.</p> <p>As decisões de aprovação não podem ser concedidas a tarefas ou emissões.</p> <p>As notificações sobre alterações na linha do tempo, atribuições, ações necessárias, aprovações não são enviadas aos usuários na equipe do projeto.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema, pois o projeto é considerado como concluído.</p> <p>Você pode impedir que os usuários executem determinadas ações quando um projeto é marcado como inativo. Para obter mais informações sobre como restringir ações em projetos inativos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Em Espera</td> 
   <td>O projeto ainda não terminou, mas devido a alguns atrasos, o projeto precisa ser temporariamente suspenso. O gerente do projeto opta por usar esse status para alertar os usuários na equipe do projeto sobre a interrupção do trabalho no projeto, no momento atual.</td> 
   <td> <p>Por padrão, os usuários da equipe do projeto não podem ver o projeto em suas listas de Projetos na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto desaparecem de sua Lista de Trabalho. </p> <p>As decisões de aprovação não podem ser concedidas a tarefas ou emissões.</p> <p>As notificações sobre alterações na linha do tempo, atribuições, ações necessárias, aprovações não são enviadas aos usuários na equipe do projeto.</p> <p> <p><b>OBSERVAÇÃO</b>: Quando você coloca um projeto em espera, a linha do tempo do projeto não é interrompida. O projeto ainda pode ser exibido como Em risco ou Em problemas, mesmo se ninguém estiver trabalhando ativamente no projeto. Alguns ajustes manuais das datas das tarefas pendentes podem ser necessários ao retornar o projeto para Atual novamente, para que o projeto possa mostrar o progresso atualizado.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Solicitado(a)</td> 
   <td>O status do projeto é automaticamente marcado como Solicitado pelo sistema, quando o caso comercial em uma solicitação de projeto foi concluído e enviado para aprovação. Para obter mais informações sobre a solicitação de um projeto usando um caso comercial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Por padrão, os usuários da equipe do projeto não podem ver o projeto em suas listas de Projetos na área Projetos do Workfront. As tarefas e os problemas no projeto que são atribuídos a elas não preenchem a Lista de Trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto por uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Aprovado</td> 
   <td>O status do projeto é automaticamente marcado como Aprovado, quando o caso comercial em uma solicitação de projeto foi aprovado. Para obter mais informações sobre a solicitação de um projeto usando um caso comercial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Os usuários da equipe do projeto podem ver o projeto em suas listas de Projetos por padrão, na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto não preenchem a Lista de trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto por uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>Rejeitado</td> 
   <td>O status do projeto é automaticamente marcado como Rejeitado, quando o caso comercial em uma solicitação de projeto foi rejeitado. Para obter mais informações sobre a solicitação de um projeto usando um caso comercial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Por padrão, os usuários da equipe do projeto não podem ver o projeto em suas listas de Projetos na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto não preenchem a Lista de trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto por uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Ideia</td> 
   <td>O status do projeto é automaticamente marcado como Idea quando você envia uma solicitação do projeto. Para obter mais informações sobre a solicitação de um projeto usando um caso comercial, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Por padrão, os usuários da equipe do projeto não podem ver o projeto em suas listas de Projetos na área Projetos do Workfront. As tarefas e os problemas atribuídos a elas no projeto não preenchem a Lista de trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto por uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Os seguintes status de projeto não podem ser alterados para um status de inativo, em espera ou concluído:
>
>* Solicitado(a)
>* Ideia
>* Aprovado
>* Rejeitada (ou equivalente)
>

