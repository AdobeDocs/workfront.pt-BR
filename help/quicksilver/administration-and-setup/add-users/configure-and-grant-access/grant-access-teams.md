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
ht-degree: 4%

---

# Conceder acesso às equipes

Como administrador do Adobe Workfront, você pode usar um nível de acesso para definir o acesso de um usuário às equipes no Workfront, como explicado em [Visão geral dos níveis de acesso](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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

## Configurar o acesso dos usuários para editar usuários usando um nível de acesso personalizado

1. Comece a criar ou editar o nível de acesso, como explicado em [Criar ou modificar níveis de acesso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Clique no ícone de engrenagem ![](assets/gear-icon-settings.png) no **Exibir** ou **Editar** à direita de Equipes, selecione as habilidades que deseja conceder em **Ajustar as configurações**.

   * **Exibir**: Se você estiver configurando como os usuários com qualquer licença podem exibir equipes, altere qualquer uma das seguintes opções:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Exibir equipes associadas aos meu grupos</td>
         <td>
          <p><b>Ativado</b>: Quando os usuários procuram equipes em um campo de tipo avançado em Equipe , eles podem ver as equipes associadas a seus grupos, sejam ou não membros da equipe. </p>
          <p><b>Desabilitado</b>: Quando os usuários procuram equipes em um campo de antecipação de tipo de equipe, os usuários podem ver as equipes associadas a seus grupos somente onde são membros da equipe</p><p>Essa opção é ativada por padrão.</p>
          </td>
        </tr>
        <tr>
         <td role="rowheader">Exibir todas as equipes</td>
         <td><p>Quando essa opção é ativada e os usuários procuram equipes em um campo de tipo Equipe antecipada, os usuários podem ver e selecionar qualquer equipe.</p><p>Essa opção é ativada por padrão. </p></td>
        </tr>
       </tbody>
      </table>

   * **Editar**: Se você estiver configurando como os usuários com uma licença do Plano e uma licença do Trabalho podem gerenciar equipes, altere qualquer uma das seguintes opções:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader">Criar</td>
         <td><p>Permite que usuários com uma licença do Plano ou licença do Trabalho criem equipes.</p><p>Essa opção é ativada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Excluir</td>
         <td><p> Permite que usuários com uma licença do Plano excluam as equipes que eles têm acesso para editar (não disponível para usuários com uma licença do Trabalho).</p><p>Essa opção é ativada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar equipes nos grupos que eu gerencio (somente administradores de grupo)</td>
         <td><p>Permite que os usuários da licença do Plano designados como administradores de grupo editem equipes associadas aos grupos que gerenciam.</p><p>Essa opção é ativada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Editar equipes nas quais estou</td>
         <td><p>Permite que usuários Planejam licença ou Licença de Trabalho para editar equipes em que são membros.</p><p>Essa opção é desativada por padrão.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Exibir equipes associadas aos meu grupos</td>
         <td>
         <p><b>Ativado</b> Quando os usuários procuram equipes em um campo de tipo avançado em Equipe , eles podem ver as equipes associadas a seus grupos, sejam ou não membros da equipe. </p>
         <p><b>Desabilitado</b>: Quando os usuários procuram equipes em um campo de antecipação de tipo de equipe, os usuários podem ver as equipes associadas a seus grupos somente onde são membros da equipe</p><p>Essa opção é ativada por padrão.</p>
         </td>
        </tr>
        <tr>
         <td role="rowheader">Exibir todas as equipes</td>
         <td><p>Quando essa opção é ativada e os usuários procuram equipes em um campo de tipo Equipe antecipada, os usuários podem ver e selecionar qualquer equipe.</p><p>Essa opção é ativada por padrão. </p></td>
        </tr>
       </tbody>
      </table>

1. Clique no X para fechar o **Ajustar as configurações** caixa.
1. (Opcional) Para definir as configurações de acesso para outros objetos e áreas no nível de acesso em que você está trabalhando, continue com um dos artigos listados em [Configuração do acesso ao Adobe Workfront](../../../administration-and-setup/add-users/configure-and-grant-access/configure-access.md), como [Conceder acesso a tarefas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md) e [Conceder acesso aos dados financeiros](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).
1. Quando terminar, clique em **Salvar**.

>[!NOTE]
>
>* As seguintes opções são verdadeiras, independentemente das configurações de nível de acesso:
   >
   >   * Os proprietários de equipes sempre podem exibir e editar suas equipes
   >   * Os usuários sempre têm acesso para visualizar as equipes em que estão
>
* A configuração de qualquer opção disponível para Exibir e Editar (como &quot;Exibir equipes associadas a meus grupos&quot;) é retida se você decidir selecionar Exibir em vez de Editar ou Editar em vez de Exibir em um nível de acesso.
>


## Acesso às equipes por tipo de licença

Para obter informações sobre o que os usuários em cada nível de acesso podem fazer com problemas, consulte a seção [Equipes](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md#teams) no artigo [Funcionalidade disponível para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/functionality-available-for-each-object-type.md).
