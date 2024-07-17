---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurar efeito em horas em que um objeto é excluído e restaurado
description: Você pode configurar o que acontece com as horas quando alguém exclui um projeto, tarefa ou problema no qual as horas são registradas. A opção escolhida também determina o que acontece com as horas se o projeto, tarefa ou problema for restaurado posteriormente. (Para obter mais informações sobre como restaurar itens no Workfront, consulte Restaurar itens excluídos.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Configurar efeito em horas em que um objeto é excluído e restaurado

Você pode configurar o que acontece com as horas quando alguém exclui um projeto, tarefa ou problema no qual as horas são registradas. A opção escolhida também determina o que acontece com as horas se o projeto, tarefa ou problema for restaurado posteriormente. (Para obter mais informações sobre como restaurar itens no Workfront, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configure como as horas são gerenciadas quando um item é excluído e restaurado

1. Clique no ícone ![](assets/main-menu-icon.png) do **Menu Principal** no canto superior direito do Adobe Workfront e em **Configurar** ![](assets/gear-icon-settings.png).

1. Expanda **Folhas de horas e horas** e clique em **Preferências**.

1. Localize a seção **Preferências de exclusão de projetos, tarefas ou problemas**.
1. (Condicional) Para configurar como as horas são gerenciadas quando um projeto é excluído, selecione uma das seguintes opções na seção **Ao excluir projetos**:

   * Manter as horas reportadas já adicionadas às planilhas de horas como horas gerais (Se este projeto for restaurado no futuro, as horas permanecerão na planilha de horas)\
     Essa opção é selecionada por padrão.
   * Excluir horas reportadas (Se este projeto for restaurado no futuro, as horas reportadas serão restauradas no projeto)

1. (Condicional) Para configurar como as horas são gerenciadas quando uma tarefa ou problema é excluído, selecione uma das seguintes opções na seção **Ao excluir tarefas ou problemas**:

   * Mover as horas reportadas para o projeto onde a tarefa ou problema se encontra (Se esta tarefa ou este problema for restaurado mais tarde, as horas permanecerão no projeto)\
     Essa opção é selecionada por padrão.
   * Excluir horas reportadas (Se esta tarefa ou este problema for restaurado mais tarde, as horas reportadas serão restauradas na tarefa ou no problema)

1. Clique em **Salvar**.
