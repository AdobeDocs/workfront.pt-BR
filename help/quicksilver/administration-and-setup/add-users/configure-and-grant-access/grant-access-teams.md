---
title: Conceder acesso às equipes
description: Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário às equipes no Workfront
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 915d1520-f5c4-4e33-b645-cb219289383c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '685'
ht-degree: 5%

---

# Conceder acesso às equipes

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário às equipes no Workfront, conforme explicado na [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

## Requisitos de acesso

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
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, conforme explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no botão **Exibir** ou **Editar** à direita de Equipes e selecione as habilidades que deseja conceder em **Ajustar suas configurações**.

   * **Exibir**: se você estiver configurando como os usuários com qualquer licença podem exibir equipes, altere qualquer uma das seguintes opções:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Exibir equipes associadas aos meu grupos</td>
         <td>
          <p><b>Habilitado</b>: quando os usuários procuram equipes em um campo Team type-ahead, eles podem ver as equipes associadas a seus grupos, sejam ou não membros da equipe. </p>
          <p><b>Desabilitado</b>: quando os usuários procuram equipes em um campo Tipo antecipado de equipe, os usuários podem ver as equipes associadas a seus grupos somente onde eles são membros da equipe</p><p>Essa opção está ativada por padrão.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Exibir todas as equipes</td>
         <td><p>Quando essa opção está habilitada e os usuários procuram equipes em um campo Tipo de equipe antecipada, os usuários podem ver e selecionar qualquer equipe.</p><p>Essa opção está ativada por padrão. </p></td>
        </tr>
       </tbody>
      </table>

   * **Editar**: se você estiver configurando como os usuários com uma licença de Plano e de Trabalho podem gerenciar equipes, altere qualquer uma das seguintes opções:

     <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Criar</td>
         <td><p>Permite que usuários com uma licença de Plano ou de Trabalho criem equipes.</p><p>Essa opção está ativada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Excluir</td>
         <td><p> Permite que usuários com uma licença de Plano excluam as equipes que eles têm acesso para editar (indisponível para usuários com uma licença de Trabalho).</p><p>Essa opção está ativada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar equipes nos grupos que eu gerencio (somente administradores de grupo)</td>
         <td><p>Permite que os usuários de licença do Plano designados como administradores de grupo editem equipes associadas aos grupos que gerenciam.</p><p>Essa opção está ativada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar equipes nas quais participo</td>
         <td><p>Permite que os usuários Planejem a licença ou a licença de Trabalho para editar equipes das quais são membros.</p><p>Essa opção está desabilitada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Exibir equipes associadas aos meu grupos</td>
         <td>
         <p><b>Habilitado</b> Quando os usuários procuram equipes em um campo Team type-ahead, eles podem ver as equipes associadas a seus grupos, sejam ou não membros da equipe. </p>
         <p><b>Desabilitado</b>: quando os usuários procuram equipes em um campo Tipo antecipado de equipe, os usuários podem ver as equipes associadas a seus grupos somente onde eles são membros da equipe</p><p>Essa opção está ativada por padrão.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Exibir todas as equipes</td>
         <td><p>Quando essa opção está habilitada e os usuários procuram equipes em um campo Tipo de equipe antecipada, os usuários podem ver e selecionar qualquer equipe.</p><p>Essa opção está ativada por padrão. </p></td>
        </tr>
       </tbody>
      </table>

1. Clique no X para fechar a caixa **Ajustar suas configurações**.
1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configurar acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso a dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

>[!NOTE]
>
>* Os itens a seguir são verdadeiros, independentemente das configurações de nível de acesso:
>
>   * Os proprietários de equipes sempre podem visualizar e editar suas equipes
>   * Os usuários sempre têm acesso para ver as equipes em que estão
>
>* A configuração de qualquer opção disponível para Exibir e Editar (como &quot;Exibir equipes associadas a meus grupos&quot;) é mantida se você decidir selecionar Exibir em vez de Editar ou Editar em vez de Exibir em um nível de acesso.
>

## Acesso a equipes por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com problemas, consulte a seção [Equipes](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
