---
product-area: projects
navigation-topic: manage-projects
title: Exigir que o tempo seja aprovado para um projeto
description: Você pode configurar o projeto para exigir que as horas registradas no projeto sejam aprovadas pelo Proprietário do projeto. Quando configuradas dessa forma, as horas devem ser aprovadas pelo Proprietário do projeto antes de serem qualificadas para serem usadas em um registro de cobrança.
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '785'
ht-degree: 0%

---

# Exigir que o tempo seja aprovado para um projeto

<!--audited: 08/2024-->

Você pode configurar o projeto para exigir que as horas registradas no projeto sejam aprovadas pelo Proprietário do projeto. Quando configuradas dessa forma, as horas devem ser aprovadas pelo Proprietário do projeto antes de serem qualificadas para serem usadas em um registro de cobrança.\
Para obter mais informações sobre registros de cobrança, consulte o artigo [Criar registros de cobrança](../../../manage-work/projects/project-finances/create-billing-records.md).

>[!NOTE]
>
>Habilitar esta opção não remove a capacidade do aprovador da folha de horas de aprovar horas na folha de horas. Se o Proprietário do projeto não aprovar ou rejeitar as horas, o aprovador da folha de horas ainda poderá aprovar as horas em uma folha de horas.

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
   <td> <p>Para exigir que o tempo seja aprovado no projeto:</p>
   <ul><li><p>Standard</p></li>
   <li><p>Plano</p></li></ul>

<p>Para aprovar horas registradas em um projeto:</p>
   <ul><li><p>Leve ou superior</p></li>
   <li><p>Revisar ou superior</p></li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Editar acesso a projetos</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permissões de objeto</td> 
   <td> <p>Exibir permissões para o projeto ou superior</p>
  </tr> 
  <tr> 
   <td role="rowheader">Acesso adicional</td> 
   <td> <p>Você deve atender a pelo menos uma das seguintes condições para aprovar horas em um projeto:</p> 
    <ul> 
     <li>Você é o Proprietário do Projeto com o acesso e as permissões especificadas acima. Nesse caso, você poderá fazer o seguinte se uma das condições abaixo existir: 
      <ul>
       <li>Se você tiver Gerenciar permissões no projeto, poderá aprovar ou rejeitar horas registradas no projeto por qualquer outro usuário.</li>
       <li> Se tiver acesso ao Contribute ou à Visualização para o projeto, você poderá aprovar ou rejeitar apenas as horas registradas por você ou por qualquer outro usuário que reportar você.<br></li>
      </ul></li> 
     <li>Você tem uma licença de Plano com acesso administrativo a Planilhas de Horas e Horas. Neste caso:
      <ul>
       <li>Você pode aprovar ou rejeitar qualquer hora nos projetos para os quais tem pelo menos permissões de exibição. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>To require time to be approved on the project:</p>
   <ul><li>New: Standard</li>
   <li>Current: Plan</li></ul>
   
   <p>To approve hours logged on a project:</p>
   <ul><li>New: Light or higher</li>
   <li>Review or higher</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects or higher</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project or higher</p>
  </tr> 
  <tr> 
   <td role="rowheader">Additional access</td> 
   <td> <p>You must meet at least one of the following conditions to approve time on a project:</p> 
    <ul> 
     <li>You are the Project Owner with the access and permissions specified above. In this case, you can do the following if one of the conditions below exists: 
      <ul>
       <li>If you have Manage permissions on the project, you can approve or reject hours logged on the project by any other user.</li>
       <li> If you have Contribute or View access to the project you will be able to approve or reject only the hours logged by you or any other user that reports you.<br></li>
      </ul></li> 
     <li>You have a Plan license with administrative access to Timesheets &amp; Hours. In this case:
      <ul>
       <li>You can approve or reject any hours on the projects you have at least permissions to View. </li>
      </ul></li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>-->

## Exigir que o tempo seja aprovado para um projeto

Para exigir a aprovação do gerente de projeto para horas no projeto:

1. Vá para o projeto em que deseja solicitar aprovação para horas.
1. Clique no ícone **Mais** ícone ![Mais ícone](assets/more-icon.png) à direita do nome do projeto e clique em **Editar**.\
   A caixa de diálogo Editar projeto será exibida.

1. Na seção **Configurações do Projeto**, selecione **Solicitar aprovação para este projeto**.
1. Clique em **Salvar**.\
   Agora, quando as horas são registradas e aprovadas, essas horas ficam bloqueadas e não podem ser alteradas pelo usuário que as inseriu no projeto ou na folha de horas. Somente um administrador do Workfront pode ajustar o tempo registrado.

## Aprovar e rejeitar horas em um projeto

Como gerente de projeto, você pode aprovar ou rejeitar horas registradas para tarefas, problemas ou o projeto.

Aprovar as horas no nível do projeto não tem nenhum impacto na folha de horas de nenhum dos usuários que registraram as horas. Por exemplo, as horas no projeto podem ser aprovadas pelo gerente de projeto, mas a folha de horas ainda não foi aprovada pelo gerente do usuário ou pelo aprovador da folha de horas.

Se você configurar um projeto para exigir aprovação nas horas registradas, o gerente do projeto deverá aprovar as horas para que elas estejam disponíveis para serem incluídas em um registro de cobrança do projeto. Para obter mais informações sobre como criar registros de cobrança, consulte o artigo [Criar registros de cobrança](../../../manage-work/projects/project-finances/create-billing-records.md).

Para aprovar ou rejeitar horas em um projeto:

1. Vá para o projeto.
1. Clique na área **Horas** no painel esquerdo.

1. As horas registradas para problemas, tarefas e a exibição do projeto devem ter o status de **Enviadas**.\
   Clique na caixa à esquerda das entradas de hora para selecionar as horas que deseja aprovar.

1. Clique no ícone **Aprovar** ![](assets/approve-hours-icon.png) na parte superior da lista de horas.\
   O status das horas muda para **Aprovado**.\
   Se você rejeitar as horas aprovadas posteriormente, o status das horas mudará para **Não Aprovado**.\
   Quando você inclui as horas aprovadas em um registro de cobrança, o status das horas muda para **Faturadas e Aprovadas**. Horas adicionadas a um registro de cobrança não podem ser excluídas. Para obter mais informações sobre como criar registros de cobrança, consulte o artigo [Criar registros de cobrança](../../../manage-work/projects/project-finances/create-billing-records.md)

1. (Opcional) Clique no ícone **de** Rejeitar![](assets/reject-hours-icon.png) para rejeitar as entradas de tempo do projeto.\
   O status das horas muda para **Rejected**.

   >[!NOTE]
   >
   >   Se as horas selecionadas estiverem incluídas em um Registro de faturamento que foi marcado como Faturado ou Faturado e Aprovado, os ícones Aprovar e Rejeitar não serão exibidos. Você só pode aprovar horas que ainda não foram faturadas em um Registro de faturamento.

