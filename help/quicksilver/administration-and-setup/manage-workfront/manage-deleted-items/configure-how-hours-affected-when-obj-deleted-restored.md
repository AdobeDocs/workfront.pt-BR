---
user-type: administrator
product-area: system-administration
navigation-topic: manage-deleted-items
title: Configurar o efeito em horas quando um objeto é excluído e restaurado
description: Você pode configurar o que acontece com as horas quando alguém exclui um projeto, tarefa ou problema no qual as horas são registradas. A opção escolhida também determina o que acontece com as horas se o projeto, tarefa ou problema for restaurado posteriormente. (Para obter mais informações sobre como restaurar itens no Workfront, consulte Restaurar itens excluídos.)
feature: System Setup and Administration
role: Admin
exl-id: 466c3972-8108-49a6-98f6-f65f5fcc3617
TQID: https://experienceleague.adobe.com/-qjytcjOGAEltoclAl6xXJ-EuvW9hD0CrwMy8T3c-5g
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 360
ht-degree: 10%

---

# Configurar efeito em horas quando um objeto é excluído e restaurado

Você pode configurar o que acontece com as horas quando alguém exclui um projeto, tarefa ou problema no qual as horas são registradas. A opção escolhida também determina o que acontece com as horas se o projeto, tarefa ou problema for restaurado posteriormente. (Para obter mais informações sobre como restaurar itens no Workfront, consulte [Restaurar itens excluídos](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).)

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td><p>Qualquer</p></td> 
  </tr> 
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Administrador de sistema</td> 
  </tr> 
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configure como as horas são gerenciadas quando um item é excluído e restaurado

{{step-1-to-setup}}

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
