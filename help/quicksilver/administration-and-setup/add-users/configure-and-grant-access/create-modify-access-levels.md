---
title: Criar e modificar níveis de acesso personalizados
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode criar níveis de acesso personalizados e aplicá-los aos usuários.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 4cab7bed6cb4c25d96e70ccce2ece7f6d156f435
workflow-type: tm+mt
source-wordcount: '1463'
ht-degree: 6%

---

# Criar e modificar níveis de acesso personalizados

<!--Audited: 12/2023-->

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help. -->

Como administrador do Adobe Workfront, você pode criar níveis de acesso personalizados e aplicá-los aos usuários. Ao trabalhar com níveis de acesso, é importante entender como eles trabalham em conjunto com as permissões de objeto que os usuários concedem quando compartilham objetos entre si. Para obter mais informações sobre níveis de acesso, consulte:

* [Visão geral dos novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)

>[!IMPORTANT]
>
>É altamente recomendável que você deixe os níveis de acesso incorporados inalterados para que possa consultá-los após configurar os usuários. Para personalizar um nível de acesso, copie o nível de acesso padrão e modifique a cópia. Você pode fazer isso para todos os níveis de acesso, exceto para Administrador do sistema e Usuário externo.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>Novo: Padrão
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Criar ou editar um nível de acesso personalizado

{{step-1-to-setup}}

1. Clique em **Níveis de acesso** no painel esquerdo.
1. Selecione o nível de acesso que você deseja copiar e personalizar e clique em **Copiar**.

   Ou

   Se você estiver editando um nível de acesso existente (copiado anteriormente), clique em seu nome.

1. Na caixa exibida, siga um destes procedimentos para começar a configurar o nível de acesso personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>Digite um nome para o seu nível de acesso. </p> <p>Se você acabou de copiar um nível de acesso para criar um novo, o nome padrão é Nome do Nível de Acesso (Cópia), onde Nome do Nível de Acesso é o nível de acesso copiado.</p> <p><strong>Dica</strong>: recomendamos que você inclua o nome original do nível de acesso no nome da cópia. Por exemplo, na empresa ACME, uma cópia do nível de acesso Standard pode se chamar ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição </td> 
      <td>Digite uma descrição para o nível de acesso. É útil listar aqui o que um usuário com esse nível de acesso poderá acessar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Licença</td> 
      <td>Certifique-se de que a licença selecionada aqui seja a mais associada ao tipo de nível de acesso que você está criando ou editando. A licença selecionada determina quais configurações estão disponíveis para o nível de acesso. Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Visão geral das novas licenças</a> ou <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Visão geral das licenças</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se o **Standard** ou o **Plan** estiver selecionado na caixa **Tipo de Licença**, role até a seção **Permitir acesso administrativo para** e selecione permissões de acesso administrativo para aqueles que terão esse nível de acesso.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processos de Aprovação</td> 
      <td>Crie e gerencie processos de aprovação para uso em todo o sistema e para grupos específicos.<p>Sem esse acesso, os usuários podem criar apenas processos de aprovação adhoc em itens que eles tenham acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Empresas</td> 
      <td>Adicione novas empresas e edite as existentes no Workfront.<br><p>Sem esse acesso, os usuários só poderão visualizar empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td>Crie e gerencie todos os formulários personalizados dentro do grupo. <br><p>Sem esse acesso, os usuários só podem anexar formulários existentes aos objetos aos quais têm acesso para contribuir ou gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxas de câmbio</td> 
      <td> Adicionar nova moeda no Workfront. <p>Sem esse acesso, o usuário pode adicionar uma moeda existente somente a um projeto que criar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td>Exibir todas as despesas em objetos no Workfront.<p>Sem esse acesso, o usuário só poderá exibir o seguinte:</p>
       <ul>
        <li>Despesas com projetos, tarefas ou problemas que gerenciam</li>
        <li>Suas próprias despesas</li>
        <li>As despesas de seus subordinados</li>
       </ul><p><b>OBSERVAÇÃO</b>: isso não permite que o usuário crie novos Tipos de Despesas.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Funções de trabalho</td> 
      <td> Com esse acesso, o usuário pode fazer o seguinte: 
       <ul> 
        <li>Exibir e editar funções de trabalho existentes</li> 
        <li>Adicionar novas funções de trabalho</li> 
        <li>Editar taxas de custo e cobrança de função</li> 
       </ul> 
       <p>Para obter informações importantes sobre o acesso a dados financeiros disponíveis para um usuário do Standard ou do Planner com acesso administrativo a funções de trabalho, consulte <a href="#standard-or-planner-users-with-administrative-access-to-job-roles">Usuários do Standard ou do Planner com acesso administrativo a funções de trabalho</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etapas no meu grupo</td> 
      <td>Exibir todos os caminhos de etapas no sistema no menu Caminhos de Etapas na Configuração. Os usuários também podem editar ou excluir caminhos de marcos pertencentes a qualquer um de seus grupos. Os usuários não podem gerenciar (editar ou excluir) caminhos de marcos que não estão atribuídos ao grupo de grupos.<p>Sem esse acesso, os usuários só poderão visualizar os caminhos de marcos existentes e aplicá-los aos projetos que tiverem acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de lembrete</td> 
      <td>Crie e gerencie notificações de lembrete no Workfront.<p>Sem esse acesso, os usuários ficam limitados a receber e visualizar notificações.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Horas e planilhas de horas</td> 
      <td> Os administradores de grupo podem atribuir perfis de planilha de horas a usuários nos grupos e subgrupos que eles gerenciam. <p>Sem essa opção ativada, os administradores de grupo não podem atribuir perfis de folha de horas a outros usuários nos grupos e subgrupos que gerenciam, embora possam criá-los.</p> <p>Todos os outros usuários com uma licença Padrão ou de Plano podem exibir todas as horas e planilhas de horas no Workfront.</p> <p>Sem essa opção ativada, os usuários poderão exibir horas somente em:</p> 
       <ul> 
        <li>Projetos, tarefas ou problemas que eles gerenciam</li> 
        <li>Sua própria planilha de horas</li> 
        <li>Uma planilha de horas de alguém que reporta a eles</li> 
        <li>Uma planilha de horas que eles aprovam</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Definir restrições adicionais** e defina qualquer uma das restrições a seguir para o nível de acesso.

   >[!IMPORTANT]
   >
   >Para usuários externos, como fornecedores (qualquer pessoa que não esteja em sua organização), recomendamos que você restrinja o acesso a tarefas, projetos, atualizações, anúncios, outras empresas, equipes e grupos.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nunca dê acesso a todo o projeto, quando atribuído a uma tarefa ou problema</td> 
      <td> Impede que os usuários atribuídos a tarefas ou problemas também obtenham permissões para o projeto principal, mesmo que as permissões do projeto permitam isso.<p>Para obter mais informações sobre como configurar as permissões em um projeto, consulte a seção <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> no artigo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar projetos</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nunca herdar o acesso a documentos de projetos, tarefas, problemas, etc.</td> 
      <td>Impede que os documentos herdem as permissões definidas em seu objeto pai.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver apenas atualizações em que tenham sido incluídas na conversa</td> 
      <td> Permite que os usuários vejam apenas os comentários nos quais o nome ou o nome da equipe foi incluído. <p> <p><b>OBSERVAÇÃO</b>: isso impede que os usuários assinem itens no Workfront. Para obter mais informações sobre como assinar itens, consulte <a href="../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md" class="MCXref xref">Assinar itens no Adobe Workfront</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que os usuários apaguem os comentários </td> 
      <td> Impede que os usuários excluam os comentários feitos nos itens.  <p><b>OBSERVAÇÃO</b>: ninguém pode excluir os comentários de outros usuários.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizar apenas empresas, grupos e equipes aos quais pertencem</td> 
      <td>Permite que os usuários visualizem e compartilhem itens somente com empresas, grupos e equipes aos quais pertencem.<p><strong>OBSERVAÇÃO</strong>: os usuários com licenças de Solicitante não podem exibir empresas às quais não pertencem, mesmo que esta opção esteja selecionada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir visibilidade das Horas planejadas ou Horas efetivas</td> 
      <td>Impede que os usuários vejam as Horas Planejadas e Reais dos itens de trabalho aos quais têm acesso. No entanto, eles podem ver as Horas efetivas que se registram ou as horas que são registradas por alguém que reporta a eles.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que os usuários excluam as notificações</td> 
      <td>Impede que os usuários excluam anúncios no Centro de Notificações. Para obter mais informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar comunicados</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional e opcional) Se seu sistema Workfront estiver configurado para usuários que pertencem a várias empresas, restrinja a visibilidade a outros usuários com base na empresa à qual pertencem na seção **As pessoas de outras empresas só devem ver os usuários de**.

   É possível restringir os usuários para ver apenas os usuários de sua própria empresa ou da empresa designada como a empresa primária. A empresa principal geralmente representa a conta da Workfront na qual a maioria dos usuários trabalha. Para obter mais informações sobre a empresa primária, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Se dois usuários pertencerem a duas empresas diferentes, mas ambos puderem ver os usuários da empresa primária, eles poderão ver a área Atualizações associada à empresa primária.

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Clique em **Salvar**.

   Após criar o nível de acesso, você pode atribuí-lo a um usuário (a menos que seja um nível de acesso de Administrador do sistema).

   Para obter mais informações, consulte [Editar perfil de usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Para obter informações sobre como um administrador de Adobe atribui um nível de acesso de Administrador do Sistema a um usuário, consulte [Conceder a um usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Usuários padrão ou do Planejador com acesso administrativo às funções de trabalho {#planner-users}

Se você conceder a um usuário Padrão ou Planejador acesso administrativo a funções de trabalho, a configuração Editar taxas de custo e faturamento de função será automaticamente ativada para o usuário.

Posteriormente, se você desativar o acesso administrativo a funções de trabalho para o usuário, as funções de trabalho ainda estarão visíveis para o usuário, pois a configuração Editar taxas de custo e cobrança de função ainda está ativada.

Se isso acontecer e você precisar remover o acesso do usuário para visualizar funções de trabalho, será necessário desativar a configuração de permissão Editar taxas de custo e cobrança de função. Para obter instruções, consulte [Conceder acesso a dados financeiros](grant-access-financial.md).
