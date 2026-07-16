---
title: Definir permissões padrão para registros
description: É possível definir permissões padrão para registros ao modificar o tipo de registro ou as configurações do espaço de trabalho. Você pode conceder permissões Abertas ou Restritas a todos os registros que serão adicionados a um tipo de registro.
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 9ef64f5a39c94426b2158c6504b913c8cb749c8e
workflow-type: tm+mt
source-wordcount: '674'
ht-degree: 4%

---


# Definir permissões padrão para registros

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   
<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}


É possível definir permissões padrão para registros ao modificar o tipo de registro ou as configurações do espaço de trabalho.

Você pode conceder permissões Abertas ou Restritas a todos os registros que serão adicionados a um tipo de registro.


## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo. 

<!--
at GA, check that the Workfront plans article linked below has Planning info
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
   <td role="rowheader"><p>Pacote do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer Workfront ou Fluxo de trabalho com um pacote do Planning</p> 
Ou
<p>Qualquer pacote de produto do Workfront Planning como independente</p>

</tr>

<tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td><p>Qualquer</p> 
   <p><b>Nota</b></p>
   <p>Somente pessoas com uma licença Standard podem receber permissões de Gerenciamento para registros. Todas as outras licenças só podem ter permissões de Exibição e a opção Gerenciar está esmaecida para elas.</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td>  <p>Gerenciar permissões para um espaço de trabalho e um tipo de registro</p>  
   <p><b>IMPORTANTE</b></p>
   <p>Somente usuários com permissões para Gerenciar um espaço de trabalho podem compartilhar um registro</p></td> 
  </tr>
</tbody> 
</table>

Para obter mais informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Considerações para definir permissões de registro padrão

Considere o seguinte ao configurar as permissões de registro padrão:

* Somente uma regra de permissão padrão pode estar ativa por tipo de registro por vez.
* A alteração da regra afeta apenas os registros criados após a alteração. Os registros existentes mantêm as permissões atuais.
* Os administradores do sistema e gerentes de espaço de trabalho sempre retêm o acesso Gerenciar a todos os registros, independentemente da regra.
* Depois que um registro é criado, suas permissões podem ser alteradas independentemente na caixa de diálogo de compartilhamento sem afetar a regra padrão.
* Para tipos de registros globais, cada espaço de trabalho (primário e secundário) pode configurar sua própria regra padrão, e novos registros assumirão a regra do espaço de trabalho em que foram criados.

## Configurar permissões de registro padrão para um espaço de trabalho

1. Ir para um espaço de trabalho > **Mais** menu ![Mais menu](assets/more-menu.png) > **Configurações** > **Tipos de registros**.

   ![Área de configurações de tipos de registros do Workspace](assets/workspace-record-types-settings-area.png)

1. (Opcional) Clique dentro da célula de um **Tipo de registro** para editar os nomes dos tipos de registro.

1. Na coluna **Padrão de novas permissões de registro**, clique na célula do tipo de registro cujas permissões você deseja atualizar.

1. Escolha entre as seguintes opções:

   * **Abrir**: todos os colaboradores do espaço de trabalho podem gerenciar registros recém-criados. Esse é o comportamento padrão atual para todos os tipos de registro existentes e novos.
   * **Restrito**: somente o criador de registros e qualquer pessoa adicionada explicitamente podem editar registros recém-criados. Todos os outros recebem acesso somente para visualização.

1. (Condicional) Se você estiver alterando as permissões padrão de **Restrito** para **Aberto**, clique em **Alternar** na caixa **Alternar para Aberto** para confirmar sua escolha.
1. (Condicional) Se você selecionou **Restrito**, adicione editores adicionais na coluna **Quem pode editar registros**. Você pode adicionar usuários, grupos, equipes, funções ou empresas.

   >[!NOTE]
   >
   >* O criador do registro é sempre incluído e não pode ser removido.
   >* Você só pode selecionar entidades que já tenham permissões do Contribute ou do Manage para o tipo de registro.

   As alterações são salvas automaticamente. Depois de salva, a regra entra em vigor imediatamente e se aplica automaticamente a todos os registros criados para esse tipo de registro a partir de agora.

## Configurar permissões de registro padrão para um tipo de registro

1. Ir para um tipo de registro > **Mais** menu ![Mais menu](assets/more-menu.png) > **Configurações** > **Configurações de registro**.

   ![Guia Configurações de registro na área Configurações de tipo de registro](assets/record-settings-tab-in-record-type-settings-area.png)

1. No campo **Tipo de permissão do registro**, clique em uma das seguintes opções:

   * **Abrir**: todos os colaboradores do espaço de trabalho podem gerenciar registros recém-criados. Esse é o comportamento padrão atual para todos os tipos de registro existentes e novos.
   * **Restrito**: somente o criador de registros e qualquer pessoa adicionada explicitamente podem editar registros recém-criados. Todos os outros recebem acesso somente para visualização.
1. (Condicional) Se você estiver alterando as permissões padrão de **Restrito** para **Aberto**, clique em **Alternar** na caixa **Alternar para Aberto** para confirmar sua escolha.
1. (Condicional) Se você selecionou **Restrito**, adicione editores no campo **Quem pode editar registros**. Você pode adicionar usuários, grupos, equipes, funções ou empresas.

   >[!NOTE]
   >
   >* O criador do registro é sempre incluído e não pode ser removido.
   >* Você só pode selecionar entidades que já tenham permissões do Contribute ou do Manage para o tipo de registro.

   As alterações são salvas automaticamente. Depois de salva, a regra entra em vigor imediatamente e se aplica automaticamente a todos os registros criados para esse tipo de registro a partir de agora.