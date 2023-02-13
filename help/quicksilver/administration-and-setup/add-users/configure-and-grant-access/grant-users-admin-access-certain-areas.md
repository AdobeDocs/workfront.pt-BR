---
title: Conceder aos usuários acesso administrativo a determinadas áreas
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para conceder aos usuários uma licença do Plano acesso administrativo a determinadas áreas do sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 253a116e04e0b3a729331f5d0a29405e82808390
workflow-type: tm+mt
source-wordcount: '846'
ht-degree: 2%

---

# Conceder aos usuários acesso administrativo a determinadas áreas

<!--Linked in several places, do not rename or change URL.-->

Como administrador do Adobe Workfront, você pode usar um nível de acesso para conceder aos usuários uma licença do Plano acesso administrativo a determinadas áreas do sistema.

>[!NOTE]
>
>Isso é diferente de conceder a um usuário acesso administrativo total ao Workfront, o que é explicado em [Conceder ao usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)&#x200B;

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
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Conceder aos usuários do Plano acesso administrativo a determinadas áreas do Workfront

>[!IMPORTANT]
>
>É altamente recomendável deixar os níveis de acesso integrados inalterados para que você possa fazer referência a eles depois de configurar seus usuários. Para personalizar um nível de acesso, copie o nível de acesso padrão e modifique a cópia. (Você pode fazer isso para cada nível de acesso, exceto Administrador do sistema e Usuário externo.)

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Níveis de acesso**.
1. Clique no nome do nível de acesso que deseja usar para conceder aos usuários acesso administrativo a determinadas áreas do Workfront.
1. No **Permitir acesso administrativo para** , caixas de seleção para conceder o acesso administrativo necessário.

   Essas opções permitem que você conceda os seguintes recursos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processos de Aprovação</td> 
      <td><p>Crie e gerencie processos de aprovação para uso em todo o sistema e para grupos específicos.</p><p>Sem esse acesso, os usuários podem criar somente processos de aprovação ad-hoc em itens que têm acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Empresas</td> 
      <td><p>Adicionar novas empresas e editar empresas existentes no Workfront</p>
      <p>Sem esse acesso, os usuários só poderão visualizar empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td><p>Crie e edite (adicione, edite e exclua os campos) formulários personalizados em seu grupo.</p><p>Sem esse acesso, os usuários só podem anexar formulários existentes a objetos nos quais tenham acesso para contribuir ou gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxas de câmbio</td> 
      <td> <p>Adicionar nova moeda no Workfront.</p> <p>Sem esse acesso, o usuário só pode adicionar uma moeda existente a um projeto que criar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td><p>Exibir todas as despesas com objetos no Workfront.</p><p>Isso não permite que o usuário crie novos Tipos de Despesa.</p><p>Sem esse acesso, o usuário só poderá visualizar o seguinte:</p>
       <ul>
        <li>Despesas com projetos, tarefas ou problemas que gerem</li>
        <li>Suas próprias despesas</li>
        <li>As despesas dos seus subordinados</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Funções de trabalho</td> 
      <td> <p>Com esse acesso, o usuário tem permissão para fazer o seguinte:</p> 
       <ul> 
        <li>Exibir e editar funções de trabalho existentes</li> 
        <li>Adicionar novas funções de trabalho</li> 
        <li>Editar taxas de custo e faturamento de função</li> 
       </ul> <p><b>IMPORTANTE</b>: Se você conceder a um Usuário do Planejador acesso administrativo a funções de cargo, a configuração Acesso a Dados Financeiros Editar Faturamento de Função e Taxas de Custo será ativada automaticamente para o usuário. Posteriormente, se você desativar o acesso administrativo às funções do job para o usuário do Planejador, as funções do job ainda estarão visíveis para o usuário, pois a configuração Editar Faturamento de Função e Taxas de Custo ainda estará ativada. Se isso acontecer e você precisar remover o acesso do usuário para exibir funções de trabalho, será necessário desativar a configuração de permissão Editar Faturamento de Função e Taxas de Custo do usuário. Para obter instruções, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso aos dados financeiros</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etapas no meu grupo</td> 
      <td>Visualize todos os caminhos de marcos no sistema, no menu Caminhos de marcos, em Configurar. Os usuários também podem editar ou excluir caminhos de marcos pertencentes a qualquer um de seus grupos. Os usuários não podem gerenciar (editar ou excluir) os caminhos de marcos que não são atribuídos a nenhum de seus grupos.<br><p>Sem esse acesso, os usuários só podem visualizar os caminhos de marcos existentes e aplicá-los aos projetos que têm acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de lembrete</td> 
      <td>Crie e gerencie notificações de lembrete no Workfront.<br>Sem esse acesso, os usuários estão limitados a receber e exibir notificações.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Horas e planilhas de horas</td> 
      <td> <p>Permite que os usuários visualizem todas as horas e folhas de horas no Workfront.</p> <p>Quando essa opção está desativada, os usuários podem exibir somente horas em:</p> 
       <ul> 
        <li>Projetos, tarefas ou problemas que eles gerenciam</li> 
        <li>Sua própria folha de ponto</li> 
        <li>Uma folha de ponto de alguém que reporta para ele</li> 
        <li>Uma folha de ponto que eles aprovam</li> 
       </ul> <p><b>Nota</b>:  <p>Se essa opção estiver ativada ou desativada, os administradores de grupo podem criar perfis de folha de ponto para os grupos e subgrupos que gerenciam e atribuí-los a membros do grupo cujos perfis de usuário têm acesso para editar.</p> <p>Ativar essa opção pode fornecer acesso excessivo a alguns administradores de grupo, pois eles podem exibir as folhas de horas geradas pelos perfis da folha de ponto (e as horas) para todos os usuários no sistema, não apenas para aqueles nos grupos que administram. Você pode desativar essa opção para administradores de grupo que não precisam de muito acesso.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Quando terminar, clique em **Salvar**.
1. Atribua o novo nível de acesso a um usuário, conforme descrito em [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Você pode permitir que os usuários tenham acesso administrativo aos usuários. Para obter mais informações sobre como conceder aos usuários acesso administrativo aos usuários para que eles possam gerenciar contas de usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
