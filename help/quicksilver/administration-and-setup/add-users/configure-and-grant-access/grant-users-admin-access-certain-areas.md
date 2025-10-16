---
title: Conceder aos usuários acesso administrativo a determinadas áreas
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para conceder aos usuários uma licença de Plano acesso administrativo a determinadas áreas do sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 9d12895d-cf7f-41c6-a2ac-bb731770c187
source-git-commit: 2a83e5a415ff254cf5525d6f44ecb0e447e7e70a
workflow-type: tm+mt
source-wordcount: '807'
ht-degree: 2%

---

# Conceder aos usuários acesso administrativo a determinadas áreas

<!--Linked in several places, do not rename or change URL.-->

Como administrador do Adobe Workfront, você pode usar um nível de acesso para conceder aos usuários uma licença de Plano acesso administrativo a determinadas áreas do sistema.

>[!NOTE]
>
>Isso é diferente de conceder a um usuário acesso administrativo total ao Workfront, que é explicado em [Conceder a um usuário acesso administrativo total](../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md).&#x200B;

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>   <p>Standard</p>
   <p>Plano</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Conceder aos usuários do Plano acesso administrativo a determinadas áreas do Workfront

>[!IMPORTANT]
>
>É altamente recomendável que você deixe os níveis de acesso incorporados inalterados para que possa consultá-los após configurar os usuários. Para personalizar um nível de acesso, copie o nível de acesso padrão e modifique a cópia. (Você pode fazer isso para todos os níveis de acesso, exceto para Administrador do sistema e Usuário externo.)

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Níveis de Acesso**.
1. Clique no nome do nível de acesso que deseja usar para conceder aos usuários acesso administrativo a determinadas áreas do Workfront.
1. Na seção **Permitir acesso administrativo para**, marque as caixas para conceder o acesso administrativo necessário.

   Essas opções permitem conceder os seguintes recursos:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Processos de Aprovação</td> 
      <td><p>Crie e gerencie processos de aprovação para uso em todo o sistema e para grupos específicos.</p><p>Sem esse acesso, os usuários podem criar apenas processos de aprovação ad hoc em itens que eles tenham acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Empresas</td> 
      <td><p>Adicionar novas empresas e editar empresas existentes no Workfront</p>
      <p>Sem esse acesso, os usuários só poderão visualizar empresas existentes.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formulários personalizados</td> 
      <td><p>Criar e editar (adicionar, editar e excluir os campos) formulários personalizados dentro de seus grupos.</p><p>Sem esse acesso, os usuários só podem anexar formulários existentes a objetos nos quais têm acesso para contribuir ou gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Taxas de câmbio</td> 
      <td> <p>Adicionar nova moeda no Workfront.</p> <p>Sem esse acesso, o usuário só poderá adicionar uma moeda existente a um projeto que criar.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Despesas</td> 
      <td><p>Exibir todas as despesas em objetos no Workfront.</p><p>Isso não permite que o usuário crie novos Tipos de Despesas.</p><p>Sem esse acesso, o usuário só poderá exibir o seguinte:</p>
       <ul>
        <li>Despesas com projetos, tarefas ou problemas que gerenciam</li>
        <li>Suas próprias despesas</li>
        <li>As despesas de seus subordinados</li>
       </ul></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Funções de trabalho</td> 
      <td> <p>Com esse acesso, o usuário pode fazer o seguinte:</p> 
       <ul> 
        <li>Exibir e editar funções de trabalho existentes</li> 
        <li>Adicionar novas funções de trabalho</li> 
        <li>Editar taxas de custo e cobrança de função</li> 
       </ul> <p><b>IMPORTANTE</b>: se você conceder a um usuário do Planejador acesso administrativo a funções de trabalho, a configuração do Acesso a dados financeiros Editar taxas de custo e cobrança de função será habilitada automaticamente para o usuário. Posteriormente, se você desativar o acesso administrativo a funções de trabalho para o usuário Planejador, as funções de trabalho ainda estarão visíveis para o usuário, pois a configuração Editar taxas de custo e faturamento de função ainda está ativada. Se isso acontecer e você precisar remover o acesso do usuário para visualizar funções de trabalho, será necessário desativar a configuração de permissão Editar taxas de custo e cobrança de função. Para obter instruções, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Conceder acesso a dados financeiros</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Etapas no meu grupo</td> 
      <td>Exibir todos os caminhos de etapas no sistema no menu Caminhos de Etapas na Configuração. Os usuários também podem editar ou excluir caminhos de marcos pertencentes a qualquer um de seus grupos. Os usuários não podem gerenciar (editar ou excluir) os caminhos de marcos que não estão atribuídos a nenhum dos grupos.<br><p>Sem esse acesso, os usuários só poderão visualizar os caminhos de marcos existentes e aplicá-los aos projetos que tiverem acesso para gerenciar.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificações de lembrete</td> 
      <td>Crie e gerencie notificações de lembrete no Workfront.<br>Sem esse acesso, os usuários ficam limitados a receber e visualizar notificações.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Horas e planilhas de horas</td> 
      <td> <p>Permite que os usuários visualizem todas as horas e planilhas de horas no Workfront.</p> <p>Quando essa opção está desativada, os usuários podem exibir apenas horas em:</p> 
       <ul> 
        <li>Projetos, tarefas ou problemas que eles gerenciam</li> 
        <li>Sua própria planilha de horas</li> 
        <li>Uma planilha de horas de alguém que reporta a eles</li> 
        <li>Uma planilha de horas que eles aprovam</li> 
       </ul> <p><b>NOTA</b>:  <p>Se essa opção estiver ativada ou desativada, os administradores de grupo poderão criar perfis de planilha de horas para os grupos e subgrupos que gerenciam e atribuí-los aos membros do grupo cujos perfis de usuário eles têm acesso para editar.</p> <p>Habilitar essa opção pode fornecer muito acesso para alguns administradores de grupo, pois eles podem visualizar as folhas de horas geradas pelos perfis de folha de horas (e as horas) para todos os usuários no sistema, não apenas para aqueles nos grupos que eles administram. Você pode desativar essa opção para administradores de grupo que não precisam desse acesso.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Quando terminar, clique em **Salvar**.
1. Atribua o novo nível de acesso a um usuário, conforme descrito em [Adicionar usuários](../../../administration-and-setup/add-users/create-and-manage-users/add-users.md).

   >[!NOTE]
   >
   >Você pode permitir que os usuários tenham acesso administrativo aos usuários. Para obter mais informações sobre como conceder aos usuários acesso administrativo aos usuários para que eles possam gerenciar contas de usuários, consulte [Conceder acesso aos usuários](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md).
