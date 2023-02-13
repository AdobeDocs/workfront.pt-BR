---
title: 2.4 Melhorias do projeto
description: 2.4 Melhorias do projeto
author: Luke
draft: Probably
feature: Product Announcements
exl-id: 41372dd8-5002-4f8b-a5ac-a577c8b05d11
source-git-commit: 6cd6b1433fb56b92872f0ad80bb1a700fc0854cc
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 2%

---

# 2.4 Melhorias do projeto

Esta página descreve todas as melhorias do projeto feitas com a versão 2.4 para o ambiente de visualização. Esses aprimoramentos serão disponibilizados na semana de 3 de outubro de 2022.

Para obter uma lista de todas as alterações disponíveis com a versão 22.4, consulte [Visão geral da versão 2.4](/help/quicksilver/product-announcements/product-releases/22.4-release-activity/22-4-release-overview.md).

## Detalhes do antecessor disponíveis

Para exibir os detalhes dos antecessores de uma tarefa, agora é possível passar o mouse sobre o número do antecessor na coluna Predecessors . A caixa de detalhes exibe a tarefa predecessora e o projeto que estão sendo referenciados, as datas de início e término planejadas para a tarefa predecessora e o número de predecessores e sucessores da tarefa predecessora. Você pode expandir os detalhes do projeto para ver mais informações sobre ele. Informações adicionais estão incluídas para os antecessores de vários projetos.

Para obter mais informações, consulte [Criar uma relação de antecessor na lista de tarefas](/help/quicksilver/manage-work/tasks/use-prdcssrs/create-predecessors-on-task-list.md).

## Atribuir várias equipes a uma tarefa ou problema

Para lhe dar muito mais flexibilidade na maneira como você gerencia tarefas e problemas, tornamos possível atribuir várias equipes a uma tarefa ou problema. Anteriormente, somente uma equipe podia ser atribuída a uma tarefa ou problema.

>[!NOTE]
>
>No momento, essa funcionalidade não está disponível no Balanceador de carga de trabalho na área Equipes.

Para obter mais informações, consulte [Atribuir tarefas](/help/quicksilver/manage-work/tasks/assign-tasks/assign-tasks.md) e [Atribuir problemas](/help/quicksilver/manage-work/issues/manage-issues/assign-issues.md).

## Seleção de usuário inteligente para funções de projeto nas áreas Editar e Detalhes

Melhoramos a forma como os usuários são exibidos ao adicioná-los aos seguintes campos de projeto na caixa Editar e na seção Detalhes do projeto:

* Proprietário do projeto

* Patrocinador do Projeto

* Gerenciador de Recursos

Agora, ao adicionar um usuário a qualquer um desses campos nas áreas Editar ou Detalhes, além do nome e avatar, sua Função principal e seu email também são exibidos. Isso ajuda a distinguir entre vários usuários com nomes semelhantes ou idênticos.

Para obter mais informações, consulte [Editar projetos](/help/quicksilver/manage-work/projects/manage-projects/edit-projects.md).

OBSERVAÇÃO: Campos de usuário adicionais para projetos, tarefas e problemas serão atualizados com essa funcionalidade em versões futuras.

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412390/){target=_blank}

## Os campos de data calculados são sempre salvos com base no Tempo Universal Coordenado (UTC)

Agora, você pode ter certeza de que todas as funções de data em campos calculados funcionam de forma consistente e produzem o mesmo resultado para todos, independentemente de como uma expressão de dados personalizada é atualizada, ou onde os usuários estão colaborando no objeto em todo o mundo.

Todos os cálculos agora são calculados e salvos por um padrão — Tempo Universal Coordenado (UTC) — não pelas configurações de fuso horário definidas para a instância de sua organização e o perfil de usuário individual. No entanto, os cálculos são exibidos em um formulário personalizado com base nos fusos horários individuais de cada usuário definidos em seu navegador.

Anteriormente, as configurações de tempo em cálculos geravam confusão quando variavam nessas situações:

* Se alguém recalcular uma expressão de campo calculado usando &quot;Atualizar cálculos anteriores&quot; no construtor de formulários, os resultados da função de data serão determinados pelo fuso horário UTC de sua organização.

* Se alguém editou o objeto e fez com que a expressão de campo calculado fosse recalculada, os resultados da função de data seriam determinados pelo fuso horário local do usuário. Os resultados do campo de data calculada neste cenário também serão calculados com base no UTC.

Para obter mais informações, consulte [Trabalhar em vários fusos horários](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

## Aprimoramentos de formulário personalizado: Adobe XD e o filtro rápido

Com base em seus comentários, introduzimos as seguintes melhorias para melhorar sua experiência ao gerenciar formulários personalizados:

* Adicione um arquivo Adobe XD para tornar um formulário personalizado mais visual e informativo. Quando o formulário é anexado a um objeto, os usuários que trabalham com ele podem visualizar e interagir com o arquivo de XD a partir do formulário.

   Para obter mais informações, consulte [Adicionar ou editar uma imagem ou outro widget de ativo em um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* Use o Filtro rápido para localizar facilmente os itens na lista de formulários e campos personalizados modernizados. Aproveite também uma aparência aprimorada ao gerenciar formulários e campos.

   Para obter mais informações sobre o Filtro rápido, consulte [Aplicar o filtro rápido a uma lista](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/apply-quick-filter-list.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412469/){target=_blank}

## Beta público - Nova experiência de filtro para projetos, tarefas e problemas

A filtragem em listas de projetos, tarefas e problemas foi reprojetada para ajudá-lo a criar e compartilhar filtros rapidamente. Os recursos incluem:

* Uma interface &quot;beta builder&quot; intuitiva para criar um novo filtro

* A capacidade de marcar um filtro como favorito

* Empilhamento de filtro (aplicando mais de um filtro salvo)

* Duplicação de filtros

* Compartilhamento de filtros

* Remover filtros compartilhados com você


A nova experiência de filtro também está disponível em listas de folha de ponto e no Planejador de cenário.

O modo de texto permanece disponível para edição avançada de filtro, e os administradores do sistema ainda podem atribuir filtros padrão para todos os usuários por meio dos modelos de layout.

### Onde isso estará disponível?

* Listas de projetos/tarefas/problemas

* Planejador de cenários

* Folhas de horas


### Queremos seu feedback!

Com esse público Beta, os usuários têm a oportunidade de enviar feedback diretamente para a equipe que trabalha na experiência de filtros clicando no botão de feedback. Aguardamos com expectativa a possibilidade de ouvir você e seus usuários sobre a nova experiência de filtro em beta público. Se sua equipe quiser se encontrar com o produto diretamente para fornecer comentários adicionais, sinta-se à vontade para agendar uma reunião aqui: https://calendly.com/wf-product-and-design-research/filtersfeedbackpublicbeta?month=2022-08&amp;date=2022-08-25

### O que vem a seguir?

* Nova experiência de agrupamentos e exibições (também conhecidos como colunas)

   Começaremos a trabalhar na nova experiência de agrupamentos e visualizações (também conhecida como colunas) para que ela seja consistente com a nova experiência de filtros e tenha alguns dos mesmos recursos excelentes da experiência de novos filtros.

* Implementar novos filtros em outras áreas do Adobe Workfront

   Trabalharemos com equipes em todo o produto para implementar a nova experiência de filtros em outras áreas no Workfront.


Queremos oferecer valor a você iterativamente, para que continuemos a oferecer resultados à medida que as novas experiências e outras áreas estiverem prontas. Fique ligado para mais atualizações interessantes.

Para obter mais informações, consulte [Visão geral dos filtros no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/filters-overview.md) e [Criar ou editar filtros no Adobe Workfront](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/create-filters.md).

[Veja uma demonstração em vídeo desse recurso.](https://video.tv.adobe.com/v/3412391/)
