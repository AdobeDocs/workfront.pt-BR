---
title: Desativar ou reativar um formulário personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Você pode reativar ou desativar um formulário personalizado. Recomendamos desativar os formulários personalizados em vez de excluir os formulários que não são mais usados para manter os dados históricos.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 6d9a409d-8d16-4c58-ad02-f60aa1ac1714
source-git-commit: a7be72f0a594a21baed2592d8a2e467118ab1b7f
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 0%

---

# Desativar ou reativar um formulário personalizado

Você pode reativar ou desativar um formulário personalizado. Recomendamos desativar os formulários personalizados em vez de excluir os formulários que não são mais usados para manter os dados históricos.

>[!NOTE]
>
>Se um formulário personalizado estiver desativado, mas ainda fizer parte de um tópico da fila ou da definição da fila de solicitações, ele será anexado a novas solicitações. Se não quiser que o formulário esteja nas solicitações, remova-o manualmente da fila de solicitações.

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso para a funcionalidade neste artigo.

Você deve ter o seguinte acesso para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront</p> </td> 
   <td>Qualquer</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença do Adobe Workfront</td> 
   <td>
   <p>Novo: Padrão</p>
   <p>ou</p>
   <p>Atual: Plano</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p></td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desativar um formulário personalizado

É possível desativar formulários personalizados que não são mais usados sem perder os dados históricos associados. Os usuários não podem adicionar um formulário personalizado inativo aos objetos, mas ainda podem exibir e adicionar dados aos seus campos em objetos nos quais ele já foi anexado.

Os campos em um formulário personalizado inativo também ainda estão disponíveis para edição em linha em uma Exibição. Se um usuário adicionar um campo de um formulário personalizado inativo durante uma edição em linha, o formulário será anexado ao objeto automaticamente, mesmo que o formulário personalizado esteja desativado.

Para desativar um formulário personalizado:

{{step-1-to-setup}}

1. No painel esquerdo, escolha **Forms Personalizado**.
1. Na área **Forms**, selecione o formulário personalizado que deseja desativar.
1. Na coluna Está ativo, escolha **Falso** e clique fora da coluna. O formulário não está mais ativo.

## Reativar um formulário personalizado

Se você reativar um formulário personalizado, ele manterá as configurações que tinha antes e os usuários poderão interagir com ele como se nunca tivesse sido desativado.

{{step-1-to-setup}}

1. No painel esquerdo, escolha **Forms Personalizado**.
1. Na área **Forms**, selecione o formulário personalizado que deseja reativar.
1. Na coluna Está ativo, escolha **Verdadeiro** e clique fora da coluna. O formulário agora está ativo.
