---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Excluir tipos de objeto em um formulário personalizado
description: Em um formulário personalizado existente, você pode excluir os tipos de objeto associados ao formulário. Depois disso, os usuários não poderão mais anexar o formulário a objetos desse tipo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 0%

---

# Excluir tipos de objeto em um formulário personalizado

<span class="preview">As informações destacadas nesta página se referem a funcionalidades ainda não disponíveis no geral. Ela está disponível somente no ambiente de Pré-visualização para todos os clientes ou no ambiente Produção para clientes que ativaram versões rápidas.</span>

<span class="preview">Para obter informações sobre lançamentos rápidos, consulte [Habilitar ou desabilitar versões rápidas para sua organização](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">Para obter informações sobre a versão atual, consulte [Visão geral da versão do segundo trimestre de 2024](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

Em um formulário personalizado existente, você pode excluir os tipos de objeto associados ao formulário. Depois disso, os usuários não poderão mais anexar o formulário a objetos desse tipo.

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

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
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Excluir tipos de objeto em um formulário personalizado

Você pode excluir tipos de objetos de um formulário personalizado existente.

Um formulário personalizado deve ter pelo menos um tipo de objeto.

>[!CAUTION]
>
>Se as pessoas já tiverem anexado o formulário personalizado a objetos do tipo que você deseja excluir e adicionado dados a ele, esses dados serão excluídos permanentemente quando você excluir esse tipo de objeto no formulário. Pode incluir informações históricas que os usuários precisarão mais tarde.
>
>Em geral, recomendamos minimizar o número de vezes que você edita um formulário personalizado que já está em uso. Não há um sistema de notificação para alertar as pessoas que usam o formulário personalizado sobre suas alterações.

{{step-1-to-setup}}

1. Clique em **Forms personalizado** no painel esquerdo.
1. Selecione o formulário personalizado que deseja editar e clique em **Editar** <span class="preview">ou ![Ícone Editar](assets/edit-icon.png).</span>
1. Clique no X em qualquer uma das **Tipos de objeto** que deseja excluir do formulário e, em seguida, clique em **Excluir** na mensagem de aviso que é exibida.

   ![](assets/click-x-object-types.jpg)

1. (Opcional) Repita a etapa anterior para qualquer outro tipo de objeto que você deseja remover do formulário.
1. Clique em **Concluído** e, em seguida, clique em **Salvar e fechar**.
