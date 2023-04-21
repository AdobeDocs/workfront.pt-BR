---
title: Como os níveis de acesso e as permissões funcionam em conjunto
user-type: administrator
content-type: reference
product-area: system-administration
keywords: acessar,modelo,funil,diagrama,níveis,permissões
navigation-topic: access-levels
description: O administrador do Adobe Workfront determina qual nível de acesso cada usuário deve ter. Esse nível de acesso define o que os usuários podem ver e fazer com tipos de objetos e áreas no sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 594e002c-19e3-4baa-b5f8-223c3fdf8ca8
source-git-commit: df73ba291f0a0ab6492e6fabfb6de578ba7e1f1b
workflow-type: tm+mt
source-wordcount: '906'
ht-degree: 2%

---

# Como os níveis de acesso e as permissões funcionam em conjunto

O administrador do Adobe Workfront determina qual nível de acesso cada usuário deve ter. Esse nível de acesso define o que os usuários podem ver e fazer com tipos de objetos e áreas no sistema.

Além disso, os usuários têm acesso a objetos individuais quando outros usuários compartilham e concedem certas permissões a esses objetos.

Assim, as atividades que um usuário pode fazer com um objeto são definidas por uma combinação do nível de acesso e das permissões fornecidas a ele para esse projeto.

![](assets/security-model-hierachy.png)

Por exemplo, se o seu nível de acesso indicar que você pode criar tarefas, mas as permissões recebidas em um projeto específico não permitem adicionar tarefas a ele, você não pode adicionar tarefas ao projeto, mesmo que possa criar tarefas em outro lugar no Workfront.

Este artigo explica como essa combinação funciona.

## Nível de acesso

O nível de acesso atribuído a cada usuário por um administrador do Workfront é necessário para fazer logon no Workfront.

Os níveis de acesso padrão são:

* Administrador do sistema (anexado à licença do Plano)
* Planejador (anexado à licença do Plano)
* Trabalhador (anexado à licença Trabalho)
* Revisor (anexo à licença de revisão)
* Solicitante (anexado à licença Solicitar)
* Usuário externo (anexado à licença de Email externo)

A licença do Workfront para cada nível de acesso padrão determina o que está disponível e configurável no nível de acesso. Para obter informações sobre as licenças do Workfront, consulte [Visão geral das licenças do Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).

Para os usuários atribuídos a ele, um nível de acesso define o que eles podem ver e fazer com os seguintes tipos de objetos e áreas no Workfront:

* Projetos
* Tarefas
* Problemas
* Portfólios
* Relatórios, painéis e calendários
* Filtros, exibições e agrupamentos
* Documentos
* Outros usuários
* Modelos
* Dados financeiros
* Gerenciamento de recursos
* Planejador de cenários
* Workfront Goals

Em um nível de acesso personalizado, é possível definir as configurações desses objetos e áreas para alterar o acesso que os usuários têm a eles. Dependendo da licença associada ao nível de acesso, bem como do tipo de objeto ou área, você pode configurar o nível de acesso para não permitir acesso, visualizar acesso ou editar acesso a um objeto ou área.

>[!IMPORTANT]
>
>É altamente recomendável deixar os níveis de acesso integrados inalterados para que você possa fazer referência a eles depois de configurar seus usuários. Para personalizar um nível de acesso, copie o nível de acesso padrão e modifique a cópia. (Você pode fazer isso para cada nível de acesso, exceto Administrador do sistema e Usuário externo.)

Para obter uma explicação detalhada de cada um dos níveis de acesso padrão, consulte [Níveis de acesso integrados no Adobe Workfront](../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md).

Para obter instruções sobre como atribuir um nível de acesso a um usuário, consulte [Editar o perfil de um usuário](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Permissões

Ao compartilhar um objeto com alguém no sistema, um usuário pode conceder ao recipient qualquer uma das seguintes permissões para o objeto .

* **Exibir**: Esse nível de permissão permite que o recipient compartilhe o objeto de uma das seguintes maneiras:

   * Em todo o sistema, para que todos os usuários possam visualizá-lo (não disponível para todos os objetos)
   * Com usuários externos que não têm uma licença Workfront (não disponível para todos os objetos)
   * Com um endereço de email (disponível somente para documentos)

* **Contribute**: (não disponível para todos os objetos)
* **Gerenciar**: Quando alguém compartilha um objeto, os direitos do recipient ao objeto são determinados por uma combinação do nível de acesso do recipient e das permissões para o objeto que foram concedidas pelo compartilhador. O menor grau de acesso disponível nessa combinação é o que determina o que o recipient pode fazer com o objeto.

   >[!INFO]
   >
   >**Exemplo:** Se o nível de acesso do destinatário não permitir a edição do projeto, essa pessoa não poderá editar ou excluir um projeto mesmo que o compartilhador tenha concedido permissões para gerenciá-lo.
   >
   >Ou, se o nível de acesso do destinatário permitir a edição do projeto, mas o compartilhador tiver concedido permissões somente para visualização a um projeto, o usuário não poderá editar ou excluir o projeto.

A tabela a seguir compara o acesso geral de um usuário aos objetos (definido pelo nível de acesso do usuário) às permissões de um objeto compartilhado específico:

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
   <td> <p>Herdado de um objeto compartilhado de classificação superior 
   </td> 
   <td> </td> 
   <td>✓</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Se um usuário compartilhar um objeto com determinadas permissões e esse objeto tiver qualquer objeto filho abaixo dele, o recipient herdará as mesmas permissões para esses objetos filho.
>* Se um nível de acesso impedir que os usuários excluam determinados objetos, isso não impede que eles excluam objetos filhos contidos nesses objetos.
>


## Mais cenários de exemplo

Quando Olivia compartilha um projeto do Workfront com Tony, o acesso de Tony a ele é determinado por uma combinação de duas coisas:

* Nível de acesso do Tony, atribuído pelo administrador do Workfront
* Permissões de Tony ao projeto, especificadas por Olivia

As ações de Tony no projeto podem ser ainda mais restritas no projeto, mas não podem ser irrestritas além do permitido no seu nível de acesso:

* Se o nível de acesso de Tony não lhe permite criar tarefas, ele não pode adicionar tarefas ao projeto, mesmo que Olivia lhe tenha dado permissões para adicionar tarefas a ele.
* Se o nível de acesso de Tony permitir que ele crie tarefas, mas Olivia não concedeu permissões para adicionar tarefas ao projeto, ele não poderá adicionar tarefas a esse projeto, mas poderá adicionar tarefas a outros projetos nos quais recebeu permissões para isso.
