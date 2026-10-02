---
title: Configurar compartilhamento para campos e widgets personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Por padrão, ao adicionar um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como rótulo e nome da API. Você pode alterar isso controlando com quem ele pode ser compartilhado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
TQID: 'https://experienceleague.adobe.com/KyrIWEpIQQb-f8YODUPz3-RbP5wFww8Vu7Ffy33wUog'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ecee8b1aadd804a45ff0830e04e77981a3269cff
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 5%
---
# Configurar compartilhamento para campos e widgets personalizados

Por padrão, ao adicionar um novo campo ou widget personalizado a um formulário personalizado, qualquer pessoa no sistema com acesso a formulários personalizados pode editar as propriedades desse item, como rótulo e nome da API. Você pode alterar isso controlando com quem ele pode ser compartilhado.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar o compartilhamento de um campo ou widget personalizado

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Para compartilhar na lista de formulários e campos:

   1. Clique em **Campos** para abrir a área Campos.
   1. Selecione o campo que você deseja compartilhar e clique em ![Ícone Compartilhar](assets/share-icon.png).

1. Para compartilhar no designer do formulário:
   1. Abra um formulário personalizado ou crie um novo formulário personalizado.
   1. No designer do formulário, selecione o campo que deseja compartilhar e clique em **Compartilhar** na área de edição de campos à direita.

1. Na caixa de compartilhamento, em **Conceder acesso ao campo**, comece digitando o nome do usuário, da equipe, da função de trabalho, do grupo, da empresa ou do perfil comercial com o qual deseja compartilhar o item e pressione **Enter** quando o nome for exibido.
1. Se quiser ser mais específico sobre como compartilhar o item, clique no menu suspenso à direita do nome e use uma das seguintes opções:

   * **Exibir**: clique no ícone **Configurações Avançadas** ![ícone Configurações Avançadas](assets/configure-options-icon.png) para especificar se você deseja que os usuários possam adicionar o item a um formulário personalizado ou compartilhá-lo com outros usuários.
   * **Gerenciar**: permite acesso para editar o campo personalizado e visualizá-lo na biblioteca de campos e no designer do formulário. Clique no ícone **Configurações Avançadas** ícone ![Configurações Avançadas](assets/configure-options-icon.png) para especificar se você deseja que os usuários possam excluir o item do sistema ou compartilhá-lo com outros usuários.

1. (Opcional) Repita as etapas 5 a 6 para adicionar outros nomes à lista e configurar suas opções.
1. (Opcional) Escolha uma opção de compartilhamento em todo o sistema para o campo:

   * **Todos no sistema podem editar** (a opção padrão)

     Ao adicionar um campo ou widget personalizado e não limitar o compartilhamento, todos os usuários no sistema que têm acesso a formulários personalizados podem visualizá-lo e editar suas propriedades.

   * **Todos no sistema podem visualizar**

     Todas as pessoas no sistema que têm acesso a formulários personalizados podem visualizar o campo, mas não editá-lo.

   * **Somente pessoas convidadas podem acessar**

     Limita o acesso somente àqueles que você adicionou à lista.

   ![Opções de compartilhamento](assets/share-field-in-designer.png)

1. Clique em **Salvar**.

## Acesso herdado a campos e widgets personalizados quando um formulário personalizado é compartilhado

Quando alguém compartilha um formulário personalizado com um grupo, função de trabalho, equipe, empresa ou perfil comercial, os destinatários herdam o acesso de Visualização a todos os campos e widgets personalizados que estão no formulário. Esse nível de acesso a esses itens no formulário é sempre retido para que o formulário possa funcionar para os recipients conforme pretendido pela pessoa que o criou. Isso é verdade mesmo para recipients que têm acesso para Editar ao formulário.

Você pode descobrir quem herdou acesso a um campo ou widget personalizado e remover o acesso a ele.

>[!NOTE]
>
>Se um recipient tiver Acesso de gerenciamento a um campo ou widget personalizado no formulário personalizado compartilhado, esse acesso será retido para o recipient.

### Descubra quem herdou acesso a um campo ou widget personalizado {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Clique em **Campos** e selecione o campo, a imagem ou o widget de acesso.
1. Na caixa exibida, clique em **Permissões Herdadas** e exiba os nomes exibidos.
1. Clique em **Cancelar**.

### Remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

Se você precisar remover o acesso a um campo ou widget personalizado em um formulário personalizado que foi compartilhado, será necessário cancelar o compartilhamento do formulário. Para obter instruções, consulte a seção [Remover acesso a um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form) no artigo [Compartilhar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).


