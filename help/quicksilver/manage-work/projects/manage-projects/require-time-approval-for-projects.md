---
product-area: projects
navigation-topic: manage-projects
title: Exigir tempo para ser aprovado para um projeto
description: Exigir tempo para ser aprovado para um projeto
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 0%

---

# Exigir tempo para ser aprovado para um projeto

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: THIS IS LINKED TO THE UI IN A TOOLTIP IN THE EDIT PROJECT MODAL) </p>
-->

Você pode configurar o projeto para exigir que as horas registradas no projeto sejam aprovadas pelo Proprietário do projeto. Quando configurado dessa forma, as horas devem ser aprovadas primeiro pelo Proprietário do projeto antes que possam ser elegíveis para serem usadas em um registro de cobrança.\
Para obter mais informações sobre registros de faturamento, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Habilitar essa opção não remove a capacidade de um aprovador da folha de ponto aprovar a hora na folha de ponto. Se o Proprietário do projeto não aprovar ou rejeitar a hora, um aprovador da folha de ponto ainda poderá aprovar a hora em uma folha de ponto.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront*</td> 
   <td> <p>Qualquer Um</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Plano para exigir tempo para ser aprovado no projeto</p>
   <p>Revisar ou superior para aprovar horas conectadas em um projeto</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos ou superior</p> <p><b>Nota</b>

Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode alterar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o projeto ou superior</p> <p>Para obter informações sobre como solicitar acesso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acesso a objetos </a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Acesso adicional</td> 
   <td> <p>Você deve atender pelo menos uma das seguintes condições para aprovar tempo em um projeto:</p> 
    <ul> 
     <li>Você é o Proprietário do projeto com o acesso e as permissões especificadas acima. Nesse caso, você pode fazer o seguinte se uma das condições abaixo existir: 
      <ul>
       <li>Se você tiver permissões de Gerenciamento no projeto, poderá aprovar ou rejeitar horas conectadas ao projeto por qualquer outro usuário.</li>
       <li> Se você tiver acesso ao Contribute ou à Exibição , poderá aprovar ou rejeitar apenas as horas registradas por você ou por qualquer outro usuário que relatar você.<br></li>
      </ul></li> 
     <li>Você tem uma licença do Plan com acesso administrativo a Folhas de horas e horas. Nesse caso:
      <ul>
       <li>Você pode aprovar ou rejeitar qualquer hora nos projetos que tenha pelo menos permissões para Exibir. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir qual plano, tipo de licença ou acesso você tem, entre em contato com o administrador da Workfront.

## Exigir tempo para ser aprovado para um projeto

Para exigir aprovação do gerente de projeto para horas no projeto:

1. Vá para o projeto onde deseja solicitar aprovação para horas.
1. Clique no botão **Mais** ícone ![](assets/more-icon.png) à direita do nome do projeto, clique em **Editar**.\
   A caixa de diálogo Editar projeto é exibida.

1. No **Configurações do projeto** seção , selecione **Exigir tempo para ser aprovado para este projeto**.
1. Clique em **Salvar**.\
   Agora, quando a hora é registrada e aprovada, essas horas são bloqueadas e não podem ser alteradas pelo usuário que as inseriu no projeto ou na folha de ponto. Somente um administrador do Workfront pode ajustar o tempo registrado.

## Aprovar e rejeitar tempo em um projeto

Como gerente de projeto, você pode aprovar ou rejeitar horas registradas para tarefas, problemas ou o projeto.

Aprovar as horas no nível do projeto não afeta a folha de ponto de qualquer um dos usuários que registraram as horas. Por exemplo, as horas no projeto podem ser aprovadas pelo gerente do projeto, mas a folha de horas ainda não foi aprovada pelo gerente do usuário ou pelo aprovador da folha de horas. 

Se você configurar um projeto para exigir aprovação nas horas registradas, o gerente do projeto deverá aprovar as horas para que elas estejam disponíveis para serem incluídas em um registro de faturamento do projeto. Para obter mais informações sobre como criar registros de faturamento, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md).

Para aprovar ou rejeitar horas em um projeto:

1. Vá para o projeto.
1. Clique no botão **Horas** no painel esquerdo. Pode ser localizado na guia **Mostrar mais** área.

1. As horas registradas para problemas, tarefas e a exibição do projeto devem ter um status de **Enviado**.\
   Clique na caixa à esquerda das entradas de hora para selecionar as horas que deseja aprovar.

1. Clique em **Aprovar**.\
   O status das horas muda para **Aprovado**.\
   Se você rejeitar posteriormente as horas aprovadas, o status das horas será alterado para **Não Aprovado**.\
   Ao incluir as horas aprovadas em um registro de faturamento, o status das horas muda para **Faturado e Aprovado**. As horas adicionadas a um registro de faturamento não podem ser excluídas. Para obter mais informações sobre como criar registros de faturamento, consulte o artigo [Criar registros de faturamento](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Opcional) Clique em **Rejeitar** para rejeitar as entradas de tempo no projeto.\
   O status das horas muda para **Rejeitada**.
