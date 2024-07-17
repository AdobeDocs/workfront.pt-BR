---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Status personalizados em um grupo que é movido ou excluído
description: Este artigo explica o que acontece com os status personalizados de grupo quando você move ou exclui um grupo.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 83885d86-eb00-46cc-93e9-e3364b6125e8
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '849'
ht-degree: 0%

---

# Status personalizados em um grupo que é movido ou excluído

Este artigo explica o que acontece com os status personalizados de grupo quando você move ou exclui um grupo.

## Status personalizados em um grupo movido

Considere os cenários a seguir que descrevem o que acontece com os status personalizados de grupo quando você move um grupo para um novo local em outro grupo.

Para obter informações sobre como mover um grupo, consulte [Mover um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/move-a-group.md).

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Quando um grupo é movido para outro grupo </td> 
   <td> <p>Todos os status do grupo movido permanecem com ele. Elas não são adicionadas aos status do novo grupo pai do grupo.</p> <p>Mas o grupo movido herda todos os status bloqueados no grupo ou nos grupos que agora estão mais altos em sua hierarquia. E, a partir de agora, se um administrador bloquear um status no topo da hierarquia, o grupo movido herdará esse status.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando um status em ambos os grupos tem a mesma chave, mas atributos diferentes</td> 
   <td> <p>Suponha que dois subgrupos diferentes herdem o mesmo status desbloqueado de um grupo principal. Os administradores de grupo dos 2 grupos personalizam o status para seus grupos de maneiras diferentes.</p> <p>Mais tarde, um dos dois grupos é movido para o outro. Agora, ambos têm um status com a mesma chave, mas ela tem atributos diferentes nos dois grupos.</p> <p>Nesse caso, uma das seguintes opções é verdadeira:</p> 
    <ul> 
     <li>Se o status no novo grupo pai for desbloqueado, o status no grupo movido manterá seus atributos, não afetados pela movimentação.</li> 
     <li>Se o status no novo grupo pai estiver bloqueado, os atributos do status no grupo pai substituirão aqueles do status no grupo movido.</li> 
    </ul> <p>Para obter informações sobre chaves de status, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Criar ou editar um status</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>Quando um grupo movido tem status herdados de seu grupo pai anterior </td> 
   <td> <p>Todos os status personalizados herdados do grupo pai anterior vêm com o grupo movido e se tornam seus próprios status personalizados. Eles não estão mais conectados ao grupo pai anterior.</p> 
    <ul> 
     <li>Se o grupo pai anterior editar um status personalizado bloqueado após a movimentação, as alterações não afetarão o status do subgrupo movido.</li> 
     <li>Se o grupo principal anterior bloquear um status personalizado que foi desbloqueado quando o grupo foi movido, o status do subgrupo movido não será bloqueado.</li> 
     <li>O grupo movido agora pode desbloquear status que foram bloqueados quando os herdou do grupo pai anterior.</li> 
    </ul> 
     <p><b>EXEMPLO:</b><p> 
     <p>Olivia, a administradora do grupo de marketing, cria dois status para o grupo. Ela nomeia uma Primeira Revisão, com a chave ABC, e a bloqueia. Ela nomeia a outra Final Review, com a chave XYZ, e não a bloqueia.</p> 
     <p>Ela também cria um subgrupo no grupo Marketing chamado Marketing de produto. No momento em que é criado, ele herda automaticamente a Primeira revisão e a Revisão final do grupo de Marketing.</p> 
     <p>Mais tarde, Olivia move o subgrupo Marketing de Produto no grupo Produto. Tanto a Primeira revisão quanto a Revisão final acompanham o grupo Marketing do produto até seu novo local no grupo Produto.</p> 
     <p>Embora a Primeira revisão tenha sido bloqueada antes da movimentação, o administrador do grupo de Marketing do produto pode editá-la agora, pois ela não é mais um status herdado controlado pelo grupo principal de onde veio.</p> 
     <p>A Revisão final é desbloqueada e editável como sempre foi.</p> 
     <p>Para o grupo de Marketing, Olivia altera as cores da Primeira Revisão e Revisão Final e as renomeia como Primeira Revisão Editada e Revisão Final Editada. Ela também bloqueia Final Review-Edited. Enquanto isso, no grupo Marketing do produto, as cores e os nomes dos status Primeira revisão e Revisão final não mudam.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Status personalizados em um grupo que é excluído

Ao deletar um grupo ou subgrupo, você reatribui as informações associadas a ele, inclusive seus status personalizados, a outro grupo ou subgrupo. Os status do grupo excluído são adicionados aos do grupo de destino.

Se um dos status do grupo excluído também estava sendo usado pelo grupo de destino (o status em ambos os grupos tem a mesma chave) e o grupo de destino personalizou o status de maneiras diferentes, as configurações da versão do grupo de destino substituem as configurações da versão do grupo movido.

>[!INFO]
>
>**EXEMPLO:**
>
>O administrador de grupo do Grupo A renomeia um status de nível de sistema desbloqueado para seu grupo. O administrador de grupo de um Grupo B também renomeia esse status para seu grupo. Embora o status tenha nomes diferentes nos dois grupos, ele tem a mesma chave.
>
>Mais tarde, o Grupo A é excluído e todas as suas informações são reatribuídas ao Grupo B.
>
>* O nome da versão do Grupo B do status substitui o nome da versão do Grupo A.
>* Se o status tiver sido aplicado a um objeto por alguém do Grupo A antes da exclusão desse grupo, o nome do status no objeto será atualizado para o nome do status usado pelo Grupo B.
>
>Para obter informações sobre a chave de um status, consulte a tabela neste artigo em [Criar ou editar um status personalizado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md#create) [Criar ou editar um status para um grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md#create).
>
>Para obter informações sobre como excluir um grupo, consulte [Excluir um grupo](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md).
