---
product-area: documents
navigation-topic: approvals
title: Fazer upload de uma nova versão do documento e solicitar uma aprovação
description: Você pode fazer upload de uma nova versão do documento e solicitar aprovação de outros usuários no Adobe Workfront.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 8270a107ba2501eddbb27f52c843c337aa1f8a99
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---

# Fazer upload de uma nova versão do documento e solicitar uma aprovação

Se um documento estiver marcado e precisar de trabalho em uma revisão anterior, você poderá fazer upload de uma nova versão para o documento original e iniciar outra rodada de aprovações. Após carregar uma nova versão do documento, as versões anteriores serão bloqueadas.

Se o nome do arquivo da nova versão for diferente do nome do arquivo da versão anterior, o Workfront exibirá o documento com o nome de arquivo mais recente.

Quando uma nova versão é adicionada a um documento com aprovações pendentes, a aprovação da versão anterior é exibida como Retirado. O processo de aprovação anterior é encerrado, mesmo que alguns participantes ainda não tenham tomado uma decisão.

Se a versão mais recente do documento for excluída, as versões anteriores permanecerão bloqueadas. Se precisar editar uma versão anterior, desbloqueie-a manualmente.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p> Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licenças da Adobe Workfront*</td> 
   <td> <p>Atual: solicitação ou superior</p>
   ou
   <p>Novo: Colaborador ou superior</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a documentos</p> <p>Observação: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Editar acesso ao objeto associado ao documento</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">Solicitar acesso aos objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para descobrir seu plano, tipo de licença ou acesso, entre em contato com o administrador do Workfront.

+++

## Usar o recurso arrastar e soltar para adicionar uma nova versão

>[!NOTE]
>
>Arrastar e soltar não funciona com o Internet Explorer.

1. Vá para a área Documentos onde o documento é carregado.
1. Na área de trabalho ou em uma guia separada do navegador, arraste a nova versão do documento para cima da versão existente no Workfront.

   Ao arrastar a nova versão, é possível passar o mouse sobre uma pasta de documentos do Workfront para abri-la. Você pode rolar para cima e para baixo arrastando os arquivos até a parte superior ou inferior da tela.

1. Solte a nova versão sobre o arquivo existente na guia **Documentos**.

1. Depois que o documento for carregado, clique nele e abra o painel Resumo do documento.

1. Role para baixo até a seção **Aprovações** no painel Resumo do documento e clique em **Adicionar**.

![Adicionar aprovadores no resumo do documento](assets/doc-summary-add-approvers.png)

1. (Opcional) Defina um prazo para a aprovação. Os usuários e as equipes são notificados por email 72 horas e, em seguida, 24 horas antes do prazo especificado.

1. Para adicionar rapidamente revisores e aprovadores da versão anterior, clique no botão adicionar ao lado dos nomes listados abaixo.
   <!--need screenshot when working-->

1. (Opcional) altere a função de aprovador/revisor.

1. Para adicionar novos aprovadores e revisores, clique em **Revisor** ou **Aprovador** e comece a digitar o usuário ou a equipe.

   ![Adicionar aprovador e prazo final](assets/add-approver-and-deadline.png)
