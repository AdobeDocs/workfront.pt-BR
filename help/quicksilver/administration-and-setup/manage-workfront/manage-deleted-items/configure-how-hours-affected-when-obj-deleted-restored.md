---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurar o efeito em horas quando um objeto é excluído e restaurado
description: Você pode configurar o que acontece com horas quando alguém exclui um projeto, tarefa ou problema no qual as horas são registradas. A opção escolhida também determina o que acontece com as horas se o projeto, a tarefa ou o problema for restaurado posteriormente. (Para obter mais informações sobre como restaurar itens no Workfront, consulte Restaurar itens excluídos.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Configurar o efeito em horas quando um objeto é excluído e restaurado

Você pode configurar o que acontece com horas quando alguém exclui um projeto, tarefa ou problema no qual as horas são registradas. A opção escolhida também determina o que acontece com as horas se o projeto, a tarefa ou o problema for restaurado posteriormente. (Para obter mais informações sobre como restaurar itens no Workfront, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

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
   <td> <p>Você deve ser um administrador do Workfront.</p> <p><b>OBSERVAÇÃO</b>: Caso ainda não tenha acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais em seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar como as horas são gerenciadas quando um item é excluído e restaurado

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. Expandir **Folhas de Horas e Horas**, depois clique em **Preferências**.

1. Localize a variável **Preferências de Exclusão de Projeto, Tarefa ou Emissão** seção.
1. (Condicional) Para configurar como as horas são gerenciadas quando um projeto é excluído, selecione uma das seguintes opções na **Ao excluir projetos** seção:

   * Manter horas registradas já adicionadas às folhas de horas como horas gerais (Se este projeto for restaurado posteriormente, as horas permanecerão na folha de horas)\
      Essa opção é selecionada por padrão.
   * Excluir quaisquer horas registradas (Se este projeto for restaurado posteriormente, as horas registradas serão restauradas para o projeto)

1. (Condicional) Para configurar como as horas são gerenciadas quando uma tarefa ou problema é excluído, selecione uma das seguintes opções na **Ao excluir tarefas ou problemas** seção:

   * Mova quaisquer horas registradas para o projeto em que a tarefa ou emissão reside (Se esta tarefa ou problema for restaurado posteriormente, as horas permanecerão no projeto)\
      Essa opção é selecionada por padrão.
   * Excluir quaisquer horas registradas (Se essa tarefa ou problema for restaurado posteriormente, as horas registradas serão restauradas para a tarefa ou problema)

1. Clique em **Salvar**.
