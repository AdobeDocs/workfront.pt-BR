---
product-area: projects
navigation-topic: manage-projects
title: Exigir que o tempo seja aprovado para um projeto
description: Exigir que o tempo seja aprovado para um projeto
author: Alina
feature: Work Management
exl-id: e4a27640-9f5c-4a9f-82cc-3384694594af
source-git-commit: 3d96d7b7073ad194f291afe370ae813d3482bc9e
workflow-type: tm+mt
source-wordcount: '754'
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

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td> <p>Qualquer</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td> <p>Para exigir que o tempo seja aprovado no projeto:</p>
   <ul><li>Novo: Padrão</li>
   <li>Atual: Plano</li></ul>

<p>Para aprovar horas registradas em um projeto:</p>
   <ul><li>Novo: Claro ou superior</li>
   <li>Revisar ou superior</li>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Editar acesso a Projetos ou superior</p>  </td> 
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

*Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

1. (Opcional) Clique no ícone ![](assets/reject-hours-icon.png) de **Rejeitar** para rejeitar as entradas de tempo do projeto.\
   O status das horas muda para **Rejected**.

   >[!NOTE]
   >
   >   Se as horas selecionadas estiverem incluídas em um Registro de faturamento que foi marcado como Faturado ou Faturado e Aprovado, os ícones Aprovar e Rejeitar não serão exibidos. Você só pode aprovar horas que ainda não foram faturadas em um Registro de faturamento.

