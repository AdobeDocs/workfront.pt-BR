---
title: Exibir todos os relatórios que usam um determinado campo personalizado ou widget
description: Você pode adicionar uma visualização personalizada na área Forms personalizado que mostra quais relatórios estão usando um campo ou widget personalizado específico. Isso é útil quando você precisa editar ou excluir o campo ou widget, pois ele pode já estar implementado em um ou mais relatórios. É importante avaliar se esses relatórios precisarão de ajustes para continuar funcionando corretamente.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 554e08c22f6ee142a9ced8fa991d0126b6360b0c
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# Exibir todos os relatórios que usam um campo ou widget personalizado específico

Você pode adicionar uma visualização personalizada na área Forms personalizado que mostra quais relatórios estão usando um campo ou widget personalizado específico. Isso é útil quando você precisa editar ou excluir o campo ou widget, pois ele pode já estar implementado em um ou mais relatórios. É importante avaliar se esses relatórios precisarão de ajustes para continuar funcionando corretamente.

Para obter informações sobre campos e widgets personalizados em formulários personalizados, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td> <p>Acesso administrativo a formulários personalizados</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obter mais detalhes sobre as informações nesta tabela, consulte [Requisitos de acesso na documentação do Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Listar os relatórios que usam um campo ou widget personalizado específico

{{step-1-to-setup}}

1. No painel esquerdo, clique em **Forms Personalizado**.
1. Clique em **Campos** para exibir um relatório que lista todos os campos e widgets personalizados da sua instância do Workfront.

1. Clique no menu **Exibir** e verifique se há exibições personalizadas na lista que incluam a coluna **Relatórios** (que não é uma coluna padrão nesta guia).

   A coluna Relatórios é o local onde você pode ver quais relatórios estão usando cada campo e widget personalizado que foi adicionado a um formulário personalizado em seu sistema. É possível que alguém já tenha criado uma exibição que inclui a coluna **Relatórios**.

1. Se você não vir um modo de exibição que inclua a coluna **Relatórios**, crie um novo modo de exibição que o inclua:

   1. Clique no menu **Exibir** e em **Nova exibição**.

   1. Na página **Nova Exibição** que aparece, na caixa próxima ao canto superior esquerdo, substitua **Nova Exibição de Parâmetros** por um nome descritivo para a exibição, como *Campos e widgets*.

   1. Clique em **Adicionar coluna** próximo ao canto inferior direito.
   1. Na caixa **Mostrar nesta coluna** que é exibida próxima ao canto superior esquerdo, comece digitando *relatório* e selecione **Relatórios** quando ele aparecer na lista abaixo da caixa.

   1. (Condicional) Se quiser mover a coluna **Relatórios** que você acabou de adicionar para uma posição horizontal diferente, arraste o cabeçalho na área **Visualização da coluna**, na parte inferior da página.

   1. Clique em **Concluído** e em **Salvar exibição**.

1. Clique no menu suspenso **Exibir** e selecione o nome da exibição personalizada que você acabou de criar.
1. Na coluna **Nome**, localize o campo ou widget personalizado que você planeja editar ou excluir, em seguida, verifique a coluna **Relatórios** nessa linha para ver quais relatórios o usam, se houver.

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
   > 1. Próximo ao canto superior esquerdo, clique em **Novo relatório** e em **Parâmetro** na lista exibida.
   > 1. Clique em **Adicionar coluna** próximo ao canto inferior direito.
   > 1. Na caixa **Mostrar nesta coluna** que é exibida próxima ao canto superior esquerdo, comece digitando *relatório* e selecione **Relatórios** quando ele aparecer na lista abaixo da caixa.
   > 1. (Condicional) Se quiser mover a coluna **Relatórios** que você acabou de adicionar para uma posição horizontal diferente, arraste o cabeçalho na área **Visualização da coluna**, na parte inferior da página.
   > 1. Clique em **Concluído** e em **Salvar+Fechar**.
   > 1. Digite um nome descritivo para o relatório, como *Campos e widgets*.
