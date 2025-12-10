---
title: Listar os níveis de acesso e as licenças de seus usuários
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,nível,licença
navigation-topic: access-levels
description: Você pode ver qual nível de acesso e licença estão atribuídos a cada usuário em uma lista de usuários ou relatório.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 5d85509d-276a-411e-813c-8b1fa2f512db
source-git-commit: 3d0a6932bda338af1e6b3dcba49bfc0ac486d919
workflow-type: tm+mt
source-wordcount: '334'
ht-degree: 5%

---

# Liste os níveis de acesso e as licenças de seus usuários

>[!NOTE]
>
>As informações neste artigo se referem aos níveis de acesso herdados. Para obter informações sobre os níveis de acesso atuais, consulte [Visão geral sobre novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

Você pode ver qual nível de acesso e licença estão atribuídos a cada usuário em uma lista de usuários ou relatório.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

Você deve ter o seguinte:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plano do Adobe Workfront*</td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso de visualização para usuários. Para obter mais informações sobre o acesso para exibir usuários, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">Conceder acesso aos usuários</a>.</p> <p><b>OBSERVAÇÃO</b>: se você ainda não tiver acesso, pergunte ao administrador do Workfront se ele definiu restrições adicionais no seu nível de acesso. Para obter informações sobre como um administrador do Workfront pode modificar seu nível de acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Criar ou modificar níveis de acesso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qual plano, tipo de licença ou acesso você tem, contate o administrador do Workfront.

+++

## Liste os níveis de acesso e as licenças de seus usuários

{{step-1-to-users}}

Por padrão, todos os usuários definidos como Ativos são exibidos na lista.

1. No menu suspenso **Exibir**, selecione **Licenças**.

   A coluna Licença exibe o nome da licença atribuída a cada usuário.

1. No menu suspenso **Agrupamento**, clique em **Tipo de Licença**.

   Essa exibição agrupa os usuários que têm os mesmos tipos de licença.

1. (Opcional) Para filtrar a lista por uma licença específica:

   1. Clique no menu suspenso **Filtro** e em **Novo Filtro**.

   1. Clique em **Adicionar uma Regra de Filtro**.
   1. Comece digitando **Licença** e selecione-a quando ela aparecer na lista.
   1. Com o modificador **Equal** selecionado, comece digitando o nome da licença pela qual deseja filtrar a lista.

      Você pode especificar mais de um tipo de licença.

   1. Clique em **Salvar filtro**.

      A lista exibe somente os usuários associados aos tipos de licença especificados no filtro.

   >[!TIP]
   >
   >Você também pode agrupar a lista por tipos de licença ou filtrá-la por uma licença específica.

