---
user-type: administrator
content-type: reference;how-to-procedural
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
title: Status de projeto do sistema
description: O Workfront tem 9 status de projeto de sistema incorporados. Os primeiros 3 na tabela abaixo são obrigatórios, o que significa que você pode desbloqueá-los, renomeá-los e reordená-los, mas não pode ocultá-los ou excluí-los. A alteração do status de um projeto geralmente é um processo manual. No entanto, às vezes, o status de um projeto é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6b8dd52b-1696-4e5d-bcbb-5b6d3b736df0
source-git-commit: f4ef463ebdc9a4a7a0802e5394d7820ebc447aa9
workflow-type: tm+mt
source-wordcount: '1572'
ht-degree: 0%

---

# Status de projeto do sistema

O Workfront tem 9 status de projeto de sistema incorporados.

Os primeiros 3 na tabela abaixo são obrigatórios, o que significa que você pode desbloqueá-los, renomeá-los e reordená-los, mas não pode ocultá-los ou excluí-los.

A alteração do status de um projeto geralmente é um processo manual. No entanto, há alguns cenários descritos na lista a seguir quando o status de um projeto é alterado automaticamente, dependendo de outros fatores que estão acontecendo no sistema.

Os seguintes status de projeto são fornecidos com a instância do Workfront:

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
   <th>Este status de projeto ocorre quando</th> 
   <th>O que acontece neste status</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Planejamento (status obrigatório)</td> 
   <td> <p>O gerente de projeto está planejando a linha do tempo do projeto, a atribuição das tarefas e as aprovações. O gerente de projeto define esse status em um projeto manualmente.</p> <p><b>DICA</p> <p> Recomendamos que você defina o status padrão para novos projetos no Workfront como Planning. Como administrador do Workfront, você pode alterar o status padrão de todos os novos projetos na área Projetos das Preferências do projeto.</p> </td> 
   <td> <p>Os usuários na equipe do projeto podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto não preenchem sua Lista de trabalho. Somente aprovações e itens de trabalho aceitos são exibidos na Lista de trabalho da página inicial.</p> <p>Nenhuma notificação é enviada enquanto um projeto tem esse status.</p> <p>Recomendamos que todas as alterações que podem acionar uma atualização na linha do tempo do projeto, ou qualquer alteração nas atribuições de tarefas e problemas, sejam feitas enquanto o projeto estiver no status Planejamento. Isso minimiza a quantidade de notificações que os usuários recebem.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Atual (status obrigatório)</td> 
   <td> <p>Os usuários estão trabalhando nisso. O gerente de projeto deve transformar um projeto em Atual para sinalizar que ele foi iniciado.</p> <p>Este é o status padrão para novos projetos no Workfront.</p> <p><b>DICA</b></p>

<p> Como administrador do Workfront, você pode alterar o status padrão para novos projetos na área Projetos das Preferências do projeto. Para obter mais informações, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </td> 
   <td> <p>Os usuários na equipe do projeto podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto preenchem sua Lista de trabalho. Eles podem começar a aceitar trabalhos em tarefas e problemas e movê-los para a lista Trabalhando em.</p> <p>Além disso, em um projeto Atual, todas as notificações sobre alterações na linha do tempo, atribuições, ações necessárias e aprovações são enviadas aos usuários na equipe do projeto.</p> <p>E a linha do tempo do projeto é calculada automaticamente pelo sistema, se o Tipo de atualização do projeto estiver definido como Automático, Ao alterar ou Automático e Ao alterar.</p> <p>Dica: é uma boa ideia manter os ajustes do plano do projeto em um nível mínimo quando um projeto estiver com esse status, para que os usuários não recebam muitas notificações.</p> </td> 
  </tr> 
  <tr> 
   <td>Concluído (status obrigatório)</td> 
   <td> <p> O projeto foi concluído:</p> 
     <p>Se o Modo de conclusão do projeto estiver definido como Manual, o gerente de projeto escolherá esse status manualmente para informar aos usuários na equipe do projeto que eles devem parar de trabalhar no projeto.</p> 
    <p>Se o Modo de conclusão do projeto estiver definido como Automático, o Workfront marcará automaticamente um projeto como Concluído quando todas as tarefas e problemas no projeto forem marcados como Concluídos. 
    <p><b>IMPORTANTE</b> </p>
    <p>Você pode marcar um projeto como Concluído somente quando todas as tarefas, problemas e aprovações do projeto forem resolvidas.</p> </td> 
   <td>
    <p>Os usuários na equipe do projeto não podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto não preenchem suas listas de Solicitações de trabalho ou Trabalhando em. </p>
    <p>Todas as notificações relacionadas ao projeto, exceto uma notificação de alteração de status, param de ser enviadas aos usuários na equipe do projeto.</p>
    <p>A linha do tempo do projeto não é mais calculada pelo sistema. </p>
    <p>Não é possível copiar o projeto.</p>
    <p>Você pode impedir que os usuários executem ações adicionais quando um projeto é marcado como Concluído. </p><p>Para obter mais informações sobre como restringir ações em projetos marcados como Concluídos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p></td> 
  </tr> 
  <tr> 
   <td>Parado</td> 
   <td>O projeto ainda não foi concluído, mas devido a bloqueios ou alterações no escopo, o projeto não pode continuar a ser trabalhado e foi abandonado. O gerente de projeto altera o status para Desativado para alertar os usuários na equipe do projeto de que este projeto nunca será concluído e que eles não devem mais trabalhar nele.</td> 
   <td> <p>Os usuários na equipe do projeto não podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto desaparecem da Lista de trabalho.</p> <p>Decisões de aprovação não podem ser concedidas a tarefas ou problemas.</p> <p>Notificações sobre alterações de linha do tempo, atribuições, ações necessárias e aprovações não são enviadas aos usuários na equipe do projeto.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema, pois o projeto é percebido como concluído.</p> <p>Você pode impedir que os usuários executem determinadas ações quando um projeto é marcado como Desativado. Para obter mais informações sobre como restringir ações em projetos mortos, consulte <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">Configurar preferências de projeto em todo o sistema</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Em Espera</td> 
   <td>O projeto ainda não foi concluído, mas devido a alguns atrasos, o projeto precisa ser temporariamente suspenso. O gerente de projeto escolhe usar esse status para alertar os usuários na equipe do projeto para que parem de trabalhar no projeto, no momento atual.</td> 
   <td> <p>Os usuários na equipe do projeto não podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto desaparecem da Lista de trabalho. </p> <p>Decisões de aprovação não podem ser concedidas a tarefas ou problemas.</p> <p>Notificações sobre alterações de linha do tempo, atribuições, ações necessárias e aprovações não são enviadas aos usuários na equipe do projeto.</p> <p> <p><b>NOTA</b>: quando você coloca um projeto em espera, a linha do tempo do projeto não para. O projeto ainda pode ser exibido como Em risco ou Com problema, mesmo se ninguém estiver trabalhando ativamente no projeto. Alguns ajustes manuais das datas das tarefas abertas restantes podem ser necessários ao retornar o projeto para Atual novamente, para que o projeto possa mostrar o progresso atualizado.</p> </p> </td> 
  </tr> 
  <tr> 
   <td>Solicitado(a)</td> 
   <td>O status do projeto é marcado automaticamente como Solicitado pelo sistema quando o business case de uma solicitação de projeto é concluído e enviado para aprovação. Para obter mais informações sobre como solicitar um projeto usando um business case, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Os usuários na equipe do projeto não podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas no projeto atribuídos a eles não preenchem sua Lista de trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Aprovado</td> 
   <td>O status do projeto é marcado automaticamente como Aprovado, quando o business case de uma solicitação de projeto for aprovado. Para obter mais informações sobre como solicitar um projeto usando um business case, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Os usuários na equipe do projeto podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto não preenchem sua Lista de trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema. </p> </td> 
  </tr> 
  <tr> 
   <td>Rejeitado</td> 
   <td>O status do projeto é marcado automaticamente como Rejeitado, quando o business case de uma solicitação de projeto for rejeitado. Para obter mais informações sobre como solicitar um projeto usando um business case, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Os usuários na equipe do projeto não podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto não preenchem sua Lista de trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
  <tr> 
   <td>Ideia</td> 
   <td>O status do projeto é marcado automaticamente como Ideia ao enviar uma solicitação de projeto. Para obter mais informações sobre como solicitar um projeto usando um business case, consulte <a href="../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md" class="MCXref xref">Revisar projetos solicitados</a>.</td> 
   <td> <p>Os usuários na equipe do projeto não podem ver o projeto em suas listas de Projetos por padrão (sem um filtro personalizado), na área Projetos do Workfront. As tarefas e problemas atribuídos a eles no projeto não preenchem sua Lista de trabalho.</p> <p>Todas as notificações relacionadas ao projeto, exceto uma notificação de alteração de status, não são enviadas a nenhum usuário.</p> <p>A linha do tempo do projeto não é calculada automaticamente pelo sistema.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>Os status de projeto a seguir não podem ser alterados para um status Morto, Em espera ou Concluído:
>
>* Solicitado(a)
>* Ideia
>* Aprovado
>* Rejeitado (ou seu equivalente)
>
