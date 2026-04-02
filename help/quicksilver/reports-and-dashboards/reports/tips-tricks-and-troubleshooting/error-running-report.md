---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Mensagem de erro ao executar um relatório: ''Você não está conectado no momento''.'
description: Saiba mais sobre a mensagem de erro "Você não está conectado no momento".
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 31%

---

# Mensagem de erro ao executar um relatório: “Você não está conectado(a) no momento.”

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
     <p>Padrão</p>
     <p>Trabalho ou maior</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a relatórios, painéis, calendários</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Gerenciar permissões para um relatório</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações contidas nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


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
