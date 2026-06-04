---
title: Como os níveis de acesso e as permissões herdadas funcionam juntos
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,modelo,funnel,diagrama,níveis,permissões
navigation-topic: access-levels
description: O administrador do Adobe Workfront determina o nível de acesso que cada usuário deve ter. Esse nível de acesso define o que os usuários podem ver e fazer com os tipos de objetos e áreas no sistema.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
TQID: https://experienceleague.adobe.com/yO-2iQdJUwZgAE93N-7Tqw3V8j3-JfYv0PrKohb-3o8
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
subfeature_v2: id: d3382524-5489-431b-bde9-271ab257bc37id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: d095671a-1355-40aa-8b5f-06c33c68080bid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 908
ht-degree: 48%

---

# Como os níveis de acesso e as permissões herdadas funcionam juntos

>[!NOTE]
>
>As informações contidas neste artigo referem-se aos níveis de acesso legados. Para obter informações sobre os níveis de acesso atuais, consulte [Visão geral dos novos níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md).

O administrador do Adobe Workfront determina o nível de acesso que cada usuário deve ter. Esse nível de acesso define o que os usuários podem ver e fazer com os tipos de objetos e áreas no sistema.

Os usuários também obtêm acesso a objetos individuais quando outros usuários compartilham e concedem determinadas permissões nesses objetos.


![Hierarquia do modelo de segurança](assets/security-model-hierachy.png)

Por exemplo, se o seu nível de acesso disser que você pode criar tarefas, mas as permissões que você receber em um projeto específico não permitirem adicionar tarefas a ele, você não poderá adicionar tarefas no projeto, mesmo que possa criar tarefas em outro lugar no Workfront.

Este artigo explica como essa combinação funciona.

## Nível de acesso

O nível de acesso atribuído a cada usuário por um administrador do Workfront é necessário para fazer logon no Workfront.

Os níveis de acesso padrão são:

* Administrador de sistema (anexado à licença do plano)
* Planejador (anexado à licença do Plano)
* Trabalhador (anexado à licença de Trabalho)
* Revisor (anexado à licença de revisão)
* Solicitante (anexado à licença de solicitação)
* Usuário externo (anexado à licença de Email externo)

A licença do Workfront para cada nível de acesso padrão determina o que está disponível e pode ser configurado no nível de acesso. Para obter informações sobre as licenças do Workfront, consulte [visão geral das licenças do Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Para os usuários atribuídos a ele, um nível de acesso define o que eles podem ver e fazer com os seguintes tipos de objeto e áreas no Workfront:

* Projetos
* Tarefas
* Problemas
* Portfólios
* Relatórios, painéis e calendários
* Filtros, visualizações e agrupamentos
* Documentos
* Outros usuários
* Modelos
* Dados financeiros
* Gerenciamento de recursos
* Planejador de cenários
* Workfront Goals

Em um nível de acesso personalizado, você pode definir as configurações desses objetos e áreas para alterar o nível de acesso que os usuários têm a eles. Dependendo da licença associada ao nível de acesso, bem como ao tipo de objeto ou área, você pode configurar o nível de acesso para não permitir nenhum acesso, acesso de visualização ou acesso de edição a um objeto ou área.

>[!IMPORTANT]
>
>É altamente recomendável deixar os níveis de acesso integrados inalterados para que possa consultá-los após configurar os usuários. Para personalizar um nível de acesso, copie o nível de acesso padrão e modifique a cópia. (Você pode fazer isso para todos os níveis de acesso, exceto para Administrador do sistema e Usuário externo.)

Para obter uma explicação detalhada de cada nível de acesso padrão, consulte [Níveis de acesso predefinidos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Para obter instruções sobre como atribuir um nível de acesso a um usuário, consulte [Editar perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Permissões

Ao compartilhar um objeto com alguém no sistema, um usuário pode conceder ao recipient qualquer uma das seguintes permissões para o objeto.

* **Visualização**: esse nível de permissão permite que o destinatário compartilhe o objeto de uma das seguintes maneiras:

   * Em todo o sistema, para que todos os usuários possam visualizá-lo (não disponível para todos os objetos)
   * Com usuários externos que não têm uma licença do Workfront (não disponível para todos os objetos)
   * Com um endereço de email (disponível somente para documentos)

* **Contribute**: (não disponível para todos os objetos)
* **Gerenciamento**: quando alguém compartilha um objeto, os direitos do destinatário ao objeto são determinados por uma combinação entre o nível de acesso do destinatário e as permissões do objeto que foram concedidas pelo compartilhador. O nível de acesso mais baixo disponível nessa combinação é o que determina o que o destinatário pode fazer com o objeto.

  >[!INFO]
  >
  >**Exemplo:** se o nível de acesso do destinatário não permitir a edição de projetos, essa pessoa não poderá editar nem excluir um projeto, mesmo que o compartilhador tenha concedido permissões para gerenciá-lo.
  >
  >Ou, se o nível de acesso do destinatário permitir a edição do projeto, mas quem compartilhou concedeu permissões somente de visualização para um projeto, o usuário não poderá editar ou excluir o projeto.

A tabela a seguir compara o acesso geral de um usuário aos objetos (definido pelo nível de acesso do usuário) com permissões para um objeto compartilhado específico:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th>Nível de acesso </th> 
   <th>Permissões </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Concedido por um administrador do Workfront no nível de acesso de um usuário</td> 
   <td>✓</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Concedido por um usuário que compartilha um objeto no nível do objeto</td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
  <tr> 
   <td> <p>Herdado de um objeto compartilhado de classificação mais alta 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Se um usuário compartilhar um objeto com determinadas permissões e esse objeto tiver objetos secundários abaixo dele, o destinatário herdará as mesmas permissões para eles também.
>* Se um nível de acesso impedir que os usuários excluam determinados objetos, isso não os impedirá de excluir objetos secundários contidos nesses objetos.
>

## Mais exemplos de cenários

Quando Olivia compartilha um projeto do Workfront com Tony, o acesso de Tony ao projeto é determinado por uma combinação de dois fatores:

* O nível de acesso de Tony, atribuído pelo administrador do Workfront
* As permissões de Tony para o projeto, especificadas por Olivia

As ações de Tony no projeto podem ser ainda mais restringidas no próprio projeto, mas não podem ser irrestritas além do que é permitido em seu nível de acesso:

* Se o nível de acesso de Tony não permitir que ele crie tarefas, ele não poderá adicionar tarefas ao projeto, mesmo que Olivia tenha lhe dado permissões para adicionar tarefas.
* Se o nível de acesso de Tony permitir que ele crie tarefas, mas Olivia não tiver concedido permissões para adicionar tarefas ao projeto, ele não poderá adicionar tarefas a esse projeto, mas poderá adicionar tarefas a outros projetos nos quais tenha recebido permissões para isso.
