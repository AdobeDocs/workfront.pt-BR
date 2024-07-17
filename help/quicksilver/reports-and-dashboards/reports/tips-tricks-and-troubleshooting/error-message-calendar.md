---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Mensagem de erro no calendário: 'Este calendário tem os direitos de exibição de um usuário desativado'."
description: Saiba mais sobre a mensagem de erro "Este calendário tem os direitos de exibição de um usuário desativado".
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 0%

---

# Mensagem de erro no calendário: &quot;Este calendário tem os direitos de exibição de um usuário desativado&quot;.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano, Trabalho</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões de um calendário</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

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
