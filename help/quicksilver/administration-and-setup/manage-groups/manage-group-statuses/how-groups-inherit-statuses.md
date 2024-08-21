---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: Como os grupos herdam status
description: Ao listar os status disponíveis para um grupo, você vê o seguinte
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 3937fd72-fa54-4777-9ec4-1f097df7a2ee
source-git-commit: bd1a66950c6e16ef7eb05d385bd99fc2d3be35cc
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 0%

---

# Como os grupos herdam status

Ao listar os status disponíveis para um grupo, você vê o seguinte

* Status personalizados criados para o grupo, conforme explicado em [Criar ou editar um status de grupo](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Status herdados do sistema e de hierarquias superiores na hierarquia do grupo, conforme explicado neste artigo.

## Herdar status

Seu grupo herda os status quando qualquer uma das situações a seguir ocorre:

* Você cria o grupo.
* Um administrador bloqueia um status em um grupo de nível superior.
* Um administrador exclui outro grupo e escolhe o seu grupo para assumir o lugar dele.

A tabela abaixo explica cada uma dessas circunstâncias.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Ao criar um grupo</td> 
   <td> <p>Quando você cria um novo grupo, ele herda automaticamente:</p> 
    <ul> 
     <li>Status desbloqueados no grupo um nível acima, se o novo grupo for um subgrupo.</li> 
    </ul> 
    <ul> 
     <li>Status bloqueados no nível do sistema.</li> 
    </ul> 
     <b>EXEMPLO:</b></span></span> 
     <p>Suponha que um grupo chamado Marketing tenha dois subgrupos chamados Marketing Communications and Branding.</p> 
     <p>Um administrador de grupo do grupo de marketing cria um novo status personalizado chamado Descoberta.</p> 
     <p>Posteriormente, você cria um novo subgrupo no grupo Marketing e o chama de Advertising.</p> 
     <p>Seu subgrupo herda o status Descoberta porque você criou o grupo depois que o outro administrador criou o status Descoberta desbloqueado.</p> 
     <p>Como os subgrupos Comunicações de marketing e Identidade visual já existiam abaixo do grupo de marketing quando isso aconteceu, eles não herdam o status de Descoberta desbloqueado.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando um administrador bloqueia um status em um nível superior</td> 
   <td> <p>Quando um administrador do Workfront bloqueia um status no nível do sistema, seu grupo o herda junto com todos os outros grupos no sistema.</p> <p>Da mesma forma, quando um administrador bloqueia um status para um grupo acima do seu, o grupo o herda junto com quaisquer outros subgrupos abaixo do grupo superior.</p> <p><b>OBSERVAÇÃO</b>: posteriormente, se um administrador desbloquear um desses status no nível do sistema ou em um grupo acima do seu grupo, o grupo manterá o status herdado anteriormente. Agora é uma versão separada do status e você pode personalizá-lo apenas para o seu grupo.</p> 
    <p><b>EXEMPLO:</b></p>
    <p>O administrador do grupo de marketing bloqueia o status de descoberta mencionado acima para garantir que todos os três subgrupos o tenham.</p> 
    <p>Junto com seu grupo da Advertising, os grupos de Comunicações de marketing e Marcas têm o status de Descoberta agora. Eles a herdaram quando ela estava bloqueada no grupo Marketing acima deles.</p> 
    <p>O administrador do grupo de marketing desbloqueia o status da descoberta para que todos os três subgrupos tenham sua própria versão do status da descoberta. Agora, você e os administradores dos outros dois grupos podem personalizar o status da Descoberta para atender às necessidades dos seus grupos.</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Quando um administrador exclui um grupo</td> 
   <td> <p>Quando um administrador exclui um grupo e escolhe o seu lugar no sistema, o grupo herda os status personalizados do grupo excluído se ele ainda não existir no grupo.</p> 
   <p><b>EXEMPLO: </b></p>
     <p>Um grupo chamado Mensagens precisa ser mesclado com seu grupo do Advertising, portanto, um administrador do Workfront exclui o grupo de Mensagens e escolhe seu grupo para assumir o lugar.</p> 
     <p>O grupo de Mensagens tinha um status exclusivo chamado Em Andamento. O grupo Advertising agora tem esse status disponível para uso.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

## Herdar configurações de status

Quando você cria um grupo de nível superior, ele herda as seguintes configurações do nível do sistema. Quando você cria um subgrupo, ele herda as seguintes configurações do próximo grupo superior.

* Configurações de status padrão

  Para obter informações sobre esses itens, consulte [Usar status personalizados como status padrão](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/use-custom-statuses-as-default-statuses.md).

* Configurações da ordem de exibição de status

  Para obter informações sobre esses itens, consulte [Reordenar status de nível de sistema e de grupo](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/reorder-system-statuses.md).

Se alguém alterar essas configurações após a criação do grupo, os status não serão afetados.
