---
title: Introdução ao Adobe Workfront Planning Designer
description: Usando o Adobe Planning Designer, você pode gerar um novo espaço de trabalho, completo com tipos de registro e campos no Workfront Planning, adicionar objetos a um espaço de trabalho ou exibir o histórico de alterações em registros.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 1%

---


# Introdução ao Adobe Workfront Planning Designer

{{planning-important-intro}}

Usando o Adobe Planning Designer, você pode gerar um novo espaço de trabalho, completo com tipos de registro e campos no Workfront Planning, adicionar objetos a um espaço de trabalho ou exibir o histórico de alterações em registros.

>[!IMPORTANT]
>
>No momento, o Planning Designer está disponível apenas para usuários que participam do estágio beta fechado.

## Requisitos de acesso <!--edit theses-->

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e do Planning</p>
<p>Qualquer pacote de Fluxo de Trabalho e Planejamento</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inscrevendo-se no programa Beta Fechado para o Designer de Planejamento

<!--edit this Or create a new article under Beta programs?? -->

Atualmente, você pode solicitar a participação no programa Beta Fechado para o Designer de Planejamento.

## Considerações sobre o Planning Designer

<!--these are from the AI Assistant - edit these-->

* Para usar o Planning Designer, primeiro é necessário habilitar o Assistente de IA para sua organização. O seguinte deve estar ativado para que o Assistente de IA esteja disponível para todos em sua organização:

   * O Assistente de IA deve estar ativado para sua organização antes de estar disponível para usuários em sua empresa. Para obter informações, consulte [Visão geral do Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
   * Depois que a Workfront ativar o Assistente de IA para sua organização, ele estará disponível para o administrador principal do Workfront. Para obter informações, consulte [Configurar informações básicas do sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

   * O administrador do Workfront deve ativar o Assistente de IA para todos os outros usuários. Para obter mais informações, consulte [Habilitar ou desabilitar o Assistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

   * O Assistente de IA funciona no contexto de cada página. As solicitações que você está enviando para o Assistente de IA devem fazer referência à funcionalidade que está disponível na página que você abriu.

* Para usar o Planning Designer, um administrador do sistema deve habilitá-lo na área Preferências do Sistema da sua Configuração.

* As ações executadas pelo Assistente de IA na área Planejamento se encontram no contexto das permissões do Workfront Planning e do nível de acesso do Workfront. Para obter informações, consulte os seguintes artigos:

   * [Visão geral das permissões de compartilhamento no Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Visão geral do tipo de licença ao usar o Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* As alterações feitas pelo Assistente de IA em nome do usuário são rastreadas no painel Histórico do registro.

* Você pode usar comandos para desfazer suas ações. Por exemplo, você pode digitar &quot;Desfazer a última alteração&quot; para reverter a alteração.

* Ao criar, atualizar ou excluir um objeto por meio do AI Assistant, o AI Assistant exibe as ações desejadas e solicita a confirmação. Você pode confirmar ou cancelar as ações.

—>

## Funcionalidade atualmente disponível para o Planning Designer

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

Você pode usar o Planning Designer ou o Assistente de IA para executar qualquer uma das seguintes ações:

* Criar e configurar espaços de trabalho

* Criar tipos de registro

* Criar campos ou campos de fórmula

* Criar, excluir, duplicar e restaurar registros

* Editar, atualizar, anexar um campo em um registro

* Vincular registros a outros registros

* Acessar histórico de alterações de registro

* Criar exibições personalizadas

* Criar registros importando um documento. A criação de registros a partir de um documento importado está disponível somente no Planning Designer, e não no AI Assistant. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Localize a Designer do Planning no Workfront Planning

É possível acessar o Planning Designer na página principal do Workfront Planning.

<!--add screen shot-->

Você também pode usar o Assistente de IA para aproveitar a mesma funcionalidade que o Planning Designer oferece.

## Ativar o Designer de planejamento para sua organização

Como administrador do Workfront, você deve primeiro habilitar o Planning Designer para sua organização.

<!--add steps here-->

## Criar ou atualizar objetos usando o Planning Designer

Você pode criar ou atualizar objetos no Workfront Planning usando o Planning Designer ou o Assistente de IA, a menos que especificado de outra forma.

1. Faça logon no Workfront e clique no ícone **Menu Principal**, ![Menu principal Pontos](assets/dots-main-menu.png), no canto superior direito da tela, ou no ícone **Menu Principal**, ![Menu principal Linhas](assets/lines-main-menu.png), no canto superior esquerdo, se disponível.

1. Clique em **Planning**. A área Planejamento é aberta.

1. Clique em **Design com IA**.

1. No espaço fornecido, comece a digitar comandos para o Assistente de IA e, em seguida, clique em Inserir quando terminar.

   <!--add screen shot-->

   Por exemplo, você pode digitar uma solicitação semelhante às seguintes:

   * Crie e configure um espaço de trabalho com cinco tipos de registro para gerenciar campanhas

   * Criar campanhas de marketing para cada mês do ano atual

   * Adicionar um campo de campanha para o Status do espaço de trabalho de Design de marketing

   * Excluir todos os registros em um Status de Obsoleto

   * Atualizar todas as campanhas do Planning para um status Ativo

   * Conectar campanhas a personalidades no espaço de trabalho de Design de marketing

   * Exibir o histórico de alterações para a campanha &quot;Dia dos namorados&quot;

   * Crie uma exibição de linha do tempo para campanhas no espaço de trabalho de Design de marketing

   * Criar registros importando um documento. A criação de registros a partir de um documento importado está disponível somente no Planning Designer, e não no AI Assistant.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

   Uma visualização visual é exibida com uma amostra do que o Assistente pode criar.

1. Depois de receber uma resposta bem-sucedida, siga os links fornecidos na linha de comando para criar, atualizar ou revisar o objeto de sua solicitação.




