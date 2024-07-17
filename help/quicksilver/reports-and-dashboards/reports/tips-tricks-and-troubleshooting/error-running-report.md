---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "Mensagem de erro ao executar um relatório: 'Você não está conectado no momento'."
description: Saiba mais sobre a mensagem de erro "Você não está conectado no momento".
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 3%

---

# Mensagem de erro ao executar um relatório: &quot;Você não está conectado no momento&quot;.

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
   <td> <p>Gerenciar permissões para um relatório</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

## Problema

Ao executar um relatório ou exibi-lo em um painel, o seguinte erro retorna:\
*Vamos tentar novamente. Você não está logado no momento.*

Nenhum resultado é exibido no relatório.

## Causa

No momento, o relatório está definido para ser executado como um usuário desativado.

## Solução

Você deve ter permissões de gerenciamento no relatório para poder alterar as configurações do relatório.\
Para ajustar o relatório e ver os resultados:

1. Vá para o relatório.
1. Clique em **Ações de Relatório** > **Editar** > **Configurações de Relatório**.

1. Especifique o nome de um usuário ativo no **Execute este relatório com os Direitos de Acesso do campo:**.\
   Ou\
   Deixe em branco o **Executar este relatório com os Direitos de Acesso do campo:**.

1. Clique em **Concluído**.
1. Clique em **Salvar + Fechar**.\
   O erro não deve aparecer novamente ao executar este relatório.
