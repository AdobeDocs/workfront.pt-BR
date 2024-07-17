---
title: Como os níveis de acesso e as permissões funcionam juntos
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acesso,modelo,funil,diagrama,níveis,permissões
navigation-topic: access-levels
description: O administrador do Adobe Workfront determina o nível de acesso que cada usuário deve ter. Esse nível de acesso define o que os usuários podem ver e fazer com os tipos de objetos e áreas no sistema.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: 09afa5808fd4078def16da7a9ccf393c99f47d03
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 2%

---

# Como os níveis de acesso e as permissões funcionam juntos

O administrador do Adobe Workfront determina o nível de acesso que cada usuário deve ter. Esse nível de acesso define o que os usuários podem ver e fazer com os tipos de objetos e áreas no sistema.

Os usuários também obtêm acesso a objetos individuais quando outros usuários compartilham e concedem determinadas permissões nesses objetos.


![](assets/security-model-hierachy.png)

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
>É altamente recomendável que você deixe os níveis de acesso incorporados inalterados para que possa consultá-los após configurar os usuários. Para personalizar um nível de acesso, copie o nível de acesso padrão e modifique a cópia. (Você pode fazer isso para todos os níveis de acesso, exceto para Administrador do sistema e Usuário externo.)

Para obter uma explicação detalhada de cada nível de acesso padrão, consulte [Níveis de acesso predefinidos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Para obter instruções sobre como atribuir um nível de acesso a um usuário, consulte [Editar perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Permissões

Ao compartilhar um objeto com alguém no sistema, um usuário pode conceder ao recipient qualquer uma das seguintes permissões para o objeto.

* **Exibir**: este nível de permissão permite que o destinatário compartilhe o objeto de uma das seguintes maneiras:

   * Em todo o sistema, para que todos os usuários possam visualizá-lo (não disponível para todos os objetos)
   * Com usuários externos que não têm uma licença do Workfront (não disponível para todos os objetos)
   * Com um endereço de email (disponível somente para documentos)

* **Contribute**: (não disponível para todos os objetos)
* **Gerenciar**: quando alguém compartilha um objeto, os direitos do destinatário ao objeto são determinados por uma combinação do nível de acesso do destinatário e das permissões do objeto que foram concedidas pelo compartilhador. O grau mais baixo de acesso disponível nessa combinação é o que determina o que o recipient pode fazer com o objeto.

  >[!INFO]
  >
  >**Exemplo:** se o nível de acesso do destinatário não permitir a edição de projetos, essa pessoa não poderá editar nem excluir um projeto, mesmo que o compartilhador tenha concedido permissões para gerenciá-lo.
  >
  >Ou, se o nível de acesso do recipient permitir a edição do projeto, mas o compartilhador conceder permissões somente de visualização para um projeto, o usuário não poderá editar nem excluir o projeto.

A tabela a seguir compara o acesso geral de um usuário a objetos (definido pelo nível de acesso do usuário) com permissões para um objeto compartilhado específico:

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
   <td>✓ µ</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>Concedido por um usuário que compartilha um objeto no nível do objeto</td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
  <tr> 
   <td> <p>Herdado de um objeto compartilhado de classificação mais alta 
   </td> 
   <td> </td> 
   <td>✓ µ</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Se um usuário compartilhar um objeto com determinadas permissões e esse objeto tiver quaisquer objetos filho abaixo dele, o recipient herdará as mesmas permissões para esses objetos filho.
>* Se um nível de acesso impedir que os usuários excluam determinados objetos, isso não os impedirá de excluir objetos filho contidos nesses objetos.
>

## Mais exemplos de cenários

Quando Olivia compartilha um projeto do Workfront com Tony, o acesso de Tony a ele é determinado por uma combinação de duas coisas:

* Nível de acesso de Tony, atribuído pelo administrador do Workfront
* As permissões de Tony para o projeto, especificado por Olivia

As ações de Tony no projeto podem ser restritas ainda mais no projeto, mas elas não podem ser irrestritas além do que é permitido em seu nível de acesso:

* Se o nível de acesso de Tony não permite que ele crie tarefas, ele não pode adicionar tarefas ao projeto, mesmo se Olivia lhe deu permissões para adicionar tarefas a ele.
* Se o nível de acesso de Tony permite que ele crie tarefas, mas Olivia não concedeu permissões para adicionar tarefas ao projeto, ele não pode adicionar tarefas a esse projeto, mas ele pode adicionar tarefas a outros projetos onde ele tem permissões para fazê-lo.
