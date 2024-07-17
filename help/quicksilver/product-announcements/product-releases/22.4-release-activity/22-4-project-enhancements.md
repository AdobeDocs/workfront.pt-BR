---
title: 22.4 Aprimoramentos do projeto
description: 22.4 Aprimoramentos do projeto
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '965'
ht-degree: 2%

---

# 22.4 Aprimoramentos do projeto

Esta página descreve todas as melhorias feitas no Project com a versão 22.4 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas na semana de 3 de outubro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.4, consulte a [Visão geral da versão 22.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Detalhes do predecessor agora disponíveis

Para exibir os detalhes dos predecessores de uma tarefa, agora é possível passar o mouse sobre o número do predecessor na coluna Predecessores. A caixa de detalhes exibe a tarefa predecessora e o projeto que está sendo referenciado, as datas de início e término planejadas para a tarefa predecessora e o número de predecessores e sucessores da tarefa predecessora. Você pode expandir os detalhes do projeto para ver mais informações sobre o projeto. Informações adicionais são incluídas para predecessoras entre projetos.

Para obter mais informações, consulte [Criar uma relação de predecessora na lista de tarefas](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Atribuir várias equipes a uma tarefa ou problema

Para oferecer muito mais flexibilidade na maneira como você gerencia tarefas e problemas, possibilitamos atribuir várias equipes a uma tarefa ou problema. Anteriormente, somente uma equipe podia ser atribuída a uma tarefa ou problema.

>[!NOTE]
>
>Essa funcionalidade não está disponível no Balanceador de carga de trabalho na área Equipes.

Para obter mais informações, consulte [Atribuir tarefas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) e [Atribuir problemas](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Seleção de usuário inteligente para funções de projeto nas áreas Editar e Detalhes

Melhoramos a forma como os usuários são exibidos ao adicioná-los aos seguintes campos de projeto na caixa Editar e na seção Detalhes do projeto:

* Proprietário do projeto

* Patrocinador do Projeto

* Gerenciador de Recursos

Agora, quando você adiciona um usuário a qualquer um desses campos nas áreas Editar ou Detalhes, além do nome e avatar, a função principal e o email também são exibidos. Isso ajuda a distinguir entre vários usuários com nomes semelhantes ou idênticos.

Para obter mais informações, consulte [Editar Projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

OBSERVAÇÃO: campos de usuário adicionais para projetos, tarefas e problemas serão atualizados com essa funcionalidade em versões futuras.

[Exibir uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Os campos de data calculados são sempre salvos com base no Tempo Universal Coordenado (UTC)

Agora, você pode ter certeza de que todas as funções de data em campos calculados funcionam de forma consistente e produzem o mesmo resultado para todos, independentemente de como uma expressão de dados personalizada é atualizada ou onde os usuários estão colaborando no objeto em todo o mundo.

Todos os cálculos agora são calculados e salvos por um padrão — Tempo universal coordenado (UTC) — e não pelas configurações de fuso horário definidas para a instância de sua organização e seu perfil de usuário individual. No entanto, os cálculos são exibidos em um formulário personalizado com base nos fusos horários individuais de cada usuário definidos em seu navegador.

Anteriormente, as configurações de tempo nos cálculos causavam confusão quando variavam nessas situações:

* Se alguém recalculou uma expressão de campo calculado usando &quot;Atualizar cálculos anteriores&quot; no construtor de formulários, os resultados da função de data foram determinados pelo fuso horário UTC da organização.

* Se alguém editou o objeto e isso causou o recálculo da expressão de campo calculado, os resultados da função de data foram determinados pelo fuso horário local do usuário. Os resultados do campo de data calculados neste cenário também serão calculados com base no UTC.

Para obter mais informações, consulte [Trabalhando em fusos horários](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Aprimoramentos de formulários personalizados: Adobe XD e o Filtro rápido

Com base em seus comentários, introduzimos as seguintes melhorias para melhorar a sua experiência ao gerenciar formulários personalizados:

* Adicione um arquivo Adobe XD para tornar um formulário personalizado mais visual e informativo. Quando o formulário é anexado a um objeto, os usuários que trabalham com o objeto podem visualizar e interagir com o arquivo XD de dentro do formulário.

  Para obter mais informações, consulte [Adicionar ou editar uma imagem ou outro widget de ativo em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Use o Filtro rápido para localizar facilmente itens na lista modernizada de formulários e campos personalizados. Além disso, desfrute de uma aparência aprimorada ao gerenciar formulários e campos.

  Para obter mais informações sobre o Filtro Rápido, consulte [Aplicar o filtro rápido a uma lista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Exibir uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Beta público - Nova experiência de filtro para projetos, tarefas e problemas

A filtragem em listas de projetos, tarefas e problemas foi reprojetada para ajudar você a criar e compartilhar filtros rapidamente. Os recursos incluem:

* Uma interface intuitiva de &quot;construtor beta&quot; para criar um novo filtro

* A capacidade de marcar um filtro como favorito

* Empilhamento de filtros (aplicando mais de um filtro salvo)

* Duplicar filtros

* Compartilhamento de filtros

* Remoção de filtros compartilhados com você


A nova experiência de filtro também está disponível em listas de folha de horas e no Planejador de cenários.

O modo de texto permanece disponível para edição avançada de filtros e os administradores do sistema ainda podem atribuir filtros padrão para todos os usuários por meio dos modelos de layout.

### Onde isso estará disponível?

* Listas de projetos/tarefas/problemas

* Planejador de cenários

* Planilhas de horas


### Queremos seus comentários!

Com esse Beta público, os usuários têm a oportunidade de enviar feedback diretamente para a equipe que está trabalhando na experiência dos filtros, clicando no botão de feedback. Esperamos receber notícias suas e de seus usuários sobre a nova experiência de filtro no beta público. Se sua equipe quiser se reunir com o produto diretamente para fornecer feedback adicional, sinta-se livre para agendar uma reunião aqui: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### O que vem a seguir?

* Nova experiência de agrupamentos e exibições (também conhecida como colunas)

  Começaremos a trabalhar na nova experiência de agrupamentos e visualizações (também conhecida como colunas), de modo que seja consistente com a nova experiência de filtros e tenha alguns dos mesmos excelentes recursos que a nova experiência de filtros.

* Implementar novos filtros em outras áreas do Adobe Workfront

  Trabalharemos com equipes no produto para implementar a nova experiência de filtros em outras áreas no Workfront.


Queremos agregar valor a você iterativamente para que continuemos a agregar valor à medida que as novas experiências e outras áreas estiverem prontas. Fique ligado para obter mais atualizações interessantes.

Para obter mais informações, consulte [Visão geral dos filtros](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Criar ou editar filtros no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Exibir uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412391/)
