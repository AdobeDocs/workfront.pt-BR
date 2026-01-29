---
title: Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning
description: Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.
feature: Workfront Planning
role: User, Admin
author: Alina, Becky
recommendations: noDisplay, noCatalog
exl-id: 058148db-1795-4d39-be87-271008ae3d47
source-git-commit: f5d6918889b7fed1159274105ee706a027f621bf
workflow-type: tm+mt
source-wordcount: '1192'
ht-degree: 1%

---

# Adicionar uma aprovação a um formulário de solicitação no Adobe Workfront Planning

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--take Preview and Production references at Production time-->

<span class="preview">As informações destacadas nesta página referem-se a funcionalidades que ainda não estão disponíveis. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes. Depois das versões mensais para produção, os mesmos recursos também ficam disponíveis no ambiente de produção para clientes que ativaram versões rápidas. </span>

<span class="preview">Para obter informações sobre versões rápidas, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Você pode adicionar um processo de aprovação a um formulário de solicitação do Adobe Workfront Planning para iniciar uma aprovação para cada solicitação submetida, antes que ele crie um registro.

Este artigo descreve como um gerente de espaço de trabalho pode adicionar uma aprovação a um formulário de solicitação associado a um tipo de registro.

Para obter informações sobre como criar um formulário de solicitação no Workfront Planning, consulte [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

Para obter informações sobre como enviar uma solicitação a um tipo de registro para criar um registro, consulte [Enviar solicitações do Adobe Workfront Planning para criar registros](/help/quicksilver/planning/requests/submit-requests.md).

## Requisitos de acesso

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
<p>Qualquer pacote do Workfront e qualquer pacote do Planning</p>
Ou
<p>Qualquer pacote de fluxo de trabalho e qualquer pacote de planejamento</p>

<p>Para obter mais informações sobre o que está incluído em cada pacote do Workfront Planning, entre em contato com o representante de conta da Workfront.</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Padrão</p> 
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

## Adicionar uma aprovação a um formulário de solicitação no ambiente de produção

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
   >* Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o registro não será criado. A solicitação permanece na área Solicitações do Workfront.
   >
   >* Se você adicionar mais de um aprovador e a opção Somente uma decisão é obrigatória não estiver ativada, todos os aprovadores deverão tomar uma decisão antes que uma solicitação seja aprovada ou rejeitada.
   >
   >* Se uma equipe estiver definida como um aprovador, somente uma decisão será necessária da equipe.


1. (Opcional) Clique em **Publicar** se você nunca compartilhou o formulário de solicitação antes.

   Ou

   Clique em **Compartilhar** para compartilhar o formulário e em **Copiar link**.
1. (Opcional) Depois que um usuário usa o link compartilhado e envia uma solicitação, o Workfront Planning envia uma notificação de aprovação no aplicativo e um email aos aprovadores.

   >[!NOTE]
   >
   >   A instância da Workfront de sua organização deve ser integrada à Adobe Unified Experience para que os usuários possam receber notificações por email e no aplicativo.


   Para obter informações sobre aprovação de solicitações, consulte [Aprovar uma solicitação](/help/quicksilver/planning/requests/approve-request.md).

<div class="preview">

## Adicionar regras de aprovação a um formulário de solicitação

>[!NOTE]
>
>Essa funcionalidade está disponível somente no ambiente de Pré-visualização.

As regras de aprovação definem o processo de aprovação com base nos valores de campo em nas solicitações enviadas.

Por exemplo, se um formulário de solicitação tiver o campo &quot;Tipo de campanha&quot;, poderá ser criada uma regra que envia a solicitação para uma pessoa quando o campo tem o valor &quot;Digital&quot; e outra pessoa quando ele tem o valor &quot;Imprimir&quot;.

Considere o seguinte ao adicionar regras de aprovação:

* Você pode adicionar um ou vários aprovadores a uma regra de aprovação.
* Se pelo menos um aprovador rejeitar a solicitação, ela será rejeitada e o registro não será criado. A solicitação permanece na área Solicitações do Workfront.
* Se você adicionar mais de um aprovador e a opção Somente uma decisão é obrigatória não estiver ativada, todos os aprovadores deverão tomar uma decisão antes que uma solicitação seja aprovada ou rejeitada.
* Se uma equipe for definida como um aprovador, somente uma decisão será necessária para um membro da equipe.

Para definir regras de aprovação para um formulário de solicitação:

1. Comece a criar um formulário de solicitação para um tipo de registro, conforme descrito em [Criar e gerenciar um formulário de solicitação no Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).
1. Clique em **Configurações**.

   A guia Settings é exibida.

1. Para começar a configurar as regras de aprovação, clique em **Aprovações** ![ícone Aprovações](assets/approvals-icon-on-form.png) no painel esquerdo.

1. (Opcional) Se quiser definir um processo de aprovação padrão, adicione pelo menos um usuário ou equipe ao campo **Aprovadores** da área **Regra de aprovação padrão** e clique na caixa de seleção **Somente uma decisão é necessária** se quiser que o registro seja criado depois que qualquer um dos aprovadores padrão o aprovar.

   ![Área de regra de aprovação padrão](assets/default-approvers.png)

   <!--below bullet list is duplicated in the Add approval to a request form article-->

1. (Opcional) Comece a adicionar regras de aprovação. Para cada regra de aprovação, faça o seguinte:

   1. Clique em **Adicionar regra de aprovação**
   1. Clique no título do espaço reservado **Regra de aprovação sem título** e insira um nome para a regra de aprovação.
   1. Clique em **Selecionar um campo** e selecione o campo que ativa a regra.
   1. Selecione o operador para a regra. Os operadores variam de acordo com o tipo de campo.
   1. Se o operador selecionado exigir um valor, clique no ícone de adição e adicione um ou mais valores.
   1. (Opcional) Clique em **Adicionar condição** para adicionar mais condições e conectá-las por instruções **And** ou **Or** configurando as condições adicionais como nas etapas C-E.
   1. Na área **Ações** da regra de aprovação, no campo **Aprovadores**, adicione pelo menos um usuário ou equipe a ser definido como o aprovador quando a condição for atendida.
   1. (Condicional) Se desejar que o registro seja criado depois que qualquer um dos aprovadores o aprovar, marque a caixa de seleção **Somente uma decisão é necessária**.

1. Clique em **Salvar** para salvar as regras de aprovação.
1. (Opcional) Clique em **Publicar** se você nunca compartilhou o formulário de solicitação antes.

</div>
