---
title: Exibir todos os relatórios que usam um campo ou widget personalizado específico
description: Você pode adicionar uma exibição personalizada na área Forms personalizada que mostra quais relatórios estão usando um campo ou widget personalizado específico. Isso é útil quando é necessário editar ou excluir o campo ou widget, pois ele já pode ser implementado em um ou mais relatórios. É importante avaliar se esses relatórios precisarão de ajustes para manter o funcionamento correto.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Exibir todos os relatórios que usam um campo ou widget personalizado específico

Você pode adicionar uma exibição personalizada na área Forms personalizada que mostra quais relatórios estão usando um campo ou widget personalizado específico. Isso é útil quando é necessário editar ou excluir o campo ou widget, pois ele já pode ser implementado em um ou mais relatórios. É importante avaliar se esses relatórios precisarão de ajustes para manter o funcionamento correto.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas neste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plano Adobe Workfront*</p> </td> 
   <td>Qualquer Um</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licença da Adobe Workfront*</td> 
   <td>Plano</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configurações de nível de acesso*</td> 
   <td> <p>Acesso administrativo a formulários personalizados</p> <p>Para obter informações sobre como os administradores do Workfront concedem esse acesso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder aos usuários acesso administrativo a determinadas áreas</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para descobrir que plano, tipo de licença ou configurações de nível de acesso você possui, entre em contato com o administrador da Workfront.

## Listar os relatórios que usam um campo ou widget personalizado específico

1. Clique no botão **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront, em seguida, clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizada**.
1. Abra o **Campos** para exibir um relatório listando todos os campos e widgets personalizados na instância do Workfront.

   ![](assets/fields-tab.png)

1. Clique no botão **Exibir** menu suspenso no cabeçalho na parte superior da lista, em seguida, verifique se há exibições personalizadas na lista que incluem o **Relatórios** (que não é uma coluna padrão nessa guia).

   A coluna Relatórios é onde você pode ver quais relatórios estão usando cada campo e widget personalizado que foi adicionado a um formulário personalizado em seu sistema. É possível que alguém já tenha criado uma exibição que inclua a variável **Relatórios** coluna.

1. Se você não vir uma exibição que inclui a variável **Relatórios** criar uma nova exibição que inclua:

   1. Clique no botão **Exibir** menu suspenso e, em seguida, clique em **Nova exibição**.

   1. No **Nova exibição** página exibida, na caixa próxima ao canto superior esquerdo, substitua **Nova exibição de parâmetro** com um nome descritivo para a exibição, como *Campos e widgets*.

   1. Clique em **Adicionar coluna** próximo ao canto inferior direito.
   1. No **Mostrar nesta coluna** caixa que é exibida próximo ao canto superior esquerdo, comece a digitar *relatório*, em seguida selecione **Relatórios** quando aparecer na lista abaixo da caixa.

   1. (Condicional) Se você deseja mover a variável **Relatórios** que acabou de adicionar a uma posição horizontal diferente, arraste o cabeçalho na **Visualização de coluna** na parte inferior da página.

   1. Clique em **Concluído**, depois clique em **Salvar exibição**.

1. Clique no botão **Exibir** selecione o nome da exibição personalizada que acabou de criar.
1. No **Nome** , encontre o campo personalizado ou o widget que você planeja editar ou excluir e, em seguida, olhe a **Relatórios** nessa linha para ver quais relatórios a utilizam, se houver.

   Para localizar as informações dessa coluna, o Workfront pesquisa os campos e widgets personalizados em todos os filtros, exibições e agrupamentos de relatórios.

   Se você vir um sinal de mais, pode clicar nessa linha de texto para exibir uma caixa listando todos os relatórios adicionais que usam o campo ou widget.

   >[!NOTE]
   >
   >O tempo de carregamento inicial dessa ferramenta pode levar de 10 segundos a 2,5 minutos, dependendo da quantidade de dados no sistema.

   >[!TIP]
   >
   >Se não tiver tempo para investigar os relatórios que estão usando o campo personalizado ou o widget, clique em Exportar para criar um arquivo que os lista. Você pode compartilhar esse arquivo com qualquer pessoa proprietária de um relatório que esteja usando o campo ou widget e discutir a alteração que precisa ocorrer, o impacto que ele pode ter no relatório e o que precisa ser feito para garantir que o relatório continue a funcionar corretamente.
   >
   >Esta exibição também está disponível em um relatório de Parâmetro:
   >      
   > 1. No Menu principal, clique em **Relatórios**.
   > 1. Próximo ao canto superior esquerdo, clique em **Novo relatório**, depois clique em **Parâmetro** na lista que é exibida.
   > 1. Clique em **Adicionar coluna** próximo ao canto inferior direito.
   > 1. No **Mostrar nesta coluna** caixa que é exibida próximo ao canto superior esquerdo, comece a digitar *relatório*, em seguida selecione **Relatórios** quando aparecer na lista abaixo da caixa.
   > 1. (Condicional) Se você deseja mover a variável **Relatórios** que acabou de adicionar a uma posição horizontal diferente, arraste o cabeçalho na **Visualização de coluna** na parte inferior da página.
   > 1. Clique em **Concluído**, depois clique em **Salvar+Fechar**.
   > 1. Digite um nome descritivo para o relatório, como *Campos e widgets*.

