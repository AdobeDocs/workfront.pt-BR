---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Mensagem de erro no calendário: ''Este calendário tem os direitos de exibição de um usuário desativado''.'
description: Saiba mais sobre a mensagem de erro "Este calendário tem os direitos de exibição de um usuário desativado".
author: Jenny
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 1%

---

# Mensagem de erro no calendário: &quot;Este calendário tem os direitos de exibição de um usuário desativado&quot;.

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
     <p>Standard</p>
     <p>Trabalhar ou superior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um calendário</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Problema

Você recebe o seguinte erro ao acessar um calendário compartilhado com você: 

*Este calendário tem os direitos de exibição de um usuário desativado. Peça a um administrador que corrija os privilégios do calendário.*

## Causa

O usuário que criou este calendário (seu proprietário original) é um usuário que foi desativado. 

## Solução

Você pode resolver isso da seguinte maneira:

1. Copiar o calendário original. Ao copiar um calendário, você se torna o proprietário do calendário. O calendário copiado deve mostrar todas as informações do calendário original.\
   Para obter mais informações sobre como copiar um calendário, consulte [Copiar um relatório de calendário](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. Compartilhar o calendário copiado com os mesmos usuários do calendário original. Todos os usuários devem ver as mesmas informações no novo calendário.
1. (Opcional e condicional) Se você tiver permissões para gerenciar o calendário original, remova todos os outros usuários com os quais o calendário é compartilhado da área de Compartilhamento do calendário. Isso elimina a confusão dos usuários que estão tentando exibir o calendário errado.
