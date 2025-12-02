---
title: Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning
description: Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: de568156315ff9094d938600c91b55e185d53765
workflow-type: tm+mt
source-wordcount: '688'
ht-degree: 0%

---

# Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.

Este artigo descreve como um gerente de espaço de trabalho pode adicionar uma aprovação a um formulário de solicitação associado a um tipo de registro.

Para obter informações sobre como criar um formulário de solicitação no Workfront Planning, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Para obter informações sobre como enviar uma solicitação a um tipo de registro para criar um registro, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Pacotes Adobe Workfront</p></td> 
   <td> 
<p>Qualquer pacote do Workfront e qualquer pacote do Planning</p>
Ou
<p>Qualquer pacote de fluxo de trabalho e qualquer pacote de planejamento</p>

<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Standard</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>   <p>Gerenciar permissões para um espaço de trabalho e tipo de registro</a> </p>  
   <p>Os administradores do sistema têm permissões para todos os espaços de trabalho, incluindo aqueles que não criaram</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obter mais informações sobre requisitos de acesso do Workfront, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações sobre a adição de aprovações a um formulário de solicitação

* Você pode adicionar um ou vários aprovadores a um formulário de solicitação. Você pode adicionar somente usuários como aprovadores.
* Você pode exibir informações de aprovação em um registro criado submetendo um formulário de solicitação nos campos Aprovado por e Data de aprovação. Para obter informações, consulte [Criar campos](/help/quicksilver/planning/fields/create-fields.md).
* Quando você adiciona vários aprovadores a um formulário de solicitação, todos os aprovadores devem aceitar a solicitação antes que um registro seja criado no Workfront Planning.
* Se todos os aprovadores aprovarem a solicitação, um registro será criado para o tipo de registro associado ao formulário de solicitação.
* Se pelo menos um aprovador rejeitar a solicitação e todos os outros aprovarem, uma solicitação será criada para a área Solicitações no Workfront, mas nenhum registro será criado para o tipo de registro associado ao formulário de solicitação.
* Adicionar aprovações a um formulário de solicitação é opcional. O Workfront Planning cria imediatamente um registro quando uma solicitação é submetida, se o form de solicitação não estiver associado a uma aprovação.

## Adicionar uma aprovação a um formulário de solicitação

1. Comece a criar um formulário de solicitação para um tipo de registro, conforme descrito em [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Clique em **Configuração**.

   A área **Configuração** é exibida.

   ![Guia Configuração](assets/configuration-tab.png)
1. No campo **Aprovadores**, comece digitando o nome de um usuário ou equipe que você deseja definir como um aprovador, em seguida, selecione-o quando ele for exibido na lista.
1. (Opcional e condicional) Se você tiver definido mais de um aprovador e só precisar de um aprovador para tomar uma decisão, habilite a opção **Somente uma decisão é necessária**.

   <!--most of the Note below is duplicated in the Create a request form article-->

   >[!NOTE]
   >
   >
   >* Você pode adicionar um ou vários aprovadores a um formulário de solicitação.
   >
   >* Se você adicionar mais de um aprovador e a opção Somente uma decisão é necessária não estiver ativada, todos os aprovadores deverão aprovar a solicitação antes que o Workfront Planning crie um registro.
   >
   >* Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o registro não será criado. A solicitação permanece na guia Planejamento da seção Enviado na área Solicitações do Workfront.
   >
   >* Se você adicionar mais de um aprovador e a opção Somente uma decisão é obrigatória não estiver ativada, todos os aprovadores deverão tomar uma decisão antes que uma solicitação seja aprovada ou rejeitada.
   >
   >* Se uma equipe estiver definida como um aprovador, somente uma decisão será necessária da equipe.


1. (Opcional) Clique em **Publicar** se você nunca compartilhou o formulário de solicitação antes

   Ou

   Clique em **Compartilhar** para compartilhar o formulário e em **Copiar link**.
1. (Opcional) Depois que um usuário usa o link compartilhado e envia uma solicitação, o Workfront Planning envia uma notificação de aprovação no aplicativo e um email aos aprovadores.

   >[!NOTE]
   >
   >   A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para que os usuários possam receber notificações por email e no aplicativo.


   Para obter informações sobre aprovação de solicitações, consulte [Aprovar uma solicitação](/help/quicksilver/planning/requests/approve-request.md).
