---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Gerenciar licenças disponíveis em seu sistema
description: Como administrador do Adobe Workfront, você pode acessar informações sobre sua conta da Workfront, incluindo o número de licenças compradas para sua organização, bem como o número dessas licenças em uso no momento.
author: Lisa, Jenny
feature: System Setup and Administration
role: Admin
exl-id: ea580dd0-efb7-4f56-beb3-07ad044efc8a
source-git-commit: 01a80f6140650ca12aaee14115f79449dcfa2a18
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 0%

---

# Gerenciar licenças disponíveis em seu sistema

<!-- Audited: 12/2023 -->

Como administrador do Adobe Workfront, você pode acessar informações sobre sua conta da Workfront, incluindo o número de licenças compradas para sua organização, bem como o número dessas licenças em uso no momento.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td><p>Standard</p> <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td>Você deve ser um administrador do Workfront. </td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


>[!NOTE]
>
>As instruções a seguir se aplicam aos pacotes Select, Prime e Ultimate.
>
>Para o pacote Select:
>
>1. Os administradores do sistema não podem definir limites para Grupos padrão.
>2. Os administradores de sistema podem ver apenas o número total de licenças usadas em todos os Grupos Padrão.
>3. Os administradores de grupo não podem acessar a página Licenças.
>
>Para os pacotes do Prime e do Ultimate:
>
>1. Os administradores do sistema podem adicionar Grupos padrão à página Licenças para visualizar a utilização de licenças nesses grupos e também podem definir limites de licença.
>2. Os administradores de grupo podem acessar a página Licenças e visualizar a utilização de licenças nos grupos que eles gerenciam que foram adicionados à página Licenças por administradores do sistema.
>3. Os administradores de grupo não podem visualizar informações de outros grupos padrão ou adicionar máximos.

+++

## Exibir as licenças de sua organização

O número de licenças em uso é atualizado automaticamente à medida que você atribui níveis de acesso aos usuários adicionados ao Workfront. Para obter mais informações, consulte [Adicionar usuários](../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

Para exibir informações de licença em seu sistema:

{{step-1-to-setup}}

1. Na parte inferior do painel esquerdo, clique em **Sistema** > **Licenças**.

   Para obter mais informações sobre as licenças listadas nesta página, consulte [Visão geral das licenças](../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

   >[!NOTE]
   >
   >Licenças de comprovação estão disponíveis somente para clientes que compraram o complemento pago do Workfront Proof, além da licença do Workfront. Para obter informações sobre este complemento, consulte [Workfront Proof: índice do artigo](../../workfront-proof/workfront-proof.md).

1. (Condicional) Se você vir a mensagem **Para definir um máximo, é necessário adicionar um Grupo Doméstico**, adicionar um Grupo Doméstico no sistema conforme explicado na seção [Adicionar ou remover um Grupo Doméstico da página Licenças](#add-or-remove-a-home-group-to-the-licenses-page) deste artigo.

   >[!NOTE]
   >
   >Para os novos planos, o plano Select não permite que os administradores visualizem licenças por Grupo padrão. Você só pode ver o número geral de licenças usadas. Os planos da Prime e da Ultimate permitem definir a contagem máxima de licenças por grupo padrão.

## Exibir informações sobre licenças para complementos do Workfront

Se sua organização tiver o complemento Workfront Proof pago, o número de licenças usadas e o número de licenças disponíveis serão exibidos. Por exemplo, **5 de 10 licenças de prova** indica que a organização está usando atualmente 5 das 10 licenças Workfront Proof que adquiriu.

![Licença para complementos do Workfront](assets/updated-licenses-page.png)

Se sua organização adquiriu o Workfront Goals, as informações de licença desse produto também são exibidas aqui. Nesse caso, você pode exibir as seguintes informações:

* O número total de licenças do Workfront Goals que sua empresa adquiriu
* O número de licenças do Workfront Goals associadas aos usuários. Este é o número de usuários aos quais foi concedido acesso de Visualização a Metas em seus respectivos níveis de acesso.

Para obter informações sobre as Metas do Workfront, consulte [Visão geral das Metas do Adobe Workfront](../../workfront-goals/goal-management/wf-goals-overview.md). Para obter informações sobre acesso às Metas do Workfront, consulte [Conceder acesso às Metas do Adobe Workfront](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md).

>[!NOTE]
>
>O Workfront permite atribuir mais licenças do Workfront Goals que você adquiriu. No entanto, quando você atribuir mais licenças do que o permitido pelo contrato do Workfront Goals, um gerente de conta da Workfront entrará em contato com você para informar que você excedeu o número contratual.
>

<!--
If an organization has other paid add-on products, their license information also displays here. If the organization doesn't have any paid add-on products, nothing displays here. (Drafted this because not sure this is accurate: Scenario Planner is an add-on product and its licenses are not displayed there.)
-->

>[!TIP]
>
>Os usuários sem acesso administrativo podem usar um relatório de Grupo para exibir a contagem de licenças. Na guia Relatório, crie um novo relatório de grupo e adicione as seguintes colunas:
>
>* Limite de Tipo de Licença: Limite de Trabalhadores
>* Limite de Tipo de Licença: Limite do Planejador
>
>Para saber mais sobre como criar um relatório, consulte [Criar um relatório personalizado](../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Exibir informações sobre prova mensal e alocações de decisão do documento

>[!IMPORTANT]
>
>Os limites de decisão de prova e documento se aplicam apenas aos usuários nas novas licenças. Para obter mais informações, consulte [Visão geral das novas licenças](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).

As decisões de prova e documento são limitadas a todas as licenças não pagas do Workfront. Limites redefinidos por usuário a cada mês.

Os limites de decisão para cada licença diferem dependendo do plano em que você está. Você pode visualizar a alocação mensal em Configurar > Licenças.

Para obter mais informações sobre limites de prova e decisão de documento, consulte [Visão geral sobre documento limitado e decisão de prova para usuários não pagos](/help/quicksilver/review-and-approve-work/proof-doc-decision-limits.md).

![Alocação de decisão mensal](assets/monthly-decision-allotment.png)

## Adicionar ou remover um Grupo Padrão da página de licenças {#add-or-remove-a-home-group-to-the-licenses-page}

Cada usuário pode ser atribuído a apenas um Grupo padrão. O Workfront fornece uma contagem de licenças orientada por grupo calculando quantas licenças estão alocadas e são usadas atualmente em cada Grupo padrão.

Se você vir a mensagem **Para definir um máximo, é necessário adicionar um Grupo Doméstico** na página de Licenças. É necessário adicionar pelo menos um Grupo Doméstico à página de Licenças.

>[!IMPORTANT]
>
>* Para gerenciar licenças com grupos padrão, recomendamos configurar Grupos padrão específicos para unidades de negócios antes de atualizar a contagem máxima de licenças. Para obter mais informações, consulte [Visão geral de Grupos Domésticos](../../administration-and-setup/manage-groups/groups-overview/home-groups.md).
>* Você pode adicionar somente grupos de nível superior como Grupos padrão, não subgrupos. Se um usuário tiver um subgrupo atribuído como Grupo inicial, sua licença será adicionada à contagem de licenças do grupo de nível superior acima desse subgrupo.
>

Para adicionar ou remover um Grupo Inicial da página Licenças:

{{step-1-to-setup}}

1. Na parte inferior do painel esquerdo, clique em **Sistema** > **Licenças**.

1. Clique em **Gerenciar Lista de Grupos**.
1. Comece a digitar o nome do grupo de nível superior na caixa **Grupos Padrão**.
1. Para adicionar o grupo, clique no nome quando ele aparecer.

   Ou

   Para remover o grupo, clique no ícone X à direita do nome.

1. Clique em **Salvar**.

Como administrador do Workfront, você pode definir contagens máximas de licença para os Grupos Padrão para impedir que uma unidade de negócios use licenças do Workfront adquiridas para outras unidades de negócios. Para obter instruções, consulte [Definir a contagem máxima de licenças para um Grupo Padrão](#set-the-maximum-license-count-for-a-home-group) neste artigo.

## Definir a contagem máxima de licenças para um Grupo padrão {#set-the-maximum-license-count-for-a-home-group}

Como administrador do Workfront, você pode definir contagens máximas de licença para os Grupos padrão do sistema. Isso permite impedir que uma unidade de negócios use licenças da Workfront adquiridas para outras unidades de negócios na organização.

Por padrão, a contagem máxima de licenças é definida como N/D, o que significa que não há limite.

Os administradores de grupo podem exibir o número de licenças alocadas e usadas em um Grupo padrão gerenciado. Para obter mais informações, consulte [Exibir o número de licenças alocadas e usadas em um grupo](../../administration-and-setup/manage-groups/create-and-manage-groups/view-number-licenses-allocated-used-group.md).

Para definir a contagem máxima de licenças para um Grupo padrão:

{{step-1-to-setup}}

1. Na parte inferior do painel esquerdo, clique em **Sistema** > **Licenças**.

1. Localize o Grupo padrão na lista.
1. Na coluna **Max** do grupo, clique no valor para o qual você deseja definir um máximo.
1. Digite o número máximo e pressione Enter.

   ![Máximo de licenças do grupo](assets/updated-max.png)

   >[!NOTE]
   >
   >Para redefinir o valor máximo de licença de um grupo para o padrão, não digite 0. Em vez disso, exclua o número na caixa. Definir o valor máximo de licença como 0 indica que não há licenças alocadas para esse grupo.
