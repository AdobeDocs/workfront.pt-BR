---
title: Exibir todos os relatórios que usam um campo ou widget personalizado específico
description: Você pode adicionar uma visualização personalizada na área Forms personalizado que mostra quais relatórios estão usando um campo ou widget personalizado específico. Isso é útil quando você precisa editar ou excluir o campo ou widget, pois ele pode já estar implementado em um ou mais relatórios. É importante avaliar se esses relatórios precisarão de ajustes para continuar funcionando corretamente.
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Exibir todos os relatórios que usam um campo ou widget personalizado específico

Você pode adicionar uma visualização personalizada na área Forms personalizado que mostra quais relatórios estão usando um campo ou widget personalizado específico. Isso é útil quando você precisa editar ou excluir o campo ou widget, pois ele pode já estar implementado em um ou mais relatórios. É importante avaliar se esses relatórios precisarão de ajustes para continuar funcionando corretamente.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Adicionar um campo personalizado a um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) e [Adicionar ou editar um widget de ativo em um formulário personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## Requisitos de acesso

Você deve ter o seguinte para executar as etapas deste artigo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plano do Adobe Workfront*</p> </td> 
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

&#42;Para descobrir quais configurações de plano, tipo de licença ou nível de acesso você tem, entre em contato com o administrador do Workfront.

## Listar os relatórios que usam um campo ou widget personalizado específico

1. Clique em **Menu principal** ícone ![](assets/main-menu-icon.png) no canto superior direito do Adobe Workfront e clique em **Configuração** ![](assets/gear-icon-settings.png).

1. No painel esquerdo, clique em **Forms personalizado**.
1. Abra o **Campos** guia para exibir um relatório listando todos os campos e widgets personalizados na instância do Workfront.

   ![](assets/fields-tab.png)

1. Clique em **Exibir** no cabeçalho na parte superior da lista, em seguida, verifique se há exibições personalizadas na lista que incluam **Relatórios** (que não é uma coluna padrão nesta guia).

   A coluna Relatórios é o local onde você pode ver quais relatórios estão usando cada campo e widget personalizado que foi adicionado a um formulário personalizado em seu sistema. É possível que alguém já tenha criado uma visualização que inclui a variável **Relatórios** coluna.

1. Se você não vir uma visualização que inclua a variável **Relatórios** crie uma nova exibição que a inclua:

   1. Clique em **Exibir** e, em seguida, clique em **Nova visualização**.

   1. No **Nova visualização** que aparece, na caixa próxima ao canto superior esquerdo, substituir **Nova Exibição de Parâmetro** com um nome descritivo para a exibição, como *Campos e widgets*.

   1. Clique em **Adicionar coluna** próximo ao canto inferior direito.
   1. No **Mostrar nesta coluna** que é exibido próximo ao canto superior esquerdo, comece a digitar *relatório* e selecione **Relatórios** quando ele aparecer na lista abaixo da caixa.

   1. (Condicional) Se desejar mover a variável **Relatórios** coluna que você acabou de adicionar a uma posição horizontal diferente, arraste o cabeçalho na **Visualização da coluna** na parte inferior da página.

   1. Clique em **Concluído** e, em seguida, clique em **Salvar visualização**.

1. Clique em **Exibir** e selecione o nome da exibição personalizada que acabou de criar.
1. No **Nome** , localize o campo ou widget personalizado que deseja editar ou excluir e, em seguida, consulte o **Relatórios** coluna nessa linha para ver quais relatórios a usam, se houver.

   Para localizar as informações desta coluna, o Workfront pesquisa os campos e widgets personalizados em todos os filtros, visualizações e agrupamentos de relatório.

   Se você vir um sinal de mais, clique nessa linha de texto para exibir uma caixa listando todos os relatórios adicionais que usam o campo ou widget.

   >[!NOTE]
   >
   >O tempo de carregamento inicial dessa ferramenta pode levar de 10 segundos a 2,5 minutos, dependendo da quantidade de dados no sistema.

   >[!TIP]
   >
   >Se não tiver tempo para investigar os relatórios que estão usando o campo ou widget personalizado, você pode clicar em Exportar para criar um arquivo que os liste. Você pode compartilhar esse arquivo com qualquer um que possua um relatório que esteja usando o campo ou widget e discutir a alteração que precisa ocorrer, o impacto que ele pode ter no relatório e o que precisa ser feito para garantir que o relatório continue funcionando corretamente.
   >
   >Essa exibição também está disponível em um relatório de Parâmetro:
   >      
   > 1. No menu principal, clique em **Relatórios**.
   > 1. Ao lado do canto superior esquerdo, clique em **Novo Relatório** e, em seguida, clique em **Parâmetro** na lista exibida.
   > 1. Clique em **Adicionar coluna** próximo ao canto inferior direito.
   > 1. No **Mostrar nesta coluna** que é exibido próximo ao canto superior esquerdo, comece a digitar *relatório* e selecione **Relatórios** quando ele aparecer na lista abaixo da caixa.
   > 1. (Condicional) Se desejar mover a variável **Relatórios** coluna que você acabou de adicionar a uma posição horizontal diferente, arraste o cabeçalho na **Visualização da coluna** na parte inferior da página.
   > 1. Clique em **Concluído** e, em seguida, clique em **Salvar+Fechar**.
   > 1. Digite um nome descritivo para o relatório, como *Campos e widgets*.
