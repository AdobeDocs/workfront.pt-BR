---
content-type: reference
navigation-topic: notifications
title: 'Notificações: aprovações unificadas'
description: As notificações a seguir alertam sobre as atividades de aprovação da experiência de Aprovações unificadas. Para obter informações sobre como configurar as notificações recebidas, consulte Modificar suas próprias notificações por email.
author: Courtney
feature: Get Started with Workfront
exl-id: 6e60a9ec-4fe0-4f3d-a4dd-8dc09d11b834
last-update: 2026-10-20T00:00:00.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: c042179c-157b-516d-b27c-e3bf303e8567
    internal-label: Get Started with Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 7957c410d4a0e39b23b4f5a3d29a794e5deec72a
workflow-type: tm+mt
source-wordcount: '1052'
ht-degree: 0%
---
# Notificações: aprovações unificadas

{{highlighted-preview}}

Use as notificações a seguir para se manter informado sobre a atividade para revisão e aprovações unificadas. Para obter informações sobre como configurar as notificações por email recebidas, consulte [Modificar suas próprias notificações por email](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>Essas notificações estão disponíveis somente como notificações instantâneas e não estão disponíveis em um resumo diário.


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Notificação</th> 
   <th>Campos incluídos</th> 
   <th>Status padrão</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>Aprovação concluída - Aprovada</strong> </p> <p>Uma aprovação de documento termina com uma decisão final de Aprovado.</p> <p>O assunto do email de notificação instantânea é: <em>Decisão final: (Documento) aprovado</em></p> </td> 
   <td> <p>Decisão final<br>Documento<br>Data de solicitação da aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aprovação concluída - Aprovada com alterações</strong> </p> <p>Uma aprovação de documento termina com uma decisão final de Aprovado com alterações.</p> <p>O assunto do email de notificação instantânea é: <em>Decisão final: (Documento) aprovado com alterações</em></p> </td> 
   <td> <p>Decisão final<br>Documento<br>Data de solicitação da aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Aprovação concluída - Precisa de trabalho</strong> </p> <p>Uma aprovação de documento termina com uma decisão final de Trabalho necessário.</p> <p>O assunto do email de notificação instantânea é: <em>Decisão final: (Documento) precisa de trabalho</em></p> </td> 
   <td> <p>Decisão final<br>Documento<br>Data de solicitação da aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Prazo final se aproximando</strong> </p> <p>Uma aprovação de documento da qual você faz parte está se aproximando do prazo.</p> <p>O assunto do email de notificação instantânea é: <em>Prazo de aprovação iminente para (Documento)</em></p> </td> 
   <td> <p>Solicitante<br>Sua função<br>Equipe<br>Data de solicitação da aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Prazo final expirado</strong> </p> <p>Uma aprovação de documento da qual você faz parte ultrapassa o prazo sem uma decisão final.</p> <p>O assunto do email de notificação instantânea é: <em>Prazo de aprovação expirado para (Documento)</em></p> </td> 
   <td> <p>Corrigido o título<br>Data de solicitação de aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Estágio</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Revisão concluída</strong> </p> <p>Um revisor conclui sua revisão em uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>(Documento) foi revisado</em></p> </td> 
   <td> <p>Revisor<br>Documento<br> Botão "Ir para revisão"<br>Bloco de detalhes: nome do documento, detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando faz parte da aprovação:</em><br>Visualização do documento<br>Estágio<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Limite de aprovação de vídeo se aproximando (80%)</strong> </p> <p>Uma aprovação de vídeo atinge 80% do limite de aprovação de vídeo do seu plano.</p> <p>O assunto do email de notificação instantânea é: <em>Você está perto do limite anual de solicitações de aprovação de vídeo no Workfront</em></p> </td> 
   <td> Título e texto do corpo<br>Solicitação de aprovações de vídeo (uso atual)<br>Limite total (o limite)<br>Outros destinatários<br>"Botão Exibir no Workfront"<br>"Botão Atualizar para empresa FIO" </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Limite de aprovação de vídeo atingido</strong> </p> <p>Uma aprovação de vídeo atinge o limite de aprovação de vídeo do plano.</p> <p>O assunto do email de notificação instantânea é: <em>Você atingiu o limite anual de solicitações de aprovação de vídeo no Workfront</em></p> </td> 
   <td> Título e texto do corpo<br>Solicitação de aprovações de vídeo (uso atual)<br>Limite total (o limite)<br>Outros destinatários<br>"Botão Exibir no Workfront"<br>"Botão Atualizar para empresa FIO" </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisão tomada - Aprovada</strong> </p> <p>Um aprovador toma uma decisão de Aprovado em uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>(Documento) aprovado por (Nome)</em></p> </td> 
   <td> <p>Tomador de decisão<br>Decisão<br>Documento e versão<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisão tomada - Aprovada com alterações</strong> </p> <p>Um aprovador toma uma decisão de Aprovado com alterações em uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>(Documento) aprovado com alterações por (Nome)</em></p> </td> 
   <td> <p>Tomador de decisão<br>Decisão<br>Documento e versão<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Decisão tomada - Precisa funcionar</strong> </p> <p>Um aprovador toma a decisão de Precisa trabalhar em uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>(Documento) precisa ser trabalhado por (Nome)</em></p> </td> 
   <td> <p>Tomador de decisão<br>Decisão<br>Documento e versão<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Documentos adicionados ou removidos de uma aprovação agrupada</strong> </p> <p>Os documentos são adicionados ou removidos de uma aprovação de documento agrupada da qual você faz parte.</p> <p>O assunto do email de notificação instantânea é: <em>Um documento foi adicionado ou removido de uma aprovação da qual você faz parte</em></p> </td> 
   <td> <p><strong>Adicionado:</strong><br>Solicitante<br>Nome do grupo<br>Visualização da miniatura<br>Datas<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do grupo, Número de ativos, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Mensagem personalizada<br>Projeto</p> <p><strong>Removido:</strong><br>Solicitante<br>Nome do grupo<br>Visualização da miniatura (nenhum botão ou bloco de Detalhes)</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Todas as revisões concluídas</strong> </p> <p>Cada revisor conclui sua revisão em uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>Todas as revisões foram concluídas em (Documento)</em></p> </td> 
   <td> <p>Documento<br>Data de solicitação de aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lembrete - 24 horas</strong> </p> <p>Você tem 24 horas para revisar e aprovar o documento.</p> <p>O assunto do email de notificação instantânea é: <em>Lembrete: sua aprovação é necessária em (Documento)</em></p> </td> 
   <td> <p>Solicitante<br>Sua função<br>Equipe<br>Data de solicitação da aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Lembrete - 72 horas</strong> </p> <p>Você tem 72 horas para revisar e aprovar o documento.</p> <p>O assunto do email de notificação instantânea é: <em>Lembrete: sua aprovação é necessária em (Documento)</em></p> </td> 
   <td> <p>Solicitante<br>Sua função<br>Equipe<br>Data de solicitação da aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adicionado como aprovador ou revisor</strong> </p> <p>Você foi adicionado como aprovador ou revisor em uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>Sua aprovação é necessária em (Documento)</em></p> </td> 
   <td> <p>Solicitante<br>Sua função<br>Equipe<br>Data de solicitação da aprovação<br>Data de vencimento<br>"Botão Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada<br>Preparo<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Removido como aprovador ou revisor</strong> </p> <p>Você foi removido como aprovador ou revisor de uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>Sua aprovação não é mais necessária em (Documento)</em></p> </td> 
   <td> <p>Solicitante<br>Documento e versão<br>Função<br>Equipe (nenhum botão ou bloco Detalhes)</p> <p><em>Incluído quando parte da aprovação:</em><br>Visualização do documento<br>Mensagem personalizada</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Função alterada</strong> </p> <p>Sua função de aprovador ou revisor é alterada em uma aprovação de documento.</p> <p>O assunto do email de notificação instantânea é: <em>Sua função no (Documento) foi alterada</em></p> </td> 
   <td> <p>Solicitante<br>Documento e versão<br>Alteração da direção da função<br> Botão "Ir para revisão"<br>Bloco de detalhes: Nome do documento, Detalhes do documento, Todos os destinatários</p> <p><em>Incluído quando faz parte da aprovação:</em><br>Visualização do documento<br>Estágio<br>Projeto</p> </td> 
   <td><strong>Instantâneo</strong> </td> 
  </tr> 
 </tbody> 
</table>
