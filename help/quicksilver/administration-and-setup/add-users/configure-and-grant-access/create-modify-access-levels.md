---
title: Criar ou modificar níveis de acesso personalizados
user-type: administrator
product-area: system-administration;user-management
navigation-topic: configure-access-to-workfront
description: Como administrador do Adobe Workfront, você pode criar níveis de acesso personalizados e aplicá-los aos usuários.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d2a73d24-51d3-42e2-9c09-7f4bc30b2caa
source-git-commit: 62d1b9563d83bd82b569e143f69e379e2f4ffbc2
workflow-type: tm+mt
source-wordcount: '1402'
ht-degree: 6%

---

# Criar e modificar níveis de acesso personalizados

<!--Don't delete, draft, or change the title of this article. The UI links to it via context-sensitive help.-->

Como administrador do Adobe Workfront, você pode criar níveis de acesso personalizados e aplicá-los aos usuários. À medida que você trabalha com níveis de acesso, é importante entender como eles trabalham junto com as permissões de objeto que os usuários concedem quando compartilham objetos uns com os outros. Para obter mais informações sobre níveis de acesso, consulte

* [Nova visão geral dos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md)
* [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

>[!IMPORTANT]
>
>É altamente recomendável deixar os níveis de acesso integrados inalterados para que você possa fazer referência a eles depois de configurar seus usuários. Para personalizar um nível de acesso, copie o nível de acesso padrão e modifique a cópia. Você pode fazer isso para todos os níveis de acesso, exceto Administrador do sistema e Usuário externo.

## Requisitos de acesso

Você deve ter o seguinte acesso para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plano Adobe Workfront</td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença Adobe Workfront</td> 
   <td>Plano atual: Padrão
   <p>ou</p>
   <p>Plano herdado: Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

## Criar ou editar um nível de acesso personalizado

{{step-1-to-setup}}

1. Clique em **Níveis de acesso** no painel esquerdo.
1. Selecione o nível de acesso que deseja copiar e personalizar e clique em **Copiar**.

   Ou

   Se estiver editando um nível de acesso existente (que você copiou anteriormente), clique no nome.

1. Na caixa exibida, execute qualquer um dos procedimentos a seguir para começar a configurar o nível de acesso personalizado:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nome</td> 
      <td> <p>Digite um nome para seu nível de acesso. </p> <p>Se você acabou de copiar um nível de acesso para criar um novo, o nome padrão é Nome do nível de acesso (Cópia), onde Nome do nível de acesso é o nível de acesso que você copiou.</p> <p><strong>Ponta</strong>: Recomendamos que você inclua o nome original do nível de acesso no nome da cópia. Por exemplo, na empresa ACME, uma cópia do nível de acesso Padrão pode ser chamada ACME Standard.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descrição </td> 
      <td>Digite uma descrição para o nível de acesso. É útil listar aqui o que um usuário com esse nível de acesso poderá acessar.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de Licença</td> 
      <td>Certifique-se de que a licença selecionada aqui seja a mais associada ao tipo de nível de acesso que você está criando ou editando. A licença selecionada determina quais configurações estão disponíveis para o nível de acesso. Para obter mais informações, consulte <a href="/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md" class="MCXref xref">Visão geral de novas licenças</a> ou <a href="/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md">Visão geral das licenças</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Se **Padrão** ou **Plano** é selecionado no **Tipo de licença** , role até a seção **Permitir acesso administrativo para** e selecione permissões de acesso administrativo para aqueles que terão esse nível de acesso.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processos de Aprovação</td> 
      <td>Crie e gerencie processos de aprovação para uso em todo o sistema e para grupos específicos.<p>Sem esse acesso, os usuários podem criar apenas processos de aprovação ad hoc em itens que têm acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Empresas</td> 
      <td>Adicione novas empresas e edite empresas existentes no Workfront.<br><p>Sem esse acesso, os usuários só poderão visualizar empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td>Crie e gerencie todos os formulários personalizados em seu grupo. <br><p>Sem esse acesso, os usuários só podem anexar formulários existentes aos objetos aos quais têm acesso para contribuir ou gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxas de câmbio</td> 
      <td> <p>Adicionar nova moeda no Workfront.</p> <p>Sem esse acesso, o usuário pode adicionar uma moeda existente somente a um projeto que criar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td>Exibir todas as despesas com objetos no Workfront.<p>Sem esse acesso, o usuário só poderá visualizar o seguinte:</p>
       <ul>
        <li>Despesas com projetos, tarefas ou problemas que gerem</li>
        <li>Suas próprias despesas</li>
        <li>As despesas dos seus subordinados</li>
       </ul><p><b>OBSERVAÇÃO</b>: Isso não permite que o usuário crie novos Tipos de Despesa.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Funções de trabalho</td> 
      <td> <p>Com esse acesso, o usuário tem permissão para fazer o seguinte:</p> 
       <ul> 
        <li>Exibir e editar funções de trabalho existentes</li> 
        <li>Adicionar novas funções de trabalho</li> 
        <li>Editar taxas de custo e faturamento de função</li> 
       </ul> 
       <p>Para obter informações importantes sobre o acesso a dados financeiros que está disponível para um usuário do Standard ou do Planner com acesso administrativo a funções de jobs, consulte <a href="#planner-users-with-administrative-access-to-job-roles">Usuários padrão ou do Planner com acesso administrativo a funções de cargo</a>.</p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etapas no meu grupo</td> 
      <td>Visualize todos os caminhos de marcos no sistema, no menu Caminhos de marcos, em Configurar. Os usuários também podem editar ou excluir caminhos de marcos pertencentes a qualquer um de seus grupos. Os usuários não podem gerenciar (editar ou excluir) caminhos de marcos que não são atribuídos a seus grupos.<p>Sem esse acesso, os usuários só podem visualizar os caminhos de marcos existentes e aplicá-los aos projetos que têm acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de lembrete</td> 
      <td>Crie e gerencie notificações de lembrete no Workfront.<p>Sem esse acesso, os usuários estão limitados a receber e exibir notificações.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Horas e planilhas de horas</td> 
      <td> <p>Os administradores de grupo podem atribuir perfis de folha de ponto aos usuários nos grupos e subgrupos que gerenciam.</p> <p>Sem essa opção ativada, os administradores de grupo não podem atribuir perfis de folha de ponto a outros usuários nos grupos e subgrupos que gerenciam, embora possam criá-los.</p> <p>Todos os outros usuários com uma licença Standard ou Plan podem exibir todas as horas e folhas de horas no Workfront.</p> <p>Sem essa opção ativada, os usuários podem exibir horas somente em:</p> 
       <ul> 
        <li>Projetos, tarefas ou problemas que eles gerenciam</li> 
        <li>Sua própria folha de ponto</li> 
        <li>Uma folha de ponto de alguém que reporta para ele</li> 
        <li>Uma folha de ponto que eles aprovam</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. Clique em **Definir restrições adicionais**, em seguida, defina qualquer uma das restrições a seguir para o nível de acesso.

   >[!IMPORTANT]
   >
   >Para usuários externos, como fornecedores (qualquer pessoa que não esteja em sua organização), recomendamos que você restrinja o acesso a tarefas, projetos, atualizações, anúncios, outras empresas, equipes e grupos.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nunca dê acesso a todo o projeto, quando atribuído a uma tarefa ou problema</td> 
      <td> Impede que os usuários atribuídos a tarefas ou problemas também obtenham permissões para o projeto pai, mesmo que as permissões do projeto permitam isso.<p>Para obter mais informações sobre como configurar as permissões em um projeto, consulte a seção <a href="../../../manage-work/projects/manage-projects/edit-projects.md#access" class="MCXref xref"></a> no artigo <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Editar projetos</a>.</p></td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Nunca herdar o acesso a documentos de projetos, tarefas, problemas, etc.</td> 
      <td>Impede que os documentos herdem as permissões definidas em seu objeto pai.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ver apenas atualizações em que tenham sido incluídas na conversa</td> 
      <td> <p>Permite que os usuários vejam apenas comentários onde o nome ou o nome da equipe foram incluídos.</p> <p> <p><b>OBSERVAÇÃO</b>: Isso impede que os usuários se inscrevam em itens no Workfront. Para obter mais informações sobre a assinatura de itens, consulte <a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">Adicionar usuários</a>.</p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que os usuários apaguem os comentários </td> 
      <td> <p>Impede que os usuários excluam os comentários que fazem nos itens. </p> <p><b>OBSERVAÇÃO</b>: Ninguém pode excluir os comentários de outros usuários.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visualizar apenas empresas, grupos e equipes aos quais pertencem</td> 
      <td>Permite que os usuários visualizem e compartilhem itens somente com empresas, grupos e equipes às quais pertencem.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir visibilidade das Horas planejadas ou Horas efetivas</td> 
      <td>Impede que os usuários vejam as Horas Planejadas e Reais dos itens de trabalho aos quais têm acesso. No entanto, eles podem ver as Horas reais em que se registram, ou as horas registradas por alguém que se reporta a eles.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nunca permitir que os usuários excluam as notificações</td> 
      <td>Impede que os usuários excluam anúncios na Central de Anúncios. Para obter mais informações, consulte <a href="../../../administration-and-setup/get-started-wf-administration/view-send-announcements.md" class="MCXref xref">Enviar anúncios</a>.</td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional e opcional) Se o sistema Workfront estiver configurado para usuários que pertencem a várias empresas, restrinja a visibilidade a outros usuários com base na empresa à qual eles pertencem na seção **As pessoas em outras empresas devem visualizar somente os usuários de**.

   Você pode restringir os usuários para ver apenas usuários de sua própria empresa ou da empresa designada como a principal empresa. Para obter mais informações sobre a empresa principal, consulte [Criar e editar empresas](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

   >[!NOTE]
   >
   >Se dois usuários pertencerem a duas empresas diferentes, mas ambos puderem ver os usuários da empresa principal, eles poderão ver a área Atualizações associada à empresa principal.

1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Clique em **Salvar**.

   Depois que o nível de acesso é criado, é possível atribuí-lo a um usuário (a menos que seja um nível de acesso de Administrador do sistema).

   Para obter mais informações, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

   Para obter informações sobre como um administrador do Adobe atribui um nível de acesso de Administrador do sistema a um usuário, consulte [Conceder ao usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).

## Usuários padrão ou do Planner com acesso administrativo a funções de cargo {#planner-users}

Se você conceder acesso administrativo de usuário Padrão ou Planejador a funções de cargo, a configuração Editar Faturamento de Função e Taxas de Custo será automaticamente ativada para o usuário automaticamente.

Posteriormente, se você desativar o acesso administrativo às funções de trabalho para o usuário, as funções de trabalho ainda estarão visíveis para o usuário porque a configuração Editar Faturamento de Função e Taxas de Custo ainda está ativada.

Se isso acontecer e você precisar remover o acesso do usuário para exibir funções de trabalho, será necessário desativar a configuração de permissão Editar Faturamento de Função e Taxas de Custo do usuário. Para obter instruções, consulte [Conceder acesso aos dados financeiros](grant-access-financial.md).
