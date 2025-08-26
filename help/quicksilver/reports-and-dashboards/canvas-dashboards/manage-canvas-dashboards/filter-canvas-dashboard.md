---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Filtrar um painel da tela
description: Você pode aplicar um filtro a um Painel da tela de desenho depois de ele ter sido criado.
author: Courtney and Jenny
feature: Reports and Dashboards
source-git-commit: fcce7c6b9a2d10069a4b6c50b7b7a244ac538a33
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 0%

---

# Filtrar um painel da tela

>[!IMPORTANT]
>
>No momento, o recurso Painéis do Canvas está disponível apenas para usuários que participam da fase beta. Para obter mais informações, consulte [informações beta de Painéis do Canvas](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md).

É possível aplicar um filtro a um Painel da tela de desenho que contenha prompts. Um prompt funciona como um modificador de filtro que aplica critérios de filtragem adicionais para que você possa restringir ainda mais seus resultados. Esses prompts podem ser modificados toda vez que você aplicar o filtro, permitindo ajustar os resultados exibidos sem precisar editar os principais critérios de filtro do painel ou de cada relatório individual.

+++ Expanda para visualizar os requisitos de acesso. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>plano do Adobe Workfront</p></td> 
   <td> 
<p>Qualquer </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Licença do Adobe Workfront</p></td> 
   <td> 
<p>Atual: Plano </p> 
<p>Novo: Padrão</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Configurações de nível de acesso</p></td> 
   <td><p>Editar acesso a relatórios, painéis e calendários</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>Permissões de objeto</p></td> 
   <td><p>Gerenciar permissões do painel</p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Pré-requisitos

Você deve criar um painel antes que ele possa ser filtrado.

Para obter mais informações, consulte [Criar um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md).

## Filtrar um painel

Execute as seguintes etapas na ordem listada para filtrar um painel:

* [Parte 1: Criar um filtro de painel](#part-1-create-a-dashboard-filter)
* [Parte 2: Criar um prompt de painel](#part-2-define-a-dashboard-prompt)
* [Parte 3: Aplicar um prompt de painel](#step-3-apply-a-dashboard-prompt)

>[!NOTE]
>
>O filtro de painel será aplicado a todos os relatórios em que os filtros de nível de painel não estão desativados.  É possível excluir relatórios individuais da aplicação de filtros em nível de painel, expandindo o menu de ações para cada relatório e selecionando a opção **Desabilitar Filtros**.


### Parte 1: Criar um filtro de painel

Com um filtro de painel, é possível aplicar um filtro comum em todos os relatórios disponíveis em um painel sem precisar modificar os filtros para cada relatório individual.

>[!NOTE]
>
>Esses filtros só podem ser configurados por um usuário com acesso de Gerenciamento ao painel.


{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Na página **Painéis da Tela de Pintura**, selecione o painel ao qual deseja aplicar um filtro.

1. No canto superior esquerdo da página de detalhes do painel, clique em **Filtros**. O painel lateral Filtros se abre.

1. Selecione **Editar filtros**. A caixa de diálogo **Filtros do painel** é aberta.

1. (Opcional) Para adicionar uma regra, siga as etapas abaixo:

   1. Selecione o ícone **Editar** à direita da caixa de regras.

      ![Ícone Editar](assets/edit-icon.png)

   1. Clique em **Adicionar condição** e adicione as seguintes informações:
      * Selecione um campo pelo qual deseja filtrar.
      * Selecione uma opção (ou modificador de filtro) para definir que tipo de condição o campo deve atender.

   1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Prossiga para [Parte 2: Criar um prompt de painel](#part-2-define-a-dashboard-prompt).


### Parte 2: Definir um prompt de painel

Um prompt do painel oferece aos usuários a opção de aplicar filtros personalizados adicionais aos relatórios disponíveis no painel.

>[!NOTE]
>
>As opções de prompt do painel só podem ser configuradas por um usuário com acesso Gerenciar ao painel.

1. Para adicionar um prompt, siga as etapas abaixo:

   1. Selecione **Adicionar prompt**. Novos campos são exibidos no lado direito da tela.

   1. Insira um rótulo no campo **Personalizar rótulo**.

   1. Selecione o campo no qual deseja basear o prompt digitando o nome do campo e selecionando-o quando ele aparecer na lista. 

1. Para adicionar um prompt personalizado, siga as etapas abaixo:

   1. Selecione **Adicionar prompt personalizado**. Novos campos são exibidos no lado direito da tela.

   1. (Opcional) Insira um novo rótulo no campo **Personalizar rótulo**. Por padrão, o rótulo *Novo prompt personalizado* é atribuído.

   1. Clique em **Adicionar nova opção**.

   1. Digite o nome do prompt no campo **Valor da Opção**.

   1. Clique em **Adicionar condição** e especifique o campo pelo qual deseja filtrar e o modificador que define o tipo de condição que o campo deve atender.

      >[!NOTE]
      >
      >A condição de um prompt personalizado só pode ser editada usando o modo texto. Isso permite que várias condições sejam aplicadas em um único campo.


   1. (Opcional) Clique em **Adicionar grupo de filtros** para adicionar outro conjunto de critérios de filtragem. O operador padrão entre os conjuntos é AND. Clique no operador para alterá-lo para OU.

1. Clique em **Salvar** para aplicar o filtro ao painel.

1. Prossiga para [Parte 3: Aplicar um prompt de painel](#step-3-apply-a-dashboard-prompt).

### Etapa 3: Aplicar um prompt de painel

Todos os usuários com acesso a um painel podem aplicar um prompt de painel a um Painel da tela depois que o filtro e os prompts tiverem sido criados.

{{step1-to-dashboards}}

1. No painel esquerdo, clique em **Painéis do Canvas**.

1. Na página **Painéis da Tela de Pintura**, selecione o painel ao qual deseja aplicar o prompt.

1. No canto superior esquerdo da página de detalhes do painel, clique em **Filtros**. O painel lateral Filtros se abre.

1. Na seção **Mostrar registros onde...**, escolha uma condição para um ou todos os prompts exibidos. O prompt é aplicado e uma tag **Filtros do painel aplicados** é exibida no canto do widget de relatório.
   ![Selecionar condição](assets/prompts-list.png)

1. Clique no ícone **Fechar** ![Ícone Fechar](assets/close-icon.png) no canto superior direito para ocultar o painel.