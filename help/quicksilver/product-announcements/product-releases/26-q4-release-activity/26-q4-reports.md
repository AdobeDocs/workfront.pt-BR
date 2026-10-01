---
title: Melhorias na emissão de relatórios no quarto trimestre de 2026
description: Melhorias na emissão de relatórios no quarto trimestre de 2026
author: Becky
feature: Product Announcements
recommendations: noDisplay, noCatalog
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: a29813d3-f0cc-4b60-9396-13b558370803
    internal-label: Product announcements
source-git-commit: 3599b27bb1b838ebe7d0a2648e6c67333da83dc8
workflow-type: tm+mt
source-wordcount: '1434'
ht-degree: 5%
---
# Melhorias na emissão de relatórios no quarto trimestre de 2026

Esta página descreve as melhorias de relatórios feitas com a versão do quarto trimestre de 2026 para o ambiente de Pré-visualização. Essas melhorias serão disponibilizadas no ambiente de produção, conforme indicado.

Para obter uma lista de todas as alterações disponíveis neste momento do ciclo de lançamento do quarto trimestre de 2026, consulte [Visão geral da versão do quarto trimestre de 2026](/help/quicksilver/product-announcements/product-releases/26-q4-release-activity/26-q4-release-overview.md).

## Painéis do Canvas agora disponíveis na Google Cloud Platform e no Microsoft Azure

>[!NOTE]
>
>Visualização: N/D
>Versão rápida de produção: 14 de outubro de 2026
>Produção para todos: 15 de outubro de 2026

As instâncias do Workfront na Google Cloud Platform (GCP) e no Azure agora podem aceitar o beta aberto dos Painéis do Canvas. Para obter mais informações, consulte [Usar Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Registrar uma lista privada do Snowflake para Workfront Data Connect

>[!NOTE]
>
>Visualização: N/D
>Versão rápida de produção: 14 de outubro de 2026
>Produção para todos: 15 de outubro de 2026

Agora você pode compartilhar os dados do Workfront Data Connect diretamente com a conta da Snowflake de sua organização registrando uma lista privada. Esse método de conexão usa o recurso de listagem privada da Snowflake para compartilhar dados com segurança entre organizações sem expô-los publicamente, e funciona em regiões e plataformas de hospedagem.

Uma lista privada é útil quando você deseja unir seus dados do Workfront a outros dados no data warehouse da empresa. Como os dados chegam à sua própria conta do Snowflake, você pode consultá-los junto com o restante dos dados.

Para obter mais informações, consulte [Registrar uma lista privada para o Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/register-a-private-listing.md).

## As Ferramentas de MCP de relatórios agora estão disponíveis para Painéis do Canvas

>[!NOTE]
>
>Visualização: 1 de outubro de 2026
>Versão rápida de produção: 14 de outubro de 2026
>Produção para todos: 15 de outubro de 2026

Para facilitar o uso dos Painéis do Canvas, adicionamos ferramentas ao Workfront MCP. Agora, você pode criar e gerenciar Painéis do Canvas por meio do chat, e o painel e os widgets são criados para você usando os dados do Workfront. Isso funciona com clientes MCP como Claude e Cursor.

Por exemplo, você pode:

* Crie relatórios solicitando. Descreva um painel ou um gráfico em linguagem natural em vez de criá-lo manualmente.
* Edição no local. Peça para renomear um widget, alterar um filtro, trocar um tipo de gráfico ou redimensionar e as alterações se aplicam ao painel em tempo real.
* Reutilize o que você tem. Duplique um painel ou widget existente como ponto de partida, em vez de reconstruir do zero.

### Recursos compatíveis

**Painéis**

* Criar um novo painel
* Liste seus painéis (seus, compartilhados com você, todos ou favoritos) e pesquise por título
* Abrir ou exibir a estrutura de um painel
* Atualizar título, descrição, moeda, filtros e prompts
* Duplicação de um painel (com ou sem widgets, prompts e filtros)
* Excluir um painel

**Widgets**

* KPI — um único número agregado (soma, média, contagem, mínimo, máximo etc.)
* Gráfico — barra, coluna, linha e pizza; suporta gráficos simples, de várias séries e empilhados
* Tabela — tabelas de várias colunas com agrupamento de linhas
* Exibir a configuração de um widget e atualizar, copiar, redimensionar ou reposicionar, ou excluí-lo

**Opções de relatório**

* Filtrar dados com condições e grupos E/OU
* Agrupar e agregar por qualquer campo
* Fazer drill-down de um KPI ou gráfico nos registros subjacentes
* Rótulos de coluna personalizados, formatação de número, data e moeda e estilo condicional de célula
* Prompts e filtros no nível do painel

Para obter mais informações, consulte [Usar Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md).

## Copiar ou mover widgets entre Painéis do Canvas

>[!NOTE]
>
>Visualização: 1 de outubro de 2026
>Versão rápida de produção: 14 de outubro de 2026
>Produção para todos: 15 de outubro de 2026

Agora é possível copiar um widget para o mesmo painel, para outro painel ao qual você tem acesso de edição ou para um novo painel. Você também pode mover um widget para outro painel ao qual tem acesso de edição ou para um novo painel.

Ao copiar um widget, uma caixa de diálogo agora é aberta, onde você seleciona o painel de destino e onde deseja copiar ou mover o widget. Anteriormente, o Report Builder abria imediatamente.

## Filtrar os relacionamentos entre coleções nos Painéis do Canvas

>[!NOTE]
>
>Visualização: 1 de outubro de 2026
>Versão rápida de produção: 14 de outubro de 2026
>Produção para todos: 15 de outubro de 2026

Ao criar um filtro em um Painel da tela, agora é possível filtrar os relacionamentos de coleção, que são campos vinculados a um grupo de registros relacionados, em vez de a um único registro. Por exemplo, você pode filtrar o status de tarefas pertencentes a um projeto para mostrar uma lista de projetos que têm tarefas no status &quot;Novo&quot;.

Anteriormente, a filtragem em relações de coleção exigia o modo de texto.

Para obter mais informações, consulte [Referência do filtro de relatório para Painéis da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md).

## Copiar painéis nos painéis da tela

>[!NOTE]
>
>Visualização: 3 de setembro de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Agora você pode Copiar um Painel da Tela usando a nova ação **Copiar painel**. Essa ação está disponível para qualquer usuário cujo nível de acesso conceda direitos de edição ou criação aos Painéis, mesmo que ele só tenha acesso de visualização ao painel específico que está sendo copiado. Os usuários sem direitos de edição ou criação para Painéis não veem essa ação.

Ao copiar um painel, você pode renomeá-lo, atualizar sua descrição e moeda e escolher quais widgets, filtros de painel e prompts de painel devem ser transferidos para a cópia.

As configurações de Executar como usuário em widgets só serão preservadas se você for o usuário designado ou um administrador do sistema. As preferências de compartilhamento não são copiadas para o novo painel, e uma mensagem de confirmação com um link para o novo painel é exibida assim que a cópia é concluída.

Anteriormente, não havia como copiar um painel; os usuários precisavam reconstruir painéis do zero para criar variações específicas de público-alvo.

## Campo Tipo de aprovação nos Painéis de Controle da Tela

>[!NOTE]
>
>Produção para todos: 28 de agosto de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

A entidade Approval agora inclui um campo **Tipo de Aprovação**, que permite que os usuários façam a distinção entre aprovações de prova, aprovações de versão de documento, aprovações de entrada e outros tipos de aprovação.

## Atualização da terminologia de aprovação nos Painéis do Canvas

>[!NOTE]
>
>Produção para todos: 28 de agosto de 2026
>[!BADGE Fora do cronograma]{type=Neutral}

Os seguintes nomes de campo usados em Painéis de tela para aprovações de documentos e trabalhos foram renomeados para maior clareza:

| Nome anterior | Novo nome |
| --- | --- |
| Aprovação de documento | Aprovação |
| Estágio de aprovação do documento | Estágio de aprovação |
| Participante do estágio de aprovação do documento | Participante do estágio de aprovação |
| Processo de aprovação | Processo de aprovação do trabalho |
| Estágio de aprovação | Etapa de aprovação do trabalho |
| Status do aprovador | Status do aprovador do trabalho |
| Aguardando aprovação | Aguardando aprovação do trabalho |

Essa alteração não afeta a forma como os relatórios atuais funcionam.

## Relatórios de tabela dinâmica em Painéis da tela de desenho

>[!NOTE]
>
>Visualização: 27 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

O novo tipo de relatório de tabela dinâmica nos Painéis da tela agrega dados com roll-ups precisos e completos. Você pode criar métricas como contagens, somas e médias diretamente no painel e, em seguida, detalhar os registros subjacentes atrás de qualquer total.

Para obter mais informações, consulte [Criar um relatório de tabela dinâmica em um Painel da Tela](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-pivot-table-report.md).

## Imposição de datas de término para relatórios agendados

>[!NOTE]
>
>Visualização: 13 de agosto de 2026
>Versão rápida de produção: 17 de setembro de 2026
>Produção para todos: 15 de outubro de 2026

Os relatórios agendados agora exigem uma data de término para evitar entrega indefinida. Os cronogramas que passarem da data final serão desativados automaticamente.

As programações existentes foram atualizadas com datas de término para melhorar a confiabilidade e reduzir o uso desnecessário do sistema. A Workfront também oferece visibilidade e avisos adicionais para ajudar você a gerenciar os ciclos de vida do agendamento de relatórios à medida que se aproximam da data de término.

Para obter mais informações, consulte [Agendar uma entrega automática de relatório](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

## Campos de referência nativos estão disponíveis para listas e relatórios

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Agora é possível adicionar campos de referência nativos a listas e relatórios no Workfront.

Um campo de referência nativo é um campo personalizado. Quando o campo está em um formulário personalizado anexado a um objeto, o campo é preenchido a partir dos dados do objeto. Por exemplo, se o campo fizer referência ao campo Descrição e estiver em um formulário personalizado anexado a um projeto, ele extrairá a descrição do projeto. (O campo pode mostrar “N/A” se não houver dados disponíveis.)

Para obter informações sobre como criar campos de referência nativos, incluindo a lista de campos nativos com suporte, consulte [Criar um formulário personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
Para obter informações sobre como adicionar campos a relatórios, consulte [Criar um relatório personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Ordem consistente para valores de campo de seleção múltipla em listas e relatórios herdados

>[!NOTE]
>
>Visualização: 30 de julho de 2026
>Versão rápida de produção: 13 de agosto de 2026
>Produção para todos: 15 de outubro de 2026

Agora você vê as opções selecionadas para seleção múltipla de campos personalizados em uma ordem consistente e previsível em listas e relatórios herdados. A ordem dos campos é determinada pela organização dos campos no formulário personalizado.

![A ordem dos campos de formulário personalizados corresponde à ordem dos valores selecionados em uma lista ou relatório](assets/new-field-order-multi-select.png)

Anteriormente, as opções selecionadas eram exibidas na ordem em que você as escolhia ou em uma ordem inconsistente, o que tornava as linhas mais difíceis de serem digitalizadas e comparadas.

Observação: a nova classificação não se aplica se o campo estiver usando o modo de texto.
