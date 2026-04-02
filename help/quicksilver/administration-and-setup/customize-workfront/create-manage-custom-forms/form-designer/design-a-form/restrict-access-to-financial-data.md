---
title: Restringir o acesso a dados financeiros em campos personalizados
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Ao criar um campo personalizado, é possível definir configurações opcionais para restringir o acesso a dados financeiros.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
source-git-commit: 5cdaccd9381b02f183b837208eaac4389b0b7a24
workflow-type: tm+mt
source-wordcount: '629'
ht-degree: 9%

---


# Restringir o acesso a dados financeiros em campos personalizados

{{highlighted-preview-article-level}}

Ao criar um campo personalizado, é possível definir configurações opcionais para restringir o acesso a dados financeiros. Dessa forma, os usuários que têm determinadas permissões definidas em seus níveis de acesso podem ver os dados e são impedidos de ver dados financeiros aos quais não deveriam ter acesso.

Para obter informações sobre como criar um campo personalizado, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

Para obter informações sobre níveis de acesso, consulte [Visão geral sobre níveis de acesso](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/access-level-overview.md). Para obter informações sobre compartilhamento e permissões, consulte [Visão geral das permissões de compartilhamento em objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Requisitos de acesso

+++ Expanda para visualizar os requisitos de acesso da funcionalidade neste artigo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Pacote do Adobe Workfront</td> 
   <td>Qualquer</td> 
  </tr>  
  <tr> 
   <td>Licença do Adobe Workfront</td> 
   <td><p>Padrão</p>
       <p>Plano</p></td>
  </tr> 
  <tr> 
   <td>Configurações de nível de acesso</td> 
   <td>Acesso administrativo a formulários personalizados</td> 
  </tr>  
 </tbody> 
</table>

Para obter informações, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Restringir o acesso a dados financeiros em um campo personalizado

1. Crie um novo formulário personalizado ou abra um formulário existente.

   Para obter informações, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Adicione um campo personalizado ao formulário ou selecione um campo existente.

   Esses tipos de campos podem ser restritos com base no acesso a dados financeiros:

   * Texto de linha única
   * Parágrafo
   * Menu suspenso de seleção única
   * Menu suspenso de seleção múltipla
   * Grupo de caixas de seleção
   * Botões de opção
   * Pesquisa externa
   * Pesquisa externa com seleção múltipla
   * Calculado

1. No campo **Formato**, selecione **Moeda**.

   >[!NOTE]
   >
   >Para campos calculados, qualquer formato é permitido. Todos os outros tipos de campo devem usar o formato **Moeda** ou o campo **Tipo de permissão de finanças** não estará disponível.

1. (Opcional) Somente para campos calculados, ative a opção **Permissão automática** para permitir que as permissões financeiras venham automaticamente dos campos na fórmula.

1. Selecione uma opção para o **tipo de permissão Finanças**.

   Os usuários devem ter esse tipo de permissão financeira antes de visualizar ou editar esse campo personalizado no formulário.

   * **Nenhuma permissão necessária:** todos os usuários podem ver este campo
   * **Geral:** os usuários devem ter permissões para editar ou exibir Finanças Gerais
   * **Cobrança:** Os usuários devem ter permissões para editar ou exibir taxas de cobrança
   * **Custo:** Os usuários devem ter permissões para editar ou exibir taxas de custo

   Para campos calculados:

   * O campo **Tipo de permissão financeira** não estará disponível para a configuração manual de permissões se o campo **Permissão automática** estiver ativado.
   * Os campos usados na fórmula determinam se o campo de permissão está ativo. Se o campo de permissão estiver em branco (e as permissões automáticas não estiverem ativadas), os campos na fórmula não oferecerão suporte às permissões financeiras.
   * O acesso é necessário para todos os campos na fórmula. Por exemplo, se dois campos forem usados em um campo calculado, um deles tiver permissão de faturamento aplicada e o segundo tiver permissão de custo aplicada, o usuário deverá ter permissões para visualizar as taxas de faturamento e de custo para ver o valor calculado.

1. Para salvar as alterações, clique em **Aplicar** e continue criando o formulário.

   Ou

   Clique em **Salvar e fechar**.

## Exemplo

Dois projetos são compartilhados com um usuário:

* O usuário tem permissão para editar todas as opções financeiras no primeiro projeto
* O usuário tem permissão para exibir taxas de faturamento e finanças gerais no segundo projeto

Quando o usuário edita o primeiro projeto, todos os campos financeiros no formulário personalizado são editáveis. Quando o usuário edita o segundo projeto, os campos definidos como **Lista** ou **Geral** são somente visualização e os campos definidos como **Custo** não estão visíveis.

Quando o usuário visualiza os projetos em uma lista ou relatório:

* Os campos financeiros podem ser visualizados ou editados de acordo com as permissões e as configurações do relatório
* Os campos financeiros ficam em branco se o usuário não tiver permissões para visualizá-los

A exportação de detalhes do projeto mostra os mesmos valores de campo financeiro (ou campos em branco) que na lista.

Ao editar ambos os projetos em massa, os campos de faturamento e finanças gerais são exibidos como somente leitura e os campos de custo mostram N/D.

