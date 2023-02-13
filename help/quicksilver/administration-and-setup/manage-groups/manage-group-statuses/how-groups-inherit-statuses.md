---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Como os grupos herdam os status
description: Ao listar os status disponíveis para um grupo, você vê o seguinte
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 0%

---

# Como os grupos herdam os status

Ao listar os status disponíveis para um grupo, você vê o seguinte

* Status personalizados criados para o grupo, conforme explicado em [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Status herdados do sistema e do mais alto na hierarquia do grupo, conforme explicado neste artigo.

## Herdar status

Seu grupo herda os status quando qualquer um dos itens a seguir ocorrer:

* Crie o grupo.
* Um administrador bloqueia um status em um grupo de nível superior.
* Um administrador exclui outro grupo e escolhe seu grupo para tomar seu lugar.

O quadro abaixo explica cada uma dessas circunstâncias.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ao criar um grupo</td> 
   <td> <p>Ao criar um novo grupo, ele herda automaticamente:</p> 
    <ul> 
     <li>Status desbloqueados no grupo um nível acima, se o novo grupo for um subgrupo.</li> 
    </ul> 
    <ul> 
     <li>Status bloqueados no nível do sistema .</li> 
    </ul> 
     <b>EXEMPLO:</b></span></span> 
     <p>Suponha que um grupo chamado Marketing tenha 2 subgrupos chamados Marketing Communications e Branding.</p> 
     <p>Um administrador de grupo do grupo Marketing cria um novo status personalizado chamado Discovery.</p> 
     <p>Posteriormente, você cria um novo subgrupo no grupo Marketing e o chama de Publicidade.</p> 
     <p>O subgrupo herda o status Discovery porque você criou o grupo depois que o outro administrador criou o status Descoberta desbloqueada.</p> 
     <p>Como os subgrupos Marketing Communications and Branding já existiam abaixo do grupo Marketing quando isso aconteceu, eles não herdam o status de Descoberta desbloqueada.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando um administrador bloqueia um status em um nível superior</td> 
   <td> <p>Quando um administrador do Workfront bloqueia um status no nível do sistema, seu grupo o herda junto com todos os outros grupos no sistema.</p> <p>Da mesma forma, quando um administrador bloqueia um status para um grupo acima do seu grupo, o grupo o herda junto com qualquer outro subgrupo abaixo do grupo superior.</p> <p><b>OBSERVAÇÃO</b>: Posteriormente, se um administrador desbloquear um desses status no nível do sistema ou em um grupo acima do seu grupo, o grupo manterá o status que herdou anteriormente. Agora é uma versão separada do status e você pode personalizá-la apenas para o seu grupo.</p> 
    <p><b>EXEMPLO:</b></p>
    <p>O administrador do grupo de marketing bloqueia o status de Descoberta mencionado acima para garantir que todos os 3 subgrupos o tenham.</p> 
    <p>Junto com seu grupo de Publicidade, os grupos de Comunicações e Marcas de Marketing têm o status de Descoberta agora. Eles herdaram quando estava bloqueado no grupo de marketing acima deles.</p> 
    <p>Em seguida, o administrador do grupo de marketing desbloqueia o status de Descoberta para que todos os três subgrupos tenham sua própria versão do status de Descoberta. Agora você e os administradores dos outros 2 grupos podem personalizar o status de Descoberta para atender às necessidades de seus grupos.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando um administrador exclui um grupo</td> 
   <td> <p>Quando um administrador exclui um grupo e escolhe o seu para ocupar o seu lugar no sistema, o seu grupo herda os status personalizados do grupo excluído, se eles ainda não existirem no seu grupo.</p> 
   <p><b>EXEMPLO: </b></p>
     <p>Um grupo chamado Mensagens precisa se mesclar ao seu grupo Publicidade, de modo que um administrador do Workfront exclua o grupo Mensagens e escolha seu grupo para tomar seu lugar.</p> 
     <p>O grupo Mensagens tinha um status exclusivo chamado Em Andamento. Seu grupo de publicidade agora tem esse status disponível para uso.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Herdando configurações de status

Ao criar um grupo de nível superior, ele herda as seguintes configurações do nível do sistema. Ao criar um subgrupo, ele herda as seguintes configurações do próximo grupo superior.

* Configurações de status padrão

   Para obter informações sobre isso, consulte [Usar status personalizados como status padrão](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configurações da ordem de exibição de status

   Para obter informações sobre isso, consulte [Reordenar os status do sistema e do grupo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Se alguém alterar essas configurações após a criação do seu grupo, seus status não serão afetados.
